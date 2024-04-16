# Comparing `tmp/ProQuo-1.1.0.tar.gz` & `tmp/proquo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProQuo-1.1.0.tar", last modified: Tue Apr  9 11:40:04 2024, max compression
+gzip compressed data, was "proquo-1.1.1.tar", last modified: Tue Apr 16 08:27:38 2024, max compression
```

## Comparing `ProQuo-1.1.0.tar` & `proquo-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-09 10:43:28.000000 ProQuo-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    20157 2024-04-09 11:40:04.046290 ProQuo-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/ProQuo.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20157 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1697 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-09 11:40:04.000000 ProQuo-1.1.0/ProQuo.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     6201 2024-04-09 10:43:28.000000 ProQuo-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/cli/
--rw-rw-rw-   0 root         (0) root         (0)     1663 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/Helper.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/OptionValueCheckAction.py
--rw-rw-rw-   0 root         (0) root         (0)    27538 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/ProQuoCLI.py
--rw-rw-rw-   0 root         (0) root         (0)    16699 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/cli/ProQuoLmCLI.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/core/
--rw-rw-rw-   0 root         (0) root         (0)     9749 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Helper.py
--rw-rw-rw-   0 root         (0) root         (0)    38350 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/ProQuo.py
--rw-rw-rw-   0 root         (0) root         (0)    11983 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/ProQuoLm.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Quote.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/QuoteRef.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/core/Reference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.038290 ProQuo-1.1.0/proquo/match/
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/match/MatchRef.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/match/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/linking/
--rw-rw-rw-   0 root         (0) root         (0)     2435 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/linking/LinkingModelTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1788 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/linking/LinkingVectorizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/reference/
--rw-rw-rw-   0 root         (0) root         (0)     4868 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/reference/ReferenceModelTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1535 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/reference/ReferenceVectorizer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/model/relation/
--rw-rw-rw-   0 root         (0) root         (0)     2905 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationModelBertTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationModelLstmTrainer.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationVectorizerBert.py
--rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/model/relation/RelationVectorizerLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/model/relation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/linking/
--rw-rw-rw-   0 root         (0) root         (0)     2160 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/linking/TestLinking.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.042290 ProQuo-1.1.0/proquo/testing/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/reference/TestReference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/testing/relation/
--rw-rw-rw-   0 root         (0) root         (0)     1850 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/relation/TestRelationBert.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/testing/relation/TestRelationLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/testing/relation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/linking/
--rw-rw-rw-   0 root         (0) root         (0)     1916 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/linking/TrainLinking.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/linking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/reference/
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/reference/TrainReference.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/reference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-09 11:40:04.046290 ProQuo-1.1.0/proquo/training/relation/
--rw-rw-rw-   0 root         (0) root         (0)     1494 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/relation/TrainRelationBert.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-09 10:43:28.000000 ProQuo-1.1.0/proquo/training/relation/TrainRelationLstm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-09 11:38:48.000000 ProQuo-1.1.0/proquo/training/relation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2024-04-09 10:43:28.000000 ProQuo-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-09 11:40:04.046290 ProQuo-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-04-16 08:17:11.000000 proquo-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    26278 2024-04-16 08:27:38.749500 proquo-1.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/ProQuo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26278 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1697 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-16 08:27:38.000000 proquo-1.1.1/ProQuo.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    12322 2024-04-16 08:17:11.000000 proquo-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.741500 proquo-1.1.1/proquo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/cli/
+-rw-rw-rw-   0 root         (0) root         (0)     1663 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/cli/Helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/cli/OptionValueCheckAction.py
+-rw-rw-rw-   0 root         (0) root         (0)    27538 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/cli/ProQuoCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)    16798 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/cli/ProQuoLmCLI.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/Helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    38350 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/ProQuo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11983 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/ProQuoLm.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/Quote.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/QuoteRef.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/core/Reference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/match/
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/match/MatchRef.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/match/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/model/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/linking/LinkingModelTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/linking/LinkingVectorizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/model/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/model/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/reference/ReferenceModelTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/reference/ReferenceVectorizer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/model/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/model/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     2905 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/relation/RelationModelBertTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/relation/RelationModelLstmTrainer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/relation/RelationVectorizerBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/model/relation/RelationVectorizerLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/model/relation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/testing/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     2160 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/testing/linking/TestLinking.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/testing/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.745500 proquo-1.1.1/proquo/testing/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/testing/reference/TestReference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/testing/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/proquo/testing/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/testing/relation/TestRelationBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/testing/relation/TestRelationLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/testing/relation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/proquo/training/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/training/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/proquo/training/linking/
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/training/linking/TrainLinking.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/training/linking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/proquo/training/reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/training/reference/TrainReference.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/training/reference/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 08:27:38.749500 proquo-1.1.1/proquo/training/relation/
+-rw-rw-rw-   0 root         (0) root         (0)     1494 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/training/relation/TrainRelationBert.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-16 08:17:11.000000 proquo-1.1.1/proquo/training/relation/TrainRelationLstm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-16 08:27:11.000000 proquo-1.1.1/proquo/training/relation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2024-04-16 08:17:11.000000 proquo-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 08:27:38.749500 proquo-1.1.1/setup.cfg
```

### Comparing `ProQuo-1.1.0/LICENSE` & `proquo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/PKG-INFO` & `proquo-1.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProQuo
-Version: 1.1.0
+Version: 1.1.1
 Summary: ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,210 +217,267 @@
 Requires-Dist: kpcommons~=0.0.2
 Requires-Dist: transformers~=4.39.3
 Requires-Dist: torch~=2.2.2
 Requires-Dist: scikit-learn~=1.2.1
 Requires-Dist: keras-preprocessing~=1.1.2
 
 # Readme
-`ProQuo` and `ProQuoLM` are a tools for the detection of short quotations (<= 4 words) between two texts, a source text and
-a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly
-marked with quotations marks. For more information, see below.
-
-## Overview
-The main purpose of this tool is to use the pretrained models for the detection of short quotations.
-Both approaches, `ProQuo` and `ProQuoLM` are separate. In our evaluation (see citation below) we found both approaches
-to perform at the same level while `ProQuoLm` is less complex as it is mainly a fine-tuned language model.
-The library also supports training and testing of custom models for reference classification, relation classification
-and linking classification.
+This repository contains two tools, `ProQuo` and `ProQuoLM`. Both are tools for the detection of short quotations
+(<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text.
+Quotations in the target text need to be marked with quotations marks. For more information, see below.
+
+The main purpose of this tool is to use the pretrained models for the detection of short quotations. While we found both
+approaches (`ProQuo` and `ProQuoLM`) to perform at the same level (for details, see our [publication](https://jcls.io/article/id/3590/)),
+`ProQuoLm` is easier to use, better maintained and the **recommended approach**.
 
-**Note**: `ProQuoLM` is easier to use, faster, better documented, better maintained, better tested and the recommended
-approach to use.
-
-## Quotation marks
-By default, the 'best', i.e. most common combination of opening and closing quotation mark in the specific text is used.
+## Quotation Marks
+By default, the "best", that is, most common, combination of opening and closing quotation mark in the specific text is used.
 The following combinations are automatically tried:
 
 1. " and "
 2. „ and “
 3. „ and "
 4. “ and “
 5. » and «
 6. « and »
 7. ‘ and ’
 
-If this is not the desired behaviour, quotations marks can be manually defined, using the command line options
-`--open-quote` and `--close-quote` to define which opening and closing quotation marks to use.
+If this is not the desired behaviour, quotations marks can be manually defined using the command line options
+`--open-quote` and `--close-quote`.
 
-## Pretrained models and training data
+## Approaches Overview
+`ProQuo` is a specialized pipeline which uses a [model for reference classification](proquo/model/reference/ReferenceModelTrainer.py)
+and a [model for relation extraction](proquo/model/relation/RelationModelBertTrainer.py) between quotations and (page)
+references to distinguish between relevant quotations (that is, quotations from the source text) and quotations
+from other sources. In a third step, a rule-based algorithm is used to link the identified quotations to their source.
 
-The pretrained models and training data are made available and can be downloaded from [here](https://scm.cms.hu-berlin.de/schluesselstellen/proquodata).
+`ProQuoLM` uses a [fine-tuned BERT model](https://huggingface.co/Fredr0id/proquolm) in two ways: to distinguish between
+relevant quotations and quotations from other sources and to link the quotations to their source.
 
+## Pretrained Models and Training Data
+The pretrained models and training data are made available and can be downloaded from [here](https://scm.cms.hu-berlin.de/schluesselstellen/proquodata).
 For `ProQuoLm`, we also provide a model on [Hugging Face](https://huggingface.co/Fredr0id/proquolm). This is used by default.
 
 ## Installation
 
 ### From PyPi
-
 **Note**: Both tools are part of the same PyPi package. So the following command installs both.
 
 ~~~
 pip install ProQuo
 ~~~
 
-### From source
+### From Source
 Checkout this repository and then run:
 
 ~~~
 python -m pip install .
 ~~~
 
-This installs `ProQuo` and all dependencies except `tensorflow` which needs to be installed manually depending on
-the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was
-tested is 2.14.1.
+### Dependencies
+Both installation methods install all dependencies except `tensorflow` which needs to be installed manually depending on
+the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was tested is 2.14.1.
 
 For `RelationModelLstmTrainer`, `tensorflow-text` is needed. `RelationModelLstmTrainer` should normally not be needed as
 `RelationModelBertTrainer` performs better and is the default in the pipeline.
 
 ## Usage
-There are two ways to use the tool: in code and from the command line. Both are described in the following sections.
+The following sections describe how to use ProQuo on the command line.
 
 ### Quotation detection
-There are two approaches which can be used for quotation detection: A specialized pipeline and a general language model based approach.
-To run the (recommended) language model approach with the default model, use the following command:
+To run `ProQuoLM` with the default model, use the following command:
 
 ~~~
-proquolm compare
-path_to_source_text
-path_to_target_text
---text
---output-type text
+proquolm compare path_to_source_text path_to_target_text --text --output-type text
+~~~
+
+<details>
+<summary>All ProQuoLM command line options</summary>
+
 ~~~
+usage: proquolm compare [-h] [--tokenizer TOKENIZER] [--model MODEL]
+                        [--lower-case | --no-lower-case]
+                        [--output-folder-path OUTPUT_FOLDER_PATH]
+                        [--create-dated-subfolder | --no-create-dated-subfolder]
+                        [--text | --no-text] [--output-type {json,text,csv}]
+                        [--csv-sep CSV_SEP] [--open-quote OPEN_QUOTE]
+                        [--close-quote CLOSE_QUOTE]
+                        [--include-long-matches-in-result]
+                        [--max-num-processes MAX_NUM_PROCESSES]
+                        source-file-path target-path
+
+ProQuoLm compare allows the user to find short quotations (<= 4 words) in two
+texts, a source text and a target text. The target text is the text quoting
+the source text. Quotations in the target text need to be clearly marked with
+quotations marks.
+
+positional arguments:
+  source-file-path      Path to the source text file
+  target-path           Path to the target text file or folder
+
+options:
+  -h, --help            show this help message and exit
+  --tokenizer TOKENIZER
+                        Name of the tokenizer to load from Hugging Face or
+                        path to the tokenizer folder
+  --model MODEL         Name of the model to load from Hugging Face or path to
+                        the model folder
+  --lower-case, --no-lower-case
+                        Run model inference on lower case text (default: True)
+  --output-folder-path OUTPUT_FOLDER_PATH
+                        The output folder path. If this option is set the
+                        output will be saved to a file created in the
+                        specified folder
+  --create-dated-subfolder, --no-create-dated-subfolder
+                        Create a subfolder named with the current date to
+                        store the results (default: False)
+  --text, --no-text     Include matched text in the returned data structure
+                        (default: True)
+  --output-type {json,text,csv}
+                        The output type
+  --csv-sep CSV_SEP     output separator for csv (default: '\t')
+  --open-quote OPEN_QUOTE
+                        The quotation open character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --close-quote CLOSE_QUOTE
+                        The quotation close character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --include-long-matches-in-result
+                        Include matches longer than 4 words in the output
+  --max-num-processes MAX_NUM_PROCESSES
+                        Maximum number of processes to use for parallel
+                        processing. This can significantly speed up the
+                        process.
+~~~
+
+</details>
 
-To run the specialized pipeline, use the following command:
+To run `ProQuo`, use the following command:
 
 ~~~
-proquo compare
-path_to_source_text
-path_to_target_text
+proquo compare path_to_source_text path_to_target_text
 path_to_the_reference_vocab_file
 path_to_the_reference_model_file
 path_to_the_relation_tokenizer_folder
 path_to_the_relation_model_folder
 --text
 --output-type text
 ~~~
 
 `--output-type text` prints the results to the command line. To save the results to a file, use `--output-type csv` or
 `--output-type json`. `--text` includes the quotation text in the output.
 
 The output will look something like this:
+
 ~~~
-10	15	500	505	quote	quote
+10      15	    500	505	quote	quote
 1000	1016	20	36	some other quote	some other quote
 ~~~
+
 The first two numbers are the character start and end positions in the source text and the other two numbers are the
 character start and end positions in the target text.
 
-#### Note
-There are a number of command line arguments to configure the output format, for example, to save the result to a csv
-file. For all options, use the following commands:
-
-~~~
-proquo compare -h
-~~~
-
-~~~
-proquolm compare -h
-~~~
-
-### Training and testing a model
-
-#### Reference model
-The following command can be used to train a reference model:
-
-~~~
-proquo train reference
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of two strings and a class,
-tab separated, for example:
-
-~~~
-S. 47   S. 35	1
-63	DKV III, 17	0
-~~~
-
-To test the model, run:
-
-~~~
-proquo test reference
-path_to_test_set.txt
-path_to_the_reference_vocab_file
-path_to_the_reference_model_file
-~~~
-
-#### Relation model
-The following command can be used to train a bert relation model:
-
-~~~
-proquo train relation
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
---arch
-"bert"
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of a string and a class,
-tab separated, for example:
-
-~~~
-some context, some text <Q> some quote </Q> ( <OREF> ). some more text ( <REF> )   0
-~~~
-
-To test the model, run:
-
-~~~
-proquo test relation bert
-path_to_test_set.txt
-path_to_the_tokenizer_folder
-path_to_the_model_folder
-~~~
-
-#### Linking model
-The following command can be used to train a linking model:
-
-~~~
-proquolm train
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of two strings and a class,
-tab separated, for example:
+<details>
+<summary>All ProQuo command line options</summary>
 
 ~~~
-some text for context, <S> candidate </S> some more text  start of second text, some context <T> candidate </T> text text text  0
-~~~
-
-To test the model, run:
-
-~~~
-proquolm test
-path_to_test_set.txt
-path_to_the_tokenizer_folder
-path_to_the_model_folder
-~~~
+usage: proquo compare [-h] [--quid-match-path QUID_MATCH_PATH]
+                      [--output-folder-path OUTPUT_FOLDER_PATH]
+                      [--create-dated-subfolder] [--no-create-dated-subfolder]
+                      [--parallel-print-files [PARALLEL_PRINT_FILES ...]]
+                      [--parallel-print-first-page PARALLEL_PRINT_FIRST_PAGE]
+                      [--parallel-print-last-page PARALLEL_PRINT_LAST_PAGE]
+                      [--text] [--no-text] [--ref] [--no-ref]
+                      [--output-type {json,text,csv}] [--csv-sep CSV_SEP]
+                      [--open-quote OPEN_QUOTE] [--close-quote CLOSE_QUOTE]
+                      [--include-long-matches-in-result]
+                      [--max-num-processes MAX_NUM_PROCESSES]
+                      source-file-path target-path ref-vocab-file-path
+                      ref-model-file-path rel-tokenizer-folder-path
+                      rel-model-folder-path
+
+ProQuo compare allows the user to find short quotations (<= 4 words) in two
+texts, a source text and a target text. The target text is the text quoting
+the source text. Quotations in the target text need to be clearly marked with
+quotations marks.
+
+positional arguments:
+  source-file-path      Path to the source text file
+  target-path           Path to the target text file or folder
+  ref-vocab-file-path   Path to the reference vocab text file
+  ref-model-file-path   Path to the reference model file
+  rel-tokenizer-folder-path
+                        Path to the relation tokenizer folder
+  rel-model-folder-path
+                        Path to the relation model folder
+
+options:
+  -h, --help            show this help message and exit
+  --quid-match-path QUID_MATCH_PATH
+                        Path to the file or folder with quid matches. If this
+                        option is not set, then Quid is used to find long
+                        matches.
+  --output-folder-path OUTPUT_FOLDER_PATH
+                        The output folder path. If this option is set the
+                        output will be saved to a file created in the
+                        specified folder
+  --create-dated-subfolder
+                        Create a subfolder named with the current date to
+                        store the results
+  --no-create-dated-subfolder
+                        Do not create a subfolder named with the current date
+                        to store the results
+  --parallel-print-files [PARALLEL_PRINT_FILES ...]
+                        Filenames of files which quote a parallel print
+                        edition
+  --parallel-print-first-page PARALLEL_PRINT_FIRST_PAGE
+                        Number of the first page with parallel print
+  --parallel-print-last-page PARALLEL_PRINT_LAST_PAGE
+                        Number of the last page with parallel print
+  --text                Include matched text in the returned data structure
+  --no-text             Do not include matched text in the returned data
+                        structure
+  --ref                 Include matched reference in the returned data
+                        structure
+  --no-ref              Do not include matched reference in the returned data
+                        structure
+  --output-type {json,text,csv}
+                        The output type
+  --csv-sep CSV_SEP     output separator for csv (default: '\t')
+  --open-quote OPEN_QUOTE
+                        The quotation open character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --close-quote CLOSE_QUOTE
+                        The quotation close character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --include-long-matches-in-result
+                        Include matches longer than 4 words in the output
+  --max-num-processes MAX_NUM_PROCESSES
+                        Maximum number of processes to use for parallel
+                        processing.This can significantly speed up the
+                        process.
+~~~
+
+</details>
+
+## Parallel processing
+`ProQuo` and `ProQuoLM` use [Quid](https://scm.cms.hu-berlin.de/schluesselstellen/quid) in the background which supports
+using multiple processes when comparing multiple target texts with the source texts. To use Quid with multiple processes
+the command line option `--max-num-processes` is used. The default is 1.
+
+## Training
+The library also supports training and testing of custom models. The [Training Readme](Training-Readme.md) gives an introduction to
+training models.
 
 ## Citation
-If you use ProQuo or ProQuoLM or base your work on our code, please cite our paper:
+If you use `ProQuo` or `ProQuoLM` or base your work on our code, please cite our paper:
 ~~~
 @article{arnold2023,
   author = {Frederik Arnold, Robert Jäschke},
   title = {A Novel Approach for Identification and Linking of Short Quotations in Scholarly Texts and Literary Works},
   volume = {2},
   year = {2023},
   url = {https://jcls.io/article/id/3590/},
```

### Comparing `ProQuo-1.1.0/ProQuo.egg-info/PKG-INFO` & `proquo-1.1.1/ProQuo.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProQuo
-Version: 1.1.0
+Version: 1.1.1
 Summary: ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks.
 Author-email: Frederik Arnold <frederik.arnold@hu-berlin.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -217,210 +217,267 @@
 Requires-Dist: kpcommons~=0.0.2
 Requires-Dist: transformers~=4.39.3
 Requires-Dist: torch~=2.2.2
 Requires-Dist: scikit-learn~=1.2.1
 Requires-Dist: keras-preprocessing~=1.1.2
 
 # Readme
-`ProQuo` and `ProQuoLM` are a tools for the detection of short quotations (<= 4 words) between two texts, a source text and
-a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly
-marked with quotations marks. For more information, see below.
-
-## Overview
-The main purpose of this tool is to use the pretrained models for the detection of short quotations.
-Both approaches, `ProQuo` and `ProQuoLM` are separate. In our evaluation (see citation below) we found both approaches
-to perform at the same level while `ProQuoLm` is less complex as it is mainly a fine-tuned language model.
-The library also supports training and testing of custom models for reference classification, relation classification
-and linking classification.
+This repository contains two tools, `ProQuo` and `ProQuoLM`. Both are tools for the detection of short quotations
+(<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text.
+Quotations in the target text need to be marked with quotations marks. For more information, see below.
+
+The main purpose of this tool is to use the pretrained models for the detection of short quotations. While we found both
+approaches (`ProQuo` and `ProQuoLM`) to perform at the same level (for details, see our [publication](https://jcls.io/article/id/3590/)),
+`ProQuoLm` is easier to use, better maintained and the **recommended approach**.
 
-**Note**: `ProQuoLM` is easier to use, faster, better documented, better maintained, better tested and the recommended
-approach to use.
-
-## Quotation marks
-By default, the 'best', i.e. most common combination of opening and closing quotation mark in the specific text is used.
+## Quotation Marks
+By default, the "best", that is, most common, combination of opening and closing quotation mark in the specific text is used.
 The following combinations are automatically tried:
 
 1. " and "
 2. „ and “
 3. „ and "
 4. “ and “
 5. » and «
 6. « and »
 7. ‘ and ’
 
-If this is not the desired behaviour, quotations marks can be manually defined, using the command line options
-`--open-quote` and `--close-quote` to define which opening and closing quotation marks to use.
+If this is not the desired behaviour, quotations marks can be manually defined using the command line options
+`--open-quote` and `--close-quote`.
 
-## Pretrained models and training data
+## Approaches Overview
+`ProQuo` is a specialized pipeline which uses a [model for reference classification](proquo/model/reference/ReferenceModelTrainer.py)
+and a [model for relation extraction](proquo/model/relation/RelationModelBertTrainer.py) between quotations and (page)
+references to distinguish between relevant quotations (that is, quotations from the source text) and quotations
+from other sources. In a third step, a rule-based algorithm is used to link the identified quotations to their source.
 
-The pretrained models and training data are made available and can be downloaded from [here](https://scm.cms.hu-berlin.de/schluesselstellen/proquodata).
+`ProQuoLM` uses a [fine-tuned BERT model](https://huggingface.co/Fredr0id/proquolm) in two ways: to distinguish between
+relevant quotations and quotations from other sources and to link the quotations to their source.
 
+## Pretrained Models and Training Data
+The pretrained models and training data are made available and can be downloaded from [here](https://scm.cms.hu-berlin.de/schluesselstellen/proquodata).
 For `ProQuoLm`, we also provide a model on [Hugging Face](https://huggingface.co/Fredr0id/proquolm). This is used by default.
 
 ## Installation
 
 ### From PyPi
-
 **Note**: Both tools are part of the same PyPi package. So the following command installs both.
 
 ~~~
 pip install ProQuo
 ~~~
 
-### From source
+### From Source
 Checkout this repository and then run:
 
 ~~~
 python -m pip install .
 ~~~
 
-This installs `ProQuo` and all dependencies except `tensorflow` which needs to be installed manually depending on
-the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was
-tested is 2.14.1.
+### Dependencies
+Both installation methods install all dependencies except `tensorflow` which needs to be installed manually depending on
+the individual needs, see [Tensorflow installation](https://www.tensorflow.org/install). The latest version that was tested is 2.14.1.
 
 For `RelationModelLstmTrainer`, `tensorflow-text` is needed. `RelationModelLstmTrainer` should normally not be needed as
 `RelationModelBertTrainer` performs better and is the default in the pipeline.
 
 ## Usage
-There are two ways to use the tool: in code and from the command line. Both are described in the following sections.
+The following sections describe how to use ProQuo on the command line.
 
 ### Quotation detection
-There are two approaches which can be used for quotation detection: A specialized pipeline and a general language model based approach.
-To run the (recommended) language model approach with the default model, use the following command:
+To run `ProQuoLM` with the default model, use the following command:
 
 ~~~
-proquolm compare
-path_to_source_text
-path_to_target_text
---text
---output-type text
+proquolm compare path_to_source_text path_to_target_text --text --output-type text
+~~~
+
+<details>
+<summary>All ProQuoLM command line options</summary>
+
 ~~~
+usage: proquolm compare [-h] [--tokenizer TOKENIZER] [--model MODEL]
+                        [--lower-case | --no-lower-case]
+                        [--output-folder-path OUTPUT_FOLDER_PATH]
+                        [--create-dated-subfolder | --no-create-dated-subfolder]
+                        [--text | --no-text] [--output-type {json,text,csv}]
+                        [--csv-sep CSV_SEP] [--open-quote OPEN_QUOTE]
+                        [--close-quote CLOSE_QUOTE]
+                        [--include-long-matches-in-result]
+                        [--max-num-processes MAX_NUM_PROCESSES]
+                        source-file-path target-path
+
+ProQuoLm compare allows the user to find short quotations (<= 4 words) in two
+texts, a source text and a target text. The target text is the text quoting
+the source text. Quotations in the target text need to be clearly marked with
+quotations marks.
+
+positional arguments:
+  source-file-path      Path to the source text file
+  target-path           Path to the target text file or folder
+
+options:
+  -h, --help            show this help message and exit
+  --tokenizer TOKENIZER
+                        Name of the tokenizer to load from Hugging Face or
+                        path to the tokenizer folder
+  --model MODEL         Name of the model to load from Hugging Face or path to
+                        the model folder
+  --lower-case, --no-lower-case
+                        Run model inference on lower case text (default: True)
+  --output-folder-path OUTPUT_FOLDER_PATH
+                        The output folder path. If this option is set the
+                        output will be saved to a file created in the
+                        specified folder
+  --create-dated-subfolder, --no-create-dated-subfolder
+                        Create a subfolder named with the current date to
+                        store the results (default: False)
+  --text, --no-text     Include matched text in the returned data structure
+                        (default: True)
+  --output-type {json,text,csv}
+                        The output type
+  --csv-sep CSV_SEP     output separator for csv (default: '\t')
+  --open-quote OPEN_QUOTE
+                        The quotation open character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --close-quote CLOSE_QUOTE
+                        The quotation close character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --include-long-matches-in-result
+                        Include matches longer than 4 words in the output
+  --max-num-processes MAX_NUM_PROCESSES
+                        Maximum number of processes to use for parallel
+                        processing. This can significantly speed up the
+                        process.
+~~~
+
+</details>
 
-To run the specialized pipeline, use the following command:
+To run `ProQuo`, use the following command:
 
 ~~~
-proquo compare
-path_to_source_text
-path_to_target_text
+proquo compare path_to_source_text path_to_target_text
 path_to_the_reference_vocab_file
 path_to_the_reference_model_file
 path_to_the_relation_tokenizer_folder
 path_to_the_relation_model_folder
 --text
 --output-type text
 ~~~
 
 `--output-type text` prints the results to the command line. To save the results to a file, use `--output-type csv` or
 `--output-type json`. `--text` includes the quotation text in the output.
 
 The output will look something like this:
+
 ~~~
-10	15	500	505	quote	quote
+10      15	    500	505	quote	quote
 1000	1016	20	36	some other quote	some other quote
 ~~~
+
 The first two numbers are the character start and end positions in the source text and the other two numbers are the
 character start and end positions in the target text.
 
-#### Note
-There are a number of command line arguments to configure the output format, for example, to save the result to a csv
-file. For all options, use the following commands:
-
-~~~
-proquo compare -h
-~~~
-
-~~~
-proquolm compare -h
-~~~
-
-### Training and testing a model
-
-#### Reference model
-The following command can be used to train a reference model:
-
-~~~
-proquo train reference
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of two strings and a class,
-tab separated, for example:
-
-~~~
-S. 47   S. 35	1
-63	DKV III, 17	0
-~~~
-
-To test the model, run:
-
-~~~
-proquo test reference
-path_to_test_set.txt
-path_to_the_reference_vocab_file
-path_to_the_reference_model_file
-~~~
-
-#### Relation model
-The following command can be used to train a bert relation model:
-
-~~~
-proquo train relation
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
---arch
-"bert"
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of a string and a class,
-tab separated, for example:
-
-~~~
-some context, some text <Q> some quote </Q> ( <OREF> ). some more text ( <REF> )   0
-~~~
-
-To test the model, run:
-
-~~~
-proquo test relation bert
-path_to_test_set.txt
-path_to_the_tokenizer_folder
-path_to_the_model_folder
-~~~
-
-#### Linking model
-The following command can be used to train a linking model:
-
-~~~
-proquolm train
-path_to_train_set.txt
-path_to_val_set.txt
-path_to_the_output_folder
-~~~
-
-`path_to_train_set.txt` and `path_to_val_set.txt` contain one example per line in the form of two strings and a class,
-tab separated, for example:
+<details>
+<summary>All ProQuo command line options</summary>
 
 ~~~
-some text for context, <S> candidate </S> some more text  start of second text, some context <T> candidate </T> text text text  0
-~~~
-
-To test the model, run:
-
-~~~
-proquolm test
-path_to_test_set.txt
-path_to_the_tokenizer_folder
-path_to_the_model_folder
-~~~
+usage: proquo compare [-h] [--quid-match-path QUID_MATCH_PATH]
+                      [--output-folder-path OUTPUT_FOLDER_PATH]
+                      [--create-dated-subfolder] [--no-create-dated-subfolder]
+                      [--parallel-print-files [PARALLEL_PRINT_FILES ...]]
+                      [--parallel-print-first-page PARALLEL_PRINT_FIRST_PAGE]
+                      [--parallel-print-last-page PARALLEL_PRINT_LAST_PAGE]
+                      [--text] [--no-text] [--ref] [--no-ref]
+                      [--output-type {json,text,csv}] [--csv-sep CSV_SEP]
+                      [--open-quote OPEN_QUOTE] [--close-quote CLOSE_QUOTE]
+                      [--include-long-matches-in-result]
+                      [--max-num-processes MAX_NUM_PROCESSES]
+                      source-file-path target-path ref-vocab-file-path
+                      ref-model-file-path rel-tokenizer-folder-path
+                      rel-model-folder-path
+
+ProQuo compare allows the user to find short quotations (<= 4 words) in two
+texts, a source text and a target text. The target text is the text quoting
+the source text. Quotations in the target text need to be clearly marked with
+quotations marks.
+
+positional arguments:
+  source-file-path      Path to the source text file
+  target-path           Path to the target text file or folder
+  ref-vocab-file-path   Path to the reference vocab text file
+  ref-model-file-path   Path to the reference model file
+  rel-tokenizer-folder-path
+                        Path to the relation tokenizer folder
+  rel-model-folder-path
+                        Path to the relation model folder
+
+options:
+  -h, --help            show this help message and exit
+  --quid-match-path QUID_MATCH_PATH
+                        Path to the file or folder with quid matches. If this
+                        option is not set, then Quid is used to find long
+                        matches.
+  --output-folder-path OUTPUT_FOLDER_PATH
+                        The output folder path. If this option is set the
+                        output will be saved to a file created in the
+                        specified folder
+  --create-dated-subfolder
+                        Create a subfolder named with the current date to
+                        store the results
+  --no-create-dated-subfolder
+                        Do not create a subfolder named with the current date
+                        to store the results
+  --parallel-print-files [PARALLEL_PRINT_FILES ...]
+                        Filenames of files which quote a parallel print
+                        edition
+  --parallel-print-first-page PARALLEL_PRINT_FIRST_PAGE
+                        Number of the first page with parallel print
+  --parallel-print-last-page PARALLEL_PRINT_LAST_PAGE
+                        Number of the last page with parallel print
+  --text                Include matched text in the returned data structure
+  --no-text             Do not include matched text in the returned data
+                        structure
+  --ref                 Include matched reference in the returned data
+                        structure
+  --no-ref              Do not include matched reference in the returned data
+                        structure
+  --output-type {json,text,csv}
+                        The output type
+  --csv-sep CSV_SEP     output separator for csv (default: '\t')
+  --open-quote OPEN_QUOTE
+                        The quotation open character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --close-quote CLOSE_QUOTE
+                        The quotation close character. If this option is not
+                        set, then the type of quotation marks used in a target
+                        text is auto automatically identified.
+  --include-long-matches-in-result
+                        Include matches longer than 4 words in the output
+  --max-num-processes MAX_NUM_PROCESSES
+                        Maximum number of processes to use for parallel
+                        processing.This can significantly speed up the
+                        process.
+~~~
+
+</details>
+
+## Parallel processing
+`ProQuo` and `ProQuoLM` use [Quid](https://scm.cms.hu-berlin.de/schluesselstellen/quid) in the background which supports
+using multiple processes when comparing multiple target texts with the source texts. To use Quid with multiple processes
+the command line option `--max-num-processes` is used. The default is 1.
+
+## Training
+The library also supports training and testing of custom models. The [Training Readme](Training-Readme.md) gives an introduction to
+training models.
 
 ## Citation
-If you use ProQuo or ProQuoLM or base your work on our code, please cite our paper:
+If you use `ProQuo` or `ProQuoLM` or base your work on our code, please cite our paper:
 ~~~
 @article{arnold2023,
   author = {Frederik Arnold, Robert Jäschke},
   title = {A Novel Approach for Identification and Linking of Short Quotations in Scholarly Texts and Literary Works},
   volume = {2},
   year = {2023},
   url = {https://jcls.io/article/id/3590/},
```

### Comparing `ProQuo-1.1.0/ProQuo.egg-info/SOURCES.txt` & `proquo-1.1.1/ProQuo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/cli/Helper.py` & `proquo-1.1.1/proquo/cli/Helper.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/cli/ProQuoCLI.py` & `proquo-1.1.1/proquo/cli/ProQuoCLI.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/cli/ProQuoLmCLI.py` & `proquo-1.1.1/proquo/cli/ProQuoLmCLI.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,20 +198,21 @@
                               help='Path to the txt file containing the validation examples')
     parser_train.add_argument('output_folder_path', nargs=1, metavar='output-folder_path',
                               help='Path to the folder for storing the output model and vocabulary')
     parser_train.add_argument('--create-dated-subfolder', dest='create_dated_subfolder', default=False,
                               action=BooleanOptionalAction,
                               help='Create a subfolder named with the current date to store the results')
     parser_train.add_argument('--base-model-name', dest="base_model_name",
-                              default="bert-base-german-dbmdz-uncased", help="The model name")
+                              default="dbmdz/bert-base-german-uncased", help="The model name (default: %(default)s)")
     parser_train.add_argument('--lower-case', dest="lower_case", default=True, action=BooleanOptionalAction,
                               help="Train model on lower case text")
-    parser_train.add_argument('--batch-size', dest="batch_size", default=4, type=int, help="The batch size")
+    parser_train.add_argument('--batch-size', dest="batch_size", default=4, type=int,
+                              help="The batch size (default: %(default)d)")
     parser_train.add_argument('--num-epochs', dest="num_epochs", default=3, type=int,
-                              help="The number of epochs to train for")
+                              help="The number of epochs to train for (default: %(default)d)")
 
     parser_test = subparsers_command.add_parser('test', help=test_description, description=test_description)
 
     parser_test.add_argument('test_file_path', nargs=1, metavar='test-file-path',
                              help='Path to the txt file containing the testing examples')
     parser_test.add_argument('tokenizer_folder_path', nargs=1, metavar='tokenizer-folder-path',
                              help='Path to the vocab file')
```

### Comparing `ProQuo-1.1.0/proquo/core/Helper.py` & `proquo-1.1.1/proquo/core/Helper.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/core/ProQuo.py` & `proquo-1.1.1/proquo/core/ProQuo.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/core/ProQuoLm.py` & `proquo-1.1.1/proquo/core/ProQuoLm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/linking/LinkingModelTrainer.py` & `proquo-1.1.1/proquo/model/linking/LinkingModelTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/linking/LinkingVectorizer.py` & `proquo-1.1.1/proquo/model/linking/LinkingVectorizer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/reference/ReferenceModelTrainer.py` & `proquo-1.1.1/proquo/model/reference/ReferenceModelTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/reference/ReferenceVectorizer.py` & `proquo-1.1.1/proquo/model/reference/ReferenceVectorizer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/relation/RelationModelBertTrainer.py` & `proquo-1.1.1/proquo/model/relation/RelationModelBertTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/relation/RelationModelLstmTrainer.py` & `proquo-1.1.1/proquo/model/relation/RelationModelLstmTrainer.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/relation/RelationVectorizerBert.py` & `proquo-1.1.1/proquo/model/relation/RelationVectorizerBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/model/relation/RelationVectorizerLstm.py` & `proquo-1.1.1/proquo/model/relation/RelationVectorizerLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/testing/linking/TestLinking.py` & `proquo-1.1.1/proquo/testing/linking/TestLinking.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/testing/reference/TestReference.py` & `proquo-1.1.1/proquo/testing/reference/TestReference.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/testing/relation/TestRelationBert.py` & `proquo-1.1.1/proquo/testing/relation/TestRelationBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/testing/relation/TestRelationLstm.py` & `proquo-1.1.1/proquo/testing/relation/TestRelationLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/training/linking/TrainLinking.py` & `proquo-1.1.1/proquo/training/linking/TrainLinking.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/training/reference/TrainReference.py` & `proquo-1.1.1/proquo/training/reference/TrainReference.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/training/relation/TrainRelationBert.py` & `proquo-1.1.1/proquo/training/relation/TrainRelationBert.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/proquo/training/relation/TrainRelationLstm.py` & `proquo-1.1.1/proquo/training/relation/TrainRelationLstm.py`

 * *Files identical despite different names*

### Comparing `ProQuo-1.1.0/pyproject.toml` & `proquo-1.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ProQuo"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "Frederik Arnold", email = "frederik.arnold@hu-berlin.de"}
 ]
 description = "ProQuo is a tool for the detection of short quotations (<= 4 words) between two texts, a source text and a target text. The target text is the text quoting the source text. Quotations in the target text need to be clearly marked with quotations marks."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

