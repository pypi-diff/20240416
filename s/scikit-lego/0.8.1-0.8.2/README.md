# Comparing `tmp/scikit-lego-0.8.1.tar.gz` & `tmp/scikit-lego-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-lego-0.8.1.tar", last modified: Tue Mar 19 13:04:04 2024, max compression
+gzip compressed data, was "scikit-lego-0.8.2.tar", last modified: Tue Apr 16 12:17:58 2024, max compression
```

## Comparing `scikit-lego-0.8.1.tar` & `scikit-lego-0.8.2.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.702368 scikit-lego-0.8.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1077 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    11765 2024-03-19 13:04:04.702368 scikit-lego-0.8.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2450 2024-03-19 13:03:39.000000 scikit-lego-0.8.1/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7951 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/readme.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.666368 scikit-lego-0.8.1/scikit_lego.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    11765 2024-03-19 13:04:04.000000 scikit-lego-0.8.1/scikit_lego.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2044 2024-03-19 13:04:04.000000 scikit-lego-0.8.1/scikit_lego.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-03-19 13:04:04.000000 scikit-lego-0.8.1/scikit_lego.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      631 2024-03-19 13:04:04.000000 scikit-lego-0.8.1/scikit_lego.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2024-03-19 13:04:04.000000 scikit-lego-0.8.1/scikit_lego.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-03-19 13:04:04.702368 scikit-lego-0.8.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      182 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.670368 scikit-lego-0.8.1/sklego/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      194 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3175 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10255 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/common.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.674368 scikit-lego-0.8.1/sklego/data/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    59235 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/abalone.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18826 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/arrests.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2108 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/chickweight.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3620 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/hearts.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1340 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/heroes.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2974 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/data/penguins.zip
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18044 2024-03-19 13:03:39.000000 scikit-lego-0.8.1/sklego/datasets.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.674368 scikit-lego-0.8.1/sklego/decomposition/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      205 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/decomposition/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5335 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/decomposition/pca_reconstruction.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5152 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/decomposition/umap_reconstruction.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4265 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/dummy.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.674368 scikit-lego-0.8.1/sklego/feature_selection/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      132 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/feature_selection/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9598 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/feature_selection/mrmr.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    46591 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/linear_model.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.678368 scikit-lego-0.8.1/sklego/meta/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1282 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7590 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/_decay_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2241 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/_grouped_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8373 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/_shrinkage_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4104 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/confusion_balancer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6146 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/decay_estimator.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2945 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/estimator_transformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18461 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/grouped_predictor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7598 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/grouped_transformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25493 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/hierarchical_predictor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9056 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/ordinal_classification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3751 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/outlier_classifier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6705 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/regression_outlier_detector.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7619 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/subjective_classifier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4038 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/thresholder.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6177 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/meta/zero_inflated_regressor.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8652 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/metrics.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.682368 scikit-lego-0.8.1/sklego/mixture/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      378 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/mixture/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5365 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/mixture/bayesian_gmm_classifier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7643 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/mixture/bayesian_gmm_detector.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4726 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/mixture/gmm_classifier.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6954 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/mixture/gmm_outlier_detector.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25584 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/model_selection.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12490 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/naive_bayes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4702 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/neighbors.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1711 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/notinstalled.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10300 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/pandas_utils.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13630 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/pipeline.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.698368 scikit-lego-0.8.1/sklego/preprocessing/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1032 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8999 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/columncapper.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2848 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/dictmapper.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3533 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/formulaictransformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2656 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/identitytransformer.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8980 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/intervalencoder.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2302 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/outlier_remover.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12776 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/pandastransformers.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9144 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/projections.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3209 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/randomadder.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9919 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/preprocessing/repeatingbasis.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1388 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/testing.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1141 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/sklego/this.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-03-19 13:04:04.698368 scikit-lego-0.8.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1333 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/tests/test_datasets.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      786 2024-03-19 10:03:05.000000 scikit-lego-0.8.1/tests/test_notinstalled.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.786196 scikit-lego-0.8.2/
+-rw-r--r--   0 vincent    (501) staff       (20)     1077 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)    10406 2024-04-16 12:17:58.786012 scikit-lego-0.8.2/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     2450 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/pyproject.toml
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.772588 scikit-lego-0.8.2/scikit_lego.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)    10406 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     1984 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      631 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        7 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2024-04-16 12:17:58.786234 scikit-lego-0.8.2/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      182 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.777341 scikit-lego-0.8.2/sklego/
+-rw-r--r--   0 vincent    (501) staff       (20)      194 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3175 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/base.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10255 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/common.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.779340 scikit-lego-0.8.2/sklego/data/
+-rw-r--r--   0 vincent    (501) staff       (20)    59235 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/abalone.zip
+-rw-r--r--   0 vincent    (501) staff       (20)    18826 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/arrests.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     2108 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/chickweight.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     3620 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/hearts.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     1340 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/heroes.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     2974 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/penguins.zip
+-rw-r--r--   0 vincent    (501) staff       (20)    18044 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/datasets.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.779917 scikit-lego-0.8.2/sklego/decomposition/
+-rw-r--r--   0 vincent    (501) staff       (20)      205 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5335 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/pca_reconstruction.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5152 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/umap_reconstruction.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4265 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/dummy.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.780556 scikit-lego-0.8.2/sklego/feature_selection/
+-rw-r--r--   0 vincent    (501) staff       (20)      132 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/feature_selection/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9598 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/feature_selection/mrmr.py
+-rw-r--r--   0 vincent    (501) staff       (20)    46591 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/linear_model.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.783581 scikit-lego-0.8.2/sklego/meta/
+-rw-r--r--   0 vincent    (501) staff       (20)     1282 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7590 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/_decay_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2241 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/_grouped_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8373 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/_shrinkage_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4104 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/confusion_balancer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6146 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/decay_estimator.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2945 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/estimator_transformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    18461 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/grouped_predictor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7598 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/grouped_transformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    25493 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/hierarchical_predictor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9056 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/ordinal_classification.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4376 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/outlier_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6705 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/regression_outlier_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7619 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/subjective_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4038 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/thresholder.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6177 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/zero_inflated_regressor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8652 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/metrics.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.784210 scikit-lego-0.8.2/sklego/mixture/
+-rw-r--r--   0 vincent    (501) staff       (20)      378 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5365 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7678 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4726 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/gmm_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6989 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/mixture/gmm_outlier_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)    26016 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/model_selection.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12490 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/naive_bayes.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4702 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/neighbors.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1711 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/notinstalled.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10311 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/pandas_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13636 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/pipeline.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.785785 scikit-lego-0.8.2/sklego/preprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)     1032 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8999 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/columncapper.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3518 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/dictmapper.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4348 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/formulaictransformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3347 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/identitytransformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8980 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/intervalencoder.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2779 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/outlier_remover.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13377 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/pandastransformers.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9605 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/projections.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3209 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/randomadder.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10461 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/repeatingbasis.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1388 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/testing.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1513 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/this.py
```

### Comparing `scikit-lego-0.8.1/LICENSE` & `scikit-lego-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/PKG-INFO` & `scikit-lego-0.8.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7363 696b  : 2.1.Name: scik
 00000020: 6974 2d6c 6567 6f0a 5665 7273 696f 6e3a  it-lego.Version:
-00000030: 2030 2e38 2e31 0a53 756d 6d61 7279 3a20   0.8.1.Summary: 
+00000030: 2030 2e38 2e32 0a53 756d 6d61 7279 3a20   0.8.2.Summary: 
 00000040: 4120 636f 6c6c 6563 7469 6f6e 206f 6620  A collection of 
 00000050: 6c65 676f 2062 7269 636b 7320 666f 7220  lego bricks for 
 00000060: 7363 696b 6974 2d6c 6561 726e 2070 6970  scikit-learn pip
 00000070: 656c 696e 6573 0a41 7574 686f 723a 2056  elines.Author: V
 00000080: 696e 6365 6e74 2044 2e20 5761 726d 6572  incent D. Warmer
 00000090: 6461 6d2c 204d 6174 7468 696a 7320 4272  dam, Matthijs Br
 000000a0: 6f75 6e73 0a4d 6169 6e74 6169 6e65 723a  ouns.Maintainer:
@@ -135,602 +135,517 @@
 00000860: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
 00000870: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
 00000880: 7320 3a3a 2050 7974 686f 6e20 4d6f 6475  s :: Python Modu
 00000890: 6c65 730a 5265 7175 6972 6573 2d50 7974  les.Requires-Pyt
 000008a0: 686f 6e3a 203e 3d33 2e36 0a44 6573 6372  hon: >=3.6.Descr
 000008b0: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
 000008c0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-000008d0: 776e 0a4c 6963 656e 7365 2d46 696c 653a  wn.License-File:
-000008e0: 204c 4943 454e 5345 0a52 6571 7569 7265   LICENSE.Require
-000008f0: 732d 4469 7374 3a20 7061 6e64 6173 3e3d  s-Dist: pandas>=
-00000900: 312e 312e 350a 5265 7175 6972 6573 2d44  1.1.5.Requires-D
-00000910: 6973 743a 2073 6369 6b69 742d 6c65 6172  ist: scikit-lear
-00000920: 6e3e 3d31 2e30 0a52 6571 7569 7265 732d  n>=1.0.Requires-
-00000930: 4469 7374 3a20 696d 706f 7274 6c69 622d  Dist: importlib-
-00000940: 6d65 7461 6461 7461 3e3d 312e 303b 2070  metadata>=1.0; p
-00000950: 7974 686f 6e5f 7665 7273 696f 6e20 3c20  ython_version < 
-00000960: 2233 2e38 220a 5265 7175 6972 6573 2d44  "3.8".Requires-D
-00000970: 6973 743a 2069 6d70 6f72 746c 6962 2d72  ist: importlib-r
-00000980: 6573 6f75 7263 6573 3b20 7079 7468 6f6e  esources; python
-00000990: 5f76 6572 7369 6f6e 203c 2022 332e 3922  _version < "3.9"
-000009a0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-000009b0: 2063 7678 7079 0a52 6571 7569 7265 732d   cvxpy.Requires-
-000009c0: 4469 7374 3a20 636d 616b 653b 2065 7874  Dist: cmake; ext
-000009d0: 7261 203d 3d20 2263 7678 7079 220a 5265  ra == "cvxpy".Re
-000009e0: 7175 6972 6573 2d44 6973 743a 206f 7371  quires-Dist: osq
-000009f0: 703b 2065 7874 7261 203d 3d20 2263 7678  p; extra == "cvx
-00000a00: 7079 220a 5265 7175 6972 6573 2d44 6973  py".Requires-Dis
-00000a10: 743a 2063 7678 7079 3e3d 312e 312e 383b  t: cvxpy>=1.1.8;
-00000a20: 2065 7874 7261 203d 3d20 2263 7678 7079   extra == "cvxpy
-00000a30: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
-00000a40: 3a20 666f 726d 756c 6169 630a 5265 7175  : formulaic.Requ
-00000a50: 6972 6573 2d44 6973 743a 2066 6f72 6d75  ires-Dist: formu
-00000a60: 6c61 6963 3e3d 302e 362e 303b 2065 7874  laic>=0.6.0; ext
-00000a70: 7261 203d 3d20 2266 6f72 6d75 6c61 6963  ra == "formulaic
-00000a80: 220a 5072 6f76 6964 6573 2d45 7874 7261  ".Provides-Extra
-00000a90: 3a20 756d 6170 0a52 6571 7569 7265 732d  : umap.Requires-
-00000aa0: 4469 7374 3a20 756d 6170 2d6c 6561 726e  Dist: umap-learn
-00000ab0: 3e3d 302e 342e 363b 2065 7874 7261 203d  >=0.4.6; extra =
-00000ac0: 3d20 2275 6d61 7022 0a50 726f 7669 6465  = "umap".Provide
-00000ad0: 732d 4578 7472 613a 2061 6c6c 0a52 6571  s-Extra: all.Req
-00000ae0: 7569 7265 732d 4469 7374 3a20 7363 696b  uires-Dist: scik
-00000af0: 6974 2d6c 6567 6f5b 6376 7870 792c 666f  it-lego[cvxpy,fo
-00000b00: 726d 756c 6169 632c 756d 6170 5d3b 2065  rmulaic,umap]; e
-00000b10: 7874 7261 203d 3d20 2261 6c6c 220a 5072  xtra == "all".Pr
-00000b20: 6f76 6964 6573 2d45 7874 7261 3a20 646f  ovides-Extra: do
-00000b30: 6373 0a52 6571 7569 7265 732d 4469 7374  cs.Requires-Dist
-00000b40: 3a20 6d6b 646f 6373 3e3d 312e 352e 333b  : mkdocs>=1.5.3;
-00000b50: 2065 7874 7261 203d 3d20 2264 6f63 7322   extra == "docs"
-00000b60: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
-00000b70: 6d6b 646f 6373 2d61 7574 6f72 6566 733e  mkdocs-autorefs>
-00000b80: 3d30 2e35 2e30 3b20 6578 7472 6120 3d3d  =0.5.0; extra ==
-00000b90: 2022 646f 6373 220a 5265 7175 6972 6573   "docs".Requires
-00000ba0: 2d44 6973 743a 206d 6b64 6f63 732d 6d61  -Dist: mkdocs-ma
-00000bb0: 7465 7269 616c 3e3d 392e 342e 353b 2065  terial>=9.4.5; e
-00000bc0: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000bd0: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
-00000be0: 646f 6373 2d6d 6174 6572 6961 6c2d 6578  docs-material-ex
-00000bf0: 7465 6e73 696f 6e73 3e3d 312e 323b 2065  tensions>=1.2; e
-00000c00: 7874 7261 203d 3d20 2264 6f63 7322 0a52  xtra == "docs".R
-00000c10: 6571 7569 7265 732d 4469 7374 3a20 6d6b  equires-Dist: mk
-00000c20: 646f 6373 7472 696e 6773 3e3d 302e 3233  docstrings>=0.23
-00000c30: 2e30 3b20 6578 7472 6120 3d3d 2022 646f  .0; extra == "do
-00000c40: 6373 220a 5265 7175 6972 6573 2d44 6973  cs".Requires-Dis
-00000c50: 743a 206d 6b64 6f63 7374 7269 6e67 732d  t: mkdocstrings-
-00000c60: 7079 7468 6f6e 3e3d 312e 372e 333b 2065  python>=1.7.3; e
-00000c70: 7874 7261 203d 3d20 2264 6f63 7322 0a50  xtra == "docs".P
-00000c80: 726f 7669 6465 732d 4578 7472 613a 2074  rovides-Extra: t
-00000c90: 6573 740a 5265 7175 6972 6573 2d44 6973  est.Requires-Dis
-00000ca0: 743a 2073 6369 6b69 742d 6c65 676f 5b61  t: scikit-lego[a
-00000cb0: 6c6c 5d3b 2065 7874 7261 203d 3d20 2274  ll]; extra == "t
-00000cc0: 6573 7422 0a52 6571 7569 7265 732d 4469  est".Requires-Di
-00000cd0: 7374 3a20 7079 7465 7374 3e3d 362e 322e  st: pytest>=6.2.
-00000ce0: 353b 2065 7874 7261 203d 3d20 2274 6573  5; extra == "tes
-00000cf0: 7422 0a52 6571 7569 7265 732d 4469 7374  t".Requires-Dist
-00000d00: 3a20 7079 7465 7374 2d78 6469 7374 3e3d  : pytest-xdist>=
-00000d10: 312e 3334 2e30 3b20 6578 7472 6120 3d3d  1.34.0; extra ==
-00000d20: 2022 7465 7374 220a 5265 7175 6972 6573   "test".Requires
-00000d30: 2d44 6973 743a 2070 7974 6573 742d 636f  -Dist: pytest-co
-00000d40: 763e 3d32 2e36 2e31 3b20 6578 7472 6120  v>=2.6.1; extra 
-00000d50: 3d3d 2022 7465 7374 220a 5265 7175 6972  == "test".Requir
-00000d60: 6573 2d44 6973 743a 2070 7974 6573 742d  es-Dist: pytest-
-00000d70: 6d6f 636b 3e3d 312e 362e 333b 2065 7874  mock>=1.6.3; ext
-00000d80: 7261 203d 3d20 2274 6573 7422 0a50 726f  ra == "test".Pro
-00000d90: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-00000da0: 6c73 0a52 6571 7569 7265 732d 4469 7374  ls.Requires-Dist
-00000db0: 3a20 6d61 7470 6c6f 746c 6962 3e3d 332e  : matplotlib>=3.
-00000dc0: 302e 323b 2065 7874 7261 203d 3d20 2275  0.2; extra == "u
-00000dd0: 7469 6c73 220a 5265 7175 6972 6573 2d44  tils".Requires-D
-00000de0: 6973 743a 206a 7570 7974 6572 3e3d 312e  ist: jupyter>=1.
-00000df0: 302e 303b 2065 7874 7261 203d 3d20 2275  0.0; extra == "u
-00000e00: 7469 6c73 220a 5265 7175 6972 6573 2d44  tils".Requires-D
-00000e10: 6973 743a 206a 7570 7974 6572 6c61 623e  ist: jupyterlab>
-00000e20: 3d30 2e33 352e 343b 2065 7874 7261 203d  =0.35.4; extra =
-00000e30: 3d20 2275 7469 6c73 220a 5072 6f76 6964  = "utils".Provid
-00000e40: 6573 2d45 7874 7261 3a20 6465 760a 5265  es-Extra: dev.Re
-00000e50: 7175 6972 6573 2d44 6973 743a 2073 6369  quires-Dist: sci
-00000e60: 6b69 742d 6c65 676f 5b61 6c6c 2c64 6f63  kit-lego[all,doc
-00000e70: 732c 7465 7374 5d3b 2065 7874 7261 203d  s,test]; extra =
-00000e80: 3d20 2264 6576 220a 5265 7175 6972 6573  = "dev".Requires
-00000e90: 2d44 6973 743a 2070 7265 2d63 6f6d 6d69  -Dist: pre-commi
-00000ea0: 743e 3d31 2e31 382e 333b 2065 7874 7261  t>=1.18.3; extra
-00000eb0: 203d 3d20 2264 6576 220a 5265 7175 6972   == "dev".Requir
-00000ec0: 6573 2d44 6973 743a 2072 7566 663e 3d30  es-Dist: ruff>=0
-00000ed0: 2e31 2e36 3b20 6578 7472 6120 3d3d 2022  .1.6; extra == "
-00000ee0: 6465 7622 0a0a 5b21 5b44 6f77 6e6c 6f61  dev"..[![Downloa
-00000ef0: 6473 5d28 6874 7470 733a 2f2f 7374 6174  ds](https://stat
-00000f00: 6963 2e70 6570 792e 7465 6368 2f62 6164  ic.pepy.tech/bad
-00000f10: 6765 2f73 6369 6b69 742d 6c65 676f 2f6d  ge/scikit-lego/m
-00000f20: 6f6e 7468 295d 2868 7474 7073 3a2f 2f77  onth)](https://w
-00000f30: 7777 2e70 6570 792e 7465 6368 2f70 726f  ww.pepy.tech/pro
-00000f40: 6a65 6374 732f 7363 696b 6974 2d6c 6567  jects/scikit-leg
-00000f50: 6f29 0a5b 215b 5665 7273 696f 6e5d 2868  o).[![Version](h
-00000f60: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000f70: 6473 2e69 6f2f 7079 7069 2f76 2f73 6369  ds.io/pypi/v/sci
-00000f80: 6b69 742d 6c65 676f 295d 2868 7474 7073  kit-lego)](https
-00000f90: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000fa0: 6563 742f 7363 696b 6974 2d6c 6567 6f2f  ect/scikit-lego/
-00000fb0: 290a 5b21 5b43 6f6e 6461 2056 6572 7369  ).[![Conda Versi
-00000fc0: 6f6e 5d28 6874 7470 733a 2f2f 696d 672e  on](https://img.
-00000fd0: 7368 6965 6c64 732e 696f 2f63 6f6e 6461  shields.io/conda
-00000fe0: 2f76 6e2f 636f 6e64 612d 666f 7267 652f  /vn/conda-forge/
-00000ff0: 7363 696b 6974 2d6c 6567 6f2e 7376 6729  scikit-lego.svg)
-00001000: 5d28 6874 7470 733a 2f2f 616e 6163 6f6e  ](https://anacon
-00001010: 6461 2e6f 7267 2f63 6f6e 6461 2d66 6f72  da.org/conda-for
-00001020: 6765 2f73 6369 6b69 742d 6c65 676f 290a  ge/scikit-lego).
-00001030: 215b 5d28 6874 7470 733a 2f2f 696d 672e  ![](https://img.
-00001040: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
-00001050: 622f 6c69 6365 6e73 652f 6b6f 616e 696e  b/license/koanin
-00001060: 672f 7363 696b 6974 2d6c 6567 6f29 0a21  g/scikit-lego).!
-00001070: 5b5d 2868 7474 7073 3a2f 2f69 6d67 2e73  [](https://img.s
-00001080: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-00001090: 7976 6572 7369 6f6e 732f 7363 696b 6974  yversions/scikit
-000010a0: 2d6c 6567 6f29 0a21 5b5d 2868 7474 7073  -lego).![](https
-000010b0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-000010c0: 6f2f 6769 7468 7562 2f63 6f6e 7472 6962  o/github/contrib
-000010d0: 7574 6f72 732f 6b6f 616e 696e 672f 7363  utors/koaning/sc
-000010e0: 696b 6974 2d6c 6567 6f29 0a5b 215b 5275  ikit-lego).[![Ru
-000010f0: 6666 5d28 6874 7470 733a 2f2f 696d 672e  ff](https://img.
-00001100: 7368 6965 6c64 732e 696f 2f65 6e64 706f  shields.io/endpo
-00001110: 696e 743f 7572 6c3d 6874 7470 733a 2f2f  int?url=https://
-00001120: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00001130: 6e74 656e 742e 636f 6d2f 6173 7472 616c  ntent.com/astral
-00001140: 2d73 682f 7275 6666 2f6d 6169 6e2f 6173  -sh/ruff/main/as
-00001150: 7365 7473 2f62 6164 6765 2f76 322e 6a73  sets/badge/v2.js
-00001160: 6f6e 295d 2868 7474 7073 3a2f 2f67 6974  on)](https://git
-00001170: 6875 622e 636f 6d2f 6173 7472 616c 2d73  hub.com/astral-s
-00001180: 682f 7275 6666 290a 5b21 5b44 4f49 5d28  h/ruff).[![DOI](
-00001190: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
-000011a0: 7267 2f62 6164 6765 2f31 3636 3833 3639  rg/badge/1668369
-000011b0: 3339 2e73 7667 295d 2868 7474 7073 3a2f  39.svg)](https:/
-000011c0: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
-000011d0: 652f 6c61 7465 7374 646f 692f 3136 3638  e/latestdoi/1668
-000011e0: 3336 3933 3929 0a0a 2320 7363 696b 6974  36939)..# scikit
-000011f0: 2d6c 6567 6f0a 0a3c 6120 6872 6566 3d22  -lego..<a href="
-00001200: 6874 7470 733a 2f2f 6b6f 616e 696e 672e  https://koaning.
-00001210: 6769 7468 7562 2e69 6f2f 7363 696b 6974  github.io/scikit
-00001220: 2d6c 6567 6f2f 223e 3c69 6d67 2073 7263  -lego/"><img src
-00001230: 3d22 696d 6167 6573 2f6c 6f67 6f2e 706e  ="images/logo.pn
-00001240: 6722 2077 6964 7468 3d22 3335 2522 2068  g" width="35%" h
-00001250: 6569 6768 743d 2233 3525 2220 616c 6967  eight="35%" alig
-00001260: 6e3d 2272 6967 6874 2220 2f3e 3c2f 613e  n="right" /></a>
-00001270: 0a0a 5765 206c 6f76 6520 7363 696b 6974  ..We love scikit
-00001280: 206c 6561 726e 2062 7574 2076 6572 7920   learn but very 
-00001290: 6f66 7465 6e20 7765 2066 696e 6420 6f75  often we find ou
-000012a0: 7273 656c 7665 7320 7772 6974 696e 670a  rselves writing.
-000012b0: 6375 7374 6f6d 2074 7261 6e73 666f 726d  custom transform
-000012c0: 6572 732c 206d 6574 7269 6373 2061 6e64  ers, metrics and
-000012d0: 206d 6f64 656c 732e 2054 6865 2067 6f61   models. The goa
-000012e0: 6c20 6f66 2074 6869 7320 7072 6f6a 6563  l of this projec
-000012f0: 740a 6973 2074 6f20 6174 7465 6d70 7420  t.is to attempt 
-00001300: 746f 2063 6f6e 736f 6c69 6461 7465 2074  to consolidate t
-00001310: 6865 7365 2069 6e74 6f20 6120 7061 636b  hese into a pack
-00001320: 6167 6520 7468 6174 206f 6666 6572 730a  age that offers.
-00001330: 636f 6465 2071 7561 6c69 7479 2f74 6573  code quality/tes
-00001340: 7469 6e67 2e20 5468 6973 2070 726f 6a65  ting. This proje
-00001350: 6374 2073 7461 7274 6564 2061 7320 6120  ct started as a 
-00001360: 636f 6c6c 6162 6f72 6174 696f 6e20 6265  collaboration be
-00001370: 7477 6565 6e0a 6d75 6c74 6970 6c65 2063  tween.multiple c
-00001380: 6f6d 7061 6e69 6573 2069 6e20 7468 6520  ompanies in the 
-00001390: 4e65 7468 6572 6c61 6e64 7320 6275 7420  Netherlands but 
-000013a0: 6861 7320 7369 6e63 6520 7265 6365 6976  has since receiv
-000013b0: 6564 2063 6f6e 7472 6962 7574 696f 6e73  ed contributions
-000013c0: 0a66 726f 6d20 6172 6f75 6e64 2074 6865  .from around the
-000013d0: 2067 6c6f 6265 2e20 4974 2077 6173 2069   globe. It was i
-000013e0: 6e69 7469 6174 6564 2062 7920 5b4d 6174  nitiated by [Mat
-000013f0: 7468 696a 7320 4272 6f75 6e73 5d28 6874  thijs Brouns](ht
-00001400: 7470 733a 2f2f 7777 772e 6d62 726f 756e  tps://www.mbroun
-00001410: 732e 636f 6d2f 290a 616e 6420 5b56 696e  s.com/).and [Vin
-00001420: 6365 6e74 2044 2e20 5761 726d 6572 6461  cent D. Warmerda
-00001430: 6d5d 2868 7474 7073 3a2f 2f6b 6f61 6e69  m](https://koani
-00001440: 6e67 2e69 6f29 2061 7320 6120 746f 6f6c  ng.io) as a tool
-00001450: 2074 6f20 7465 6163 6820 7065 6f70 6c65   to teach people
-00001460: 2068 6f77 0a74 6f20 636f 6e74 7269 6275   how.to contribu
-00001470: 7465 2074 6f20 6f70 656e 2073 6f75 7263  te to open sourc
-00001480: 652e 0a0a 4e6f 7465 2074 6861 7420 7765  e...Note that we
-00001490: 2772 6520 6e6f 7420 666f 726d 616c 6c79  're not formally
-000014a0: 2061 6666 696c 6961 7465 6420 7769 7468   affiliated with
-000014b0: 2074 6865 2073 6369 6b69 742d 6c65 6172   the scikit-lear
-000014c0: 6e20 7072 6f6a 6563 7420 6174 2061 6c6c  n project at all
-000014d0: 2c0a 6275 7420 7765 2061 696d 2074 6f20  ,.but we aim to 
-000014e0: 7374 7269 6374 6c79 2061 6468 6572 6520  strictly adhere 
-000014f0: 746f 2074 6865 6972 2073 7461 6e64 6172  to their standar
-00001500: 6473 2e0a 0a54 6865 2073 616d 6520 686f  ds...The same ho
-00001510: 6c64 7320 7769 7468 206c 6567 6f2e 204c  lds with lego. L
-00001520: 4547 4fc2 ae20 6973 2061 2074 7261 6465  EGO.. is a trade
-00001530: 6d61 726b 206f 6620 7468 6520 4c45 474f  mark of the LEGO
-00001540: 2047 726f 7570 206f 6620 636f 6d70 616e   Group of compan
-00001550: 6965 7320 7768 6963 6820 646f 6573 206e  ies which does n
-00001560: 6f74 2073 706f 6e73 6f72 2c20 6175 7468  ot sponsor, auth
-00001570: 6f72 697a 6520 6f72 2065 6e64 6f72 7365  orize or endorse
-00001580: 2074 6869 7320 7072 6f6a 6563 742e 0a0a   this project...
-00001590: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
-000015a0: 0a49 6e73 7461 6c6c 2060 7363 696b 6974  .Install `scikit
-000015b0: 2d6c 6567 6f60 2076 6961 2070 6970 2077  -lego` via pip w
-000015c0: 6974 680a 0a60 6060 6261 7368 0a70 7974  ith..```bash.pyt
-000015d0: 686f 6e20 2d6d 2070 6970 2069 6e73 7461  hon -m pip insta
-000015e0: 6c6c 2073 6369 6b69 742d 6c65 676f 0a60  ll scikit-lego.`
-000015f0: 6060 0a0a 5669 6120 5b63 6f6e 6461 5d28  ``..Via [conda](
-00001600: 6874 7470 733a 2f2f 636f 6e64 612e 696f  https://conda.io
-00001610: 2f70 726f 6a65 6374 732f 636f 6e64 612f  /projects/conda/
-00001620: 656e 2f6c 6174 6573 742f 2920 7769 7468  en/latest/) with
-00001630: 0a0a 6060 6062 6173 680a 636f 6e64 6120  ..```bash.conda 
-00001640: 696e 7374 616c 6c20 2d63 2063 6f6e 6461  install -c conda
-00001650: 2d66 6f72 6765 2073 6369 6b69 742d 6c65  -forge scikit-le
-00001660: 676f 0a60 6060 0a0a 416c 7465 726e 6174  go.```..Alternat
-00001670: 6976 656c 792c 2074 6f20 6564 6974 2061  ively, to edit a
-00001680: 6e64 2063 6f6e 7472 6962 7574 6520 796f  nd contribute yo
-00001690: 7520 6361 6e20 666f 726b 2f63 6c6f 6e65  u can fork/clone
-000016a0: 2061 6e64 2072 756e 3a0a 0a60 6060 6261   and run:..```ba
-000016b0: 7368 0a70 7974 686f 6e20 2d6d 2070 6970  sh.python -m pip
-000016c0: 2069 6e73 7461 6c6c 202d 6520 222e 5b64   install -e ".[d
-000016d0: 6576 5d22 0a70 7974 686f 6e20 7365 7475  ev]".python setu
-000016e0: 702e 7079 2064 6576 656c 6f70 0a60 6060  p.py develop.```
-000016f0: 0a0a 2323 2044 6f63 756d 656e 7461 7469  ..## Documentati
-00001700: 6f6e 0a0a 5468 6520 646f 6375 6d65 6e74  on..The document
-00001710: 6174 696f 6e20 6361 6e20 6265 2066 6f75  ation can be fou
-00001720: 6e64 205b 6865 7265 5d28 6874 7470 733a  nd [here](https:
-00001730: 2f2f 6b6f 616e 696e 672e 6769 7468 7562  //koaning.github
-00001740: 2e69 6f2f 7363 696b 6974 2d6c 6567 6f2f  .io/scikit-lego/
-00001750: 292e 0a0a 2323 2055 7361 6765 0a0a 5765  )...## Usage..We
-00001760: 206f 6666 6572 2063 7573 746f 6d20 6d65   offer custom me
-00001770: 7472 6963 732c 206d 6f64 656c 7320 616e  trics, models an
-00001780: 6420 7472 616e 7366 6f72 6d65 7273 2e20  d transformers. 
-00001790: 596f 7520 6361 6e20 696d 706f 7274 2074  You can import t
-000017a0: 6865 6d20 6a75 7374 206c 696b 6520 796f  hem just like yo
-000017b0: 7520 776f 756c 640a 696e 2073 6369 6b69  u would.in sciki
-000017c0: 742d 6c65 6172 6e2e 0a0a 6060 6070 7974  t-learn...```pyt
-000017d0: 686f 6e0a 2320 7468 6520 7363 696b 6974  hon.# the scikit
-000017e0: 206c 6561 726e 2073 7475 6666 2077 6520   learn stuff we 
-000017f0: 6c6f 7665 0a66 726f 6d20 736b 6c65 6172  love.from sklear
-00001800: 6e2e 7072 6570 726f 6365 7373 696e 6720  n.preprocessing 
-00001810: 696d 706f 7274 2053 7461 6e64 6172 6453  import StandardS
-00001820: 6361 6c65 720a 6672 6f6d 2073 6b6c 6561  caler.from sklea
-00001830: 726e 2e70 6970 656c 696e 6520 696d 706f  rn.pipeline impo
-00001840: 7274 2050 6970 656c 696e 650a 0a23 2066  rt Pipeline..# f
-00001850: 726f 6d20 7363 696b 6974 206c 6567 6f20  rom scikit lego 
-00001860: 7374 7566 6620 7765 2061 6464 0a66 726f  stuff we add.fro
-00001870: 6d20 736b 6c65 676f 2e70 7265 7072 6f63  m sklego.preproc
-00001880: 6573 7369 6e67 2069 6d70 6f72 7420 5261  essing import Ra
-00001890: 6e64 6f6d 4164 6465 720a 6672 6f6d 2073  ndomAdder.from s
-000018a0: 6b6c 6567 6f2e 6d69 7874 7572 6520 696d  klego.mixture im
-000018b0: 706f 7274 2047 4d4d 436c 6173 7369 6669  port GMMClassifi
-000018c0: 6572 0a0a 2e2e 2e0a 0a6d 6f64 203d 2050  er.......mod = P
-000018d0: 6970 656c 696e 6528 5b0a 2020 2020 2822  ipeline([.    ("
-000018e0: 7363 616c 6522 2c20 5374 616e 6461 7264  scale", Standard
-000018f0: 5363 616c 6572 2829 292c 0a20 2020 2028  Scaler()),.    (
-00001900: 2272 616e 646f 6d5f 6e6f 6973 6522 2c20  "random_noise", 
-00001910: 5261 6e64 6f6d 4164 6465 7228 2929 2c0a  RandomAdder()),.
-00001920: 2020 2020 2822 6d6f 6465 6c22 2c20 474d      ("model", GM
-00001930: 4d43 6c61 7373 6966 6965 7228 2929 0a5d  MClassifier()).]
-00001940: 290a 0a2e 2e2e 0a60 6060 0a0a 2323 2046  )......```..## F
-00001950: 6561 7475 7265 730a 0a48 6572 6527 7320  eatures..Here's 
-00001960: 6120 6c69 7374 206f 6620 6665 6174 7572  a list of featur
-00001970: 6573 2074 6861 7420 7468 6973 206c 6962  es that this lib
-00001980: 7261 7279 2063 7572 7265 6e74 6c79 206f  rary currently o
-00001990: 6666 6572 733a 0a0a 2d20 6073 6b6c 6567  ffers:..- `skleg
-000019a0: 6f2e 6461 7461 7365 7473 2e6c 6f61 645f  o.datasets.load_
-000019b0: 6162 616c 6f6e 6560 206c 6f61 6473 2069  abalone` loads i
-000019c0: 6e20 7468 6520 6162 616c 6f6e 6520 6461  n the abalone da
-000019d0: 7461 7365 740a 2d20 6073 6b6c 6567 6f2e  taset.- `sklego.
-000019e0: 6461 7461 7365 7473 2e6c 6f61 645f 6172  datasets.load_ar
-000019f0: 7265 7374 7360 206c 6f61 6473 2069 6e20  rests` loads in 
-00001a00: 6120 6461 7461 7365 7420 7769 7468 2066  a dataset with f
-00001a10: 6169 726e 6573 7320 636f 6e63 6572 6e73  airness concerns
-00001a20: 0a2d 2060 736b 6c65 676f 2e64 6174 6173  .- `sklego.datas
-00001a30: 6574 732e 6c6f 6164 5f63 6869 636b 656e  ets.load_chicken
-00001a40: 6020 6c6f 6164 7320 696e 2074 6865 206a  ` loads in the j
-00001a50: 6f79 6675 6c20 6368 6963 6b77 6569 6768  oyful chickweigh
-00001a60: 7420 6461 7461 7365 740a 2d20 6073 6b6c  t dataset.- `skl
-00001a70: 6567 6f2e 6461 7461 7365 7473 2e6c 6f61  ego.datasets.loa
-00001a80: 645f 6865 726f 6573 6020 6c6f 6164 7320  d_heroes` loads 
-00001a90: 6120 6865 726f 6573 206f 6620 7468 6520  a heroes of the 
-00001aa0: 7374 6f72 6d20 6461 7461 7365 740a 2d20  storm dataset.- 
-00001ab0: 6073 6b6c 6567 6f2e 6461 7461 7365 7473  `sklego.datasets
-00001ac0: 2e6c 6f61 645f 6865 6172 7473 6020 6c6f  .load_hearts` lo
-00001ad0: 6164 7320 6120 6461 7461 7365 7420 6162  ads a dataset ab
-00001ae0: 6f75 7420 6865 6172 7473 0a2d 2060 736b  out hearts.- `sk
-00001af0: 6c65 676f 2e64 6174 6173 6574 732e 6c6f  lego.datasets.lo
-00001b00: 6164 5f70 656e 6775 696e 7360 206c 6f61  ad_penguins` loa
-00001b10: 6473 2061 206c 6f76 656c 7920 6461 7461  ds a lovely data
-00001b20: 7365 7420 6162 6f75 7420 7065 6e67 7569  set about pengui
-00001b30: 6e73 0a2d 2060 736b 6c65 676f 2e64 6174  ns.- `sklego.dat
-00001b40: 6173 6574 732e 6665 7463 685f 6372 6564  asets.fetch_cred
-00001b50: 6974 6361 7264 6020 6665 7463 6820 6120  itcard` fetch a 
-00001b60: 6672 6175 6420 6461 7461 7365 7420 6672  fraud dataset fr
-00001b70: 6f6d 206f 7065 6e6d 6c0a 2d20 6073 6b6c  om openml.- `skl
-00001b80: 6567 6f2e 6461 7461 7365 7473 2e6d 616b  ego.datasets.mak
-00001b90: 655f 7369 6d70 6c65 7365 7269 6573 6020  e_simpleseries` 
-00001ba0: 6d61 6b65 2061 2073 696d 756c 6174 6564  make a simulated
-00001bb0: 2074 696d 6573 6572 6965 730a 2d20 6073   timeseries.- `s
-00001bc0: 6b6c 6567 6f2e 7061 6e64 6173 5f75 7469  klego.pandas_uti
-00001bd0: 6c73 2e61 6464 5f6c 6167 7360 2061 6464  ls.add_lags` add
-00001be0: 7320 6c61 6720 7661 6c75 6573 2069 6e20  s lag values in 
-00001bf0: 6120 7061 6e64 6173 2064 6174 6166 7261  a pandas datafra
-00001c00: 6d65 0a2d 2060 736b 6c65 676f 2e70 616e  me.- `sklego.pan
-00001c10: 6461 735f 7574 696c 732e 6c6f 675f 7374  das_utils.log_st
-00001c20: 6570 6020 6120 7573 6566 756c 2064 6563  ep` a useful dec
-00001c30: 6f72 6174 6f72 2074 6f20 6c6f 6720 796f  orator to log yo
-00001c40: 7572 2070 6970 656c 696e 6520 7374 6570  ur pipeline step
-00001c50: 730a 2d20 6073 6b6c 6567 6f2e 6475 6d6d  s.- `sklego.dumm
-00001c60: 792e 5261 6e64 6f6d 5265 6772 6573 736f  y.RandomRegresso
-00001c70: 7260 2064 756d 6d79 2062 656e 6368 6d61  r` dummy benchma
-00001c80: 726b 2074 6861 7420 7072 6564 6963 7473  rk that predicts
-00001c90: 2072 616e 646f 6d20 7661 6c75 6573 0a2d   random values.-
-00001ca0: 2060 736b 6c65 676f 2e6c 696e 6561 725f   `sklego.linear_
-00001cb0: 6d6f 6465 6c2e 4465 6164 5a6f 6e65 5265  model.DeadZoneRe
-00001cc0: 6772 6573 736f 7260 2065 7870 6572 696d  gressor` experim
-00001cd0: 656e 7461 6c20 6665 6174 7572 6520 7468  ental feature th
-00001ce0: 6174 2068 6173 2061 2064 6561 647a 6f6e  at has a deadzon
-00001cf0: 6520 696e 2074 6865 2063 6f73 7420 6675  e in the cost fu
-00001d00: 6e63 7469 6f6e 0a2d 2060 736b 6c65 676f  nction.- `sklego
-00001d10: 2e6c 696e 6561 725f 6d6f 6465 6c2e 4465  .linear_model.De
-00001d20: 6d6f 6772 6170 6869 6350 6172 6974 7943  mographicParityC
-00001d30: 6c61 7373 6966 6965 7260 206c 6f67 6973  lassifier` logis
-00001d40: 7469 6320 636c 6173 7369 6669 6572 2063  tic classifier c
-00001d50: 6f6e 7374 7261 696e 6564 206f 6e20 6465  onstrained on de
-00001d60: 6d6f 6772 6170 6869 6320 7061 7269 7479  mographic parity
-00001d70: 0a2d 2060 736b 6c65 676f 2e6c 696e 6561  .- `sklego.linea
-00001d80: 725f 6d6f 6465 6c2e 4571 7561 6c4f 7070  r_model.EqualOpp
-00001d90: 6f72 7475 6e69 7479 436c 6173 7369 6669  ortunityClassifi
-00001da0: 6572 6020 6c6f 6769 7374 6963 2063 6c61  er` logistic cla
-00001db0: 7373 6966 6965 7220 636f 6e73 7472 6169  ssifier constrai
-00001dc0: 6e65 6420 6f6e 2065 7175 616c 206f 7070  ned on equal opp
-00001dd0: 6f72 7475 6e69 7479 0a2d 2060 736b 6c65  ortunity.- `skle
-00001de0: 676f 2e6c 696e 6561 725f 6d6f 6465 6c2e  go.linear_model.
-00001df0: 5072 6f62 5765 6967 6874 5265 6772 6573  ProbWeightRegres
-00001e00: 7369 6f6e 6020 6c69 6e65 6172 206d 6f64  sion` linear mod
-00001e10: 656c 2074 6861 7420 7472 6561 7473 2063  el that treats c
-00001e20: 6f65 6666 6963 6965 6e74 7320 6173 2070  oefficients as p
-00001e30: 726f 6261 6269 6c69 7374 6963 2077 6569  robabilistic wei
-00001e40: 6768 7473 0a2d 2060 736b 6c65 676f 2e6c  ghts.- `sklego.l
-00001e50: 696e 6561 725f 6d6f 6465 6c2e 4c6f 7765  inear_model.Lowe
-00001e60: 7373 5265 6772 6573 7369 6f6e 6020 6c6f  ssRegression` lo
-00001e70: 6361 6c6c 7920 7765 6967 6874 6564 206c  cally weighted l
-00001e80: 696e 6561 7220 7265 6772 6573 7369 6f6e  inear regression
-00001e90: 0a2d 2060 736b 6c65 676f 2e6c 696e 6561  .- `sklego.linea
-00001ea0: 725f 6d6f 6465 6c2e 4c41 4452 6567 7265  r_model.LADRegre
-00001eb0: 7373 696f 6e60 206c 6561 7374 2061 6273  ssion` least abs
-00001ec0: 6f6c 7574 6520 6465 7669 6174 696f 6e20  olute deviation 
-00001ed0: 7265 6772 6573 7369 6f6e 0a2d 2060 736b  regression.- `sk
-00001ee0: 6c65 676f 2e6c 696e 6561 725f 6d6f 6465  lego.linear_mode
-00001ef0: 6c2e 5175 616e 7469 6c65 5265 6772 6573  l.QuantileRegres
-00001f00: 7369 6f6e 6020 6c69 6e65 6172 2071 7561  sion` linear qua
-00001f10: 6e74 696c 6520 7265 6772 6573 7369 6f6e  ntile regression
-00001f20: 2c20 6765 6e65 7261 6c69 7a65 7320 4c41  , generalizes LA
-00001f30: 4452 6567 7265 7373 696f 6e0a 2d20 6073  DRegression.- `s
-00001f40: 6b6c 6567 6f2e 6c69 6e65 6172 5f6d 6f64  klego.linear_mod
-00001f50: 656c 2e49 6d62 616c 616e 6365 644c 696e  el.ImbalancedLin
-00001f60: 6561 7252 6567 7265 7373 696f 6e60 2070  earRegression` p
-00001f70: 756e 6973 6820 6f76 6572 2f75 6e64 6572  unish over/under
-00001f80: 2d65 7374 696d 6174 696f 6e20 6f66 2061  -estimation of a
-00001f90: 206d 6f64 656c 2064 6972 6563 746c 790a   model directly.
-00001fa0: 2d20 6073 6b6c 6567 6f2e 6e61 6976 655f  - `sklego.naive_
-00001fb0: 6261 7965 732e 4761 7573 7369 616e 4d69  bayes.GaussianMi
-00001fc0: 7874 7572 654e 4260 2063 6c61 7373 6966  xtureNB` classif
-00001fd0: 6965 7320 6279 2074 7261 696e 696e 6720  ies by training 
-00001fe0: 6120 3144 2047 4d4d 2070 6572 2063 6f6c  a 1D GMM per col
-00001ff0: 756d 6e20 7065 7220 636c 6173 730a 2d20  umn per class.- 
-00002000: 6073 6b6c 6567 6f2e 6e61 6976 655f 6261  `sklego.naive_ba
-00002010: 7965 732e 4261 7965 7369 616e 4761 7573  yes.BayesianGaus
-00002020: 7369 616e 4d69 7874 7572 654e 4260 2063  sianMixtureNB` c
-00002030: 6c61 7373 6966 6965 7320 6279 2074 7261  lassifies by tra
-00002040: 696e 696e 6720 6120 6261 7965 7369 616e  ining a bayesian
-00002050: 2031 4420 474d 4d20 7065 7220 636c 6173   1D GMM per clas
-00002060: 730a 2d20 6073 6b6c 6567 6f2e 6d69 7874  s.- `sklego.mixt
-00002070: 7572 652e 4261 7965 7369 616e 474d 4d43  ure.BayesianGMMC
-00002080: 6c61 7373 6966 6965 7260 2063 6c61 7373  lassifier` class
-00002090: 6966 6965 7320 6279 2074 7261 696e 696e  ifies by trainin
-000020a0: 6720 6120 6261 7965 7369 616e 2047 4d4d  g a bayesian GMM
-000020b0: 2070 6572 2063 6c61 7373 0a2d 2060 736b   per class.- `sk
-000020c0: 6c65 676f 2e6d 6978 7475 7265 2e42 6179  lego.mixture.Bay
-000020d0: 6573 6961 6e47 4d4d 4f75 746c 6965 7244  esianGMMOutlierD
-000020e0: 6574 6563 746f 7260 2064 6574 6563 7473  etector` detects
-000020f0: 206f 7574 6c69 6572 7320 6261 7365 6420   outliers based 
-00002100: 6f6e 2061 2074 7261 696e 6564 2062 6179  on a trained bay
-00002110: 6573 6961 6e20 474d 4d0a 2d20 6073 6b6c  esian GMM.- `skl
-00002120: 6567 6f2e 6d69 7874 7572 652e 474d 4d43  ego.mixture.GMMC
-00002130: 6c61 7373 6966 6965 7260 2063 6c61 7373  lassifier` class
-00002140: 6966 6965 7320 6279 2074 7261 696e 696e  ifies by trainin
-00002150: 6720 6120 474d 4d20 7065 7220 636c 6173  g a GMM per clas
-00002160: 730a 2d20 6073 6b6c 6567 6f2e 6d69 7874  s.- `sklego.mixt
-00002170: 7572 652e 474d 4d4f 7574 6c69 6572 4465  ure.GMMOutlierDe
-00002180: 7465 6374 6f72 6020 6465 7465 6374 7320  tector` detects 
-00002190: 6f75 746c 6965 7273 2062 6173 6564 206f  outliers based o
-000021a0: 6e20 6120 7472 6169 6e65 6420 474d 4d0a  n a trained GMM.
-000021b0: 2d20 6073 6b6c 6567 6f2e 6d65 7461 2e43  - `sklego.meta.C
-000021c0: 6f6e 6675 7369 6f6e 4261 6c61 6e63 6572  onfusionBalancer
-000021d0: 6020 6578 7065 7269 6d65 6e74 616c 2066  ` experimental f
-000021e0: 6561 7475 7265 2074 6861 7420 616c 6c6f  eature that allo
-000021f0: 7773 2079 6f75 2074 6f20 6261 6c61 6e63  ws you to balanc
-00002200: 6520 7468 6520 636f 6e66 7573 696f 6e20  e the confusion 
-00002210: 6d61 7472 6978 0a2d 2060 736b 6c65 676f  matrix.- `sklego
-00002220: 2e6d 6574 612e 4465 6361 7945 7374 696d  .meta.DecayEstim
-00002230: 6174 6f72 6020 6164 6473 2064 6563 6179  ator` adds decay
-00002240: 2074 6f20 7468 6520 7361 6d70 6c65 5f77   to the sample_w
-00002250: 6569 6768 7420 7468 6174 2074 6865 206d  eight that the m
-00002260: 6f64 656c 2061 6363 6570 7473 0a2d 2060  odel accepts.- `
-00002270: 736b 6c65 676f 2e6d 6574 612e 4573 7469  sklego.meta.Esti
-00002280: 6d61 746f 7254 7261 6e73 666f 726d 6572  matorTransformer
-00002290: 6020 6164 6473 2061 206d 6f64 656c 206f  ` adds a model o
-000022a0: 7574 7075 7420 6173 2061 2066 6561 7475  utput as a featu
-000022b0: 7265 0a2d 2060 736b 6c65 676f 2e6d 6574  re.- `sklego.met
-000022c0: 612e 4f75 746c 6965 7243 6c61 7373 6966  a.OutlierClassif
-000022d0: 6965 7260 2074 7572 6e73 206f 7574 6c69  ier` turns outli
-000022e0: 6572 206d 6f64 656c 7320 696e 746f 2063  er models into c
-000022f0: 6c61 7373 6966 6965 7273 2066 6f72 2067  lassifiers for g
-00002300: 7269 6473 6561 7263 680a 2d20 6073 6b6c  ridsearch.- `skl
-00002310: 6567 6f2e 6d65 7461 2e47 726f 7570 6564  ego.meta.Grouped
-00002320: 5072 6564 6963 746f 7260 2063 616e 2073  Predictor` can s
-00002330: 706c 6974 2074 6865 2064 6174 6120 696e  plit the data in
-00002340: 746f 2072 756e 7320 616e 6420 7275 6e20  to runs and run 
-00002350: 6120 6d6f 6465 6c20 6f6e 2065 6163 680a  a model on each.
-00002360: 2d20 6073 6b6c 6567 6f2e 6d65 7461 2e47  - `sklego.meta.G
-00002370: 726f 7570 6564 5472 616e 7366 6f72 6d65  roupedTransforme
-00002380: 7260 2063 616e 2073 706c 6974 2074 6865  r` can split the
-00002390: 2064 6174 6120 696e 746f 2072 756e 7320   data into runs 
-000023a0: 616e 6420 7275 6e20 6120 7472 616e 7366  and run a transf
-000023b0: 6f72 6d65 7220 6f6e 2065 6163 680a 2d20  ormer on each.- 
-000023c0: 6073 6b6c 6567 6f2e 6d65 7461 2e53 7562  `sklego.meta.Sub
-000023d0: 6a65 6374 6976 6543 6c61 7373 6966 6965  jectiveClassifie
-000023e0: 7260 2065 7870 6572 696d 656e 7461 6c20  r` experimental 
-000023f0: 6665 6174 7572 6520 746f 2061 6464 2061  feature to add a
-00002400: 2070 7269 6f72 2074 6f20 796f 7572 2063   prior to your c
-00002410: 6c61 7373 6966 6965 720a 2d20 6073 6b6c  lassifier.- `skl
-00002420: 6567 6f2e 6d65 7461 2e54 6872 6573 686f  ego.meta.Thresho
-00002430: 6c64 6572 6020 6d65 7461 206d 6f64 656c  lder` meta model
-00002440: 2074 6861 7420 616c 6c6f 7773 2079 6f75   that allows you
-00002450: 2074 6f20 6772 6964 7365 6172 6368 206f   to gridsearch o
-00002460: 7665 7220 7468 6520 7468 7265 7368 6f6c  ver the threshol
-00002470: 640a 2d20 6073 6b6c 6567 6f2e 6d65 7461  d.- `sklego.meta
-00002480: 2e52 6567 7265 7373 696f 6e4f 7574 6c69  .RegressionOutli
-00002490: 6572 4465 7465 6374 6f72 6020 6d65 7461  erDetector` meta
-000024a0: 206d 6f64 656c 2074 6861 7420 6669 6e64   model that find
-000024b0: 7320 6f75 746c 6965 7273 2062 7920 6164  s outliers by ad
-000024c0: 6469 6e67 2061 2074 6872 6573 686f 6c64  ding a threshold
-000024d0: 2074 6f20 7265 6772 6573 7369 6f6e 0a2d   to regression.-
-000024e0: 2060 736b 6c65 676f 2e6d 6574 612e 5a65   `sklego.meta.Ze
-000024f0: 726f 496e 666c 6174 6564 5265 6772 6573  roInflatedRegres
-00002500: 736f 7260 2070 7265 6469 6374 7320 7a65  sor` predicts ze
-00002510: 726f 206f 7220 6170 706c 6965 7320 6120  ro or applies a 
-00002520: 7265 6772 6573 7369 6f6e 2062 6173 6564  regression based
-00002530: 206f 6e20 6120 636c 6173 7369 6669 6572   on a classifier
-00002540: 0a2d 2060 736b 6c65 676f 2e70 7265 7072  .- `sklego.prepr
-00002550: 6f63 6573 7369 6e67 2e43 6f6c 756d 6e43  ocessing.ColumnC
-00002560: 6170 7065 7260 206c 696d 6974 7320 6578  apper` limits ex
-00002570: 7472 656d 6520 7661 6c75 6573 206f 6620  treme values of 
-00002580: 7468 6520 6d6f 6465 6c20 6665 6174 7572  the model featur
-00002590: 6573 0a2d 2060 736b 6c65 676f 2e70 7265  es.- `sklego.pre
-000025a0: 7072 6f63 6573 7369 6e67 2e43 6f6c 756d  processing.Colum
-000025b0: 6e44 726f 7070 6572 6020 6472 6f70 7320  nDropper` drops 
-000025c0: 6120 636f 6c75 6d6e 2066 726f 6d20 7061  a column from pa
-000025d0: 6e64 6173 0a2d 2060 736b 6c65 676f 2e70  ndas.- `sklego.p
-000025e0: 7265 7072 6f63 6573 7369 6e67 2e43 6f6c  reprocessing.Col
-000025f0: 756d 6e53 656c 6563 746f 7260 2073 656c  umnSelector` sel
-00002600: 6563 7473 2063 6f6c 756d 6e73 2062 6173  ects columns bas
-00002610: 6564 206f 6e20 636f 6c75 6d6e 206e 616d  ed on column nam
-00002620: 650a 2d20 6073 6b6c 6567 6f2e 7072 6570  e.- `sklego.prep
-00002630: 726f 6365 7373 696e 672e 496e 666f 726d  rocessing.Inform
-00002640: 6174 696f 6e46 696c 7465 7260 2074 7261  ationFilter` tra
-00002650: 6e73 666f 726d 6572 2074 6861 7420 6361  nsformer that ca
-00002660: 6e20 6465 2d63 6f72 7265 6c61 7465 2066  n de-correlate f
-00002670: 6561 7475 7265 730a 2d20 6073 6b6c 6567  eatures.- `skleg
-00002680: 6f2e 7072 6570 726f 6365 7373 696e 672e  o.preprocessing.
-00002690: 4964 656e 7469 7479 5472 616e 7366 6f72  IdentityTransfor
-000026a0: 6d65 7260 2072 6574 7572 6e73 2074 6865  mer` returns the
-000026b0: 2073 616d 6520 6461 7461 2c20 616c 6c6f   same data, allo
-000026c0: 7773 2066 6f72 2063 6f6e 6361 7465 6e61  ws for concatena
-000026d0: 7469 6e67 2070 6970 656c 696e 6573 0a2d  ting pipelines.-
-000026e0: 2060 736b 6c65 676f 2e70 7265 7072 6f63   `sklego.preproc
-000026f0: 6573 7369 6e67 2e4f 7274 686f 676f 6e61  essing.Orthogona
-00002700: 6c54 7261 6e73 666f 726d 6572 6020 6d61  lTransformer` ma
-00002710: 6b65 7320 616c 6c20 6665 6174 7572 6573  kes all features
-00002720: 206c 696e 6561 726c 7920 696e 6465 7065   linearly indepe
-00002730: 6e64 656e 740a 2d20 6073 6b6c 6567 6f2e  ndent.- `sklego.
-00002740: 7072 6570 726f 6365 7373 696e 672e 5061  preprocessing.Pa
-00002750: 6e64 6173 5479 7065 5365 6c65 6374 6f72  ndasTypeSelector
-00002760: 6020 7365 6c65 6374 7320 636f 6c75 6d6e  ` selects column
-00002770: 7320 6261 7365 6420 6f6e 2070 616e 6461  s based on panda
-00002780: 7320 7479 7065 0a2d 2060 736b 6c65 676f  s type.- `sklego
-00002790: 2e70 7265 7072 6f63 6573 7369 6e67 2e52  .preprocessing.R
-000027a0: 616e 646f 6d41 6464 6572 6020 6164 6473  andomAdder` adds
-000027b0: 2072 616e 646f 6d6e 6573 7320 696e 2074   randomness in t
-000027c0: 7261 696e 696e 670a 2d20 6073 6b6c 6567  raining.- `skleg
-000027d0: 6f2e 7072 6570 726f 6365 7373 696e 672e  o.preprocessing.
-000027e0: 5265 7065 6174 696e 6742 6173 6973 4675  RepeatingBasisFu
-000027f0: 6e63 7469 6f6e 6020 7265 7065 6174 696e  nction` repeatin
-00002800: 6720 6665 6174 7572 6520 656e 6769 6e65  g feature engine
-00002810: 6572 696e 672c 2075 7365 6675 6c20 666f  ering, useful fo
-00002820: 7220 7469 6d65 7365 7269 6573 0a2d 2060  r timeseries.- `
-00002830: 736b 6c65 676f 2e70 7265 7072 6f63 6573  sklego.preproces
-00002840: 7369 6e67 2e44 6963 744d 6170 7065 7260  sing.DictMapper`
-00002850: 2061 7373 6967 6e20 6e75 6d65 7269 6320   assign numeric 
-00002860: 7661 6c75 6573 206f 6e20 6361 7465 676f  values on catego
-00002870: 7269 6361 6c20 636f 6c75 6d6e 730a 2d20  rical columns.- 
-00002880: 6073 6b6c 6567 6f2e 7072 6570 726f 6365  `sklego.preproce
-00002890: 7373 696e 672e 4f75 746c 6965 7252 656d  ssing.OutlierRem
-000028a0: 6f76 6572 6020 6578 7065 7269 6d65 6e74  over` experiment
-000028b0: 616c 206d 6574 686f 6420 746f 2072 656d  al method to rem
-000028c0: 6f76 6520 6f75 746c 6965 7273 2064 7572  ove outliers dur
-000028d0: 696e 6720 7472 6169 6e69 6e67 0a2d 2060  ing training.- `
-000028e0: 736b 6c65 676f 2e6d 6f64 656c 5f73 656c  sklego.model_sel
-000028f0: 6563 7469 6f6e 2e47 726f 7570 5469 6d65  ection.GroupTime
-00002900: 5365 7269 6573 5370 6c69 7460 2074 696d  SeriesSplit` tim
-00002910: 6573 6572 6965 7320 4b66 6f6c 6420 666f  eseries Kfold fo
-00002920: 7220 6772 6f75 7073 2077 6974 6820 6469  r groups with di
-00002930: 6666 6572 656e 7420 616d 6f75 6e74 206f  fferent amount o
-00002940: 6620 6f62 7365 7276 6174 696f 6e73 2070  f observations p
-00002950: 6572 2067 726f 7570 0a2d 2060 736b 6c65  er group.- `skle
-00002960: 676f 2e6d 6f64 656c 5f73 656c 6563 7469  go.model_selecti
-00002970: 6f6e 2e4b 6c75 7374 6572 466f 6c64 5661  on.KlusterFoldVa
-00002980: 6c69 6461 7469 6f6e 6020 6578 7065 7269  lidation` experi
-00002990: 6d65 6e74 616c 2066 6561 7475 7265 2074  mental feature t
-000029a0: 6861 7420 646f 6573 204b 2066 6f6c 6473  hat does K folds
-000029b0: 2062 6173 6564 206f 6e20 636c 7573 7465   based on cluste
-000029c0: 7269 6e67 0a2d 2060 736b 6c65 676f 2e6d  ring.- `sklego.m
-000029d0: 6f64 656c 5f73 656c 6563 7469 6f6e 2e54  odel_selection.T
-000029e0: 696d 6547 6170 5370 6c69 7460 2074 696d  imeGapSplit` tim
-000029f0: 6573 6572 6965 7320 4b66 6f6c 6420 7769  eseries Kfold wi
-00002a00: 7468 2061 2067 6170 2062 6574 7765 656e  th a gap between
-00002a10: 2074 7261 696e 2f74 6573 740a 2d20 6073   train/test.- `s
-00002a20: 6b6c 6567 6f2e 7069 7065 6c69 6e65 2e44  klego.pipeline.D
-00002a30: 6562 7567 5069 7065 6c69 6e65 6020 6164  ebugPipeline` ad
-00002a40: 6473 2064 6562 7567 2069 6e66 6f72 6d61  ds debug informa
-00002a50: 7469 6f6e 2074 6f20 6d61 6b65 2064 6562  tion to make deb
-00002a60: 7567 6769 6e67 2065 6173 6965 720a 2d20  ugging easier.- 
-00002a70: 6073 6b6c 6567 6f2e 7069 7065 6c69 6e65  `sklego.pipeline
-00002a80: 2e6d 616b 655f 6465 6275 675f 7069 7065  .make_debug_pipe
-00002a90: 6c69 6e65 6020 7368 6f72 7468 616e 6420  line` shorthand 
-00002aa0: 6675 6e63 7469 6f6e 2074 6f20 6372 6561  function to crea
-00002ab0: 7465 2061 2064 6562 7567 6162 6c65 2070  te a debugable p
-00002ac0: 6970 656c 696e 650a 2d20 6073 6b6c 6567  ipeline.- `skleg
-00002ad0: 6f2e 6d65 7472 6963 732e 636f 7272 656c  o.metrics.correl
-00002ae0: 6174 696f 6e5f 7363 6f72 6560 2063 616c  ation_score` cal
-00002af0: 6375 6c61 7465 7320 636f 7272 656c 6174  culates correlat
-00002b00: 696f 6e20 6265 7477 6565 6e20 6d6f 6465  ion between mode
-00002b10: 6c20 6f75 7470 7574 2061 6e64 2066 6561  l output and fea
-00002b20: 7475 7265 0a2d 2060 736b 6c65 676f 2e6d  ture.- `sklego.m
-00002b30: 6574 7269 6373 2e65 7175 616c 5f6f 7070  etrics.equal_opp
-00002b40: 6f72 7475 6e69 7479 5f73 636f 7265 6020  ortunity_score` 
-00002b50: 6361 6c63 756c 6174 6573 2065 7175 616c  calculates equal
-00002b60: 206f 7070 6f72 7475 6e69 7479 206d 6574   opportunity met
-00002b70: 7269 630a 2d20 6073 6b6c 6567 6f2e 6d65  ric.- `sklego.me
-00002b80: 7472 6963 732e 705f 7065 7263 656e 745f  trics.p_percent_
-00002b90: 7363 6f72 6560 2070 726f 7879 2066 6f72  score` proxy for
-00002ba0: 206d 6f64 656c 2066 6169 726e 6573 7320   model fairness 
-00002bb0: 7769 7468 2072 6567 6172 6473 2074 6f20  with regards to 
-00002bc0: 7365 6e73 6974 6976 6520 6174 7472 6962  sensitive attrib
-00002bd0: 7574 650a 2d20 6073 6b6c 6567 6f2e 6d65  ute.- `sklego.me
-00002be0: 7472 6963 732e 7375 6273 6574 5f73 636f  trics.subset_sco
-00002bf0: 7265 6020 6361 6c63 756c 6174 6520 6120  re` calculate a 
-00002c00: 7363 6f72 6520 6f6e 2061 2073 7562 7365  score on a subse
-00002c10: 7420 6f66 2079 6f75 7220 6461 7461 2028  t of your data (
-00002c20: 6d65 616e 7420 666f 7220 6661 6972 6e65  meant for fairne
-00002c30: 7373 2074 7261 636b 696e 6729 0a0a 2323  ss tracking)..##
-00002c40: 204e 6577 2046 6561 7475 7265 730a 0a57   New Features..W
-00002c50: 6520 7761 6e74 2074 6f20 6265 2072 6174  e want to be rat
-00002c60: 6865 7220 6f70 656e 2068 6572 6520 696e  her open here in
-00002c70: 2077 6861 7420 7765 2061 6363 6570 7420   what we accept 
-00002c80: 6275 7420 7765 2064 6f20 6465 6d61 6e64  but we do demand
-00002c90: 2074 6872 6565 0a74 6869 6e67 7320 6265   three.things be
-00002ca0: 666f 7265 2074 6865 7920 6265 636f 6d65  fore they become
-00002cb0: 2061 6464 6564 2074 6f20 7468 6520 7072   added to the pr
-00002cc0: 6f6a 6563 743a 0a0a 312e 2061 6e79 206e  oject:..1. any n
-00002cd0: 6577 2066 6561 7475 7265 2063 6f6e 7472  ew feature contr
-00002ce0: 6962 7574 6573 2074 6f77 6172 6473 2061  ibutes towards a
-00002cf0: 2064 656d 6f6e 7374 7261 626c 6520 7265   demonstrable re
-00002d00: 616c 2d77 6f72 6c64 2075 7365 6361 7365  al-world usecase
-00002d10: 0a32 2e20 616e 7920 6e65 7720 6665 6174  .2. any new feat
-00002d20: 7572 6520 7061 7373 6573 2073 7461 6e64  ure passes stand
-00002d30: 6172 6420 756e 6974 2074 6573 7473 2028  ard unit tests (
-00002d40: 7765 2075 7365 2074 6865 206f 6e65 7320  we use the ones 
-00002d50: 6672 6f6d 2073 6369 6b69 742d 6c65 6172  from scikit-lear
-00002d60: 6e29 0a33 2e20 7468 6520 6665 6174 7572  n).3. the featur
-00002d70: 6520 6861 7320 6265 656e 2064 6973 6375  e has been discu
-00002d80: 7373 6564 2069 6e20 7468 6520 6973 7375  ssed in the issu
-00002d90: 6520 6c69 7374 2062 6566 6f72 6568 616e  e list beforehan
-00002da0: 640a 0a57 6520 6175 746f 6d61 7465 2061  d..We automate a
-00002db0: 6c6c 206f 6620 6f75 7220 7465 7374 696e  ll of our testin
-00002dc0: 6720 616e 6420 7573 6520 7072 652d 636f  g and use pre-co
-00002dd0: 6d6d 6974 2068 6f6f 6b73 2074 6f20 6b65  mmit hooks to ke
-00002de0: 6570 2074 6865 2063 6f64 6520 776f 726b  ep the code work
-00002df0: 696e 672e 0a                             ing..
+000008d0: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
+000008e0: 613a 2063 7678 7079 0a50 726f 7669 6465  a: cvxpy.Provide
+000008f0: 732d 4578 7472 613a 2066 6f72 6d75 6c61  s-Extra: formula
+00000900: 6963 0a50 726f 7669 6465 732d 4578 7472  ic.Provides-Extr
+00000910: 613a 2075 6d61 700a 5072 6f76 6964 6573  a: umap.Provides
+00000920: 2d45 7874 7261 3a20 616c 6c0a 5072 6f76  -Extra: all.Prov
+00000930: 6964 6573 2d45 7874 7261 3a20 646f 6373  ides-Extra: docs
+00000940: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+00000950: 2074 6573 740a 5072 6f76 6964 6573 2d45   test.Provides-E
+00000960: 7874 7261 3a20 7574 696c 730a 5072 6f76  xtra: utils.Prov
+00000970: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
+00000980: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
+00000990: 4345 4e53 450a 0a5b 215b 446f 776e 6c6f  CENSE..[![Downlo
+000009a0: 6164 735d 2868 7474 7073 3a2f 2f73 7461  ads](https://sta
+000009b0: 7469 632e 7065 7079 2e74 6563 682f 6261  tic.pepy.tech/ba
+000009c0: 6467 652f 7363 696b 6974 2d6c 6567 6f2f  dge/scikit-lego/
+000009d0: 6d6f 6e74 6829 5d28 6874 7470 733a 2f2f  month)](https://
+000009e0: 7777 772e 7065 7079 2e74 6563 682f 7072  www.pepy.tech/pr
+000009f0: 6f6a 6563 7473 2f73 6369 6b69 742d 6c65  ojects/scikit-le
+00000a00: 676f 290a 5b21 5b56 6572 7369 6f6e 5d28  go).[![Version](
+00000a10: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000a20: 6c64 732e 696f 2f70 7970 692f 762f 7363  lds.io/pypi/v/sc
+00000a30: 696b 6974 2d6c 6567 6f29 5d28 6874 7470  ikit-lego)](http
+00000a40: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000a50: 6a65 6374 2f73 6369 6b69 742d 6c65 676f  ject/scikit-lego
+00000a60: 2f29 0a5b 215b 436f 6e64 6120 5665 7273  /).[![Conda Vers
+00000a70: 696f 6e5d 2868 7474 7073 3a2f 2f69 6d67  ion](https://img
+00000a80: 2e73 6869 656c 6473 2e69 6f2f 636f 6e64  .shields.io/cond
+00000a90: 612f 766e 2f63 6f6e 6461 2d66 6f72 6765  a/vn/conda-forge
+00000aa0: 2f73 6369 6b69 742d 6c65 676f 2e73 7667  /scikit-lego.svg
+00000ab0: 295d 2868 7474 7073 3a2f 2f61 6e61 636f  )](https://anaco
+00000ac0: 6e64 612e 6f72 672f 636f 6e64 612d 666f  nda.org/conda-fo
+00000ad0: 7267 652f 7363 696b 6974 2d6c 6567 6f29  rge/scikit-lego)
+00000ae0: 0a21 5b5d 2868 7474 7073 3a2f 2f69 6d67  .![](https://img
+00000af0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000b00: 7562 2f6c 6963 656e 7365 2f6b 6f61 6e69  ub/license/koani
+00000b10: 6e67 2f73 6369 6b69 742d 6c65 676f 290a  ng/scikit-lego).
+00000b20: 215b 5d28 6874 7470 733a 2f2f 696d 672e  ![](https://img.
+00000b30: 7368 6965 6c64 732e 696f 2f70 7970 692f  shields.io/pypi/
+00000b40: 7079 7665 7273 696f 6e73 2f73 6369 6b69  pyversions/sciki
+00000b50: 742d 6c65 676f 290a 215b 5d28 6874 7470  t-lego).![](http
+00000b60: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b70: 696f 2f67 6974 6875 622f 636f 6e74 7269  io/github/contri
+00000b80: 6275 746f 7273 2f6b 6f61 6e69 6e67 2f73  butors/koaning/s
+00000b90: 6369 6b69 742d 6c65 676f 290a 5b21 5b52  cikit-lego).[![R
+00000ba0: 7566 665d 2868 7474 7073 3a2f 2f69 6d67  uff](https://img
+00000bb0: 2e73 6869 656c 6473 2e69 6f2f 656e 6470  .shields.io/endp
+00000bc0: 6f69 6e74 3f75 726c 3d68 7474 7073 3a2f  oint?url=https:/
+00000bd0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
+00000be0: 6f6e 7465 6e74 2e63 6f6d 2f61 7374 7261  ontent.com/astra
+00000bf0: 6c2d 7368 2f72 7566 662f 6d61 696e 2f61  l-sh/ruff/main/a
+00000c00: 7373 6574 732f 6261 6467 652f 7632 2e6a  ssets/badge/v2.j
+00000c10: 736f 6e29 5d28 6874 7470 733a 2f2f 6769  son)](https://gi
+00000c20: 7468 7562 2e63 6f6d 2f61 7374 7261 6c2d  thub.com/astral-
+00000c30: 7368 2f72 7566 6629 0a5b 215b 444f 495d  sh/ruff).[![DOI]
+00000c40: 2868 7474 7073 3a2f 2f7a 656e 6f64 6f2e  (https://zenodo.
+00000c50: 6f72 672f 6261 6467 652f 3136 3638 3336  org/badge/166836
+00000c60: 3933 392e 7376 6729 5d28 6874 7470 733a  939.svg)](https:
+00000c70: 2f2f 7a65 6e6f 646f 2e6f 7267 2f62 6164  //zenodo.org/bad
+00000c80: 6765 2f6c 6174 6573 7464 6f69 2f31 3636  ge/latestdoi/166
+00000c90: 3833 3639 3339 290a 0a23 2073 6369 6b69  836939)..# sciki
+00000ca0: 742d 6c65 676f 0a0a 3c61 2068 7265 663d  t-lego..<a href=
+00000cb0: 2268 7474 7073 3a2f 2f6b 6f61 6e69 6e67  "https://koaning
+00000cc0: 2e67 6974 6875 622e 696f 2f73 6369 6b69  .github.io/sciki
+00000cd0: 742d 6c65 676f 2f22 3e3c 696d 6720 7372  t-lego/"><img sr
+00000ce0: 633d 2269 6d61 6765 732f 6c6f 676f 2e70  c="images/logo.p
+00000cf0: 6e67 2220 7769 6474 683d 2233 3525 2220  ng" width="35%" 
+00000d00: 6865 6967 6874 3d22 3335 2522 2061 6c69  height="35%" ali
+00000d10: 676e 3d22 7269 6768 7422 202f 3e3c 2f61  gn="right" /></a
+00000d20: 3e0a 0a57 6520 6c6f 7665 2073 6369 6b69  >..We love sciki
+00000d30: 7420 6c65 6172 6e20 6275 7420 7665 7279  t learn but very
+00000d40: 206f 6674 656e 2077 6520 6669 6e64 206f   often we find o
+00000d50: 7572 7365 6c76 6573 2077 7269 7469 6e67  urselves writing
+00000d60: 0a63 7573 746f 6d20 7472 616e 7366 6f72  .custom transfor
+00000d70: 6d65 7273 2c20 6d65 7472 6963 7320 616e  mers, metrics an
+00000d80: 6420 6d6f 6465 6c73 2e20 5468 6520 676f  d models. The go
+00000d90: 616c 206f 6620 7468 6973 2070 726f 6a65  al of this proje
+00000da0: 6374 0a69 7320 746f 2061 7474 656d 7074  ct.is to attempt
+00000db0: 2074 6f20 636f 6e73 6f6c 6964 6174 6520   to consolidate 
+00000dc0: 7468 6573 6520 696e 746f 2061 2070 6163  these into a pac
+00000dd0: 6b61 6765 2074 6861 7420 6f66 6665 7273  kage that offers
+00000de0: 0a63 6f64 6520 7175 616c 6974 792f 7465  .code quality/te
+00000df0: 7374 696e 672e 2054 6869 7320 7072 6f6a  sting. This proj
+00000e00: 6563 7420 7374 6172 7465 6420 6173 2061  ect started as a
+00000e10: 2063 6f6c 6c61 626f 7261 7469 6f6e 2062   collaboration b
+00000e20: 6574 7765 656e 0a6d 756c 7469 706c 6520  etween.multiple 
+00000e30: 636f 6d70 616e 6965 7320 696e 2074 6865  companies in the
+00000e40: 204e 6574 6865 726c 616e 6473 2062 7574   Netherlands but
+00000e50: 2068 6173 2073 696e 6365 2072 6563 6569   has since recei
+00000e60: 7665 6420 636f 6e74 7269 6275 7469 6f6e  ved contribution
+00000e70: 730a 6672 6f6d 2061 726f 756e 6420 7468  s.from around th
+00000e80: 6520 676c 6f62 652e 2049 7420 7761 7320  e globe. It was 
+00000e90: 696e 6974 6961 7465 6420 6279 205b 4d61  initiated by [Ma
+00000ea0: 7474 6869 6a73 2042 726f 756e 735d 2868  tthijs Brouns](h
+00000eb0: 7474 7073 3a2f 2f77 7777 2e6d 6272 6f75  ttps://www.mbrou
+00000ec0: 6e73 2e63 6f6d 2f29 0a61 6e64 205b 5669  ns.com/).and [Vi
+00000ed0: 6e63 656e 7420 442e 2057 6172 6d65 7264  ncent D. Warmerd
+00000ee0: 616d 5d28 6874 7470 733a 2f2f 6b6f 616e  am](https://koan
+00000ef0: 696e 672e 696f 2920 6173 2061 2074 6f6f  ing.io) as a too
+00000f00: 6c20 746f 2074 6561 6368 2070 656f 706c  l to teach peopl
+00000f10: 6520 686f 770a 746f 2063 6f6e 7472 6962  e how.to contrib
+00000f20: 7574 6520 746f 206f 7065 6e20 736f 7572  ute to open sour
+00000f30: 6365 2e0a 0a4e 6f74 6520 7468 6174 2077  ce...Note that w
+00000f40: 6527 7265 206e 6f74 2066 6f72 6d61 6c6c  e're not formall
+00000f50: 7920 6166 6669 6c69 6174 6564 2077 6974  y affiliated wit
+00000f60: 6820 7468 6520 7363 696b 6974 2d6c 6561  h the scikit-lea
+00000f70: 726e 2070 726f 6a65 6374 2061 7420 616c  rn project at al
+00000f80: 6c2c 0a62 7574 2077 6520 6169 6d20 746f  l,.but we aim to
+00000f90: 2073 7472 6963 746c 7920 6164 6865 7265   strictly adhere
+00000fa0: 2074 6f20 7468 6569 7220 7374 616e 6461   to their standa
+00000fb0: 7264 732e 0a0a 5468 6520 7361 6d65 2068  rds...The same h
+00000fc0: 6f6c 6473 2077 6974 6820 6c65 676f 2e20  olds with lego. 
+00000fd0: 4c45 474f c2ae 2069 7320 6120 7472 6164  LEGO.. is a trad
+00000fe0: 656d 6172 6b20 6f66 2074 6865 204c 4547  emark of the LEG
+00000ff0: 4f20 4772 6f75 7020 6f66 2063 6f6d 7061  O Group of compa
+00001000: 6e69 6573 2077 6869 6368 2064 6f65 7320  nies which does 
+00001010: 6e6f 7420 7370 6f6e 736f 722c 2061 7574  not sponsor, aut
+00001020: 686f 7269 7a65 206f 7220 656e 646f 7273  horize or endors
+00001030: 6520 7468 6973 2070 726f 6a65 6374 2e0a  e this project..
+00001040: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00001050: 0a0a 496e 7374 616c 6c20 6073 6369 6b69  ..Install `sciki
+00001060: 742d 6c65 676f 6020 7669 6120 7069 7020  t-lego` via pip 
+00001070: 7769 7468 0a0a 6060 6062 6173 680a 7079  with..```bash.py
+00001080: 7468 6f6e 202d 6d20 7069 7020 696e 7374  thon -m pip inst
+00001090: 616c 6c20 7363 696b 6974 2d6c 6567 6f0a  all scikit-lego.
+000010a0: 6060 600a 0a56 6961 205b 636f 6e64 615d  ```..Via [conda]
+000010b0: 2868 7474 7073 3a2f 2f63 6f6e 6461 2e69  (https://conda.i
+000010c0: 6f2f 7072 6f6a 6563 7473 2f63 6f6e 6461  o/projects/conda
+000010d0: 2f65 6e2f 6c61 7465 7374 2f29 2077 6974  /en/latest/) wit
+000010e0: 680a 0a60 6060 6261 7368 0a63 6f6e 6461  h..```bash.conda
+000010f0: 2069 6e73 7461 6c6c 202d 6320 636f 6e64   install -c cond
+00001100: 612d 666f 7267 6520 7363 696b 6974 2d6c  a-forge scikit-l
+00001110: 6567 6f0a 6060 600a 0a41 6c74 6572 6e61  ego.```..Alterna
+00001120: 7469 7665 6c79 2c20 746f 2065 6469 7420  tively, to edit 
+00001130: 616e 6420 636f 6e74 7269 6275 7465 2079  and contribute y
+00001140: 6f75 2063 616e 2066 6f72 6b2f 636c 6f6e  ou can fork/clon
+00001150: 6520 616e 6420 7275 6e3a 0a0a 6060 6062  e and run:..```b
+00001160: 6173 680a 7079 7468 6f6e 202d 6d20 7069  ash.python -m pi
+00001170: 7020 696e 7374 616c 6c20 2d65 2022 2e5b  p install -e ".[
+00001180: 6465 765d 220a 7079 7468 6f6e 2073 6574  dev]".python set
+00001190: 7570 2e70 7920 6465 7665 6c6f 700a 6060  up.py develop.``
+000011a0: 600a 0a23 2320 446f 6375 6d65 6e74 6174  `..## Documentat
+000011b0: 696f 6e0a 0a54 6865 2064 6f63 756d 656e  ion..The documen
+000011c0: 7461 7469 6f6e 2063 616e 2062 6520 666f  tation can be fo
+000011d0: 756e 6420 5b68 6572 655d 2868 7474 7073  und [here](https
+000011e0: 3a2f 2f6b 6f61 6e69 6e67 2e67 6974 6875  ://koaning.githu
+000011f0: 622e 696f 2f73 6369 6b69 742d 6c65 676f  b.io/scikit-lego
+00001200: 2f29 2e0a 0a23 2320 5573 6167 650a 0a57  /)...## Usage..W
+00001210: 6520 6f66 6665 7220 6375 7374 6f6d 206d  e offer custom m
+00001220: 6574 7269 6373 2c20 6d6f 6465 6c73 2061  etrics, models a
+00001230: 6e64 2074 7261 6e73 666f 726d 6572 732e  nd transformers.
+00001240: 2059 6f75 2063 616e 2069 6d70 6f72 7420   You can import 
+00001250: 7468 656d 206a 7573 7420 6c69 6b65 2079  them just like y
+00001260: 6f75 2077 6f75 6c64 0a69 6e20 7363 696b  ou would.in scik
+00001270: 6974 2d6c 6561 726e 2e0a 0a60 6060 7079  it-learn...```py
+00001280: 7468 6f6e 0a23 2074 6865 2073 6369 6b69  thon.# the sciki
+00001290: 7420 6c65 6172 6e20 7374 7566 6620 7765  t learn stuff we
+000012a0: 206c 6f76 650a 6672 6f6d 2073 6b6c 6561   love.from sklea
+000012b0: 726e 2e70 7265 7072 6f63 6573 7369 6e67  rn.preprocessing
+000012c0: 2069 6d70 6f72 7420 5374 616e 6461 7264   import Standard
+000012d0: 5363 616c 6572 0a66 726f 6d20 736b 6c65  Scaler.from skle
+000012e0: 6172 6e2e 7069 7065 6c69 6e65 2069 6d70  arn.pipeline imp
+000012f0: 6f72 7420 5069 7065 6c69 6e65 0a0a 2320  ort Pipeline..# 
+00001300: 6672 6f6d 2073 6369 6b69 7420 6c65 676f  from scikit lego
+00001310: 2073 7475 6666 2077 6520 6164 640a 6672   stuff we add.fr
+00001320: 6f6d 2073 6b6c 6567 6f2e 7072 6570 726f  om sklego.prepro
+00001330: 6365 7373 696e 6720 696d 706f 7274 2052  cessing import R
+00001340: 616e 646f 6d41 6464 6572 0a66 726f 6d20  andomAdder.from 
+00001350: 736b 6c65 676f 2e6d 6978 7475 7265 2069  sklego.mixture i
+00001360: 6d70 6f72 7420 474d 4d43 6c61 7373 6966  mport GMMClassif
+00001370: 6965 720a 0a2e 2e2e 0a0a 6d6f 6420 3d20  ier.......mod = 
+00001380: 5069 7065 6c69 6e65 285b 0a20 2020 2028  Pipeline([.    (
+00001390: 2273 6361 6c65 222c 2053 7461 6e64 6172  "scale", Standar
+000013a0: 6453 6361 6c65 7228 2929 2c0a 2020 2020  dScaler()),.    
+000013b0: 2822 7261 6e64 6f6d 5f6e 6f69 7365 222c  ("random_noise",
+000013c0: 2052 616e 646f 6d41 6464 6572 2829 292c   RandomAdder()),
+000013d0: 0a20 2020 2028 226d 6f64 656c 222c 2047  .    ("model", G
+000013e0: 4d4d 436c 6173 7369 6669 6572 2829 290a  MMClassifier()).
+000013f0: 5d29 0a0a 2e2e 2e0a 6060 600a 0a23 2320  ])......```..## 
+00001400: 4665 6174 7572 6573 0a0a 4865 7265 2773  Features..Here's
+00001410: 2061 206c 6973 7420 6f66 2066 6561 7475   a list of featu
+00001420: 7265 7320 7468 6174 2074 6869 7320 6c69  res that this li
+00001430: 6272 6172 7920 6375 7272 656e 746c 7920  brary currently 
+00001440: 6f66 6665 7273 3a0a 0a2d 2060 736b 6c65  offers:..- `skle
+00001450: 676f 2e64 6174 6173 6574 732e 6c6f 6164  go.datasets.load
+00001460: 5f61 6261 6c6f 6e65 6020 6c6f 6164 7320  _abalone` loads 
+00001470: 696e 2074 6865 2061 6261 6c6f 6e65 2064  in the abalone d
+00001480: 6174 6173 6574 0a2d 2060 736b 6c65 676f  ataset.- `sklego
+00001490: 2e64 6174 6173 6574 732e 6c6f 6164 5f61  .datasets.load_a
+000014a0: 7272 6573 7473 6020 6c6f 6164 7320 696e  rrests` loads in
+000014b0: 2061 2064 6174 6173 6574 2077 6974 6820   a dataset with 
+000014c0: 6661 6972 6e65 7373 2063 6f6e 6365 726e  fairness concern
+000014d0: 730a 2d20 6073 6b6c 6567 6f2e 6461 7461  s.- `sklego.data
+000014e0: 7365 7473 2e6c 6f61 645f 6368 6963 6b65  sets.load_chicke
+000014f0: 6e60 206c 6f61 6473 2069 6e20 7468 6520  n` loads in the 
+00001500: 6a6f 7966 756c 2063 6869 636b 7765 6967  joyful chickweig
+00001510: 6874 2064 6174 6173 6574 0a2d 2060 736b  ht dataset.- `sk
+00001520: 6c65 676f 2e64 6174 6173 6574 732e 6c6f  lego.datasets.lo
+00001530: 6164 5f68 6572 6f65 7360 206c 6f61 6473  ad_heroes` loads
+00001540: 2061 2068 6572 6f65 7320 6f66 2074 6865   a heroes of the
+00001550: 2073 746f 726d 2064 6174 6173 6574 0a2d   storm dataset.-
+00001560: 2060 736b 6c65 676f 2e64 6174 6173 6574   `sklego.dataset
+00001570: 732e 6c6f 6164 5f68 6561 7274 7360 206c  s.load_hearts` l
+00001580: 6f61 6473 2061 2064 6174 6173 6574 2061  oads a dataset a
+00001590: 626f 7574 2068 6561 7274 730a 2d20 6073  bout hearts.- `s
+000015a0: 6b6c 6567 6f2e 6461 7461 7365 7473 2e6c  klego.datasets.l
+000015b0: 6f61 645f 7065 6e67 7569 6e73 6020 6c6f  oad_penguins` lo
+000015c0: 6164 7320 6120 6c6f 7665 6c79 2064 6174  ads a lovely dat
+000015d0: 6173 6574 2061 626f 7574 2070 656e 6775  aset about pengu
+000015e0: 696e 730a 2d20 6073 6b6c 6567 6f2e 6461  ins.- `sklego.da
+000015f0: 7461 7365 7473 2e66 6574 6368 5f63 7265  tasets.fetch_cre
+00001600: 6469 7463 6172 6460 2066 6574 6368 2061  ditcard` fetch a
+00001610: 2066 7261 7564 2064 6174 6173 6574 2066   fraud dataset f
+00001620: 726f 6d20 6f70 656e 6d6c 0a2d 2060 736b  rom openml.- `sk
+00001630: 6c65 676f 2e64 6174 6173 6574 732e 6d61  lego.datasets.ma
+00001640: 6b65 5f73 696d 706c 6573 6572 6965 7360  ke_simpleseries`
+00001650: 206d 616b 6520 6120 7369 6d75 6c61 7465   make a simulate
+00001660: 6420 7469 6d65 7365 7269 6573 0a2d 2060  d timeseries.- `
+00001670: 736b 6c65 676f 2e70 616e 6461 735f 7574  sklego.pandas_ut
+00001680: 696c 732e 6164 645f 6c61 6773 6020 6164  ils.add_lags` ad
+00001690: 6473 206c 6167 2076 616c 7565 7320 696e  ds lag values in
+000016a0: 2061 2070 616e 6461 7320 6461 7461 6672   a pandas datafr
+000016b0: 616d 650a 2d20 6073 6b6c 6567 6f2e 7061  ame.- `sklego.pa
+000016c0: 6e64 6173 5f75 7469 6c73 2e6c 6f67 5f73  ndas_utils.log_s
+000016d0: 7465 7060 2061 2075 7365 6675 6c20 6465  tep` a useful de
+000016e0: 636f 7261 746f 7220 746f 206c 6f67 2079  corator to log y
+000016f0: 6f75 7220 7069 7065 6c69 6e65 2073 7465  our pipeline ste
+00001700: 7073 0a2d 2060 736b 6c65 676f 2e64 756d  ps.- `sklego.dum
+00001710: 6d79 2e52 616e 646f 6d52 6567 7265 7373  my.RandomRegress
+00001720: 6f72 6020 6475 6d6d 7920 6265 6e63 686d  or` dummy benchm
+00001730: 6172 6b20 7468 6174 2070 7265 6469 6374  ark that predict
+00001740: 7320 7261 6e64 6f6d 2076 616c 7565 730a  s random values.
+00001750: 2d20 6073 6b6c 6567 6f2e 6c69 6e65 6172  - `sklego.linear
+00001760: 5f6d 6f64 656c 2e44 6561 645a 6f6e 6552  _model.DeadZoneR
+00001770: 6567 7265 7373 6f72 6020 6578 7065 7269  egressor` experi
+00001780: 6d65 6e74 616c 2066 6561 7475 7265 2074  mental feature t
+00001790: 6861 7420 6861 7320 6120 6465 6164 7a6f  hat has a deadzo
+000017a0: 6e65 2069 6e20 7468 6520 636f 7374 2066  ne in the cost f
+000017b0: 756e 6374 696f 6e0a 2d20 6073 6b6c 6567  unction.- `skleg
+000017c0: 6f2e 6c69 6e65 6172 5f6d 6f64 656c 2e44  o.linear_model.D
+000017d0: 656d 6f67 7261 7068 6963 5061 7269 7479  emographicParity
+000017e0: 436c 6173 7369 6669 6572 6020 6c6f 6769  Classifier` logi
+000017f0: 7374 6963 2063 6c61 7373 6966 6965 7220  stic classifier 
+00001800: 636f 6e73 7472 6169 6e65 6420 6f6e 2064  constrained on d
+00001810: 656d 6f67 7261 7068 6963 2070 6172 6974  emographic parit
+00001820: 790a 2d20 6073 6b6c 6567 6f2e 6c69 6e65  y.- `sklego.line
+00001830: 6172 5f6d 6f64 656c 2e45 7175 616c 4f70  ar_model.EqualOp
+00001840: 706f 7274 756e 6974 7943 6c61 7373 6966  portunityClassif
+00001850: 6965 7260 206c 6f67 6973 7469 6320 636c  ier` logistic cl
+00001860: 6173 7369 6669 6572 2063 6f6e 7374 7261  assifier constra
+00001870: 696e 6564 206f 6e20 6571 7561 6c20 6f70  ined on equal op
+00001880: 706f 7274 756e 6974 790a 2d20 6073 6b6c  portunity.- `skl
+00001890: 6567 6f2e 6c69 6e65 6172 5f6d 6f64 656c  ego.linear_model
+000018a0: 2e50 726f 6257 6569 6768 7452 6567 7265  .ProbWeightRegre
+000018b0: 7373 696f 6e60 206c 696e 6561 7220 6d6f  ssion` linear mo
+000018c0: 6465 6c20 7468 6174 2074 7265 6174 7320  del that treats 
+000018d0: 636f 6566 6669 6369 656e 7473 2061 7320  coefficients as 
+000018e0: 7072 6f62 6162 696c 6973 7469 6320 7765  probabilistic we
+000018f0: 6967 6874 730a 2d20 6073 6b6c 6567 6f2e  ights.- `sklego.
+00001900: 6c69 6e65 6172 5f6d 6f64 656c 2e4c 6f77  linear_model.Low
+00001910: 6573 7352 6567 7265 7373 696f 6e60 206c  essRegression` l
+00001920: 6f63 616c 6c79 2077 6569 6768 7465 6420  ocally weighted 
+00001930: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
+00001940: 6e0a 2d20 6073 6b6c 6567 6f2e 6c69 6e65  n.- `sklego.line
+00001950: 6172 5f6d 6f64 656c 2e4c 4144 5265 6772  ar_model.LADRegr
+00001960: 6573 7369 6f6e 6020 6c65 6173 7420 6162  ession` least ab
+00001970: 736f 6c75 7465 2064 6576 6961 7469 6f6e  solute deviation
+00001980: 2072 6567 7265 7373 696f 6e0a 2d20 6073   regression.- `s
+00001990: 6b6c 6567 6f2e 6c69 6e65 6172 5f6d 6f64  klego.linear_mod
+000019a0: 656c 2e51 7561 6e74 696c 6552 6567 7265  el.QuantileRegre
+000019b0: 7373 696f 6e60 206c 696e 6561 7220 7175  ssion` linear qu
+000019c0: 616e 7469 6c65 2072 6567 7265 7373 696f  antile regressio
+000019d0: 6e2c 2067 656e 6572 616c 697a 6573 204c  n, generalizes L
+000019e0: 4144 5265 6772 6573 7369 6f6e 0a2d 2060  ADRegression.- `
+000019f0: 736b 6c65 676f 2e6c 696e 6561 725f 6d6f  sklego.linear_mo
+00001a00: 6465 6c2e 496d 6261 6c61 6e63 6564 4c69  del.ImbalancedLi
+00001a10: 6e65 6172 5265 6772 6573 7369 6f6e 6020  nearRegression` 
+00001a20: 7075 6e69 7368 206f 7665 722f 756e 6465  punish over/unde
+00001a30: 722d 6573 7469 6d61 7469 6f6e 206f 6620  r-estimation of 
+00001a40: 6120 6d6f 6465 6c20 6469 7265 6374 6c79  a model directly
+00001a50: 0a2d 2060 736b 6c65 676f 2e6e 6169 7665  .- `sklego.naive
+00001a60: 5f62 6179 6573 2e47 6175 7373 6961 6e4d  _bayes.GaussianM
+00001a70: 6978 7475 7265 4e42 6020 636c 6173 7369  ixtureNB` classi
+00001a80: 6669 6573 2062 7920 7472 6169 6e69 6e67  fies by training
+00001a90: 2061 2031 4420 474d 4d20 7065 7220 636f   a 1D GMM per co
+00001aa0: 6c75 6d6e 2070 6572 2063 6c61 7373 0a2d  lumn per class.-
+00001ab0: 2060 736b 6c65 676f 2e6e 6169 7665 5f62   `sklego.naive_b
+00001ac0: 6179 6573 2e42 6179 6573 6961 6e47 6175  ayes.BayesianGau
+00001ad0: 7373 6961 6e4d 6978 7475 7265 4e42 6020  ssianMixtureNB` 
+00001ae0: 636c 6173 7369 6669 6573 2062 7920 7472  classifies by tr
+00001af0: 6169 6e69 6e67 2061 2062 6179 6573 6961  aining a bayesia
+00001b00: 6e20 3144 2047 4d4d 2070 6572 2063 6c61  n 1D GMM per cla
+00001b10: 7373 0a2d 2060 736b 6c65 676f 2e6d 6978  ss.- `sklego.mix
+00001b20: 7475 7265 2e42 6179 6573 6961 6e47 4d4d  ture.BayesianGMM
+00001b30: 436c 6173 7369 6669 6572 6020 636c 6173  Classifier` clas
+00001b40: 7369 6669 6573 2062 7920 7472 6169 6e69  sifies by traini
+00001b50: 6e67 2061 2062 6179 6573 6961 6e20 474d  ng a bayesian GM
+00001b60: 4d20 7065 7220 636c 6173 730a 2d20 6073  M per class.- `s
+00001b70: 6b6c 6567 6f2e 6d69 7874 7572 652e 4261  klego.mixture.Ba
+00001b80: 7965 7369 616e 474d 4d4f 7574 6c69 6572  yesianGMMOutlier
+00001b90: 4465 7465 6374 6f72 6020 6465 7465 6374  Detector` detect
+00001ba0: 7320 6f75 746c 6965 7273 2062 6173 6564  s outliers based
+00001bb0: 206f 6e20 6120 7472 6169 6e65 6420 6261   on a trained ba
+00001bc0: 7965 7369 616e 2047 4d4d 0a2d 2060 736b  yesian GMM.- `sk
+00001bd0: 6c65 676f 2e6d 6978 7475 7265 2e47 4d4d  lego.mixture.GMM
+00001be0: 436c 6173 7369 6669 6572 6020 636c 6173  Classifier` clas
+00001bf0: 7369 6669 6573 2062 7920 7472 6169 6e69  sifies by traini
+00001c00: 6e67 2061 2047 4d4d 2070 6572 2063 6c61  ng a GMM per cla
+00001c10: 7373 0a2d 2060 736b 6c65 676f 2e6d 6978  ss.- `sklego.mix
+00001c20: 7475 7265 2e47 4d4d 4f75 746c 6965 7244  ture.GMMOutlierD
+00001c30: 6574 6563 746f 7260 2064 6574 6563 7473  etector` detects
+00001c40: 206f 7574 6c69 6572 7320 6261 7365 6420   outliers based 
+00001c50: 6f6e 2061 2074 7261 696e 6564 2047 4d4d  on a trained GMM
+00001c60: 0a2d 2060 736b 6c65 676f 2e6d 6574 612e  .- `sklego.meta.
+00001c70: 436f 6e66 7573 696f 6e42 616c 616e 6365  ConfusionBalance
+00001c80: 7260 2065 7870 6572 696d 656e 7461 6c20  r` experimental 
+00001c90: 6665 6174 7572 6520 7468 6174 2061 6c6c  feature that all
+00001ca0: 6f77 7320 796f 7520 746f 2062 616c 616e  ows you to balan
+00001cb0: 6365 2074 6865 2063 6f6e 6675 7369 6f6e  ce the confusion
+00001cc0: 206d 6174 7269 780a 2d20 6073 6b6c 6567   matrix.- `skleg
+00001cd0: 6f2e 6d65 7461 2e44 6563 6179 4573 7469  o.meta.DecayEsti
+00001ce0: 6d61 746f 7260 2061 6464 7320 6465 6361  mator` adds deca
+00001cf0: 7920 746f 2074 6865 2073 616d 706c 655f  y to the sample_
+00001d00: 7765 6967 6874 2074 6861 7420 7468 6520  weight that the 
+00001d10: 6d6f 6465 6c20 6163 6365 7074 730a 2d20  model accepts.- 
+00001d20: 6073 6b6c 6567 6f2e 6d65 7461 2e45 7374  `sklego.meta.Est
+00001d30: 696d 6174 6f72 5472 616e 7366 6f72 6d65  imatorTransforme
+00001d40: 7260 2061 6464 7320 6120 6d6f 6465 6c20  r` adds a model 
+00001d50: 6f75 7470 7574 2061 7320 6120 6665 6174  output as a feat
+00001d60: 7572 650a 2d20 6073 6b6c 6567 6f2e 6d65  ure.- `sklego.me
+00001d70: 7461 2e4f 7574 6c69 6572 436c 6173 7369  ta.OutlierClassi
+00001d80: 6669 6572 6020 7475 726e 7320 6f75 746c  fier` turns outl
+00001d90: 6965 7220 6d6f 6465 6c73 2069 6e74 6f20  ier models into 
+00001da0: 636c 6173 7369 6669 6572 7320 666f 7220  classifiers for 
+00001db0: 6772 6964 7365 6172 6368 0a2d 2060 736b  gridsearch.- `sk
+00001dc0: 6c65 676f 2e6d 6574 612e 4772 6f75 7065  lego.meta.Groupe
+00001dd0: 6450 7265 6469 6374 6f72 6020 6361 6e20  dPredictor` can 
+00001de0: 7370 6c69 7420 7468 6520 6461 7461 2069  split the data i
+00001df0: 6e74 6f20 7275 6e73 2061 6e64 2072 756e  nto runs and run
+00001e00: 2061 206d 6f64 656c 206f 6e20 6561 6368   a model on each
+00001e10: 0a2d 2060 736b 6c65 676f 2e6d 6574 612e  .- `sklego.meta.
+00001e20: 4772 6f75 7065 6454 7261 6e73 666f 726d  GroupedTransform
+00001e30: 6572 6020 6361 6e20 7370 6c69 7420 7468  er` can split th
+00001e40: 6520 6461 7461 2069 6e74 6f20 7275 6e73  e data into runs
+00001e50: 2061 6e64 2072 756e 2061 2074 7261 6e73   and run a trans
+00001e60: 666f 726d 6572 206f 6e20 6561 6368 0a2d  former on each.-
+00001e70: 2060 736b 6c65 676f 2e6d 6574 612e 5375   `sklego.meta.Su
+00001e80: 626a 6563 7469 7665 436c 6173 7369 6669  bjectiveClassifi
+00001e90: 6572 6020 6578 7065 7269 6d65 6e74 616c  er` experimental
+00001ea0: 2066 6561 7475 7265 2074 6f20 6164 6420   feature to add 
+00001eb0: 6120 7072 696f 7220 746f 2079 6f75 7220  a prior to your 
+00001ec0: 636c 6173 7369 6669 6572 0a2d 2060 736b  classifier.- `sk
+00001ed0: 6c65 676f 2e6d 6574 612e 5468 7265 7368  lego.meta.Thresh
+00001ee0: 6f6c 6465 7260 206d 6574 6120 6d6f 6465  older` meta mode
+00001ef0: 6c20 7468 6174 2061 6c6c 6f77 7320 796f  l that allows yo
+00001f00: 7520 746f 2067 7269 6473 6561 7263 6820  u to gridsearch 
+00001f10: 6f76 6572 2074 6865 2074 6872 6573 686f  over the thresho
+00001f20: 6c64 0a2d 2060 736b 6c65 676f 2e6d 6574  ld.- `sklego.met
+00001f30: 612e 5265 6772 6573 7369 6f6e 4f75 746c  a.RegressionOutl
+00001f40: 6965 7244 6574 6563 746f 7260 206d 6574  ierDetector` met
+00001f50: 6120 6d6f 6465 6c20 7468 6174 2066 696e  a model that fin
+00001f60: 6473 206f 7574 6c69 6572 7320 6279 2061  ds outliers by a
+00001f70: 6464 696e 6720 6120 7468 7265 7368 6f6c  dding a threshol
+00001f80: 6420 746f 2072 6567 7265 7373 696f 6e0a  d to regression.
+00001f90: 2d20 6073 6b6c 6567 6f2e 6d65 7461 2e5a  - `sklego.meta.Z
+00001fa0: 6572 6f49 6e66 6c61 7465 6452 6567 7265  eroInflatedRegre
+00001fb0: 7373 6f72 6020 7072 6564 6963 7473 207a  ssor` predicts z
+00001fc0: 6572 6f20 6f72 2061 7070 6c69 6573 2061  ero or applies a
+00001fd0: 2072 6567 7265 7373 696f 6e20 6261 7365   regression base
+00001fe0: 6420 6f6e 2061 2063 6c61 7373 6966 6965  d on a classifie
+00001ff0: 720a 2d20 6073 6b6c 6567 6f2e 7072 6570  r.- `sklego.prep
+00002000: 726f 6365 7373 696e 672e 436f 6c75 6d6e  rocessing.Column
+00002010: 4361 7070 6572 6020 6c69 6d69 7473 2065  Capper` limits e
+00002020: 7874 7265 6d65 2076 616c 7565 7320 6f66  xtreme values of
+00002030: 2074 6865 206d 6f64 656c 2066 6561 7475   the model featu
+00002040: 7265 730a 2d20 6073 6b6c 6567 6f2e 7072  res.- `sklego.pr
+00002050: 6570 726f 6365 7373 696e 672e 436f 6c75  eprocessing.Colu
+00002060: 6d6e 4472 6f70 7065 7260 2064 726f 7073  mnDropper` drops
+00002070: 2061 2063 6f6c 756d 6e20 6672 6f6d 2070   a column from p
+00002080: 616e 6461 730a 2d20 6073 6b6c 6567 6f2e  andas.- `sklego.
+00002090: 7072 6570 726f 6365 7373 696e 672e 436f  preprocessing.Co
+000020a0: 6c75 6d6e 5365 6c65 6374 6f72 6020 7365  lumnSelector` se
+000020b0: 6c65 6374 7320 636f 6c75 6d6e 7320 6261  lects columns ba
+000020c0: 7365 6420 6f6e 2063 6f6c 756d 6e20 6e61  sed on column na
+000020d0: 6d65 0a2d 2060 736b 6c65 676f 2e70 7265  me.- `sklego.pre
+000020e0: 7072 6f63 6573 7369 6e67 2e49 6e66 6f72  processing.Infor
+000020f0: 6d61 7469 6f6e 4669 6c74 6572 6020 7472  mationFilter` tr
+00002100: 616e 7366 6f72 6d65 7220 7468 6174 2063  ansformer that c
+00002110: 616e 2064 652d 636f 7272 656c 6174 6520  an de-correlate 
+00002120: 6665 6174 7572 6573 0a2d 2060 736b 6c65  features.- `skle
+00002130: 676f 2e70 7265 7072 6f63 6573 7369 6e67  go.preprocessing
+00002140: 2e49 6465 6e74 6974 7954 7261 6e73 666f  .IdentityTransfo
+00002150: 726d 6572 6020 7265 7475 726e 7320 7468  rmer` returns th
+00002160: 6520 7361 6d65 2064 6174 612c 2061 6c6c  e same data, all
+00002170: 6f77 7320 666f 7220 636f 6e63 6174 656e  ows for concaten
+00002180: 6174 696e 6720 7069 7065 6c69 6e65 730a  ating pipelines.
+00002190: 2d20 6073 6b6c 6567 6f2e 7072 6570 726f  - `sklego.prepro
+000021a0: 6365 7373 696e 672e 4f72 7468 6f67 6f6e  cessing.Orthogon
+000021b0: 616c 5472 616e 7366 6f72 6d65 7260 206d  alTransformer` m
+000021c0: 616b 6573 2061 6c6c 2066 6561 7475 7265  akes all feature
+000021d0: 7320 6c69 6e65 6172 6c79 2069 6e64 6570  s linearly indep
+000021e0: 656e 6465 6e74 0a2d 2060 736b 6c65 676f  endent.- `sklego
+000021f0: 2e70 7265 7072 6f63 6573 7369 6e67 2e50  .preprocessing.P
+00002200: 616e 6461 7354 7970 6553 656c 6563 746f  andasTypeSelecto
+00002210: 7260 2073 656c 6563 7473 2063 6f6c 756d  r` selects colum
+00002220: 6e73 2062 6173 6564 206f 6e20 7061 6e64  ns based on pand
+00002230: 6173 2074 7970 650a 2d20 6073 6b6c 6567  as type.- `skleg
+00002240: 6f2e 7072 6570 726f 6365 7373 696e 672e  o.preprocessing.
+00002250: 5261 6e64 6f6d 4164 6465 7260 2061 6464  RandomAdder` add
+00002260: 7320 7261 6e64 6f6d 6e65 7373 2069 6e20  s randomness in 
+00002270: 7472 6169 6e69 6e67 0a2d 2060 736b 6c65  training.- `skle
+00002280: 676f 2e70 7265 7072 6f63 6573 7369 6e67  go.preprocessing
+00002290: 2e52 6570 6561 7469 6e67 4261 7369 7346  .RepeatingBasisF
+000022a0: 756e 6374 696f 6e60 2072 6570 6561 7469  unction` repeati
+000022b0: 6e67 2066 6561 7475 7265 2065 6e67 696e  ng feature engin
+000022c0: 6565 7269 6e67 2c20 7573 6566 756c 2066  eering, useful f
+000022d0: 6f72 2074 696d 6573 6572 6965 730a 2d20  or timeseries.- 
+000022e0: 6073 6b6c 6567 6f2e 7072 6570 726f 6365  `sklego.preproce
+000022f0: 7373 696e 672e 4469 6374 4d61 7070 6572  ssing.DictMapper
+00002300: 6020 6173 7369 676e 206e 756d 6572 6963  ` assign numeric
+00002310: 2076 616c 7565 7320 6f6e 2063 6174 6567   values on categ
+00002320: 6f72 6963 616c 2063 6f6c 756d 6e73 0a2d  orical columns.-
+00002330: 2060 736b 6c65 676f 2e70 7265 7072 6f63   `sklego.preproc
+00002340: 6573 7369 6e67 2e4f 7574 6c69 6572 5265  essing.OutlierRe
+00002350: 6d6f 7665 7260 2065 7870 6572 696d 656e  mover` experimen
+00002360: 7461 6c20 6d65 7468 6f64 2074 6f20 7265  tal method to re
+00002370: 6d6f 7665 206f 7574 6c69 6572 7320 6475  move outliers du
+00002380: 7269 6e67 2074 7261 696e 696e 670a 2d20  ring training.- 
+00002390: 6073 6b6c 6567 6f2e 6d6f 6465 6c5f 7365  `sklego.model_se
+000023a0: 6c65 6374 696f 6e2e 4772 6f75 7054 696d  lection.GroupTim
+000023b0: 6553 6572 6965 7353 706c 6974 6020 7469  eSeriesSplit` ti
+000023c0: 6d65 7365 7269 6573 204b 666f 6c64 2066  meseries Kfold f
+000023d0: 6f72 2067 726f 7570 7320 7769 7468 2064  or groups with d
+000023e0: 6966 6665 7265 6e74 2061 6d6f 756e 7420  ifferent amount 
+000023f0: 6f66 206f 6273 6572 7661 7469 6f6e 7320  of observations 
+00002400: 7065 7220 6772 6f75 700a 2d20 6073 6b6c  per group.- `skl
+00002410: 6567 6f2e 6d6f 6465 6c5f 7365 6c65 6374  ego.model_select
+00002420: 696f 6e2e 4b6c 7573 7465 7246 6f6c 6456  ion.KlusterFoldV
+00002430: 616c 6964 6174 696f 6e60 2065 7870 6572  alidation` exper
+00002440: 696d 656e 7461 6c20 6665 6174 7572 6520  imental feature 
+00002450: 7468 6174 2064 6f65 7320 4b20 666f 6c64  that does K fold
+00002460: 7320 6261 7365 6420 6f6e 2063 6c75 7374  s based on clust
+00002470: 6572 696e 670a 2d20 6073 6b6c 6567 6f2e  ering.- `sklego.
+00002480: 6d6f 6465 6c5f 7365 6c65 6374 696f 6e2e  model_selection.
+00002490: 5469 6d65 4761 7053 706c 6974 6020 7469  TimeGapSplit` ti
+000024a0: 6d65 7365 7269 6573 204b 666f 6c64 2077  meseries Kfold w
+000024b0: 6974 6820 6120 6761 7020 6265 7477 6565  ith a gap betwee
+000024c0: 6e20 7472 6169 6e2f 7465 7374 0a2d 2060  n train/test.- `
+000024d0: 736b 6c65 676f 2e70 6970 656c 696e 652e  sklego.pipeline.
+000024e0: 4465 6275 6750 6970 656c 696e 6560 2061  DebugPipeline` a
+000024f0: 6464 7320 6465 6275 6720 696e 666f 726d  dds debug inform
+00002500: 6174 696f 6e20 746f 206d 616b 6520 6465  ation to make de
+00002510: 6275 6767 696e 6720 6561 7369 6572 0a2d  bugging easier.-
+00002520: 2060 736b 6c65 676f 2e70 6970 656c 696e   `sklego.pipelin
+00002530: 652e 6d61 6b65 5f64 6562 7567 5f70 6970  e.make_debug_pip
+00002540: 656c 696e 6560 2073 686f 7274 6861 6e64  eline` shorthand
+00002550: 2066 756e 6374 696f 6e20 746f 2063 7265   function to cre
+00002560: 6174 6520 6120 6465 6275 6761 626c 6520  ate a debugable 
+00002570: 7069 7065 6c69 6e65 0a2d 2060 736b 6c65  pipeline.- `skle
+00002580: 676f 2e6d 6574 7269 6373 2e63 6f72 7265  go.metrics.corre
+00002590: 6c61 7469 6f6e 5f73 636f 7265 6020 6361  lation_score` ca
+000025a0: 6c63 756c 6174 6573 2063 6f72 7265 6c61  lculates correla
+000025b0: 7469 6f6e 2062 6574 7765 656e 206d 6f64  tion between mod
+000025c0: 656c 206f 7574 7075 7420 616e 6420 6665  el output and fe
+000025d0: 6174 7572 650a 2d20 6073 6b6c 6567 6f2e  ature.- `sklego.
+000025e0: 6d65 7472 6963 732e 6571 7561 6c5f 6f70  metrics.equal_op
+000025f0: 706f 7274 756e 6974 795f 7363 6f72 6560  portunity_score`
+00002600: 2063 616c 6375 6c61 7465 7320 6571 7561   calculates equa
+00002610: 6c20 6f70 706f 7274 756e 6974 7920 6d65  l opportunity me
+00002620: 7472 6963 0a2d 2060 736b 6c65 676f 2e6d  tric.- `sklego.m
+00002630: 6574 7269 6373 2e70 5f70 6572 6365 6e74  etrics.p_percent
+00002640: 5f73 636f 7265 6020 7072 6f78 7920 666f  _score` proxy fo
+00002650: 7220 6d6f 6465 6c20 6661 6972 6e65 7373  r model fairness
+00002660: 2077 6974 6820 7265 6761 7264 7320 746f   with regards to
+00002670: 2073 656e 7369 7469 7665 2061 7474 7269   sensitive attri
+00002680: 6275 7465 0a2d 2060 736b 6c65 676f 2e6d  bute.- `sklego.m
+00002690: 6574 7269 6373 2e73 7562 7365 745f 7363  etrics.subset_sc
+000026a0: 6f72 6560 2063 616c 6375 6c61 7465 2061  ore` calculate a
+000026b0: 2073 636f 7265 206f 6e20 6120 7375 6273   score on a subs
+000026c0: 6574 206f 6620 796f 7572 2064 6174 6120  et of your data 
+000026d0: 286d 6561 6e74 2066 6f72 2066 6169 726e  (meant for fairn
+000026e0: 6573 7320 7472 6163 6b69 6e67 290a 0a23  ess tracking)..#
+000026f0: 2320 4e65 7720 4665 6174 7572 6573 0a0a  # New Features..
+00002700: 5765 2077 616e 7420 746f 2062 6520 7261  We want to be ra
+00002710: 7468 6572 206f 7065 6e20 6865 7265 2069  ther open here i
+00002720: 6e20 7768 6174 2077 6520 6163 6365 7074  n what we accept
+00002730: 2062 7574 2077 6520 646f 2064 656d 616e   but we do deman
+00002740: 6420 7468 7265 650a 7468 696e 6773 2062  d three.things b
+00002750: 6566 6f72 6520 7468 6579 2062 6563 6f6d  efore they becom
+00002760: 6520 6164 6465 6420 746f 2074 6865 2070  e added to the p
+00002770: 726f 6a65 6374 3a0a 0a31 2e20 616e 7920  roject:..1. any 
+00002780: 6e65 7720 6665 6174 7572 6520 636f 6e74  new feature cont
+00002790: 7269 6275 7465 7320 746f 7761 7264 7320  ributes towards 
+000027a0: 6120 6465 6d6f 6e73 7472 6162 6c65 2072  a demonstrable r
+000027b0: 6561 6c2d 776f 726c 6420 7573 6563 6173  eal-world usecas
+000027c0: 650a 322e 2061 6e79 206e 6577 2066 6561  e.2. any new fea
+000027d0: 7475 7265 2070 6173 7365 7320 7374 616e  ture passes stan
+000027e0: 6461 7264 2075 6e69 7420 7465 7374 7320  dard unit tests 
+000027f0: 2877 6520 7573 6520 7468 6520 6f6e 6573  (we use the ones
+00002800: 2066 726f 6d20 7363 696b 6974 2d6c 6561   from scikit-lea
+00002810: 726e 290a 332e 2074 6865 2066 6561 7475  rn).3. the featu
+00002820: 7265 2068 6173 2062 6565 6e20 6469 7363  re has been disc
+00002830: 7573 7365 6420 696e 2074 6865 2069 7373  ussed in the iss
+00002840: 7565 206c 6973 7420 6265 666f 7265 6861  ue list beforeha
+00002850: 6e64 0a0a 5765 2061 7574 6f6d 6174 6520  nd..We automate 
+00002860: 616c 6c20 6f66 206f 7572 2074 6573 7469  all of our testi
+00002870: 6e67 2061 6e64 2075 7365 2070 7265 2d63  ng and use pre-c
+00002880: 6f6d 6d69 7420 686f 6f6b 7320 746f 206b  ommit hooks to k
+00002890: 6565 7020 7468 6520 636f 6465 2077 6f72  eep the code wor
+000028a0: 6b69 6e67 2e0a                           king..
```

### Comparing `scikit-lego-0.8.1/pyproject.toml` & `scikit-lego-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scikit-lego"
-version = "0.8.1"
+version = "0.8.2"
 description="A collection of lego bricks for scikit-learn pipelines"
 
 license = {file = "LICENSE"}
 readme = "readme.md"
 requires-python = ">=3.6"
 authors = [
     {name = "Vincent D. Warmerdam"},
```

### Comparing `scikit-lego-0.8.1/readme.md` & `scikit-lego-0.8.2/scikit_lego.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,60 @@
+Metadata-Version: 2.1
+Name: scikit-lego
+Version: 0.8.2
+Summary: A collection of lego bricks for scikit-learn pipelines
+Author: Vincent D. Warmerdam, Matthijs Brouns
+Maintainer: Francesco Bruzzesi
+License: MIT License
+        
+        Copyright (c) 2019 vincent d warmerdam 
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: repository, https://github.com/koaning/scikit-lego
+Project-URL: issue-tracker, https://github.com/koaning/scikit-lego/issues
+Project-URL: documentation, https://koaning.github.io/scikit-lego/
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: cvxpy
+Provides-Extra: formulaic
+Provides-Extra: umap
+Provides-Extra: all
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: utils
+Provides-Extra: dev
+License-File: LICENSE
+
 [![Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://www.pepy.tech/projects/scikit-lego)
 [![Version](https://img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/conda-forge/scikit-lego)
 ![](https://img.shields.io/github/license/koaning/scikit-lego)
 ![](https://img.shields.io/pypi/pyversions/scikit-lego)
 ![](https://img.shields.io/github/contributors/koaning/scikit-lego)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

#### html2text {}

```diff
@@ -1,8 +1,38 @@
-[![Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://
+Metadata-Version: 2.1 Name: scikit-lego Version: 0.8.2 Summary: A collection of
+lego bricks for scikit-learn pipelines Author: Vincent D. Warmerdam, Matthijs
+Brouns Maintainer: Francesco Bruzzesi License: MIT License Copyright (c) 2019
+vincent d warmerdam Permission is hereby granted, free of charge, to any person
+obtaining a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including without
+limitation the rights to use, copy, modify, merge, publish, distribute,
+sublicense, and/or sell copies of the Software, and to permit persons to whom
+the Software is furnished to do so, subject to the following conditions: The
+above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software. THE SOFTWARE IS PROVIDED "AS
+IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT
+LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
+AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE. Project-URL: repository,
+https://github.com/koaning/scikit-lego Project-URL: issue-tracker, https://
+github.com/koaning/scikit-lego/issues Project-URL: documentation, https://
+koaning.github.io/scikit-lego/ Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
+Content-Type: text/markdown Provides-Extra: cvxpy Provides-Extra: formulaic
+Provides-Extra: umap Provides-Extra: all Provides-Extra: docs Provides-Extra:
+test Provides-Extra: utils Provides-Extra: dev License-File: LICENSE [!
+[Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://
 www.pepy.tech/projects/scikit-lego) [![Version](https://img.shields.io/pypi/v/
 scikit-lego)](https://pypi.org/project/scikit-lego/) [![Conda Version](https://
 img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/
 conda-forge/scikit-lego) ![](https://img.shields.io/github/license/koaning/
 scikit-lego) ![](https://img.shields.io/pypi/pyversions/scikit-lego) ![](https:
 //img.shields.io/github/contributors/koaning/scikit-lego) [![Ruff](https://
 img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/
```

### Comparing `scikit-lego-0.8.1/scikit_lego.egg-info/SOURCES.txt` & `scikit-lego-0.8.2/scikit_lego.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 pyproject.toml
-readme.md
 setup.py
 scikit_lego.egg-info/PKG-INFO
 scikit_lego.egg-info/SOURCES.txt
 scikit_lego.egg-info/dependency_links.txt
 scikit_lego.egg-info/requires.txt
 scikit_lego.egg-info/top_level.txt
 sklego/__init__.py
@@ -60,10 +59,8 @@
 sklego/preprocessing/formulaictransformer.py
 sklego/preprocessing/identitytransformer.py
 sklego/preprocessing/intervalencoder.py
 sklego/preprocessing/outlier_remover.py
 sklego/preprocessing/pandastransformers.py
 sklego/preprocessing/projections.py
 sklego/preprocessing/randomadder.py
-sklego/preprocessing/repeatingbasis.py
-tests/test_datasets.py
-tests/test_notinstalled.py
+sklego/preprocessing/repeatingbasis.py
```

### Comparing `scikit-lego-0.8.1/scikit_lego.egg-info/requires.txt` & `scikit-lego-0.8.2/scikit_lego.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/base.py` & `scikit-lego-0.8.2/sklego/base.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/common.py` & `scikit-lego-0.8.2/sklego/common.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/abalone.zip` & `scikit-lego-0.8.2/sklego/data/abalone.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/arrests.zip` & `scikit-lego-0.8.2/sklego/data/arrests.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/chickweight.zip` & `scikit-lego-0.8.2/sklego/data/chickweight.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/hearts.zip` & `scikit-lego-0.8.2/sklego/data/hearts.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/heroes.zip` & `scikit-lego-0.8.2/sklego/data/heroes.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/data/penguins.zip` & `scikit-lego-0.8.2/sklego/data/penguins.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/datasets.py` & `scikit-lego-0.8.2/sklego/datasets.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/decomposition/pca_reconstruction.py` & `scikit-lego-0.8.2/sklego/decomposition/pca_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/decomposition/umap_reconstruction.py` & `scikit-lego-0.8.2/sklego/decomposition/umap_reconstruction.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/dummy.py` & `scikit-lego-0.8.2/sklego/dummy.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/feature_selection/mrmr.py` & `scikit-lego-0.8.2/sklego/feature_selection/mrmr.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/linear_model.py` & `scikit-lego-0.8.2/sklego/linear_model.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/__init__.py` & `scikit-lego-0.8.2/sklego/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/_decay_utils.py` & `scikit-lego-0.8.2/sklego/meta/_decay_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/_grouped_utils.py` & `scikit-lego-0.8.2/sklego/meta/_grouped_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/_shrinkage_utils.py` & `scikit-lego-0.8.2/sklego/meta/_shrinkage_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/confusion_balancer.py` & `scikit-lego-0.8.2/sklego/meta/confusion_balancer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/decay_estimator.py` & `scikit-lego-0.8.2/sklego/meta/decay_estimator.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/estimator_transformer.py` & `scikit-lego-0.8.2/sklego/meta/estimator_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/grouped_predictor.py` & `scikit-lego-0.8.2/sklego/meta/grouped_predictor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/grouped_transformer.py` & `scikit-lego-0.8.2/sklego/meta/grouped_transformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/hierarchical_predictor.py` & `scikit-lego-0.8.2/sklego/meta/hierarchical_predictor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/ordinal_classification.py` & `scikit-lego-0.8.2/sklego/meta/ordinal_classification.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/outlier_classifier.py` & `scikit-lego-0.8.2/sklego/meta/outlier_classifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,14 +19,38 @@
 
     Attributes
     ----------
     estimator_ : scikit-learn compatible outlier detection model
         The fitted underlying outlier detection model.
     classes_ : array-like of shape (2,)
         Classes used for prediction (0 or 1)
+
+    Example
+    -------
+    ```py
+    from sklearn.ensemble import IsolationForest
+    from sklego.meta.outlier_classifier import OutlierClassifier
+
+    X = [[0], [0.5], [-1], [99]]
+    y = [0, 0, 0, 1]
+
+    isolation_forest = IsolationForest()
+
+    outlier_clf = OutlierClassifier(isolation_forest)
+    _ = outlier_clf.fit(X, y)
+
+    preds = outlier_clf.predict([[100], [-0.5], [0.5], [1]])
+    # array[1. 0. 0. 0.]
+
+    proba_preds = outlier_clf.predict_proba([[100], [-0.5], [0.5], [1]])
+    # [[0.34946567 0.65053433]
+    #  [0.79707913 0.20292087]
+    #  [0.80275406 0.19724594]
+    #  [0.80275406 0.19724594]]
+    ```
     """
 
     def __init__(self, model):
         self.model = model
 
     def _is_outlier_model(self):
         """Check if the underlying model is an outlier detection model."""
```

### Comparing `scikit-lego-0.8.1/sklego/meta/regression_outlier_detector.py` & `scikit-lego-0.8.2/sklego/meta/regression_outlier_detector.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/subjective_classifier.py` & `scikit-lego-0.8.2/sklego/meta/subjective_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/thresholder.py` & `scikit-lego-0.8.2/sklego/meta/thresholder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/meta/zero_inflated_regressor.py` & `scikit-lego-0.8.2/sklego/meta/zero_inflated_regressor.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/metrics.py` & `scikit-lego-0.8.2/sklego/metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/mixture/bayesian_gmm_classifier.py` & `scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/mixture/bayesian_gmm_detector.py` & `scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from sklearn.utils.validation import FLOAT_DTYPES, check_array, check_is_fitted
 
 
 class BayesianGMMOutlierDetector(OutlierMixin, BaseEstimator):
     """The `BayesianGMMOutlierDetector` trains a Bayesian Gaussian Mixture model on a dataset `X`. Once a density is
     trained we can evaluate the likelihood scores to see if it is deemed likely.
 
-    By giving a threshold this model might then label outliers if their likelihood score is too low.
+    By providing a `threshold` this model might then label outliers if their likelihood score is too low.
+
+    !!! note
+        The parameters other than `threshold` and `method` are an exact copy of the parameters in
+        [sklearn.mixture.BayesianGaussianMixture]( https://scikit-learn.org/stable/modules/generated/sklearn.mixture.BayesianGaussianMixture.html).
 
     Parameters
     ----------
     threshold : float, default=0.99
         The limit at which the model thinks an outlier appears, must be between (0, 1).
     method : Literal["quantile", "stddev"], default="quantile"
         The method to use to apply the `threshold`.
@@ -24,18 +28,14 @@
         !!! info
             If you select `method="quantile"` then the threshold value represents the quantile value to start calling
             something an outlier.
 
             If you select `method="stddev"` then the threshold value represents the
             numbers of standard deviations before calling something an outlier.
 
-    !!! note
-        The other parameters are an exact copy of the parameters in
-        [sklearn.mixture.BayesianGaussianMixture]( https://scikit-learn.org/stable/modules/generated/sklearn.mixture.BayesianGaussianMixture.html).
-
     Attributes
     ----------
     gmm_ : BayesianGaussianMixture
         The trained Bayesian Gaussian Mixture Model.
     likelihood_threshold_ : float
         The threshold value used to determine if something is an outlier.
     """
```

### Comparing `scikit-lego-0.8.1/sklego/mixture/gmm_classifier.py` & `scikit-lego-0.8.2/sklego/mixture/gmm_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/mixture/gmm_outlier_detector.py` & `scikit-lego-0.8.2/sklego/mixture/gmm_outlier_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 from sklearn.utils.validation import FLOAT_DTYPES, check_array, check_is_fitted
 
 
 class GMMOutlierDetector(OutlierMixin, BaseEstimator):
     """The `GMMDetector` trains a Gaussian Mixture model on a dataset `X`. Once a density is trained we can evaluate the
     likelihood scores to see if it is deemed likely.
 
-    By giving a threshold this model might then label outliers if their likelihood score is too low.
+    By providing a `threshold` this model might then label outliers if their likelihood score is too low.
+
+    !!! note
+        The parameters other than `threshold` and `method` are an exact copy of the parameters in
+        [sklearn.mixture.GaussianMixture]( https://scikit-learn.org/stable/modules/generated/sklearn.mixture.GaussianMixture.html).
 
     Parameters
     ----------
     threshold : float, default=0.99
         The limit at which the model thinks an outlier appears, must be between (0, 1).
     method : Literal["quantile", "stddev"], default="quantile"
         The method to use to apply the `threshold`.
@@ -24,18 +28,14 @@
         !!! info
             If you select `method="quantile"` then the threshold value represents the quantile value to start calling
             something an outlier.
 
             If you select `method="stddev"` then the threshold value represents the
             numbers of standard deviations before calling something an outlier.
 
-    !!! note
-        The other parameters are an exact copy of the parameters in
-        [sklearn.mixture.GaussianMixture]( https://scikit-learn.org/stable/modules/generated/sklearn.mixture.GaussianMixture.html).
-
     Attributes
     ----------
     gmm_ : GaussianMixture
         The trained Gaussian Mixture model.
     likelihood_threshold_ : float
         The threshold value used to determine if something is an outlier.
     """
```

### Comparing `scikit-lego-0.8.1/sklego/model_selection.py` & `scikit-lego-0.8.2/sklego/model_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,16 +244,28 @@
             summary = get_split_info(X, i[0], j, "train", summary)
             summary = get_split_info(X, i[1], j, "valid", summary)
             j = j + 1
 
         return pd.DataFrame(summary)
 
 
-class KlusterFoldValidation:
-    """KlusterFold cross validator. Create folds based on provided cluster method
+def KlusterFoldValidation(**kwargs):
+    warn(
+        "Please use `ClusterFoldValidation` instead of `KlusterFoldValidation`."
+        "We will use correct spelling going forward and `KlusterFoldValidation` will be deprecated.",
+        DeprecationWarning,
+    )
+    return ClusterFoldValidation(**kwargs)
+
+
+class ClusterFoldValidation:
+    """Cross validator that creates folds based on provided cluster method.
+    This ensures that data points in the same cluster are not split across different folds.
+
+    !!! info "New in version 0.8.2"
 
     Parameters
     ----------
     cluster_method : Clusterer
         Clustering method to use for the fold validation.
     """
```

### Comparing `scikit-lego-0.8.1/sklego/naive_bayes.py` & `scikit-lego-0.8.2/sklego/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/neighbors.py` & `scikit-lego-0.8.2/sklego/neighbors.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/notinstalled.py` & `scikit-lego-0.8.2/sklego/notinstalled.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/pandas_utils.py` & `scikit-lego-0.8.2/sklego/pandas_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,16 @@
         Functions that take the output of the decorated function and turn it into a log.
         Note that the output of each log_function is casted to string using `str()`.
     print_fn: Callable, default=print
         Print function (e.g. `print` or `logger.info`).
     **log_func_kwargs: dict
         Keyword arguments to be passed to `log_functions`
 
-    Returns:
+    Returns
+    -------
     Callable
         The decorated function.
 
     Examples
     --------
     ```py
     @log_step_extra(lambda d: d["some_column"].value_counts())
```

### Comparing `scikit-lego-0.8.1/sklego/pipeline.py` & `scikit-lego-0.8.2/sklego/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 from sklearn.pipeline import Pipeline, _name_estimators
 from sklearn.utils.validation import check_memory
 
 
 def default_log_callback(output, execution_time, **kwargs):
     """The default log callback which logs the step name, shape of the output and the execution time of the step.
 
-    Parameters
-    ----------
-    output : tuple[np.ndarray | pd.DataFrame, estimator | transformer]
-        The output of the step and a step in the pipeline.
-    execution_time : float
-        The execution time of the step.
-
     !!! info
 
         If you write your custom callback function the input is:
 
         | Parameter        | Type             | Description                    |
         | ---------------- | ---------------- | ------------------------------ |
         | `func`           | Callable[..., T] | The function to be wrapped     |
         | `input_args`     | tuple            | The input arguments            |
         | `input_kwargs`   | dict             | The input key-word arguments   |
         | `output`         | T                | The output of the function     |
         | `execution_time` | float            | The execution time of the step |
 
+    Parameters
+    ----------
+    output : tuple[np.ndarray | pd.DataFrame, estimator | transformer]
+        The output of the step and a step in the pipeline.
+    execution_time : float
+        The execution time of the step.
     """
     logger = logging.getLogger(__name__)
     step_result, step = output
     logger.info(f"[{step}] shape={step_result.shape} " f"time={int(execution_time)}s")
 
 
 def _log_wrapper(log_callback=default_log_callback):
@@ -93,26 +92,19 @@
 
     return _
 
 
 class DebugPipeline(Pipeline):
     """A pipeline that has a log statement in between each step, useful for debugging purposes.
 
-    Parameters
-    ----------
-    log_callback : Callable | None, default=None
-        The callback function that logs information in between each intermediate step.
-        If set to `"default"`, `default_log_callback` is used.
-
-    Notes
-    -----
     See [`sklearn.pipeline.Pipeline`](https://scikit-learn.org/stable/modules/generated/sklearn.pipeline.Pipeline.html#sklearn.pipeline.Pipeline)
-    for all other variables.
+    for all other parameters other than `log_callback`.
 
     !!! note
+
         This implementation is a hack on the original sklearn Pipeline. It aims to have the same behaviour as the
         original sklearn Pipeline, while changing minimal amount of code.
 
         The log statement is added by overwriting the cache method of the memory, such that the function called in the
         cache is wrapped with a functions that calls the log callback function (`log_callback`).
 
         This hack will break when:
@@ -120,14 +112,19 @@
         - The sklearn pipeline initialization function is changed.
         - The memory is used differently in the fit.
         - The [`joblib.memory.Memory`](https://joblib.readthedocs.io/en/latest/generated/joblib.Memory.html)
             changes behaviour of the `cache` method.
         - The [`joblib.memory.Memory`](https://joblib.readthedocs.io/en/latest/generated/joblib.Memory.html)
             starts using a `_cache` method.
 
+    Parameters
+    ----------
+    log_callback : Callable | None, default=None
+        The callback function that logs information in between each intermediate step.
+        If set to `"default"`, `default_log_callback` is used.
 
     Examples
     --------
     ```py
     # Set-up for example
     import logging
     import sys
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/__init__.py` & `scikit-lego-0.8.2/sklego/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/columncapper.py` & `scikit-lego-0.8.2/sklego/preprocessing/columncapper.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/dictmapper.py` & `scikit-lego-0.8.2/sklego/preprocessing/dictmapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,42 @@
 
     Attributes
     ----------
     n_features_in_ : int
         Number of features seen during `fit`.
     dim_ : int
         Deprecated, please use `n_features_in_` instead.
+
+    Examples
+    --------
+    ```py
+    import pandas as pd
+    from sklego.preprocessing.dictmapper import DictMapper
+    from sklearn.compose import ColumnTransformer
+
+    X = pd.DataFrame({
+        "city_pop": ["Amsterdam", "Leiden", "Utrecht", "None", "Haarlem"]
+    })
+
+    mapper = {
+        "Amsterdam": 1_181_817,
+        "Leiden": 130_181,
+        "Utrecht": 367_984,
+        "Haarlem": 165_396,
+    }
+
+    ct = ColumnTransformer([("dictmapper", DictMapper(mapper, 0), ["city_pop"])])
+    X_trans = ct.fit_transform(X)
+    X_trans
+    # array([[1181817],
+    #        [ 130181],
+    #        [ 367984],
+    #        [      0],
+    #        [ 165396]])
+    ```
     """
 
     def __init__(self, mapper, default):
         self.mapper = mapper
         self.default = default
 
     def fit(self, X, y=None):
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/formulaictransformer.py` & `scikit-lego-0.8.2/sklego/preprocessing/identitytransformer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,104 +1,105 @@
-try:
-    import formulaic
-except ImportError:
-    from sklego.notinstalled import NotInstalledPackage
-
-    formulaic = NotInstalledPackage("formulaic")
-
 from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
 
-class FormulaicTransformer(TransformerMixin, BaseEstimator):
-    """The `FormulaicTransformer` offers a method to select the right columns from a dataframe as well as a DSL for
-    transformations.
+class IdentityTransformer(BaseEstimator, TransformerMixin):
+    """The `IdentityTransformer` returns what it is fed. Does not apply any transformation.
 
-    It is inspired from R formulas. This is can be useful as a first step in the pipeline.
+    The reason for having it is because you can build more expressive pipelines.
 
     Parameters
     ----------
-    formula : str
-        A formulaic-compatible formula.
-        Refer to the [formulaic documentation](https://matthewwardrop.github.io/formulaic/guides/grammar/) for more
-            details.
-    return_type : Literal["pandas", "numpy", "sparse"], default="numpy"
-        The type of the returned matrix.
-        Refer to the [formulaic documentation](https://matthewwardrop.github.io/formulaic/guides/model_specs/) for more
-            details.
+    check_X : bool, default=False
+        Whether to validate `X` to be non-empty 2D array of finite values and attempt to cast `X` to float.
+        If disabled, the model/pipeline is expected to handle e.g. missing, non-numeric, or non-finite values.
 
     Attributes
     ----------
-    formula_ : formulaic.Formula
-        The parsed formula specification.
-    model_spec_ : formulaic.ModelSpec
-        The parsed model specification.
+    n_samples_ : int
+        The number of samples seen during `fit`.
     n_features_in_ : int
-        Number of features seen during `fit`.
+        The number of features seen during `fit`.
+    shape_ : tuple[int, int]
+        Deprecated, please use `n_samples_` and `n_features_in_` instead.
+
+    Examples
+    --------
+    ```py
+    import pandas as pd
+    from sklego.preprocessing import IdentityTransformer
+
+    df = pd.DataFrame({
+        "name": ["Swen", "Victor", "Alex"],
+        "length": [1.82, 1.85, 1.80],
+        "shoesize": [42, 44, 45]
+    })
+
+    IdentityTransformer().fit_transform(df)
+    #	name	length	shoesize
+    # 0	Swen	1.82	42
+    # 1	Victor	1.85	44
+    # 2	Alex	1.80	45
+
+    #using check_X=True to validate `X` to be non-empty 2D array of finite values and attempt to cast `X` to float
+    IdentityTransformer(check_X=True).fit_transform(df.drop(columns="name"))
+    # array([[ 1.82, 42.  ],
+    #        [ 1.85, 44.  ],
+    #        [ 1.8 , 45.  ]])
+    ```
     """
 
-    def __init__(self, formula, return_type="numpy"):
-        self.formula = formula
-        self.return_type = return_type
+    def __init__(self, check_X: bool = False):
+        self.check_X = check_X
 
     def fit(self, X, y=None):
-        """Fit the `FormulaicTransformer` to the data by compiling the formula specification into a model spec.
+        """Check the input data if `check_X` is enabled and and records its shape.
 
         Parameters
         ----------
-        X : pd.DataFrame of (n_samples, n_features)
-            The data used to compile model spec.
+        X : array-like of shape (n_samples, n_features)
+            The data to fit.
         y : array-like of shape (n_samples,), default=None
             Ignored, present for compatibility.
 
         Returns
         -------
-        self : FormulaicTransformer
+        self : IdentityTransformer
             The fitted transformer.
-
-        Raises
-        ------
-        ValueError
-            If `formula` is not supported.
         """
-        self.formula_ = formulaic.Formula.from_spec(self.formula)
-
-        if self.formula_._has_structure:
-            raise ValueError(
-                f"Formula specification {repr(self.formula_)} results in a structured formula, which is not supported."
-            )
-
-        self.model_spec_ = self.formula_.get_model_matrix(X, output=self.return_type).model_spec
-        self.n_features_in_ = X.shape[1]
+        if self.check_X:
+            X = check_array(X, copy=True, estimator=self)
+        self.n_samples_, self.n_features_in_ = X.shape
         return self
 
-    def transform(self, X, y=None):
-        """Transform `X` by generating a model matrix from it based on the fit model spec.
+    def transform(self, X):
+        """Performs identity "transformation" on `X` - which is no transformation at all.
 
         Parameters
         ----------
-        X : pd.DataFrame of shape (n_samples, n_features)
-            The data for transformation will be applied.
-        y: array-like of shape (n_samples,), default=None
-            Ignored, present for compatibility.
+        X : array-like of shape (n_samples, n_features)
+            Input data.
 
         Returns
         -------
-        X : array-like of shape (n_samples, n_features), and type `return_type`
-            Transformed data.
+        array-like of shape (n_samples, n_features)
+            Unchanged input data.
 
         Raises
         ------
         ValueError
             If the number of columns from `X` differs from the number of columns when fitting.
         """
-
-        check_is_fitted(self, ["formula_", "model_spec_", "n_features_in_"])
-
+        if self.check_X:
+            X = check_array(X, copy=True, estimator=self)
+        check_is_fitted(self, "n_features_in_")
         if X.shape[1] != self.n_features_in_:
             raise ValueError(
-                "`X` must have the same number of columns in fit and transform. "
-                f"Expected {self.n_features_in_}, found {X.shape[1]}."
+                f"Wrong shape is passed to transform. Trained on {self.n_features_in_} cols got {X.shape[1]}"
             )
+        return X
 
-        X_ = self.model_spec_.get_model_matrix(X)
-        return X_
+    @property
+    def shape_(self):
+        """Returns the shape of the estimator."""
+        return (self.n_samples_, self.n_features_in_)
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/intervalencoder.py` & `scikit-lego-0.8.2/sklego/preprocessing/intervalencoder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/outlier_remover.py` & `scikit-lego-0.8.2/sklego/preprocessing/outlier_remover.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,44 @@
 
 class OutlierRemover(TrainOnlyTransformerMixin, BaseEstimator):
     """The `OutlierRemover` transformer removes outliers (train-time only) using the supplied removal model. The
     removal model should implement `.fit()` and `.predict()` methods.
 
     Parameters
     ----------
-    outlier_detector : object
+    outlier_detector : scikit-learn compatible estimator
         An outlier detector that implements `.fit()` and `.predict()` methods.
     refit : bool, default=True
-        If True, fits the estimator during `pipeline.fit()`. If False, the estimator is not fitted during
-        `pipeline.fit()`.
+        Whether or not to fit the underlying estimator during `OutlierRemover(...).fit()`.
 
     Attributes
     ----------
     estimator_ : object
         The fitted outlier detector.
+
+    Examples
+    --------
+    ```py
+    import numpy as np
+
+    from sklearn.ensemble import IsolationForest
+    from sklego.preprocessing import OutlierRemover
+
+    np.random.seed(0)
+    X = np.random.randn(10000, 2)
+
+    isolation_forest = IsolationForest()
+    isolation_forest.fit(X)
+    detector_preds = isolation_forest.predict(X)
+
+    outlier_remover = OutlierRemover(isolation_forest, refit=True)
+    outlier_remover.fit(X)
+
+    X_trans = outlier_remover.transform_train(X)
+    ```
     """
 
     def __init__(self, outlier_detector, refit=True):
         self.outlier_detector = outlier_detector
         self.refit = refit
         self.estimator_ = None
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/pandastransformers.py` & `scikit-lego-0.8.2/sklego/preprocessing/pandastransformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,41 @@
         The names of the features to keep during transform.
     X_dtypes_ : pd.Series
         The dtypes of the columns in the input DataFrame.
 
     !!! warning
 
         Raises a `TypeError` if input provided is not a DataFrame.
+
+    Examples
+    --------
+    ```py
+    import pandas as pd
+    from sklego.preprocessing import PandasTypeSelector
+
+    df = pd.DataFrame({
+        "name": ["Swen", "Victor", "Alex"],
+        "length": [1.82, 1.85, 1.80],
+        "shoesize": [42, 44, 45]
+    })
+
+    #Excluding single column
+    PandasTypeSelector(exclude="int64").fit_transform(df)
+    #	name	length
+    #0	Swen	1.82
+    #1	Victor	1.85
+    #2	Alex	1.80
+
+    #Including multiple columns
+    PandasTypeSelector(include=["int64", "object"]).fit_transform(df)
+    #	name	shoesize
+    #0	Swen	42
+    #1	Victor	44
+    #2	Alex	45
+    ```
     """
 
     def __init__(self, include=None, exclude=None):
         self.include = include
         self.exclude = exclude
 
     def fit(self, X, y=None):
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/projections.py` & `scikit-lego-0.8.2/sklego/preprocessing/projections.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,14 +151,32 @@
 
     Attributes
     ----------
     projection_ : array-like of shape (n_features, n_features)
         The projection matrix that can be used to filter information out of a dataset.
     col_ids_ : List[int] of length `len(columns)`
         The list of column ids of the sensitive columns.
+
+    Examples
+    --------
+    ```py
+    import pandas as pd
+    from sklego.preprocessing import InformationFilter
+
+    df = pd.DataFrame({
+        "user_id": [101, 102, 103],
+        "length": [1.82, 1.85, 1.80],
+        "age": [21, 37, 45]
+    })
+
+    InformationFilter(columns=["length", "age"], alpha=0.5).fit_transform(df)
+    # array([[50.10152483,  3.87905643],
+    #        [50.26253897, 19.59684308],
+    #        [52.66084873, 28.06719867]])
+    ```
     """
 
     def __init__(self, columns, alpha=1):
         self.columns = columns
         self.alpha = alpha
 
     def _check_coltype(self, X):
```

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/randomadder.py` & `scikit-lego-0.8.2/sklego/preprocessing/randomadder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.1/sklego/preprocessing/repeatingbasis.py` & `scikit-lego-0.8.2/sklego/preprocessing/repeatingbasis.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,30 @@
     width : float, default=1.0.
         Determines the width of the radial basis functions.
 
     Attributes
     ----------
     pipeline_ : ColumnTransformer
         Fitted `ColumnTransformer` object used to transform data with repeating basis functions.
+
+    Examples
+    --------
+    ```py
+    import pandas as pd
+    from sklego.preprocessing import RepeatingBasisFunction
+
+    df = pd.DataFrame({
+        "user_id": [101, 102, 103],
+        "created_day": [5, 1, 7]
+    })
+    RepeatingBasisFunction(column="created_day", input_range=(1,7)).fit_transform(df)
+    # array([[0.06217652, 0.00432024, 0.16901332, 0.89483932, 0.64118039],
+    #        [1.        , 0.36787944, 0.01831564, 0.01831564, 0.36787944],
+    #        [1.        , 0.36787944, 0.01831564, 0.01831564, 0.36787944]])
+    ```
     """
 
     def __init__(self, column=0, remainder="drop", n_periods=12, input_range=None, width=1.0):
         self.column = column
         self.remainder = remainder
         self.n_periods = n_periods
         self.input_range = input_range
```

### Comparing `scikit-lego-0.8.1/sklego/testing.py` & `scikit-lego-0.8.2/sklego/testing.py`

 * *Files identical despite different names*

