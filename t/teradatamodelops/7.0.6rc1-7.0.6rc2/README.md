# Comparing `tmp/teradatamodelops-7.0.6rc1.tar.gz` & `tmp/teradatamodelops-7.0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teradatamodelops-7.0.6rc1.tar", last modified: Tue Apr 16 09:43:51 2024, max compression
+gzip compressed data, was "teradatamodelops-7.0.6rc2.tar", last modified: Tue Apr 16 10:47:35 2024, max compression
```

## Comparing `teradatamodelops-7.0.6rc1.tar` & `teradatamodelops-7.0.6rc2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.839447 teradatamodelops-7.0.6rc1/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/LICENSE.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/MANIFEST.in
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 09:43:51.838994 teradatamodelops-7.0.6rc1/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2072 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/README.md
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.420981 teradatamodelops-7.0.6rc1/aoa/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1205 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/aoa/__init__.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.582659 teradatamodelops-7.0.6rc1/aoa/api/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1478 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/api_iterator.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4632 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3608 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1501 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_connection_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2350 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_template_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3048 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/deployment_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      781 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/iterator_base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4717 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/job_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3288 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/job_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1000 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/message_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4397 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2727 2024-04-11 11:19:05.000000 teradatamodelops-7.0.6rc1/aoa/api/project_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6237 2024-04-16 09:16:52.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6015 2024-04-16 09:23:37.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_artefacts_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4543 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      893 2024-04-16 08:05:32.000000 teradatamodelops-7.0.6rc1/aoa/api/user_attributes_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    17659 2024-04-16 09:23:24.000000 teradatamodelops-7.0.6rc1/aoa/api_client.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.638198 teradatamodelops-7.0.6rc1/aoa/cli/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4345 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/base_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6371 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/cli/evaluate_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.651820 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/.gitignore
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/readme.md
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4887 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/repo_manager.py
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/run_model.R
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3896 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/score_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4658 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/train_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.660198 teradatamodelops-7.0.6rc1/aoa/context/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/context/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3709 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/context/model_context.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.681194 teradatamodelops-7.0.6rc1/aoa/crypto/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29020 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/crypto/TJEncryptPassword.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/crypto/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6543 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/crypto/crypto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.760563 teradatamodelops-7.0.6rc1/aoa/stats/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/stats/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16963 2024-02-27 13:24:56.000000 teradatamodelops-7.0.6rc1/aoa/stats/stats.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22431 2024-04-09 08:50:48.000000 teradatamodelops-7.0.6rc1/aoa/stats/stats_util.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3494 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/stats/store.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.797357 teradatamodelops-7.0.6rc1/aoa/util/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/util/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/util/artifacts.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1531 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/util/byom.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6564 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/aoa/util/connections.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9150 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/util/sto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.813822 teradatamodelops-7.0.6rc1/scripts/
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      239 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/scripts/aoa
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    50274 2024-04-09 08:50:48.000000 teradatamodelops-7.0.6rc1/scripts/tmo
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      442 2024-04-16 09:43:51.843065 teradatamodelops-7.0.6rc1/setup.cfg
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      986 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/setup.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.837871 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1322 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/SOURCES.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/dependency_links.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/requires.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/top_level.txt
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.380822 teradatamodelops-7.0.6rc2/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/LICENSE.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/MANIFEST.in
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 10:47:35.380359 teradatamodelops-7.0.6rc2/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2202 2024-04-16 10:43:57.000000 teradatamodelops-7.0.6rc2/README.md
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.288562 teradatamodelops-7.0.6rc2/aoa/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1205 2024-04-16 10:45:01.000000 teradatamodelops-7.0.6rc2/aoa/__init__.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.310488 teradatamodelops-7.0.6rc2/aoa/api/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/api/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1641 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/api_iterator.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4591 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3711 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1699 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_connection_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2513 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/dataset_template_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3280 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/deployment_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      774 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/iterator_base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5008 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/job_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3530 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/job_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      972 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/message_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4542 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2838 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/project_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6473 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6324 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_artefacts_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4817 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/trained_model_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      926 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api/user_attributes_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    18419 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/api_client.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.323010 teradatamodelops-7.0.6rc2/aoa/cli/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4394 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/cli/base_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     7171 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/evaluate_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.328826 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/.gitignore
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/metadata_files/readme.md
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5068 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/cli/repo_manager.py
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/cli/run_model.R
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4178 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/score_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4895 2024-04-16 10:38:58.000000 teradatamodelops-7.0.6rc2/aoa/cli/train_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.330588 teradatamodelops-7.0.6rc2/aoa/context/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/context/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3837 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/context/model_context.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.334311 teradatamodelops-7.0.6rc2/aoa/crypto/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29683 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/crypto/TJEncryptPassword.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/crypto/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6611 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/crypto/crypto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.337813 teradatamodelops-7.0.6rc2/aoa/stats/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/stats/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16762 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/stats.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22482 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/stats_util.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3647 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/stats/store.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.342792 teradatamodelops-7.0.6rc2/aoa/util/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/util/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc2/aoa/util/artifacts.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1610 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/byom.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6344 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/connections.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9042 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/aoa/util/sto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.344855 teradatamodelops-7.0.6rc2/scripts/
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      245 2024-04-16 10:34:39.000000 teradatamodelops-7.0.6rc2/scripts/aoa
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    53532 2024-04-16 10:34:40.000000 teradatamodelops-7.0.6rc2/scripts/tmo
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      442 2024-04-16 10:47:35.386241 teradatamodelops-7.0.6rc2/setup.cfg
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      986 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc2/setup.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 10:47:35.379242 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1322 2024-04-16 10:47:35.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/SOURCES.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/dependency_links.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/requires.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-04-16 10:47:34.000000 teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/top_level.txt
```

### Comparing `teradatamodelops-7.0.6rc1/LICENSE-3RD-PARTY.txt` & `teradatamodelops-7.0.6rc2/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc1/LICENSE.txt` & `teradatamodelops-7.0.6rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc1/PKG-INFO` & `teradatamodelops-7.0.6rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.6rc1
+Version: 7.0.6rc2
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `teradatamodelops-7.0.6rc1/README.md` & `teradatamodelops-7.0.6rc2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,21 @@
 python setup.py clean --all
 python setup.py sdist bdist_wheel
 
 # install using pip
 pip install dist/*.whl
 ```
 
+## Code Style
+
+```bash
+pip install -r dev_requirements.txt
+python -m black aoa/* scripts/* examples/*.ipynb -t py38 -t py39 
+```
+
 ## Testing
 
 ```bash
 pip install -r dev_requirements.txt
 python -m pytest
 ```
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/__init__.py` & `teradatamodelops-7.0.6rc2/aoa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "7.0.6rc1"
+__version__ = "7.0.6rc2"
 
 # import client
 from aoa.api_client import AoaClient
 
 # import APIs into api package
 from aoa.api.dataset_api import DatasetApi
 from aoa.api.dataset_template_api import DatasetTemplateApi
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/api_iterator.py` & `teradatamodelops-7.0.6rc2/aoa/api/api_iterator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 from __future__ import absolute_import
 
 
 class ApiIterator(object):
     _pos = 0
     _current_page = 0
 
-    def __init__(self, api_func=None, entities: str = None, projection: str = None, page_size: int = None,
-                 sort: str = None):
+    def __init__(
+        self,
+        api_func=None,
+        entities: str = None,
+        projection: str = None,
+        page_size: int = None,
+        sort: str = None,
+    ):
         if api_func is None or entities is None:
             pass
         else:
             self._api_func = api_func
             self._projection = projection
             self._page_size = page_size
             self._sort = sort
-            page_info = api_func(projection=projection, page=0, size=page_size, sort=sort)['page']
-            self._total_elements = page_info['totalElements']
-            self._total_pages = page_info['totalPages']
-            self._cache = api_func(projection=projection, page=0, size=page_size, sort=sort)['_embedded'][entities]
+            page_info = api_func(
+                projection=projection, page=0, size=page_size, sort=sort
+            )["page"]
+            self._total_elements = page_info["totalElements"]
+            self._total_pages = page_info["totalPages"]
+            self._cache = api_func(
+                projection=projection, page=0, size=page_size, sort=sort
+            )["_embedded"][entities]
             self._entities = entities
 
     def __next__(self):
         if self._pos < len(self._cache):
             result = self._cache[self._pos]
             self._pos += 1
             return result
         elif self._current_page < self._total_pages - 1:
             self._current_page += 1
             self._pos = 1  # so we skip the first one in next iteration
-            self._cache = \
-            self._api_func(projection=self._projection, page=self._current_page, size=self._page_size, sort=self._sort)['_embedded'][self._entities]
+            self._cache = self._api_func(
+                projection=self._projection,
+                page=self._current_page,
+                size=self._page_size,
+                sort=self._sort,
+            )["_embedded"][self._entities]
             return self._cache[0]
         else:
             raise StopIteration
 
     def __iter__(self):
         return self
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/base_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/base_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Dict
 from aoa.api_client import AoaClient
 
 import abc
 
 
 class BaseApi(object):
-    path = ''
+    path = ""
 
     def __init__(self, aoa_client: AoaClient):
         self.aoa_client = aoa_client
 
     @abc.abstractmethod
     def _get_header_params(self):
         pass
@@ -40,15 +40,21 @@
            param_names (List[str]): list of required parameter names
            dict_obj (Dict[str, str]): dictionary to check for required parameters
         """
         for param in param_names:
             if param not in dict_obj:
                 raise ValueError("Missing required value " + str(param))
 
-    def find_all(self, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_all(
+        self,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns all entities
 
         Parameters:
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
@@ -56,24 +62,28 @@
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): all entities
         """
         header_params = self._get_header_params()
 
-        query_vars = ['projection', 'page', 'size', 'sort']
+        query_vars = ["projection", "page", "size", "sort"]
         query_vals = [projection, page, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
-        return self.aoa_client.get_request(
-            self.path,
-            header_params,
-            query_params)
+        return self.aoa_client.get_request(self.path, header_params, query_params)
 
-    def find_by_archived(self, archived: bool = False, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_by_archived(
+        self,
+        archived: bool = False,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns all entities by archived
 
         Parameters:
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
@@ -81,69 +91,61 @@
            archived (bool): whether to return archived or unarchived entities
 
         Returns:
             (dict): all entities
         """
         header_params = self._get_header_params()
 
-        query_vars = ['projection', 'page', 'size', 'sort', 'archived']
+        query_vars = ["projection", "page", "size", "sort", "archived"]
         query_vals = [projection, page, size, sort, archived]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            self.path + "search/findByArchived",
-            header_params,
-            query_params)
+            self.path + "search/findByArchived", header_params, query_params
+        )
 
     def find_by_id(self, id: str, projection: str = None):
         """
         returns the entity
 
         Parameters:
            id (str): entity id(uuid) to find
            projection (str): projection type
 
         Returns:
             (dict): entity
         """
         header_params = self._get_header_params()
 
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
-        return self.aoa_client.get_request(
-            self.path + id,
-            header_params,
-            query_params)
+        return self.aoa_client.get_request(self.path + id, header_params, query_params)
 
     def archive(self, id: str):
         """
         archives the entity
         Parameters:
            id (str): entity id(uuid) to archive
         Returns:
             (dict): entity
         """
         header_params = self._get_header_params()
 
         return self.aoa_client.post_request(
-            "/api/archives/" + self.type + "/" + id,
-            header_params,
-            {},
-            {})
+            "/api/archives/" + self.type + "/" + id, header_params, {}, {}
+        )
 
     def unarchive(self, id: str):
         """
         unarchives the entity
         Parameters:
            id (str): entity id(uuid) to unarchive
         Returns:
             (dict): entity
         """
         header_params = self._get_header_params()
 
         return self.aoa_client.delete_request(
-            "/api/archives/" + self.type + "/" + id,
-            header_params,
-            {},
-            {})
+            "/api/archives/" + self.type + "/" + id, header_params, {}, {}
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/dataset_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/dataset_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,54 +5,66 @@
 
 
 class DatasetApi(IteratorBaseApi):
     path = "/api/datasets/"
     type = "DATASET"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_by_name_like(self, name: str, projection: str = None) -> List:
         """
         returns a list of datasets matching the name
 
         Parameters:
            name (str): dataset name(string) to match
            projection (str): projection type
 
         Returns:
             (list): list of datasets
         """
-        query_vars = ['name', 'projection']
+        query_vars = ["name", "projection"]
         query_vals = [name, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByName",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_dataset_template_id(self,
-                                    dataset_template_id: str,
-                                    archived: bool = False,
-                                    projection: str = None,
-                                    page: int = None,
-                                    size: int = None,
-                                    sort: str = None):
+    def find_by_dataset_template_id(
+        self,
+        dataset_template_id: str,
+        archived: bool = False,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns a dataset of a project by name
 
         Parameters:
            dataset_template_id (str): dataset_template_id
            archived (bool): archived or not (default False)
            projection (str): projection type
@@ -60,22 +72,30 @@
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): datasets
         """
-        query_vars = ['datasetTemplateId', 'archived', 'projection', 'page', 'size', 'sort']
+        query_vars = [
+            "datasetTemplateId",
+            "archived",
+            "projection",
+            "page",
+            "size",
+            "sort",
+        ]
         query_vals = [dataset_template_id, archived, projection, page, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByDatasetTemplateId",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def save(self, dataset: Dict[str, str]):
         """
         register a dataset
 
         Parameters:
            dataset (dict): dataset to register
@@ -83,15 +103,16 @@
         Returns:
             (dict): dataset
         """
         return self.aoa_client.post_request(
             path=self.path,
             header_params=self._get_header_params(),
             query_params={},
-            body=dataset)
+            body=dataset,
+        )
 
     def render(self, id: str) -> Dict:
         """
         returns a rendered dataset
 
         Parameters:
            id (str): dataset id
@@ -99,8 +120,9 @@
         Returns:
             (dict): rendered dataset
         """
 
         return self.aoa_client.get_request(
             path=self.path + id + "/render",
             header_params=self._get_header_params(),
-            query_params={})
+            query_params={},
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/dataset_connection_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/dataset_connection_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,44 @@
 from aoa.api.iterator_base_api import IteratorBaseApi
 
 
 class DatasetConnectionApi(IteratorBaseApi):
     path = "/api/datasetConnections/"
     type = "DATASET_CONNECTION"
 
-    def find_by_archived(self, archived: bool = False, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_by_archived(
+        self,
+        archived: bool = False,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         raise NotImplementedError("Archiving not supported for DatasetConnections")
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def save(self, dataset_connection: Dict[str, str]):
         """
         register a dataset connection
 
@@ -36,8 +52,9 @@
             (dict): dataset template
         """
 
         return self.aoa_client.post_request(
             path=self.path,
             header_params=self._get_header_params(),
             query_params={},
-            body=dataset_connection)
+            body=dataset_connection,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/dataset_template_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/dataset_template_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,46 +5,56 @@
 
 
 class DatasetTemplateApi(IteratorBaseApi):
     path = "/api/datasetTemplates/"
     type = "DATASET_TEMPLATE"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_by_name_like(self, name: str, projection: str = None) -> List:
         """
         returns a list dataset template of a project by name
 
         Parameters:
            name (str): dataset name(string) to find
            projection (str): projection type
 
         Returns:
             (list): dataset template
         """
-        query_vars = ['name', 'projection']
+        query_vars = ["name", "projection"]
         query_vals = [name, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByName",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def save(self, dataset_template: Dict[str, str]):
         """
         register a dataset template
 
         Parameters:
            dataset template (dict): dataset template to register
@@ -52,23 +62,25 @@
         Returns:
             (dict): dataset template
         """
         return self.aoa_client.post_request(
             path=self.path,
             header_params=self._get_header_params(),
             query_params={},
-            body=dataset_template)
+            body=dataset_template,
+        )
 
     def render(self, id: str) -> Dict:
         """
         returns a rendered dataset template
 
         Parameters:
            id (str): dataset_template id
 
         Returns:
             (dict): rendered dataset template
         """
         return self.aoa_client.get_request(
             path=self.path + id + "/render",
             header_params=self._get_header_params(),
-            query_params={})
+            query_params={},
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/deployment_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/deployment_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,78 +4,99 @@
 
 
 class DeploymentApi(IteratorBaseApi):
     path = "/api/deployments/"
     type = "DEPLOYMENT"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
-    def find_by_archived(self, archived: bool = False, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_by_archived(
+        self,
+        archived: bool = False,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         raise NotImplementedError("Archiving not supported for Deployments")
 
-    def find_active_by_trained_model_and_engine_type(self, trained_model_id: str, engine_type: str, projection: str = None):
+    def find_active_by_trained_model_and_engine_type(
+        self, trained_model_id: str, engine_type: str, projection: str = None
+    ):
         """
         returns deployments by trained model and engine type
 
         Parameters:
            trained_model_id (str): trained model id(string) to find
            engine_type (str): engine type(string) to find
            projection (str): projection type
 
         Returns:
             (dict): deployments
         """
-        query_vars = ['trainedModelId', 'engineType', 'projection']
+        query_vars = ["trainedModelId", "engineType", "projection"]
         query_vals = [trained_model_id, engine_type, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findActiveByTrainedModelIdAndEngineType",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_by_status(self, status: str, projection: str = None):
         """
         returns deployments by status
         Parameters:
            status (str): status(string) to find
            projection (str): projection type
         Returns:
             (dict): deployments
         """
-        query_vars = ['status', 'projection']
+        query_vars = ["status", "projection"]
         query_vals = [status, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByStatus",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_active(self, projection: str = None):
         """
         returns active deployments
         Parameters:
            projection (str): projection type
         Returns:
             (dict): deployments
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findActive",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/iterator_base_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/iterator_base_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,13 +13,15 @@
 
         if show_archived:
             self.iterator_func = self.find_all
         else:
             self.iterator_func = self.find_by_archived
 
     def __iter__(self):
-        return ApiIterator(api_func=self.iterator_func,
-                           entities=self.path.split('/')[-2],
-                           projection=self.iterator_projection)
+        return ApiIterator(
+            api_func=self.iterator_func,
+            entities=self.path.split("/")[-2],
+            projection=self.iterator_projection,
+        )
 
     def __len__(self):
-        return self.find_all()['page']['totalElements']
+        return self.find_all()["page"]["totalElements"]
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/job_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/job_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,130 +3,161 @@
 from aoa.api.iterator_base_api import IteratorBaseApi
 
 
 class JobApi(IteratorBaseApi):
     path = "/api/jobs/"
     type = "JOB"
 
-    def find_by_archived(self, archived: bool = False, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_by_archived(
+        self,
+        archived: bool = False,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         raise NotImplementedError("Archiving not supported for Jobs")
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_job_events(self, job_id: str, projection: str = None):
         """
         returns events of a job
 
         Parameters:
            job_id (str): job id(uuid) to find events
            projection (str): projection type
 
         Returns:
             (dict): job events
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + job_id + '/events',
+            path=self.path + job_id + "/events",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_job_event_id(self, job_id: str, job_event_id: str, projection: str = None):
+    def find_by_job_event_id(
+        self, job_id: str, job_event_id: str, projection: str = None
+    ):
         """
         returns job event
 
         Parameters:
            job_id (str): job id(uuid)
            job_event_id (str): job event id(uuid)
            projection (str): projection type
 
         Returns:
             (dict): job event
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + job_id + '/events/' + job_event_id,
+            path=self.path + job_id + "/events/" + job_event_id,
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_job_between_intervals(self, start_time: str, end_time: str,
-                                   projection: str = None):
+    def find_job_between_intervals(
+        self, start_time: str, end_time: str, projection: str = None
+    ):
         """
         returns job events within the timestamp range
 
         Parameters:
            start_time (str): start time e.g: 2020-03-18T09:05:03.569Z
            end_time (str): end time e.g: 2020-03-24T09:05:03.569Z
            projection (str): projection type
 
         Returns:
             (dict): job events
         """
-        query_vars = ['startAt', 'endAt', 'projection']
+        query_vars = ["startAt", "endAt", "projection"]
         query_vals = [start_time, end_time, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByCreatedAtBetween",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_status(self, status: str, projection: str = None, page: int = None, size: int = None,
-                       sort: str = None):
+    def find_by_status(
+        self,
+        status: str,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns job by status
 
         Parameters:
            status (str): job status
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): job events
         """
-        query_vars = ['status', 'projection', 'page', 'sort', 'size']
+        query_vars = ["status", "projection", "page", "sort", "size"]
         query_vals = [status, projection, page, sort, size]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByStatusIn',
+            path=self.path + "search/findByStatusIn",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def wait(self, job_id: str, timeout_sec: int = 60):
         import time
 
         start_time_sec = int(time.time())
 
         while True:
             job = self.find_by_id(id=job_id, projection="expandJob")
             status = job.get("status", "UNKNOWN")
 
-            if status == 'COMPLETED':
+            if status == "COMPLETED":
                 return
             elif status in ["ERROR", "CANCELLED"]:
                 raise Exception(f"Job failed with status: {status}")
 
             if int(start_time_sec) - start_time_sec > timeout_sec:
-                raise Exception(f"Timeout waiting for job to complete. Current status: {status}")
+                raise Exception(
+                    f"Timeout waiting for job to complete. Current status: {status}"
+                )
 
             time.sleep(5)
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/job_event_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/job_event_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,87 +5,111 @@
 
 class JobEventApi(IteratorBaseApi):
 
     path = "/api/jobEvents/"
     type = "JOB_EVENT"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
-    def find_all(self, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_all(
+        self,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns all job events
 
         Parameters:
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): all job events
         """
-        query_vars = ['projection', 'page', 'sort', 'size', 'sort']
+        query_vars = ["projection", "page", "sort", "size", "sort"]
         query_vals = [projection, page, sort, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path,
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_by_id(self, job_event_id: str, projection: str = None):
         """
         returns a job event
 
         Parameters:
            job_event_id (str): job event id(uuid) to find
            projection (str): projection type
 
         Returns:
             (dict): job event
         """
-        query_vars = ['id', 'projection']
+        query_vars = ["id", "projection"]
         query_vals = [job_event_id, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findById",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_job_id(self, job_id: str, projection: str = None, page: int = None, size: int = None,
-                       sort: str = None):
+    def find_by_job_id(
+        self,
+        job_id: str,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns events of a job
 
         Parameters:
            job_id (str): job id(uuid) to find events
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): job events
         """
-        query_vars = ['jobId', 'projection', 'page', 'sort', 'size', 'sort']
+        query_vars = ["jobId", "projection", "page", "sort", "size", "sort"]
         query_vals = [job_id, projection, page, sort, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByJobId',
+            path=self.path + "search/findByJobId",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/message_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/message_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,16 +33,13 @@
             (dict): event
         """
 
         return self._send_event("jobprogress", event)
 
     def _send_event(self, topic, event):
 
-        header_params = {'Content-Type': 'application/json'}
-        query_params = {'type': 'topic'}
+        header_params = {"Content-Type": "application/json"}
+        query_params = {"type": "topic"}
 
         return self.aoa_client.post_request(
-            "{}/{}".format(self.path, topic),
-            header_params,
-            query_params,
-            event)
-
+            "{}/{}".format(self.path, topic), header_params, query_params, event
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/model_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/model_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,89 +6,98 @@
 
 class ModelApi(IteratorBaseApi):
 
     path = "/api/models/"
     type = "MODEL"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_by_source_id(self, source_model_id: str, projection: str = None):
         """
         returns a model by source model id taken from git repo
 
         Parameters:
            source_model_id (str): source model id(uuid) to find
            projection (str): projection type
 
         Returns:
             (dict): model
         """
-        query_vars = ['sourceId', 'projection']
+        query_vars = ["sourceId", "projection"]
         query_vals = [source_model_id, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            self.path + "search/findBySourceId",
-            self._get_header_params(),
-            query_params)
+            self.path + "search/findBySourceId", self._get_header_params(), query_params
+        )
 
     def find_all_commits(self, model_id: str, projection: str = None):
         """
         returns model commits
 
         Parameters:
            model_id (str): model id(uuid) for commits
            projection (str): projection type
 
         Returns:
             (dict): model commits
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            self.path + model_id + '/commits',
-            self._get_header_params(),
-            query_params)
+            self.path + model_id + "/commits", self._get_header_params(), query_params
+        )
 
-    def diff_commits(self, model_id: str, commit_id1: str, commit_id2: str, projection: str = None):
+    def diff_commits(
+        self, model_id: str, commit_id1: str, commit_id2: str, projection: str = None
+    ):
         """
         returns difference between model commits
 
         Parameters:
            model_id (str): model id(uuid)
            commit_id1 (str): id of commit to compare
            commit_id2 (str): id of commit to compare
            projection (str): projection type
 
         Returns:
             (str): difference between model commits
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            self.path + model_id +
-            '/diff/' + commit_id1 + '/' + commit_id2 + '/',
+            self.path + model_id + "/diff/" + commit_id1 + "/" + commit_id2 + "/",
             self._get_header_params(),
-            query_params)
+            query_params,
+        )
 
     def save(self, model: Dict[str, str]):
         """
         register a dataset
 
         Parameters:
            model (dict): external model to register
@@ -97,46 +106,49 @@
             (dict): model
         """
 
         return self.aoa_client.post_request(
             path=self.path,
             header_params=self._get_header_params(),
             query_params={},
-            body=model)
+            body=model,
+        )
 
     def train(self, model_id: str, training_request: Dict[str, str]):
         """
         train a model
 
         Parameters:
             model_id (str): model id(uuid)
             training_request (dict): request to train model
 
         Returns:
             (dict): job
         """
-        self.required_params(['datasetId'], training_request)
+        self.required_params(["datasetId"], training_request)
 
         return self.aoa_client.post_request(
-            path=self.path + model_id + '/train',
+            path=self.path + model_id + "/train",
             header_params=self._get_header_params(),
             query_params={},
-            body=training_request)
+            body=training_request,
+        )
 
     def import_byom(self, model_id: str, import_request: Dict[str, str]):
         """
         import a model version
 
         Parameters:
             model_id (str): model id(uuid)
             import_request (dict): request to import model version
 
         Returns:
             (dict): job
         """
-        self.required_params(['artefactImportId', 'externalId'], import_request)
+        self.required_params(["artefactImportId", "externalId"], import_request)
 
         return self.aoa_client.post_request(
-            path=self.path + model_id + '/import',
+            path=self.path + model_id + "/import",
             header_params=self._get_header_params(),
             query_params={},
-            body=import_request)
+            body=import_request,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/project_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/project_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,78 +7,88 @@
 class ProjectApi(IteratorBaseApi):
 
     path = "/api/projects/"
     type = "PROJECT"
 
     def _get_header_params(self):
         # The header for project id is required for the archive/unarchive method from base_api
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
-        header_vals = [self.aoa_client.project_id, self.aoa_client.project_id, 'application/json', 'application/json']
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
+        header_vals = [
+            self.aoa_client.project_id,
+            self.aoa_client.project_id,
+            "application/json",
+            "application/json",
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_by_name_like(self, name: str, projection: str = None) -> List:
         """
         returns a list of projects matching the given name
 
         Parameters:
            name (str): project name to search by
            projection (str): projection type
 
         Returns:
             (list): list of projects
         """
-        query_vars = ['name', 'projection']
+        query_vars = ["name", "projection"]
         query_vals = [name, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByName",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def save(self, project: Dict[str, str]):
         """
         create a project
 
         Parameters:
            project (dict): project to create
 
         Returns:
             (dict): project
         """
-        header_vars = ['Accept']
-        header_vals = ['application/json']
+        header_vars = ["Accept"]
+        header_vals = ["application/json"]
         header_params = self.generate_params(header_vars, header_vals)
 
         return self.aoa_client.post_request(
-            path=self.path,
-            header_params=header_params,
-            query_params={},
-            body=project)
+            path=self.path, header_params=header_params, query_params={}, body=project
+        )
 
     def update(self, project: Dict[str, str]):
         """
         update a project
 
         Parameters:
            project (dict): project to update
 
         Returns:
             (dict): project
         """
-        header_vars = ['Accept']
-        header_vals = ['application/json']
+        header_vars = ["Accept"]
+        header_vals = ["application/json"]
         header_params = self.generate_params(header_vars, header_vals)
 
         return self.aoa_client.put_request(
             path=self.path + self.aoa_client.project_id,
             header_params=header_params,
             query_params={},
-            body=project)
+            body=project,
+        )
 
     def is_archived(self, project_id: str):
         """
         returns the archived status of a project
         Parameters:
            project_id (str): project id to check archived status
         Returns:
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/trained_model_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/trained_model_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,182 +6,201 @@
 
 class TrainedModelApi(IteratorBaseApi):
 
     path = "/api/trainedModels/"
     type = "TRAINED_MODEL"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def find_dataset(self, trained_model_id: str, projection: str = None):
         """
         returns dataset of a trained model
 
         Parameters:
            trained_model_id (str): trained model id(uuid)
            projection (str): projection type
 
         Returns:
             (dict): dataset
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + trained_model_id + '/dataset',
+            path=self.path + trained_model_id + "/dataset",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_events(self, trained_model_id: str, projection: str = None):
         """
         returns trained model events
 
         Parameters:
            trained_model_id (str): trained model id(uuid)
            projection (str): projection type
 
         Returns:
             (dict): events of trained model
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + trained_model_id + '/events',
+            path=self.path + trained_model_id + "/events",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_by_model_id(self, model_id: str, projection: str = None):
         """
         returns a trained models by model id
 
         Parameters:
            model_id (str): model id(uuid) to find
            projection (str): projection type
 
         Returns:
             (dict): trained models
         """
-        query_vars = ['modelId', 'projection']
+        query_vars = ["modelId", "projection"]
         query_vals = [model_id, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByModelId',
+            path=self.path + "search/findByModelId",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_model_id_and_status(self, model_id: str, status: str, projection: str = None):
+    def find_by_model_id_and_status(
+        self, model_id: str, status: str, projection: str = None
+    ):
         """
         returns a trained models by model id
 
         Parameters:
            model_id (str): model id(uuid) to find
            status (str): model status
            projection (str): projection type
 
         Returns:
             (dict): trained models
         """
-        query_vars = ['modelId', 'status', 'projection']
+        query_vars = ["modelId", "status", "projection"]
         query_vals = [model_id, status, projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByModelIdAndStatus',
+            path=self.path + "search/findByModelIdAndStatus",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def evaluate(self, trained_model_id: str, evaluation_request: Dict[str, str]):
         """
         evaluate a model
 
         Parameters:
            trained_model_id (str): trained model id(uuid) to evaluate
            evaluation_request (dict): request to evaluate trained model
 
         Returns:
             (dict): job
         """
-        self.required_params(['datasetId'], evaluation_request)
+        self.required_params(["datasetId"], evaluation_request)
 
         return self.aoa_client.post_request(
-            path=self.path + trained_model_id + '/evaluate',
+            path=self.path + trained_model_id + "/evaluate",
             header_params=self._get_header_params(),
             query_params={},
-            body=evaluation_request)
+            body=evaluation_request,
+        )
 
     def approve(self, trained_model_id: str, comments: str):
         """
         approve a trained model
         :param trained_model_id:  model version
         :param comments: approval comments
         :return:
         """
         approve_request = dict()
-        approve_request['comments'] = comments
+        approve_request["comments"] = comments
 
         return self.aoa_client.post_request(
-            path=self.path + trained_model_id + '/approve',
+            path=self.path + trained_model_id + "/approve",
             header_params=self._get_header_params(),
             query_params={},
-            body=approve_request)
+            body=approve_request,
+        )
 
     def reject(self, trained_model_id: str, comments: str):
         """
         reject a trained model
         :param trained_model_id:  model version
         :param comments: approval comments
         :return:
         """
         reject_request = dict()
-        reject_request['comments'] = comments
+        reject_request["comments"] = comments
 
         return self.aoa_client.post_request(
-            path=self.path + trained_model_id + '/reject',
+            path=self.path + trained_model_id + "/reject",
             header_params=self._get_header_params(),
             query_params={},
-            body=reject_request)
+            body=reject_request,
+        )
 
     def deploy(self, trained_model_id: str, deploy_request: dict):
         """
         deploy a trained model
         :param trained_model_id:  model version
         :param deploy_request: deployment request
         :return:
         """
-        self.required_params(['engineType'], deploy_request)
+        self.required_params(["engineType"], deploy_request)
 
         return self.aoa_client.post_request(
-            path=self.path + trained_model_id + '/deploy',
+            path=self.path + trained_model_id + "/deploy",
             header_params=self._get_header_params(),
             query_params={},
-            body=deploy_request)
+            body=deploy_request,
+        )
 
     def retire(self, trained_model_id: str, retire_request: dict):
         """
         retire a trained model
         :param trained_model_id:  model version
         :param retire_request: retire request
         :return:
         """
-        self.required_params(['deploymentId'], retire_request)
+        self.required_params(["deploymentId"], retire_request)
 
         return self.aoa_client.post_request(
-            path=self.path + trained_model_id + '/retire',
+            path=self.path + trained_model_id + "/retire",
             header_params=self._get_header_params(),
             query_params={},
-            body=retire_request)
-
+            body=retire_request,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/trained_model_artefacts_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/trained_model_artefacts_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 from typing import List
 from aoa.api.base_api import BaseApi
 
 import requests
 import uuid
 import os
 
-SUPPORTED_BYOM_FORMATS = ["PMML","ONNX","H2O","H2O_DAI","DATAROBOT","DATAIKU"]
+SUPPORTED_BYOM_FORMATS = ["PMML", "ONNX", "H2O", "H2O_DAI", "DATAROBOT", "DATAIKU"]
+
 
 class TrainedModelArtefactsApi(BaseApi):
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            'application/json']
+            "application/json",
+            "application/json",
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
     def list_artefacts(self, trained_model_id: uuid):
         """
         returns all trained models
 
@@ -30,53 +37,60 @@
         Returns:
             (list): all trained model artefacts
         """
 
         return self.aoa_client.get_request(
             path="/api/trainedModels/{}/artefacts/listObjects".format(trained_model_id),
             header_params=self._get_header_params(),
-            query_params={})["objects"]
+            query_params={},
+        )["objects"]
 
     def get_signed_download_url(self, trained_model_id: uuid, artefact: str):
         """
         returns a signed url for the artefact
 
         Parameters:
            trained_model_id (uuid): Trained Model Id
            artefact (str): The artefact to generate the signed url for
 
         Returns:
             (str): the signed url
         """
-        query_params = self.generate_params(['objectKey'], [artefact])
+        query_params = self.generate_params(["objectKey"], [artefact])
 
         response = self.aoa_client.get_request(
-            path="/api/trainedModels/{}/artefacts/signedDownloadUrl".format(trained_model_id),
+            path="/api/trainedModels/{}/artefacts/signedDownloadUrl".format(
+                trained_model_id
+            ),
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
         return response["endpoint"]
 
     def get_signed_upload_url(self, trained_model_id: uuid, artefact: str):
         """
         returns a signed url for the artefact
 
         Parameters:
            trained_model_id (uuid): Trained Model Id
            artefact (str): The artefact to generate the signed url for
 
         Returns:
             (str): the signed url
         """
-        query_params = self.generate_params(['objectKey'], [artefact])
+        query_params = self.generate_params(["objectKey"], [artefact])
 
         response = self.aoa_client.get_request(
-            path="/api/trainedModels/{}/artefacts/signedUploadUrl".format(trained_model_id),
+            path="/api/trainedModels/{}/artefacts/signedUploadUrl".format(
+                trained_model_id
+            ),
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
         return response["endpoint"]
 
     def download_artefacts(self, trained_model_id: uuid, path: str = "."):
         """
         downloads all artefacts for the given trained model
 
@@ -85,74 +99,86 @@
            path (str): the path to download the artefacts to (default cwd)
 
         Returns:
             None
         """
 
         for artefact in self.list_artefacts(trained_model_id):
-            response = self.aoa_client.session.get(self.get_signed_download_url(trained_model_id, artefact))
+            response = self.aoa_client.session.get(
+                self.get_signed_download_url(trained_model_id, artefact)
+            )
 
             output_file = "{}/{}".format(path, artefact)
             if not os.path.exists(os.path.dirname(output_file)):
                 os.makedirs(os.path.dirname(output_file))
 
             with open(output_file, "wb") as f:
-                for chunk in response.iter_content(chunk_size=1024*1024):
+                for chunk in response.iter_content(chunk_size=1024 * 1024):
                     f.write(chunk)
 
-    def upload_artefacts(self, import_id: uuid, artefacts: List = None, artefacts_folder: str = None):
+    def upload_artefacts(
+        self, import_id: uuid, artefacts: List = None, artefacts_folder: str = None
+    ):
         """
         uploads artefacts for the given trained model
 
         Parameters:
            import_id (uuid): Trained Model Id
            artefacts (List): The artefact paths to upload (must specify this or artefacts_folder)
            artefacts_folder (str): The artefact folder (must specify this or artefacts list)
         Returns:
             None
         """
 
         if artefacts is None and artefacts_folder is None:
-            raise ValueError("Either artefacts or artefacts_folder argument must be specified")
+            raise ValueError(
+                "Either artefacts or artefacts_folder argument must be specified"
+            )
 
         if artefacts is not None:
             for artefact in artefacts:
                 object_key = os.path.basename(artefact)
                 self.__upload_artefact(artefact, object_key, import_id)
 
         else:
             for root, d, files in os.walk(artefacts_folder):
                 for file in files:
-                    object_key = os.path.relpath(os.path.join(root, file), artefacts_folder)
-                    self.__upload_artefact(os.path.join(root, file), object_key, import_id)
+                    object_key = os.path.relpath(
+                        os.path.join(root, file), artefacts_folder
+                    )
+                    self.__upload_artefact(
+                        os.path.join(root, file), object_key, import_id
+                    )
 
     def upload_byom_model(self, format: str, file_path: str, import_id: str = None):
-        """Simplified method to upload just a single file as BYOM model version. 
+        """Simplified method to upload just a single file as BYOM model version.
         File is renamed during upload, so any local filename could be used.
 
         Args:
             format (str): One of supported formats, e.g. PMML, ONNX, H2O
             file_path (str): local file path to a model artefact
             import_id (str, optional): by default import_id is randomly generated. If required, specific import_id could be provided.
 
         Raises:
             ValueError: if format string is not one of supported formats
 
         Returns:
             str: import_id that could be used by import_byom method
-        """        
+        """
         if format not in SUPPORTED_BYOM_FORMATS:
-            raise ValueError(f"The format {format} is not supported for simplified BYOM import, use `import_file` instead")
+            raise ValueError(
+                f"The format {format} is not supported for simplified BYOM import, use `import_file` instead"
+            )
 
         if not import_id:
             import_id = str(uuid.uuid4())
 
-        self.__upload_artefact(file_path,f"model.{format.lower()}",import_id)
+        self.__upload_artefact(file_path, f"model.{format.lower()}", import_id)
         return import_id
 
     def __upload_artefact(self, artefact, object_key, import_id):
-        signed_url = self.get_signed_upload_url(import_id,object_key)
+        signed_url = self.get_signed_upload_url(import_id, object_key)
         # don't use aoa_client.session here as we don't want to send auth info.
-        upload_resp = requests.put(signed_url,
-                                   data=open(artefact, 'rb'),
-                                   verify=self.aoa_client.session.verify)
+        upload_resp = requests.put(
+            signed_url, data=open(artefact, "rb"), verify=self.aoa_client.session.verify
+        )
         upload_resp.raise_for_status()
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/trained_model_event_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/trained_model_event_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,72 +5,95 @@
 
 class TrainedModelEventApi(IteratorBaseApi):
 
     path = "/api/trainedModelEvents/"
     type = "TRAINED_MODEL_EVENT"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Content-Type",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            'application/json',
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'application/hal+json',
-                'text/uri-list',
-                'application/x-spring-data-compact+json'])]
+            "application/json",
+            self.aoa_client.select_header_accept(
+                [
+                    "application/json",
+                    "application/hal+json",
+                    "text/uri-list",
+                    "application/x-spring-data-compact+json",
+                ]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
 
-    def find_all(self, projection: str = None, page: int = None, size: int = None, sort: str = None):
+    def find_all(
+        self,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns all trained model events
 
         Parameters:
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): all trained model events
         """
-        query_vars = ['projection', 'page', 'sort', 'size', 'sort']
+        query_vars = ["projection", "page", "sort", "size", "sort"]
         query_vals = [projection, page, sort, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path,
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
     def find_by_id(self, event_id: str, projection: str = None):
         """
         returns a trained model event
 
         Parameters:
            event_id (str): job id(uuid) to find
            projection (str): projection type
 
         Returns:
             (dict): trained model event
         """
-        query_vars = ['projection']
+        query_vars = ["projection"]
         query_vals = [projection]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
             path=self.path + event_id,
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_status(self, status: str, projection: str = None, page: int = None, size: int = None,
-                       sort: str = None):
+    def find_by_status(
+        self,
+        status: str,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns trained model events by status
 
         Parameters:
            status (str): status of trained model event
             Available values : TRAINED, EVALUATED, APPROVED, REJECTED, CHAMPION, DEPLOYED, RETIRED
            projection (str): projection type
@@ -78,40 +101,48 @@
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): trained model events
         """
-        query_vars = ['status', 'projection', 'page', 'sort', 'size', 'sort']
+        query_vars = ["status", "projection", "page", "sort", "size", "sort"]
         query_vals = [status, projection, page, sort, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByStatus',
+            path=self.path + "search/findByStatus",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
 
-    def find_by_trained_model_id(self, trained_model_id: str, projection: str = None,
-                                 page: int = None, size: int = None, sort: str = None):
+    def find_by_trained_model_id(
+        self,
+        trained_model_id: str,
+        projection: str = None,
+        page: int = None,
+        size: int = None,
+        sort: str = None,
+    ):
         """
         returns trained model events by trained model id
 
         Parameters:
            trained_model_id (str): trained model id(uuid)
            projection (str): projection type
            page (int): page number
            size (int): number of records in a page
            sort (str): column name and sorting order
            e.g. name?asc: sort name in ascending order, name?desc: sort name in descending order
 
         Returns:
             (dict): trained model events
         """
-        query_vars = ['trainedModelId', 'projection', 'page', 'sort', 'size', 'sort']
+        query_vars = ["trainedModelId", "projection", "page", "sort", "size", "sort"]
         query_vals = [trained_model_id, projection, page, sort, size, sort]
         query_params = self.generate_params(query_vars, query_vals)
 
         return self.aoa_client.get_request(
-            path=self.path + 'search/findByTrainedModelId',
+            path=self.path + "search/findByTrainedModelId",
             header_params=self._get_header_params(),
-            query_params=query_params)
+            query_params=query_params,
+        )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api/user_attributes_api.py` & `teradatamodelops-7.0.6rc2/aoa/api/user_attributes_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from aoa.api.iterator_base_api import BaseApi
 
+
 class UserAttributesApi(BaseApi):
 
     path = "/api/userAttributes/"
     type = "USER_ATTRIBUTES"
 
     def _get_header_params(self):
-        header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Accept']  # AOA-Project-ID kept for backwards compatibility
+        header_vars = [
+            "AOA-Project-ID",
+            "VMO-Project-ID",
+            "Accept",
+        ]  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
             self.aoa_client.project_id,
-            self.aoa_client.select_header_accept([
-                'application/json',
-                'text/plain',
-                '*/*'])]
+            self.aoa_client.select_header_accept(
+                ["application/json", "text/plain", "*/*"]
+            ),
+        ]
 
         return self.generate_params(header_vars, header_vals)
-        
+
     def get_default_connection(self):
 
         return self.aoa_client.get_request(
             path=self.path + "search/findByName",
             header_params=self._get_header_params(),
-            query_params=self.generate_params(["name"],["DEFAULT_CONNECTION"])
+            query_params=self.generate_params(["name"], ["DEFAULT_CONNECTION"]),
         )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/api_client.py` & `teradatamodelops-7.0.6rc2/aoa/api_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,23 +85,25 @@
         elif self.auth_mode == "client_credentials":
             self.__create_oauth_session_client_credentials()
 
         elif self.auth_mode == "bearer":
             self.__create_oauth_session_bearer()
 
         elif self.auth_mode is None:
-            raise Exception("ModelOps endpoint not configured. " +
-                            "Try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config.")
+            raise Exception(
+                "ModelOps endpoint not configured. "
+                + "Try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config."
+            )
 
         else:
             raise Exception(f"Auth mode: {self.auth_mode} not supported.")
 
     def __parse_aoa_config(self, **kwargs):
         if "config_file" in kwargs:
-            self.__parse_yaml(kwargs['config_file'])
+            self.__parse_yaml(kwargs["config_file"])
         else:
             if os.path.isfile(self.DEFAULT_CONFIG_FILE_PATH):
                 self.__parse_yaml(self.DEFAULT_CONFIG_FILE_PATH)
 
         self.__parse_env_variables()
         self.__parse_kwargs(**kwargs)
 
@@ -115,60 +117,86 @@
         self.ssl_verify = kwargs.get("ssl_verify", self.ssl_verify)
         self.auth_mode = kwargs.get("auth_mode", self.auth_mode)
 
         self.__check_legacy_mode()
 
         if self.auth_mode == "device_code":
             self.__client_id = kwargs.get("auth_client_id", self.__client_id)
-            self.__client_secret = kwargs.get("auth_client_secret", self.__client_secret)
+            self.__client_secret = kwargs.get(
+                "auth_client_secret", self.__client_secret
+            )
             self.__token_url = kwargs.get("auth_token_url", self.__token_url)
-            self.__device_auth_url = kwargs.get("auth_device_auth_url", self.__device_auth_url)
+            self.__device_auth_url = kwargs.get(
+                "auth_device_auth_url", self.__device_auth_url
+            )
 
         elif self.auth_mode == "client_credentials":
             self.__client_id = kwargs.get("auth_client_id", self.__client_id)
-            self.__client_secret = kwargs.get("auth_client_secret", self.__client_secret)
+            self.__client_secret = kwargs.get(
+                "auth_client_secret", self.__client_secret
+            )
             self.__token_url = kwargs.get("auth_token_url", self.__token_url)
 
         elif self.auth_mode == "bearer":
             self.__bearer_token = kwargs.get("auth_bearer", self.__bearer_token)
 
         if "verify_connection" in kwargs:
             self.verify_aoa_connection = kwargs["verify_connection"]
 
     def __parse_env_variables(self):
         self.aoa_url = os.environ.get("AOA_URL", self.aoa_url)
-        self.ssl_verify = os.environ.get("AOA_SSL_VERIFY", str(self.ssl_verify)).lower() == "true"
+        self.ssl_verify = (
+            os.environ.get("AOA_SSL_VERIFY", str(self.ssl_verify)).lower() == "true"
+        )
         self.auth_mode = os.environ.get("AOA_API_AUTH_MODE", self.auth_mode)
 
         self.__check_legacy_mode()
 
         if self.auth_mode == "device_code":
-            self.__client_id = os.environ.get("AOA_API_AUTH_CLIENT_ID", self.__client_id)
-            self.__client_secret = os.environ.get("AOA_API_AUTH_CLIENT_SECRET", self.__client_secret)
-            self.__token_url = os.environ.get("AOA_API_AUTH_TOKEN_URL", self.__token_url)
-            self.__device_auth_url = os.environ.get("AOA_API_AUTH_DEVICE_AUTH_URL", self.__device_auth_url)
+            self.__client_id = os.environ.get(
+                "AOA_API_AUTH_CLIENT_ID", self.__client_id
+            )
+            self.__client_secret = os.environ.get(
+                "AOA_API_AUTH_CLIENT_SECRET", self.__client_secret
+            )
+            self.__token_url = os.environ.get(
+                "AOA_API_AUTH_TOKEN_URL", self.__token_url
+            )
+            self.__device_auth_url = os.environ.get(
+                "AOA_API_AUTH_DEVICE_AUTH_URL", self.__device_auth_url
+            )
 
         elif self.auth_mode == "client_credentials":
-            self.__client_id = os.environ.get("AOA_API_AUTH_CLIENT_ID", self.__client_id)
-            self.__client_secret = os.environ.get("AOA_API_AUTH_CLIENT_SECRET", self.__client_secret)
-            self.__token_url = os.environ.get("AOA_API_AUTH_TOKEN_URL", self.__token_url)
+            self.__client_id = os.environ.get(
+                "AOA_API_AUTH_CLIENT_ID", self.__client_id
+            )
+            self.__client_secret = os.environ.get(
+                "AOA_API_AUTH_CLIENT_SECRET", self.__client_secret
+            )
+            self.__token_url = os.environ.get(
+                "AOA_API_AUTH_TOKEN_URL", self.__token_url
+            )
 
         elif self.auth_mode == "bearer":
-            self.__bearer_token = os.environ.get("AOA_API_AUTH_BEARER_TOKEN", self.__bearer_token)
+            self.__bearer_token = os.environ.get(
+                "AOA_API_AUTH_BEARER_TOKEN", self.__bearer_token
+            )
 
     def __check_legacy_mode(self):
         if self.auth_mode == "oauth-cc":
             self.auth_mode = "client_credentials"
         elif self.auth_mode == "oauth":
             self.auth_mode = "device_code"
 
     def __validate_url(self):
         if not self.aoa_url:
-            raise ValueError("ModelOps endpoint not configured. "
-                             "Try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config.")
+            raise ValueError(
+                "ModelOps endpoint not configured. "
+                "Try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config."
+            )
 
     def set_project_id(self, project_id: str):
         """
         set project id
 
         Parameters:
            project_id (str): project id(uuid)
@@ -191,17 +219,19 @@
         Return:
             (str): request header
         """
         if not accepts:
             return
 
         accepts = [x.lower() for x in accepts]
-        return ', '.join(accepts)
+        return ", ".join(accepts)
 
-    def get_request(self, path, header_params: Dict[str, str], query_params: Dict[str, str]):
+    def get_request(
+        self, path, header_params: Dict[str, str], query_params: Dict[str, str]
+    ):
         """
         wrapper for get request
 
         Parameters:
            path (str): url
            header_params (dict): header parameters
            query_params (dict): query parameters
@@ -213,23 +243,29 @@
         """
 
         self.__validate_url()
 
         resp = self.session.get(
             url=self.__strip_url(self.aoa_url) + path,
             headers=header_params,
-            params=query_params
+            params=query_params,
         )
 
         if resp.status_code == 404:
             return None
 
         return self.__validate_and_extract_body(resp)
 
-    def post_request(self, path, header_params: Dict[str, str], query_params: Dict[str, str], body: Dict[str, str]):
+    def post_request(
+        self,
+        path,
+        header_params: Dict[str, str],
+        query_params: Dict[str, str],
+        body: Dict[str, str],
+    ):
         """
         wrapper for post request
 
         Parameters:
            path (str): url
            header_params (dict): header parameters
            query_params (dict): query parameters
@@ -243,20 +279,26 @@
 
         self.__validate_url()
 
         resp = self.session.post(
             url=self.__strip_url(self.aoa_url) + path,
             headers=header_params,
             params=query_params,
-            data=json.dumps(body)
+            data=json.dumps(body),
         )
 
         return self.__validate_and_extract_body(resp)
 
-    def put_request(self, path, header_params: Dict[str, str], query_params: Dict[str, str], body: Dict[str, str]):
+    def put_request(
+        self,
+        path,
+        header_params: Dict[str, str],
+        query_params: Dict[str, str],
+        body: Dict[str, str],
+    ):
         """
         wrapper for put request
 
         Parameters:
            path (str): url
            header_params (dict): header parameters
            query_params (dict): query parameters
@@ -270,20 +312,26 @@
 
         self.__validate_url()
 
         resp = self.session.put(
             url=self.__strip_url(self.aoa_url) + path,
             headers=header_params,
             params=query_params,
-            data=json.dumps(body)
+            data=json.dumps(body),
         )
 
         return self.__validate_and_extract_body(resp)
 
-    def delete_request(self, path, header_params: Dict[str, str], query_params: Dict[str, str], body: Dict[str, str]):
+    def delete_request(
+        self,
+        path,
+        header_params: Dict[str, str],
+        query_params: Dict[str, str],
+        body: Dict[str, str],
+    ):
         """
         wrapper for delete request
         Parameters:
            path (str): url
            header_params (dict): header parameters
            query_params (dict): query parameters
            body (dict): request body
@@ -295,15 +343,15 @@
 
         self.__validate_url()
 
         resp = self.session.delete(
             url=self.__strip_url(self.aoa_url) + path,
             headers=header_params,
             params=query_params,
-            data=json.dumps(body)
+            data=json.dumps(body),
         )
 
         return self.__validate_and_extract_body(resp)
 
     def __validate_and_extract_body(self, resp):
         try:
             resp.raise_for_status()
@@ -315,27 +363,35 @@
 
         try:
             return resp.json()
         except ValueError:
             return resp.text
 
     def __strip_url(self, url):
-        return url.rstrip('/')
+        return url.rstrip("/")
 
     def __create_oauth_session_device_code(self):
         self.logger.debug("Configuring oauth with device_code grant")
 
-        if self.__client_id is None or self.__token_url is None or self.__device_auth_url is None:
-            raise Exception("Missing CLI configuration.\n" +
-                            "Please (re)copy the CLI configuration from " +
-                            "ModelOps UI -> Session Details -> CLI Config\n")
+        if (
+            self.__client_id is None
+            or self.__token_url is None
+            or self.__device_auth_url is None
+        ):
+            raise Exception(
+                "Missing CLI configuration.\n"
+                + "Please (re)copy the CLI configuration from "
+                + "ModelOps UI -> Session Details -> CLI Config\n"
+            )
 
         token = None
         if os.path.exists(self.DEFAULT_TOKEN_CACHE_FILE_PATH):
-            self.logger.debug(f"Loading cached token data from {self.DEFAULT_TOKEN_CACHE_FILE_PATH}")
+            self.logger.debug(
+                f"Loading cached token data from {self.DEFAULT_TOKEN_CACHE_FILE_PATH}"
+            )
             with open(self.DEFAULT_TOKEN_CACHE_FILE_PATH, "r") as f:
                 token = json.load(f)
 
         if not token:
             self.session = requests.session()
             self.__set_session_tls()
             token = self.__get_device_code()
@@ -349,79 +405,95 @@
             if hasattr(self, "session"):
                 session.verify = self.session.verify
                 self.session = session
             else:
                 self.session = session
                 self.__set_session_tls()
 
-            self.session.refresh_token(token_url=self.__token_url,
-                                       refresh_token=token["refresh_token"],
-                                       auth=HTTPBasicAuth(self.__client_id, self.__client_secret),
-                                       verify=self.ssl_verify)
+            self.session.refresh_token(
+                token_url=self.__token_url,
+                refresh_token=token["refresh_token"],
+                auth=HTTPBasicAuth(self.__client_id, self.__client_secret),
+                verify=self.ssl_verify,
+            )
 
             with open(self.DEFAULT_TOKEN_CACHE_FILE_PATH, "w") as f:
                 json.dump(token, f)
 
         else:
-            raise Exception(f"Token does not contain access_token. Received {self.token}")
+            raise Exception(
+                f"Token does not contain access_token. Received {self.token}"
+            )
 
     def __create_oauth_session_client_credentials(self):
         self.logger.debug("Configuring oauth with client_credentials grant")
 
-        if self.__client_id is None or self.__client_secret is None or self.__token_url is None:
-            raise Exception("AOA_API_AUTH_CLIENT_ID, AOA_API_AUTH_CLIENT_SECRET, "
-                            "AOA_API_AUTH_TOKEN_URL must be defined "
-                            "with AOA_API_AUTH_MODE of 'client_credentials'")
+        if (
+            self.__client_id is None
+            or self.__client_secret is None
+            or self.__token_url is None
+        ):
+            raise Exception(
+                "AOA_API_AUTH_CLIENT_ID, AOA_API_AUTH_CLIENT_SECRET, "
+                "AOA_API_AUTH_TOKEN_URL must be defined "
+                "with AOA_API_AUTH_MODE of 'client_credentials'"
+            )
 
-        self.session = OAuth2Session(client=BackendApplicationClient(client_id=self.__client_id))
+        self.session = OAuth2Session(
+            client=BackendApplicationClient(client_id=self.__client_id)
+        )
         self.__set_session_tls()
-        self.session.fetch_token(token_url=self.__token_url,
-                                 auth=HTTPBasicAuth(self.__client_id, self.__client_secret),
-                                 verify=self.ssl_verify)
+        self.session.fetch_token(
+            token_url=self.__token_url,
+            auth=HTTPBasicAuth(self.__client_id, self.__client_secret),
+            verify=self.ssl_verify,
+        )
 
     def __create_oauth_session_bearer(self):
         self.session = requests.session()
         self.session.headers.update({"Authorization": self.__bearer_token})
         self.__set_session_tls()
 
     def __get_device_code(self):
         device_code_response = self.session.post(
             self.__device_auth_url,
-            data={
-                "client_id": self.__client_id,
-                "scope": "openid profile"
-            }
+            data={"client_id": self.__client_id, "scope": "openid profile"},
         )
 
         if device_code_response.status_code != 200:
-            raise Exception(f"Error generating the device code. Received code {device_code_response.status_code}.")
+            raise Exception(
+                f"Error generating the device code. Received code {device_code_response.status_code}."
+            )
 
         device_code_data = device_code_response.json()
-        print("1. On your computer or mobile device navigate to: ", device_code_data['verification_uri_complete'])
+        print(
+            "1. On your computer or mobile device navigate to: ",
+            device_code_data["verification_uri_complete"],
+        )
         print("2. Enter the following code: ", device_code_data["user_code"])
 
         authenticated = False
         while not authenticated:
             print("Waiting for device code to be authorized...")
             token_response = self.session.post(
                 self.__token_url,
                 data={
                     "grant_type": "urn:ietf:params:oauth:grant-type:device_code",
                     "device_code": device_code_data["device_code"],
-                    "client_id": self.__client_id
-                }
+                    "client_id": self.__client_id,
+                },
             )
 
             token_data = token_response.json()
             if token_response.status_code == 200:
                 authenticated = True
 
             elif "error" in token_data:
                 if token_data["error"] in ("authorization_pending", "slow_down"):
-                    time.sleep(device_code_data['interval'])
+                    time.sleep(device_code_data["interval"])
                 else:
                     raise Exception(token_data["error_description"])
 
             else:
                 raise Exception(f"Bad response code {token_response.status_code}")
 
         return token_data
@@ -429,23 +501,26 @@
     def __set_session_tls(self):
         self.session.verify = self.ssl_verify
         if self.ssl_verify:
             self.__chase_tls_cert_chain()
         else:
             from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
-            self.logger.warning("Certificate validation disabled. Adding certificate verification is strongly advised")
+            self.logger.warning(
+                "Certificate validation disabled. Adding certificate verification is strongly advised"
+            )
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
     def __chase_tls_cert_chain(self):
         if self.aoa_url.startswith("https") and not (
-                "REQUESTS_CA_BUNDLE" in os.environ or "CURL_CA_BUNDLE" in os.environ):
+            "REQUESTS_CA_BUNDLE" in os.environ or "CURL_CA_BUNDLE" in os.environ
+        ):
 
             try:
-                if re.search('http|https', self.aoa_url):
+                if re.search("http|https", self.aoa_url):
                     requests.get(f"{self.aoa_url}/admin/info")
                 else:
                     raise Exception("Invalid AOA_URL")
             except requests.exceptions.SSLError:
                 from aia import AIASession
                 from tempfile import NamedTemporaryFile
 
@@ -462,10 +537,12 @@
                     ca_data = aia_session.cadata_from_url(self.aoa_url)
                     with NamedTemporaryFile("w", delete=False) as pem_file:
                         pem_file.write(ca_data)
                         pem_file.flush()
 
                     self.session.verify = pem_file.name
                 except aia.InvalidCAError:
-                    raise Exception("Attempted to find trusted root certificate via AIA chasing but not found.\n"
-                                    "Please configure REQUESTS_CA_BUNDLE or CURL_CA_BUNDLE.\n"
-                                    "Alternatively, to ignore TLS validation (not advised), export AOA_SSL_VERIFY=false")
+                    raise Exception(
+                        "Attempted to find trusted root certificate via AIA chasing but not found.\n"
+                        "Please configure REQUESTS_CA_BUNDLE or CURL_CA_BUNDLE.\n"
+                        "Alternatively, to ignore TLS validation (not advised), export AOA_SSL_VERIFY=false"
+                    )
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/base_model.py` & `teradatamodelops-7.0.6rc2/aoa/cli/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def get_model_ids(model_path, rtn_val=False):
         catalog = {}
         index = 0
         model_ids = "Use one of the following models\n"
 
         for model_folder in os.listdir(model_path):
             if os.path.exists(model_path + model_folder + "/model.json"):
-                with open(model_path + model_folder + "/model.json", 'r') as f:
+                with open(model_path + model_folder + "/model.json", "r") as f:
                     model_definition = json.load(f)
                     catalog[index] = model_definition
                     index += 1
 
         for key in catalog:
             model_ids += "{1}: {0}\n".format(catalog[key]["id"], catalog[key]["name"])
 
@@ -35,15 +35,15 @@
     def get_model_folders(model_path, rtn_val=False):
         catalog = {}
         index = 0
         model_ids = "Use one of the following models\n"
 
         for model_folder in os.listdir(model_path):
             if os.path.exists(model_path + model_folder + "/model.json"):
-                with open(model_path + model_folder + "/model.json", 'r') as f:
+                with open(model_path + model_folder + "/model.json", "r") as f:
                     model_definition = json.load(f)
                     catalog[index] = model_definition
                     index += 1
 
         for key in catalog:
             model_ids += "{1}: {0}\n".format(model_folder, catalog[key]["name"])
 
@@ -52,28 +52,28 @@
 
         raise ValueError(model_ids)
 
     @staticmethod
     def get_model_folder(model_path: str, model_id: str):
         for model_folder in os.listdir(model_path):
             if os.path.exists(model_path + model_folder + "/model.json"):
-                with open(model_path + model_folder + "/model.json", 'r') as f:
+                with open(model_path + model_folder + "/model.json", "r") as f:
                     model_definition = json.load(f)
                     if model_definition["id"] == model_id:
                         return model_folder
 
         raise ValueError("Could not find model path for model_id: {}".format(model_id))
 
     def __get_model_varargs(self, model_id):
         return {
             "model_id": model_id,
             "model_version": "cli",
             "model_table": "aoa_models_cli",
             "project_id": self.__get_project_id(),
-            "job_id": "cli"
+            "job_id": "cli",
         }
 
     def __get_project_id(self):
         path = os.path.join(self.repo_manager.base_path, ".aoa/config.yaml")
         with open(path, "r") as handle:
             return yaml.safe_load(handle)["project_id"]
 
@@ -81,17 +81,18 @@
         with open(filename) as f:
             template = Template(f.read(), autoescape=True)
 
         return template.render(jinja_ctx)
 
     def __execute_sql_script(self, filename, jinja_ctx):
         from ..util.connections import execute_sql
+
         script = self.__template_sql_script(filename, jinja_ctx)
 
-        stms = script.split(';')
+        stms = script.split(";")
 
         for stm in stms:
             stm = stm.strip()
             if stm:
                 logging.info("Executing statement: {}".format(stm))
 
                 try:
@@ -101,15 +102,18 @@
                         logging.warning("Ignoring DROP statement exception")
                     else:
                         raise e
 
     def __get_engine(self, model_definition, mode):
         if "automation" in model_definition:
 
-            if mode in model_definition["automation"] and "engine" in model_definition["automation"][mode]:
+            if (
+                mode in model_definition["automation"]
+                and "engine" in model_definition["automation"][mode]
+            ):
                 return model_definition["automation"][mode]["engine"]
 
             # legacy
             if "trainingEngine" in model_definition["automation"]:
                 return model_definition["automation"]["trainingEngine"]
 
         return model_definition["language"]
@@ -120,8 +124,7 @@
 
         with tempfile.NamedTemporaryFile(delete=False) as fp:
             fp.write(json.dumps(data_conf).encode())
 
         pkg_path, _ = os.path.split(__file__)
         cmd = f"{pkg_path}/run_model.R {model_id} {self.__get_project_id()} {mode} {fp.name} {model_dir}"
         subprocess.check_call(cmd, shell=True)
-
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/evaluate_model.py` & `teradatamodelops-7.0.6rc2/aoa/cli/evaluate_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,103 +10,158 @@
 
 class EvaluateModel(BaseModel):
 
     def __init__(self, repo_manager):
         super().__init__(repo_manager)
         self.logger = logging.getLogger(__name__)
 
-    def evaluate_model_local(self,
-                             model_id: str,
-                             base_path: str,
-                             rendered_dataset: dict):
-
-        base_path = self.repo_manager.model_catalog_path if base_path is None else os.path.join(base_path, '')
-        model_definitions_path = base_path + 'model_definitions/'
+    def evaluate_model_local(
+        self, model_id: str, base_path: str, rendered_dataset: dict
+    ):
+
+        base_path = (
+            self.repo_manager.model_catalog_path
+            if base_path is None
+            else os.path.join(base_path, "")
+        )
+        model_definitions_path = base_path + "model_definitions/"
 
         if not os.path.exists(model_definitions_path):
-            raise ValueError("model directory {0} does not exist".format(model_definitions_path))
+            raise ValueError(
+                "model directory {0} does not exist".format(model_definitions_path)
+            )
 
         model_artefacts_path = ".artefacts/{}".format(model_id)
         model_evaluation_path = "{}/evaluation".format(model_artefacts_path)
 
         if not os.path.exists("{}/output".format(model_artefacts_path)):
             raise ValueError("You must run training before trying to run evaluation.")
 
         if os.path.exists(model_evaluation_path):
-            self.logger.debug("Cleaning local model evaluation path: {}".format(model_evaluation_path))
+            self.logger.debug(
+                "Cleaning local model evaluation path: {}".format(model_evaluation_path)
+            )
             shutil.rmtree(model_evaluation_path)
 
         os.makedirs("{}/output".format(model_evaluation_path))
 
         try:
             self.__cleanup()
 
             os.makedirs("./artifacts")
 
-            os.symlink("../{}/output/".format(model_artefacts_path), "./artifacts/input", target_is_directory=True)
-            os.symlink("../{}/evaluation/output/".format(model_artefacts_path), "./artifacts/output", target_is_directory=True)
-
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
+            os.symlink(
+                "../{}/output/".format(model_artefacts_path),
+                "./artifacts/input",
+                target_is_directory=True,
+            )
+            os.symlink(
+                "../{}/evaluation/output/".format(model_artefacts_path),
+                "./artifacts/output",
+                target_is_directory=True,
+            )
+
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
 
-            with open(model_dir + "/model.json", 'r') as f:
+            with open(model_dir + "/model.json", "r") as f:
                 model_definition = json.load(f)
 
-            with open(model_dir + "/config.json", 'r') as f:
+            with open(model_dir + "/config.json", "r") as f:
                 model_conf = json.load(f)
 
             self.logger.info("Loading and executing model code")
 
             cli_model_kargs = self._BaseModel__get_model_varargs(model_id)
 
-            context = ModelContext(dataset_info=DatasetInfo.from_dict(rendered_dataset),
-                                   hyperparams=model_conf["hyperParameters"],
-                                   artifact_input_path="artifacts/input",
-                                   artifact_output_path="artifacts/output",
-                                   **cli_model_kargs)
+            context = ModelContext(
+                dataset_info=DatasetInfo.from_dict(rendered_dataset),
+                hyperparams=model_conf["hyperParameters"],
+                artifact_input_path="artifacts/input",
+                artifact_output_path="artifacts/output",
+                **cli_model_kargs,
+            )
 
             engine = self._BaseModel__get_engine(model_definition, "evaluation")
             if engine == "python":
                 sys.path.append(model_dir)
                 if os.path.isfile("{}/model_modules/evaluation.py".format(model_dir)):
-                    evaluation = importlib.import_module(".evaluation", package="model_modules")
+                    evaluation = importlib.import_module(
+                        ".evaluation", package="model_modules"
+                    )
                 else:
-                    logging.debug("No evaluation.py found. Using scoring.py -> evaluate")
-                    evaluation = importlib.import_module(".scoring", package="model_modules")
-
-                evaluation.evaluate(context=context,
-                                    data_conf=rendered_dataset,
-                                    model_conf=model_conf,
-                                    **cli_model_kargs)
+                    logging.debug(
+                        "No evaluation.py found. Using scoring.py -> evaluate"
+                    )
+                    evaluation = importlib.import_module(
+                        ".scoring", package="model_modules"
+                    )
+
+                evaluation.evaluate(
+                    context=context,
+                    data_conf=rendered_dataset,
+                    model_conf=model_conf,
+                    **cli_model_kargs,
+                )
 
             elif engine == "sql":
-                self.__evaluate_sql(context, model_dir, rendered_dataset, model_conf, **cli_model_kargs)
+                self.__evaluate_sql(
+                    context, model_dir, rendered_dataset, model_conf, **cli_model_kargs
+                )
 
             elif engine == "R":
-                self._BaseModel__run_r_model(model_id, model_dir, rendered_dataset, "evaluate")
+                self._BaseModel__run_r_model(
+                    model_id, model_dir, rendered_dataset, "evaluate"
+                )
 
             else:
-                raise Exception("Unsupported language: {}".format(model_definition["language"]))
+                raise Exception(
+                    "Unsupported language: {}".format(model_definition["language"])
+                )
 
             if os.path.exists("{}/evaluation/output/".format(model_artefacts_path)):
-                self.logger.info("Artefacts can be found in: {}/evaluation/output/".format(model_artefacts_path))
+                self.logger.info(
+                    "Artefacts can be found in: {}/evaluation/output/".format(
+                        model_artefacts_path
+                    )
+                )
             else:
-                self.logger.info("Artefacts can be found in: {}".format(model_artefacts_path))
-
-            if os.path.exists("{}/evaluation/output/metrics.json".format(model_artefacts_path)):
-                self.logger.info("Evaluation metrics can be found in: {}/evaluation/output/metrics.json".format(model_artefacts_path))
+                self.logger.info(
+                    "Artefacts can be found in: {}".format(model_artefacts_path)
+                )
+
+            if os.path.exists(
+                "{}/evaluation/output/metrics.json".format(model_artefacts_path)
+            ):
+                self.logger.info(
+                    "Evaluation metrics can be found in: {}/evaluation/output/metrics.json".format(
+                        model_artefacts_path
+                    )
+                )
 
             if os.path.exists("{}/evaluation.json".format(model_artefacts_path)):
-                self.logger.info("Evaluation metrics can be found in: {}/evaluation.json".format(model_artefacts_path))
+                self.logger.info(
+                    "Evaluation metrics can be found in: {}/evaluation.json".format(
+                        model_artefacts_path
+                    )
+                )
 
             self.__cleanup()
         except ModuleNotFoundError:
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
             self.__cleanup()
-            self.logger.error("Missing required python module, try running following command first:")
-            self.logger.error("pip install -r {}/model_modules/requirements.txt".format(model_dir))
+            self.logger.error(
+                "Missing required python module, try running following command first:"
+            )
+            self.logger.error(
+                "pip install -r {}/model_modules/requirements.txt".format(model_dir)
+            )
             raise
         except:
             self.__cleanup()
             self.logger.exception("Exception running model code")
             raise
 
     def __cleanup(self):
@@ -128,15 +183,15 @@
         sql_file = model_dir + "/model_modules/evaluation.sql"
         jinja_ctx = {
             "context": context,
             "data_conf": data_conf,
             "model_conf": model_conf,
             "model_table": kwargs.get("model_table"),
             "model_version": kwargs.get("model_version"),
-            "model_id": kwargs.get("model_id")
+            "model_id": kwargs.get("model_id"),
         }
 
         self._BaseModel__execute_sql_script(sql_file, jinja_ctx)
 
         self.logger.info("Finished evaluation")
 
         stats = DataFrame(data_conf["metrics_table"]).to_pandas(all_rows=True)
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/repo_manager.py` & `teradatamodelops-7.0.6rc2/aoa/cli/repo_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,22 @@
 
 class RepoManager(object):
 
     def __init__(self, base_path: str):
         self.base_path = base_path
         self.logger = logging.getLogger(__name__)
 
-    def add_model(self, model_id: str, model_name: str, model_desc: str, template: str, base_path: str = None):
+    def add_model(
+        self,
+        model_id: str,
+        model_name: str,
+        model_desc: str,
+        template: str,
+        base_path: str = None,
+    ):
 
         base_path = self.base_path if base_path is None else base_path
         model_path = os.path.join(base_path, "model_definitions")
 
         if not os.path.isdir(model_path):
             raise ValueError("model directory {0} does not exist".format(model_path))
 
@@ -32,29 +39,35 @@
             model["name"] = model_name
             model["description"] = model_desc
 
             name_path = model_name.strip().lower().replace(" ", "_")
 
             target_path = os.path.join(model_path, name_path)
             if os.path.isdir(target_path):
-                raise ValueError("Model path {} already exists, please try another model name".format(name_path))
+                raise ValueError(
+                    "Model path {} already exists, please try another model name".format(
+                        name_path
+                    )
+                )
 
             shutil.copytree(template, target_path)
 
-            with open(os.path.join(target_path, "model.json"), 'w') as t:
+            with open(os.path.join(target_path, "model.json"), "w") as t:
                 json.dump(model, t, indent=4)
 
     @staticmethod
-    def clone_repository(url, path, branch: str = 'master'):
+    def clone_repository(url, path, branch: str = "master"):
         repo = Repo.clone_from(url, path)
         repo.git.checkout(branch)
 
     def get_templates(self, source_path: str = None):
 
-        source_path = self.base_path if source_path is None else os.path.join(source_path, '')
+        source_path = (
+            self.base_path if source_path is None else os.path.join(source_path, "")
+        )
         model_path = os.path.join(source_path, "model_definitions")
 
         # if no models / not models repo, return empty.
         if not os.path.isdir(model_path):
             return {}
 
         templates = {}
@@ -63,31 +76,35 @@
             model_metadata_dir = os.path.join(model_path, model)
             model_metadata_file = os.path.join(model_metadata_dir, "model.json")
             if os.path.isfile(model_metadata_file):
                 with open(model_metadata_file, "r") as f:
                     model_metadata = json.load(f)
                     if not model_metadata["language"] in templates:
                         templates[model_metadata["language"]] = {}
-                    templates[model_metadata["language"]][model_metadata["id"]] = [model_metadata["name"],
-                                                                                   model_metadata_dir]
+                    templates[model_metadata["language"]][model_metadata["id"]] = [
+                        model_metadata["name"],
+                        model_metadata_dir,
+                    ]
 
         return templates
 
     def init_model_directory(self, path: str = None):
-        logging.info('Creating model directory')
+        logging.info("Creating model directory")
         if path is None:
-            path = os.path.join(os.path.abspath(os.getcwd()), '')
+            path = os.path.join(os.path.abspath(os.getcwd()), "")
 
-        self.logger.info('Creating model definitions')
+        self.logger.info("Creating model definitions")
 
-        src = os.path.join(os.path.split(__file__)[0], '') + 'metadata_files'
+        src = os.path.join(os.path.split(__file__)[0], "") + "metadata_files"
         src_files = os.listdir(src)
         for file_name in src_files:
             full_file_name = os.path.join(src, file_name)
-            if os.path.isfile(full_file_name) and not os.path.exists(os.path.join(path, file_name)):
+            if os.path.isfile(full_file_name) and not os.path.exists(
+                os.path.join(path, file_name)
+            ):
                 shutil.copy(full_file_name, path)
 
         Path(path + "model_definitions/").mkdir(parents=True, exist_ok=True)
 
         self.logger.info("model directory initialized at {0}".format(path))
 
     def read_repo_config(self):
@@ -101,15 +118,15 @@
 
     def write_repo_config(self, config, path=None):
         path = path if path else self.base_path
         config_dir = os.path.join(path, ".aoa")
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         config_file = "{}/config.yaml".format(config_dir)
 
-        with open(config_file, 'w+') as f:
+        with open(config_file, "w+") as f:
             yaml.dump(config, f, default_flow_style=False)
 
     def repo_config_exists(self, repo_path=None):
         path = repo_path if repo_path else self.base_path
         return Path(os.path.join(path, ".aoa")).is_file()
 
     def train(self, model_id: str, data_conf: dict):
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/run_model.R` & `teradatamodelops-7.0.6rc2/aoa/cli/run_model.R`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/score_model.py` & `teradatamodelops-7.0.6rc2/aoa/cli/score_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,80 +10,109 @@
 
 class ScoreModel(BaseModel):
 
     def __init__(self, repo_manager):
         super().__init__(repo_manager)
         self.logger = logging.getLogger(__name__)
 
-    def batch_score_model_local(self,
-                                model_id: str = None,
-                                base_path: str = None,
-                                rendered_dataset: dict = None):
-        base_path = self.repo_manager.model_catalog_path if base_path is None else os.path.join(base_path, '')
-        model_definitions_path = base_path + 'model_definitions/'
+    def batch_score_model_local(
+        self, model_id: str = None, base_path: str = None, rendered_dataset: dict = None
+    ):
+        base_path = (
+            self.repo_manager.model_catalog_path
+            if base_path is None
+            else os.path.join(base_path, "")
+        )
+        model_definitions_path = base_path + "model_definitions/"
 
         if not os.path.exists(model_definitions_path):
-            raise ValueError("model directory {0} does not exist".format(model_definitions_path))
+            raise ValueError(
+                "model directory {0} does not exist".format(model_definitions_path)
+            )
 
         model_artefacts_path = ".artefacts/{}".format(model_id)
 
         if not os.path.exists("{}/output".format(model_artefacts_path)):
             raise ValueError("You must run training before trying to run scoring.")
 
         try:
             self.__cleanup()
 
             os.makedirs("./artifacts")
 
-            os.symlink("../{}/output/".format(model_artefacts_path), "./artifacts/input", target_is_directory=True)
-            os.symlink("../{}/output/".format(model_artefacts_path), "./artifacts/output", target_is_directory=True)
+            os.symlink(
+                "../{}/output/".format(model_artefacts_path),
+                "./artifacts/input",
+                target_is_directory=True,
+            )
+            os.symlink(
+                "../{}/output/".format(model_artefacts_path),
+                "./artifacts/output",
+                target_is_directory=True,
+            )
+
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
 
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
-
-            with open(model_dir + "/model.json", 'r') as f:
+            with open(model_dir + "/model.json", "r") as f:
                 model_definition = json.load(f)
 
-            with open(model_dir + "/config.json", 'r') as f:
+            with open(model_dir + "/config.json", "r") as f:
                 model_conf = json.load(f)
 
             self.logger.info("Loading and executing model code")
 
             cli_model_kargs = self._BaseModel__get_model_varargs(model_id)
 
-            context = ModelContext(dataset_info=DatasetInfo.from_dict(rendered_dataset),
-                                   hyperparams=model_conf["hyperParameters"],
-                                   artifact_input_path="artifacts/input",
-                                   artifact_output_path="artifacts/output",
-                                   **cli_model_kargs)
+            context = ModelContext(
+                dataset_info=DatasetInfo.from_dict(rendered_dataset),
+                hyperparams=model_conf["hyperParameters"],
+                artifact_input_path="artifacts/input",
+                artifact_output_path="artifacts/output",
+                **cli_model_kargs,
+            )
 
             engine = self._BaseModel__get_engine(model_definition, "deployment")
             if engine == "python" or engine == "pyspark":
                 sys.path.append(model_dir)
                 scoring = importlib.import_module(".scoring", package="model_modules")
 
-                scoring.score(context=context,
-                              data_conf=rendered_dataset,
-                              model_conf=model_conf,
-                              **cli_model_kargs)
+                scoring.score(
+                    context=context,
+                    data_conf=rendered_dataset,
+                    model_conf=model_conf,
+                    **cli_model_kargs,
+                )
 
             elif engine == "sql":
                 raise Exception("not supported")
 
             elif engine == "R":
-                self._BaseModel__run_r_model(model_id, model_dir, rendered_dataset, "score.batch")
+                self._BaseModel__run_r_model(
+                    model_id, model_dir, rendered_dataset, "score.batch"
+                )
 
             else:
-                raise Exception("Unsupported language: {}".format(model_definition["language"]))
+                raise Exception(
+                    "Unsupported language: {}".format(model_definition["language"])
+                )
 
             self.__cleanup()
         except ModuleNotFoundError:
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
             self.__cleanup()
-            self.logger.error("Missing required python module, try running following command first:")
-            self.logger.error("pip install -r {}/model_modules/requirements.txt".format(model_dir))
+            self.logger.error(
+                "Missing required python module, try running following command first:"
+            )
+            self.logger.error(
+                "pip install -r {}/model_modules/requirements.txt".format(model_dir)
+            )
             raise
         except:
             self.__cleanup()
             self.logger.exception("Exception running model code")
             raise
 
     def __cleanup(self):
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/cli/train_model.py` & `teradatamodelops-7.0.6rc2/aoa/cli/train_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,81 +10,104 @@
 
 class TrainModel(BaseModel):
 
     def __init__(self, repo_manager):
         super().__init__(repo_manager)
         self.logger = logging.getLogger(__name__)
 
-    def train_model_local(self,
-                          model_id: str,
-                          base_path: str,
-                          rendered_dataset: dict):
+    def train_model_local(self, model_id: str, base_path: str, rendered_dataset: dict):
 
-        base_path = self.repo_manager.model_catalog_path if base_path is None else os.path.join(base_path, '')
-        model_definitions_path = base_path + 'model_definitions/'
+        base_path = (
+            self.repo_manager.model_catalog_path
+            if base_path is None
+            else os.path.join(base_path, "")
+        )
+        model_definitions_path = base_path + "model_definitions/"
 
         if not os.path.exists(model_definitions_path):
-            raise ValueError("model directory {0} does not exist".format(model_definitions_path))
+            raise ValueError(
+                "model directory {0} does not exist".format(model_definitions_path)
+            )
 
         model_artefacts_path = ".artefacts/{}/".format(model_id)
         model_artefacts_output_path = ".artefacts/{}/output/".format(model_id)
         if os.path.exists(model_artefacts_path):
-            self.logger.debug("Cleaning local model artefact path: {}".format(model_artefacts_path))
+            self.logger.debug(
+                "Cleaning local model artefact path: {}".format(model_artefacts_path)
+            )
             shutil.rmtree(model_artefacts_path)
 
         os.makedirs(model_artefacts_output_path)
 
         try:
             if os.path.exists("./artifacts"):
                 os.remove("./artifacts")
 
             os.symlink(model_artefacts_path, "./artifacts", target_is_directory=True)
 
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
 
-            with open(model_dir + "/model.json", 'r') as f:
+            with open(model_dir + "/model.json", "r") as f:
                 model_definition = json.load(f)
 
-            with open(model_dir + "/config.json", 'r') as f:
+            with open(model_dir + "/config.json", "r") as f:
                 model_conf = json.load(f)
 
             self.logger.info("Loading and executing model code")
 
             cli_model_kargs = self._BaseModel__get_model_varargs(model_id)
 
-            context = ModelContext(dataset_info=DatasetInfo.from_dict(rendered_dataset),
-                                   hyperparams=model_conf["hyperParameters"],
-                                   artifact_output_path="artifacts/output",
-                                   **cli_model_kargs)
+            context = ModelContext(
+                dataset_info=DatasetInfo.from_dict(rendered_dataset),
+                hyperparams=model_conf["hyperParameters"],
+                artifact_output_path="artifacts/output",
+                **cli_model_kargs,
+            )
 
             engine = self._BaseModel__get_engine(model_definition, "training")
             if engine == "python":
                 sys.path.append(model_dir)
                 training = importlib.import_module(".training", package="model_modules")
-                training.train(context=context,
-                               data_conf=rendered_dataset,
-                               model_conf=model_conf,
-                               **cli_model_kargs)
+                training.train(
+                    context=context,
+                    data_conf=rendered_dataset,
+                    model_conf=model_conf,
+                    **cli_model_kargs,
+                )
 
             elif engine == "sql":
-                self.__train_sql(context, model_dir, rendered_dataset, model_conf, **cli_model_kargs)
+                self.__train_sql(
+                    context, model_dir, rendered_dataset, model_conf, **cli_model_kargs
+                )
 
             elif engine == "R":
-                self._BaseModel__run_r_model(model_id, model_dir, rendered_dataset, "train")
+                self._BaseModel__run_r_model(
+                    model_id, model_dir, rendered_dataset, "train"
+                )
 
             else:
                 raise Exception("Unsupported engine: {}".format(engine))
 
-            self.logger.info("Artefacts can be found in: {}".format(model_artefacts_output_path))
+            self.logger.info(
+                "Artefacts can be found in: {}".format(model_artefacts_output_path)
+            )
             self.__cleanup()
         except ModuleNotFoundError:
-            model_dir = model_definitions_path + BaseModel.get_model_folder(model_definitions_path, model_id)
+            model_dir = model_definitions_path + BaseModel.get_model_folder(
+                model_definitions_path, model_id
+            )
             self.__cleanup()
-            self.logger.error("Missing required python module, try running following command first:")
-            self.logger.error("pip install -r {}/model_modules/requirements.txt".format(model_dir))
+            self.logger.error(
+                "Missing required python module, try running following command first:"
+            )
+            self.logger.error(
+                "pip install -r {}/model_modules/requirements.txt".format(model_dir)
+            )
             raise
         except:
             self.__cleanup()
             self.logger.exception("Exception running model code")
             raise
 
     def __cleanup(self):
@@ -104,15 +127,15 @@
         sql_file = model_dir + "/model_modules/training.sql"
         jinja_ctx = {
             "context": context,
             "data_conf": data_conf,
             "model_conf": model_conf,
             "model_table": kwargs.get("model_table"),
             "model_version": kwargs.get("model_version"),
-            "model_id": kwargs.get("model_id")
+            "model_id": kwargs.get("model_id"),
         }
 
         self._BaseModel__execute_sql_script(sql_file, jinja_ctx)
 
         remove_context()
 
         self.logger.info("Finished training")
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/context/model_context.py` & `teradatamodelops-7.0.6rc2/aoa/context/model_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 from typing import List, Dict
 import os
 
 
 class DatasetInfo(object):
 
-    def __init__(self, sql: str = None,
-                 entity_key: str = None,
-                 feature_names: List = None,
-                 target_names: List = None,
-                 feature_metadata: Dict = None,
-                 predictions: Dict = None,
-                 legacy_data_conf: Dict = None,
-                 **kwargs):
+    def __init__(
+        self,
+        sql: str = None,
+        entity_key: str = None,
+        feature_names: List = None,
+        target_names: List = None,
+        feature_metadata: Dict = None,
+        predictions: Dict = None,
+        legacy_data_conf: Dict = None,
+        **kwargs,
+    ):
         self.sql = sql
         self.entity_key = entity_key
         self.feature_names = feature_names
         self.target_names = target_names
         self.legacy_data_conf = legacy_data_conf
 
         if feature_metadata:
             self.feature_metadata_database = feature_metadata.get("database")
             self.feature_metadata_table = feature_metadata.get("table")
-            self.feature_metadata_monitoring_group = feature_metadata.get("monitoringGroup", "default")
+            self.feature_metadata_monitoring_group = feature_metadata.get(
+                "monitoringGroup", "default"
+            )
 
         if predictions:
             self.predictions_database = predictions.get("database")
             self.predictions_table = predictions.get("table")
 
     @classmethod
     def from_dict(cls, rendered_dataset: Dict):
         if "type" in rendered_dataset and rendered_dataset["type"] == "CatalogBody":
-            return cls(sql=rendered_dataset.get("sql"),
-                       entity_key=rendered_dataset.get("entityKey"),
-                       feature_names=rendered_dataset.get("featureNames"),
-                       feature_metadata=rendered_dataset.get("featureMetadata"),
-                       predictions=rendered_dataset.get("predictions"),
-                       target_names=rendered_dataset.get("targetNames"))
+            return cls(
+                sql=rendered_dataset.get("sql"),
+                entity_key=rendered_dataset.get("entityKey"),
+                feature_names=rendered_dataset.get("featureNames"),
+                feature_metadata=rendered_dataset.get("featureMetadata"),
+                predictions=rendered_dataset.get("predictions"),
+                target_names=rendered_dataset.get("targetNames"),
+            )
         else:
             # set dict and legacy
-            return cls(feature_metadata=rendered_dataset.get("featureMetadata"),
-                       legacy_data_conf=rendered_dataset)
+            return cls(
+                feature_metadata=rendered_dataset.get("featureMetadata"),
+                legacy_data_conf=rendered_dataset,
+            )
 
     def get_feature_metadata_fqtn(self):
         if self.feature_metadata_database and self.feature_metadata_table:
             return f"{self.feature_metadata_database}.{self.feature_metadata_table}"
         else:
             return None
 
@@ -52,44 +61,57 @@
 
     def is_legacy(self):
         return self.legacy_data_conf is not None
 
 
 class ModelContext(object):
 
-    def __init__(self, hyperparams: Dict,
-                 dataset_info: DatasetInfo,
-                 artifact_output_path: str = None,
-                 artifact_input_path: str = None,
-                 **kwargs):
+    def __init__(
+        self,
+        hyperparams: Dict,
+        dataset_info: DatasetInfo,
+        artifact_output_path: str = None,
+        artifact_input_path: str = None,
+        **kwargs,
+    ):
 
         self.hyperparams = hyperparams
         self.artifact_output_path = artifact_output_path
         self.artifact_input_path = artifact_input_path
         self.dataset_info = dataset_info
 
-        valid_var_keys = {"project_id", "model_id", "model_version", "job_id", "model_table"}
+        valid_var_keys = {
+            "project_id",
+            "model_id",
+            "model_version",
+            "job_id",
+            "model_table",
+        }
         for key in kwargs:
             if key in valid_var_keys:
                 setattr(self, key, kwargs.get(key))
 
     @property
     def artifact_output_path(self):
         return self.__artefact_output_path
 
     @artifact_output_path.setter
     def artifact_output_path(self, artifact_output_path):
         if artifact_output_path and not os.path.isdir(artifact_output_path):
-            raise ValueError(f"artefact_output_path ({artifact_output_path}) does not exist")
+            raise ValueError(
+                f"artefact_output_path ({artifact_output_path}) does not exist"
+            )
 
         self.__artefact_output_path = artifact_output_path
 
     @property
     def artifact_input_path(self):
         return self.__artefact_input_path
 
     @artifact_input_path.setter
     def artifact_input_path(self, artifact_input_path):
         if artifact_input_path and not os.path.isdir(artifact_input_path):
-            raise ValueError(f"artefact_input_path ({artifact_input_path}) does not exist")
+            raise ValueError(
+                f"artefact_input_path ({artifact_input_path}) does not exist"
+            )
 
         self.__artefact_input_path = artifact_input_path
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/crypto/TJEncryptPassword.py` & `teradatamodelops-7.0.6rc2/aoa/crypto/TJEncryptPassword.py`

 * *Files 5% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 import Crypto.Hash.SHA1
 import Crypto.Hash.SHA256
 import Crypto.Random
 import Crypto.Util.Padding
 import Crypto.Util.asn1
 import teradatasql
 
-safe_dirs = [os.path.expanduser('~'), "/mnt/sdb/myagent/_work"]
+safe_dirs = [os.path.expanduser("~"), "/mnt/sdb/myagent/_work"]
 
 
 def j2p(sName):  # convert Java names to Python names
 
     if sName == "DESede":
         return "DES3"
 
@@ -328,16 +328,24 @@
         return "MODE_" + sName
 
     return sName
 
     # end j2p
 
 
-def createPasswordEncryptionKeyFile(sTransformation, sAlgorithm, sMode, sPadding, nKeySizeInBits, sMatch, sMac,
-                                    sPassKeyFileName):
+def createPasswordEncryptionKeyFile(
+    sTransformation,
+    sAlgorithm,
+    sMode,
+    sPadding,
+    nKeySizeInBits,
+    sMatch,
+    sMac,
+    sPassKeyFileName,
+):
     nKeySizeInBytes = nKeySizeInBits // 8
 
     moduleCipher = getattr(Crypto.Cipher, j2p(sAlgorithm))
     nMode = getattr(moduleCipher, j2p(sMode))
 
     abyKey = Crypto.Random.get_random_bytes(nKeySizeInBytes)
     sKeyHexDigits = binascii.hexlify(abyKey).decode()
@@ -345,53 +353,79 @@
     moduleHash = getattr(Crypto.Hash, j2p(sMac))
     nMacBlockSizeInBytes = moduleHash.block_size
 
     abyMacKey = Crypto.Random.get_random_bytes(nMacBlockSizeInBytes)
     sMacKeyHexDigits = binascii.hexlify(abyMacKey).decode()
 
     with open(is_safe_path(sPassKeyFileName), "w", encoding="iso-8859-1") as f:
-        f.write("# Teradata SQL Driver password encryption key file\n" +
-                "version=1\n" +
-                "transformation=" + sTransformation + "\n" +
-                "algorithm=" + sAlgorithm + "\n" +
-                "match=" + sMatch + "\n" +
-                "key=" + sKeyHexDigits + "\n" +
-                "mac=" + sMac + "\n" +
-                "mackey=" + sMacKeyHexDigits + "\n")
+        f.write(
+            "# Teradata SQL Driver password encryption key file\n"
+            + "version=1\n"
+            + "transformation="
+            + sTransformation
+            + "\n"
+            + "algorithm="
+            + sAlgorithm
+            + "\n"
+            + "match="
+            + sMatch
+            + "\n"
+            + "key="
+            + sKeyHexDigits
+            + "\n"
+            + "mac="
+            + sMac
+            + "\n"
+            + "mackey="
+            + sMacKeyHexDigits
+            + "\n"
+        )
 
         return abyKey, abyMacKey
 
     # end createPasswordEncryptionKeyFile
 
 
-def createEncryptedPasswordFile(sTransformation, sAlgorithm, sMode, sPadding, sMatch, abyKey, sMac, abyMacKey,
-                                sEncPassFileName, sPassword):
+def createEncryptedPasswordFile(
+    sTransformation,
+    sAlgorithm,
+    sMode,
+    sPadding,
+    sMatch,
+    abyKey,
+    sMac,
+    abyMacKey,
+    sEncPassFileName,
+    sPassword,
+):
     moduleCipher = getattr(Crypto.Cipher, j2p(sAlgorithm))
     nMode = getattr(moduleCipher, j2p(sMode))
 
     bPadding = sPadding == "PKCS5Padding"
 
     nBlockSizeInBytes = moduleCipher.block_size
     abyIV = Crypto.Random.get_random_bytes(nBlockSizeInBytes)
 
     abyASN1EncodedIV = Crypto.Util.asn1.DerOctetString(abyIV).encode()
     sASN1EncodedIVHexDigits = binascii.hexlify(abyASN1EncodedIV).decode()
 
     mapOptions = {}
-    mapOptions['iv'] = abyIV
+    mapOptions["iv"] = abyIV
 
     if sMode == "CFB":
         nBlockSizeInBits = nBlockSizeInBytes * 8
-        mapOptions['segment_size'] = nBlockSizeInBits
+        mapOptions["segment_size"] = nBlockSizeInBits
 
     cipher = moduleCipher.new(abyKey, nMode, **mapOptions)
 
     abyPassword = sPassword.encode()
 
-    nPlaintextByteCount = (len(abyPassword) // 512 + 1) * 512  # zero-pad the password to the next 512-byte boundary
+    nPlaintextByteCount = (
+        len(abyPassword) // 512 + 1
+    ) * 512  # zero-pad the password to the next 512-byte boundary
 
     nTrailerByteCount = nPlaintextByteCount - len(abyPassword)
     abyPassword += bytearray(nTrailerByteCount)
 
     if bPadding:
         abyPassword = Crypto.Util.Padding.pad(abyPassword, nBlockSizeInBytes)
 
@@ -401,20 +435,30 @@
     abyContent = abyEncryptedPassword + sTransformation.encode() + abyASN1EncodedIV
 
     moduleHash = getattr(Crypto.Hash, j2p(sMac))
     hasher = Crypto.Hash.HMAC.new(abyMacKey, abyContent, moduleHash)
     sHashHexDigits = hasher.hexdigest()
 
     with open(is_safe_path(sEncPassFileName), "w", encoding="iso-8859-1") as f:
-        f.write("# Teradata SQL Driver encrypted password file\n" +
-                "version=1\n" +
-                "match=" + sMatch + "\n" +
-                "password=" + sEncryptedPasswordHexDigits + "\n" +
-                "params=" + sASN1EncodedIVHexDigits + "\n" +
-                "hash=" + sHashHexDigits + "\n")
+        f.write(
+            "# Teradata SQL Driver encrypted password file\n"
+            + "version=1\n"
+            + "match="
+            + sMatch
+            + "\n"
+            + "password="
+            + sEncryptedPasswordHexDigits
+            + "\n"
+            + "params="
+            + sASN1EncodedIVHexDigits
+            + "\n"
+            + "hash="
+            + sHashHexDigits
+            + "\n"
+        )
 
     # end createEncryptedPasswordFile
 
 
 def loadPropertiesFile(sFileName):
     with open(is_safe_path(sFileName), encoding="iso-8859-1") as f:
         sFileContents = f.read()
@@ -435,35 +479,49 @@
 
 
 def decryptPassword(sPassKeyFileName, sEncPassFileName):
     mapPassKey = loadPropertiesFile(sPassKeyFileName)
     mapEncPass = loadPropertiesFile(sEncPassFileName)
 
     if mapPassKey["version"] != "1":
-        raise ValueError("Unrecognized version {} in file {}".format(mapPassKey["version"], sPassKeyFileName))
+        raise ValueError(
+            "Unrecognized version {} in file {}".format(
+                mapPassKey["version"], sPassKeyFileName
+            )
+        )
 
     if mapEncPass["version"] != "1":
-        raise ValueError("Unrecognized version {} in file {}".format(mapEncPass["version"], sEncPassFileName))
+        raise ValueError(
+            "Unrecognized version {} in file {}".format(
+                mapEncPass["version"], sEncPassFileName
+            )
+        )
 
     if mapPassKey["match"] != mapEncPass["match"]:
-        raise ValueError("Match value differs between files {} and {}".format(sPassKeyFileName, sEncPassFileName))
+        raise ValueError(
+            "Match value differs between files {} and {}".format(
+                sPassKeyFileName, sEncPassFileName
+            )
+        )
 
     sTransformation = mapPassKey["transformation"]
     sAlgorithm = mapPassKey["algorithm"]
     sKeyHexDigits = mapPassKey["key"]
     sMACAlgorithm = mapPassKey["mac"]
     sMacKeyHexDigits = mapPassKey["mackey"]
 
     asTransformationParts = sTransformation.split("/")
 
     sMode = asTransformationParts[1]
     sPadding = asTransformationParts[2]
 
     if sAlgorithm != asTransformationParts[0]:
-        raise ValueError("Algorithm differs from transformation in file {}".format(sPassKeyFileName))
+        raise ValueError(
+            "Algorithm differs from transformation in file {}".format(sPassKeyFileName)
+        )
 
     # While params is technically optional, an initialization vector is required by all three block
     # cipher modes CBC, CFB, and OFB that are supported by the Teradata SQL Driver for Python.
     # ECB does not require params, but ECB is not supported by the Teradata SQL Driver for Python.
 
     sEncryptedPasswordHexDigits = mapEncPass["password"]
     sASN1EncodedIVHexDigits = mapEncPass["params"]  # required for CBC, CFB, and OFB
@@ -477,73 +535,87 @@
     abyContent = abyEncryptedPassword + sTransformation.encode() + abyASN1EncodedIV
 
     moduleHash = getattr(Crypto.Hash, j2p(sMACAlgorithm))
     hasher = Crypto.Hash.HMAC.new(abyMacKey, abyContent, moduleHash)
 
     if sHashHexDigits != hasher.hexdigest():
         raise ValueError(
-            "Hash mismatch indicates possible tampering with file {} or {}".format(sPassKeyFileName, sEncPassFileName))
+            "Hash mismatch indicates possible tampering with file {} or {}".format(
+                sPassKeyFileName, sEncPassFileName
+            )
+        )
 
     nKeySizeInBytes = len(abyKey)
     nKeySizeInBits = nKeySizeInBytes * 8
 
-    print("{} specifies {} with {}-bit key and {}".format(sPassKeyFileName, sTransformation, nKeySizeInBits,
-                                                          sMACAlgorithm))
+    print(
+        "{} specifies {} with {}-bit key and {}".format(
+            sPassKeyFileName, sTransformation, nKeySizeInBits, sMACAlgorithm
+        )
+    )
 
     moduleCipher = getattr(Crypto.Cipher, j2p(sAlgorithm))
     nMode = getattr(moduleCipher, j2p(sMode))
 
     dos = Crypto.Util.asn1.DerOctetString()
     dos.decode(abyASN1EncodedIV)
     abyIV = dos.payload
 
     mapOptions = {}
-    mapOptions['iv'] = abyIV
+    mapOptions["iv"] = abyIV
 
     nBlockSizeInBytes = moduleCipher.block_size
     nBlockSizeInBits = nBlockSizeInBytes * 8
 
     if sMode == "CFB":
-        mapOptions['segment_size'] = nBlockSizeInBits
+        mapOptions["segment_size"] = nBlockSizeInBits
 
     cipher = moduleCipher.new(abyKey, nMode, **mapOptions)
 
     abyPassword = cipher.decrypt(abyEncryptedPassword)
 
-    iZeroByte = abyPassword.index(b'\x00')
-    sPassword = abyPassword[: iZeroByte].decode()
+    iZeroByte = abyPassword.index(b"\x00")
+    sPassword = abyPassword[:iZeroByte].decode()
 
     print("Decrypted password:", sPassword)
 
     return sPassword
 
     # end decryptPassword
 
 
 def is_safe_path(file_path, raise_error=True):
     unsafe_dirs = []
     for safe_dir in safe_dirs:
-        if os.path.commonprefix([os.path.realpath(file_path), os.path.realpath(safe_dir)]) == safe_dir:
+        if (
+            os.path.commonprefix(
+                [os.path.realpath(file_path), os.path.realpath(safe_dir)]
+            )
+            == safe_dir
+        ):
             return file_path
         else:
             unsafe_dirs.append(os.path.realpath(safe_dir))
 
     if raise_error:
-        raise ValueError(f"Wrong path for the file, must be under {' or '.join(unsafe_dirs)}")
+        raise ValueError(
+            f"Wrong path for the file, must be under {' or '.join(unsafe_dirs)}"
+        )
 
     return False
 
 
 # begin main program
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     if len(sys.argv) != 9:
         print(
-            "Parameters: Transformation KeySizeInBits MAC PasswordEncryptionKeyFileName EncryptedPasswordFileName Hostname Username Password")
+            "Parameters: Transformation KeySizeInBits MAC PasswordEncryptionKeyFileName EncryptedPasswordFileName Hostname Username Password"
+        )
         sys.exit(1)
 
     sTransformation = sys.argv[1]
     sKeySizeInBits = sys.argv[2]
     sMac = sys.argv[3]
     sPassKeyFileName = is_safe_path(sys.argv[4])
     sEncPassFileName = is_safe_path(sys.argv[5])
@@ -570,26 +642,50 @@
 
     if sMac not in ["HmacSHA1", "HmacSHA256"]:
         raise ValueError("Unknown MAC algorithm " + sMac)
 
     if not sPassword:
         raise ValueError("Password cannot be zero length")
 
-    sPassword = sPassword.encode().decode('unicode_escape')  # for backslash uXXXX escape sequences
+    sPassword = sPassword.encode().decode(
+        "unicode_escape"
+    )  # for backslash uXXXX escape sequences
 
     nKeySizeInBits = int(sKeySizeInBits)
     sMatch = str(datetime.datetime.now())
 
-    abyKey, abyMacKey = createPasswordEncryptionKeyFile(sTransformation, sAlgorithm, sMode, sPadding, nKeySizeInBits,
-                                                        sMatch, sMac, sPassKeyFileName)
-
-    createEncryptedPasswordFile(sTransformation, sAlgorithm, sMode, sPadding, sMatch, abyKey, sMac, abyMacKey,
-                                sEncPassFileName, sPassword)
+    abyKey, abyMacKey = createPasswordEncryptionKeyFile(
+        sTransformation,
+        sAlgorithm,
+        sMode,
+        sPadding,
+        nKeySizeInBits,
+        sMatch,
+        sMac,
+        sPassKeyFileName,
+    )
+
+    createEncryptedPasswordFile(
+        sTransformation,
+        sAlgorithm,
+        sMode,
+        sPadding,
+        sMatch,
+        abyKey,
+        sMac,
+        abyMacKey,
+        sEncPassFileName,
+        sPassword,
+    )
 
     decryptPassword(sPassKeyFileName, sEncPassFileName)
 
-    sPassword = "ENCRYPTED_PASSWORD(file:{},file:{})".format(sPassKeyFileName, sEncPassFileName)
-
-    with teradatasql.connect(None, host=sHostname, user=sUsername, password=sPassword) as con:
+    sPassword = "ENCRYPTED_PASSWORD(file:{},file:{})".format(
+        sPassKeyFileName, sEncPassFileName
+    )
+
+    with teradatasql.connect(
+        None, host=sHostname, user=sUsername, password=sPassword
+    ) as con:
         with con.cursor() as cur:
-            cur.execute('select user, session')
+            cur.execute("select user, session")
             print(cur.fetchone())
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/crypto/crypto.py` & `teradatamodelops-7.0.6rc2/aoa/crypto/crypto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import base64, secrets, datetime
 
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
-from .TJEncryptPassword import createPasswordEncryptionKeyFile, createEncryptedPasswordFile, decryptPassword
+from .TJEncryptPassword import (
+    createPasswordEncryptionKeyFile,
+    createEncryptedPasswordFile,
+    decryptPassword,
+)
 
 backend = default_backend()
 
 default_conf = {
     "iterations": 65536,
     "bytes_key_length": 32,
     "bytes_salt_length": 16,
     "bytes_iv_length": 16,
-    "bytes_auth_tag_length": 16
+    "bytes_auth_tag_length": 16,
 }
 
 
 def _derive_key(password, salt, iterations, length):
     kdf = PBKDF2HMAC(
-        algorithm=hashes.SHA256(), length=length, salt=salt,
-        iterations=iterations, backend=backend)
+        algorithm=hashes.SHA256(),
+        length=length,
+        salt=salt,
+        iterations=iterations,
+        backend=backend,
+    )
     return kdf.derive(password)
 
 
 def aes_gcm_encrypt(message: str, password: str, conf: dict = default_conf) -> str:
     """
     Encrypts text for AOA core for e.g connection credentials. It is AES 256 bit HMAC
 
@@ -39,21 +47,23 @@
                 "bytes_auth_tag_length": 16
             }
     :return: the encrypted message
     """
     auth_tag = secrets.token_bytes(conf["bytes_auth_tag_length"])
     iv = secrets.token_bytes(conf["bytes_iv_length"])
     salt = secrets.token_bytes(conf["bytes_salt_length"])
-    key = _derive_key(password.encode(), salt, conf["iterations"], conf["bytes_key_length"])
+    key = _derive_key(
+        password.encode(), salt, conf["iterations"], conf["bytes_key_length"]
+    )
     algorithm = algorithms.AES(key)
     cipher = Cipher(algorithm, modes.GCM(iv), backend=backend)
     encryptor = cipher.encryptor()
     ciphertext = encryptor.update(message.encode())
 
-    return base64.urlsafe_b64encode(iv + salt + ciphertext + auth_tag).decode('utf-8')
+    return base64.urlsafe_b64encode(iv + salt + ciphertext + auth_tag).decode("utf-8")
 
 
 def aes_gcm_decrypt(message: str, password: str, conf: dict = default_conf) -> str:
     """
     Decrypt text which was previously encrypted by the AOA core for e.g connection credentials. It is AES 256 bit HMAC
 
     :param message: the text to decrypt
@@ -65,32 +75,48 @@
                 "bytes_salt_length": 16,
                 "bytes_iv_length": 16,
                 "bytes_auth_tag_length": 16
             }
     :return: decrypted text
     """
     data = base64.urlsafe_b64decode(message.encode())
-    (iv, salt, ciphertext, auth_tag) = data[:conf["bytes_iv_length"]], \
-                                       data[
-                                       conf["bytes_iv_length"]: conf["bytes_iv_length"] + conf["bytes_salt_length"]], \
-                                       data[conf["bytes_iv_length"] + conf["bytes_salt_length"]: -conf[
-                                           "bytes_auth_tag_length"]], \
-                                       data[-conf["bytes_auth_tag_length"]:]
-    key = _derive_key(password.encode(), salt, iterations=conf["iterations"], length=conf["bytes_key_length"])
+    (iv, salt, ciphertext, auth_tag) = (
+        data[: conf["bytes_iv_length"]],
+        data[
+            conf["bytes_iv_length"] : conf["bytes_iv_length"]
+            + conf["bytes_salt_length"]
+        ],
+        data[
+            conf["bytes_iv_length"]
+            + conf["bytes_salt_length"] : -conf["bytes_auth_tag_length"]
+        ],
+        data[-conf["bytes_auth_tag_length"] :],
+    )
+    key = _derive_key(
+        password.encode(),
+        salt,
+        iterations=conf["iterations"],
+        length=conf["bytes_key_length"],
+    )
     algorithm = algorithms.AES(key)
     cipher = Cipher(algorithm, modes.GCM(iv, salt), backend=backend)
     decryptor = cipher.decryptor()
     decrypted = decryptor.update(ciphertext)
 
-    return decrypted.decode('utf-8')
+    return decrypted.decode("utf-8")
 
 
-def td_encrypt_password(password=None, pass_key_filename='~/.aoa/userKey.properties',
-                        enc_pass_filename='~/.aoa/userPass.properties', transformation='AES/CBC/PKCS5Padding',
-                        key_size_in_bits=256, mac='HmacSHA256'):
+def td_encrypt_password(
+    password=None,
+    pass_key_filename="~/.aoa/userKey.properties",
+    enc_pass_filename="~/.aoa/userPass.properties",
+    transformation="AES/CBC/PKCS5Padding",
+    key_size_in_bits=256,
+    mac="HmacSHA256",
+):
     """
     Encrypts a password, saves the encryption key in one file, and saves the encrypted password in a second file.
     This is done using the Stored Password Protection format.
     e.g. "ENCRYPTED_PASSWORD(file:PasswordEncryptionKeyFileName,file:EncryptedPasswordFileName)"
 
     :param password: password to encrypt
     :param pass_key_filename: Specifies the location of the generated password encryption file
@@ -120,26 +146,46 @@
 
     if mac not in ["HmacSHA1", "HmacSHA256"]:
         raise ValueError("Unknown MAC algorithm " + mac)
 
     if not password:
         raise ValueError("Password cannot be zero length")
 
-    password = password.encode().decode('unicode_escape')
+    password = password.encode().decode("unicode_escape")
 
     key_size_in_bits = int(key_size_in_bits)
     match = str(datetime.datetime.now())
 
-    aby_key, aby_mac_key = createPasswordEncryptionKeyFile(transformation, algorithm, mode, padding,
-                                                           key_size_in_bits, match, mac, pass_key_filename)
-
-    createEncryptedPasswordFile(transformation, algorithm, mode, padding, match, aby_key, mac, aby_mac_key,
-                                enc_pass_filename, password)
-
-    return "ENCRYPTED_PASSWORD(file:{},file:{})".format(pass_key_filename, enc_pass_filename)
+    aby_key, aby_mac_key = createPasswordEncryptionKeyFile(
+        transformation,
+        algorithm,
+        mode,
+        padding,
+        key_size_in_bits,
+        match,
+        mac,
+        pass_key_filename,
+    )
+
+    createEncryptedPasswordFile(
+        transformation,
+        algorithm,
+        mode,
+        padding,
+        match,
+        aby_key,
+        mac,
+        aby_mac_key,
+        enc_pass_filename,
+        password,
+    )
+
+    return "ENCRYPTED_PASSWORD(file:{},file:{})".format(
+        pass_key_filename, enc_pass_filename
+    )
 
 
 def td_decrypt_password(password=None):
     """
     Decrypts a password, from the encryption key file and the encrypted password file.
     This is done using the Stored Password Protection format.
 
@@ -147,10 +193,11 @@
     :return: the decrypted password
     """
 
     if not password:
         raise ValueError("Password cannot be zero length")
 
     import re
-    password_files = re.match('^ENCRYPTED_PASSWORD\\(file:(.*),file:(.*)\\)$', password)
+
+    password_files = re.match("^ENCRYPTED_PASSWORD\\(file:(.*),file:(.*)\\)$", password)
 
     return decryptPassword(password_files[1], password_files[2])
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/stats/stats.py` & `teradatamodelops-7.0.6rc2/aoa/stats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,29 @@
 from teradataml.analytics.valib import *
 from teradataml import DataFrame
 from aoa.context.model_context import ModelContext
 from aoa.stats.stats_util import (
     _capture_stats,
     _NpEncoder,
     _parse_scoring_stats,
-    _compute_continuous_edges
+    _compute_continuous_edges,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def record_training_stats(df: DataFrame,
-                          features: List[str],
-                          targets: List[str] = [],
-                          categorical: List[str] = [],
-                          context: ModelContext = {},
-                          feature_importance: Dict[str, float] = {},
-                          **kwargs) -> Dict:
+def record_training_stats(
+    df: DataFrame,
+    features: List[str],
+    targets: List[str] = [],
+    categorical: List[str] = [],
+    context: ModelContext = {},
+    feature_importance: Dict[str, float] = {},
+    **kwargs,
+) -> Dict:
     """
     Compute and record the dataset statistics used for training. This information provides ModelOps with a snapshot
     of the dataset at this point in time (i.e. at the point of training). ModelOps uses this information for data and
     prediction drift monitoring. It can also be used for data quality monitoring as all of the information which is
     captured here is available to configure an alert on (e.g. max > some_threshold).
 
     Depending on the type of variable (categorical or continuous), different statistics and distributions are computed.
@@ -75,48 +77,58 @@
     logger.info("Computing training dataset statistics")
 
     if not features:
         raise ValueError("One or more features must be provided")
 
     # backward compatibility for when we had targets incorrectly named predictors.. remove in future version
     if "predictors" in kwargs:
-        logger.warning("Usage of `predictors` as argument to `record_training_stats` is deprecated. ")
+        logger.warning(
+            "Usage of `predictors` as argument to `record_training_stats` is deprecated. "
+        )
         targets = kwargs.pop("predictors")
 
     if not targets:
-        logger.warning("One or more targets are not provided to collect training statistics, make sure this is what you want.")
+        logger.warning(
+            "One or more targets are not provided to collect training statistics, make sure this is what you want."
+        )
 
     feature_metadata_fqtn = None
     feature_metadata_group = None
     data_stats_filename = "artifacts/output/data_stats.json"
 
     if context:
         feature_metadata_fqtn = context.dataset_info.get_feature_metadata_fqtn()
         feature_metadata_group = context.dataset_info.feature_metadata_monitoring_group
-        data_stats_filename = os.path.join(context.artifact_output_path, "data_stats.json")
+        data_stats_filename = os.path.join(
+            context.artifact_output_path, "data_stats.json"
+        )
+
+    data_stats = _capture_stats(
+        df=df,
+        features=features,
+        targets=targets,
+        categorical=categorical,
+        feature_importance=feature_importance,
+        feature_metadata_fqtn=feature_metadata_fqtn,
+        feature_metadata_group=feature_metadata_group,
+    )
 
-    data_stats = _capture_stats(df=df,
-                                features=features,
-                                targets=targets,
-                                categorical=categorical,
-                                feature_importance=feature_importance,
-                                feature_metadata_fqtn=feature_metadata_fqtn,
-                                feature_metadata_group=feature_metadata_group)
-
-    with open(data_stats_filename, 'w+') as f:
+    with open(data_stats_filename, "w+") as f:
         json.dump(data_stats, f, indent=2, cls=_NpEncoder)
 
     return data_stats
 
 
-def record_evaluation_stats(features_df: DataFrame,
-                            predicted_df: DataFrame,
-                            feature_importance: Dict[str, float] = {},
-                            context: ModelContext = None,
-                            **kwargs) -> Dict:
+def record_evaluation_stats(
+    features_df: DataFrame,
+    predicted_df: DataFrame,
+    feature_importance: Dict[str, float] = {},
+    context: ModelContext = None,
+    **kwargs,
+) -> Dict:
     """
     Compute and record the dataset statistics used for evaluation. This information provides ModelOps with a snapshot
     of the dataset at this point in time (i.e. at the point of evaluation). ModelOps uses this information for data
     and prediction drift monitoring. It can also be used for data quality monitoring as all of the information which
     is captured here is available to configure an alert on (e.g. max > some_threshold).
 
     Depending on the type of variable (categorical or continuous), different statistics and distributions are computed.
@@ -159,37 +171,43 @@
     feature_metadata_group = None
     output_data_stats_filename = "artifacts/output/data_stats.json"
     input_data_stats_filename = "artifacts/input/data_stats.json"
 
     if context:
         feature_metadata_fqtn = context.dataset_info.get_feature_metadata_fqtn()
         feature_metadata_group = context.dataset_info.feature_metadata_monitoring_group
-        output_data_stats_filename = os.path.join(context.artifact_output_path, "data_stats.json")
-        input_data_stats_filename = os.path.join(context.artifact_input_path, "data_stats.json")
+        output_data_stats_filename = os.path.join(
+            context.artifact_output_path, "data_stats.json"
+        )
+        input_data_stats_filename = os.path.join(
+            context.artifact_input_path, "data_stats.json"
+        )
 
-    with open(input_data_stats_filename, 'r') as f:
+    with open(input_data_stats_filename, "r") as f:
         training_data_stats = json.load(f)
 
-    data_stats = _parse_scoring_stats(features_df=features_df,
-                                      predicted_df=predicted_df,
-                                      data_stats=training_data_stats,
-                                      feature_importance=feature_importance,
-                                      feature_metadata_fqtn=feature_metadata_fqtn,
-                                      feature_metadata_group=feature_metadata_group)
+    data_stats = _parse_scoring_stats(
+        features_df=features_df,
+        predicted_df=predicted_df,
+        data_stats=training_data_stats,
+        feature_importance=feature_importance,
+        feature_metadata_fqtn=feature_metadata_fqtn,
+        feature_metadata_group=feature_metadata_group,
+    )
 
     # for evaluation, the core will do it (we may change this later to unify)..
-    with open(output_data_stats_filename, 'w+') as f:
+    with open(output_data_stats_filename, "w+") as f:
         json.dump(data_stats, f, indent=2, cls=_NpEncoder)
 
     return data_stats
 
 
-def record_scoring_stats(features_df: DataFrame,
-                         predicted_df: DataFrame,
-                         context: ModelContext = None) -> Dict:
+def record_scoring_stats(
+    features_df: DataFrame, predicted_df: DataFrame, context: ModelContext = None
+) -> Dict:
     """
     Compute and record the dataset statistics used for scoring. This information provides ModelOps with a snapshot
     of the dataset at this point in time (i.e. at the point of scoring). ModelOps uses this information for data
     and prediction drift monitoring. It can also be used for data quality monitoring as all of the information which
     is captured here is available to configure an alert on (e.g. max > some_threshold).
 
     Depending on the type of variable (categorical or continuous), different statistics and distributions are computed.
@@ -229,133 +247,169 @@
     feature_metadata_fqtn = None
     feature_metadata_group = None
     input_data_stats_filename = "artifacts/input/data_stats.json"
 
     if context:
         feature_metadata_fqtn = context.dataset_info.get_feature_metadata_fqtn()
         feature_metadata_group = context.dataset_info.feature_metadata_monitoring_group
-        input_data_stats_filename = os.path.join(context.artifact_input_path, "data_stats.json")
-        output_data_stats_filename = os.path.join(context.artifact_output_path, "data_stats.json")
+        input_data_stats_filename = os.path.join(
+            context.artifact_input_path, "data_stats.json"
+        )
+        output_data_stats_filename = os.path.join(
+            context.artifact_output_path, "data_stats.json"
+        )
 
-    with open(input_data_stats_filename, 'r') as f:
+    with open(input_data_stats_filename, "r") as f:
         training_data_stats = json.load(f)
 
-    data_stats = _parse_scoring_stats(features_df=features_df,
-                                      predicted_df=predicted_df,
-                                      data_stats=training_data_stats,
-                                      feature_metadata_fqtn=feature_metadata_fqtn,
-                                      feature_metadata_group=feature_metadata_group)
+    data_stats = _parse_scoring_stats(
+        features_df=features_df,
+        predicted_df=predicted_df,
+        data_stats=training_data_stats,
+        feature_metadata_fqtn=feature_metadata_fqtn,
+        feature_metadata_group=feature_metadata_group,
+    )
 
     # for evaluation, the core will do it (we may change this later to unify)..
-    with open(output_data_stats_filename, 'w+') as f:
+    with open(output_data_stats_filename, "w+") as f:
         json.dump(data_stats, f, indent=2, cls=_NpEncoder)
 
     return data_stats
 
 
 def compute_continuous_stats(features_df: DataFrame, continuous_features: List[str]):
     """This function computes bin edges for continuous features. Only numeric columns are used,
-    others are ignored with warning. For each column it computes maximum and minimum values, and 
-    attempts to split the difference into 10 bins. If only smaller number is possile - it generates 
-    the maximum number (e.g. integer column with minimum 5 and maximum 10 generates only 5 bins). 
+    others are ignored with warning. For each column it computes maximum and minimum values, and
+    attempts to split the difference into 10 bins. If only smaller number is possile - it generates
+    the maximum number (e.g. integer column with minimum 5 and maximum 10 generates only 5 bins).
     The column has to have at least two distinct values, otherwise the column is ignored.
 
     Args:
         features_df (DataFrame): Teradata DataFrame used to compute statistics metadata
         continuous_features (List): list of columns representing continuous features
 
     Returns:
         dict: Dictionary with keys corresponding to requested features, and values containing edges
-    """    
+    """
     dtypes = {r[0].lower(): r[1] for r in features_df.dtypes._column_names_and_types}
 
     # Numeric types in teradata are represented as either int, or float or decimal.Decimal,
     # so other columns shall be ignored
     # COLUMN NAME	TYPE
     # int_column	int
     # byte_column	int
     # smallint_column	int
     # decimal_column	decimal.Decimal
     # numeric_column	decimal.Decimal
     # float_column	float
     # real_column	float
     # double_precision_column	float
     # number_column	decimal.Decimal
-    lowered_features = list(map(str.lower,continuous_features))
+    lowered_features = list(map(str.lower, continuous_features))
     features = []
     for f in lowered_features:
-        if dtypes[f].startswith("decimal") or dtypes[f].startswith("float") or dtypes[f].startswith("int"):
+        if (
+            dtypes[f].startswith("decimal")
+            or dtypes[f].startswith("float")
+            or dtypes[f].startswith("int")
+        ):
             features.append(f)
         else:
-            logger.warning(f"Column {f} has a type {dtypes[f]} which is not compatible with continuous feature types. This column will be ignored.")
-
-    logger.debug(f"Executing this VAL {valib.Statistics(data=features_df, columns=features, stats_options='all').show_query()}")
+            logger.warning(
+                f"Column {f} has a type {dtypes[f]} which is not compatible with continuous feature types. This column will be ignored."
+            )
+
+    logger.debug(
+        f"Executing this VAL {valib.Statistics(data=features_df, columns=features, stats_options='all').show_query()}"
+    )
     stats = valib.Statistics(data=features_df, columns=features, stats_options="all")
     stats = stats.result.to_pandas(all_rows=True).reset_index()
     stats["xcol"] = stats["xcol"].str.lower()
-    stats = stats.set_index("xcol",drop=False)
+    stats = stats.set_index("xcol", drop=False)
 
     non_trivial_features = []
     for f in features:
         if stats.loc[f].loc["xcnt"] == 0:
             logger.warning(f"Feature {f} has only NULL values, ignored")
         elif stats.loc[f].loc["xmin"] == stats.loc[f].loc["xmax"]:
-            logger.warning(f"Feature {f} doesn't have enough unique values to be considered continuous feature "
-                           "(needs at least two distinct not null values), ignored")
+            logger.warning(
+                f"Feature {f} doesn't have enough unique values to be considered continuous feature "
+                "(needs at least two distinct not null values), ignored"
+            )
         else:
             non_trivial_features.append(f)
 
-    bins = 10 # Default number of bins; if data doesn't allow 10 bins - we generate the maximum number allowed
-    reference_edges = _compute_continuous_edges(non_trivial_features, stats, dtypes, bins=bins)
+    bins = 10  # Default number of bins; if data doesn't allow 10 bins - we generate the maximum number allowed
+    reference_edges = _compute_continuous_edges(
+        non_trivial_features, stats, dtypes, bins=bins
+    )
     edges_dict = dict(zip(non_trivial_features, reference_edges))
 
     for variable_name, edges in edges_dict.items():
         if len(edges) < bins:
-            logger.warning(f"Variable {variable_name} has only {len(edges)} bins computed when {bins} should "
-                            f"have been computed {edges}.\n"
-                            f"Please ensure the variable is not categorical (use -t categorical).")
+            logger.warning(
+                f"Variable {variable_name} has only {len(edges)} bins computed when {bins} should "
+                f"have been computed {edges}.\n"
+                f"Please ensure the variable is not categorical (use -t categorical)."
+            )
 
     column_stats = {}
     for f in edges_dict.keys():
         column_stats[f.lower()] = {"edges": edges_dict[f]}
 
     if len(column_stats) == 0:
-        raise Exception(f"No columns with computable statistics metadata were found, please see warning messages above")
-    
+        raise Exception(
+            f"No columns with computable statistics metadata were found, please see warning messages above"
+        )
+
     return column_stats
 
 
 def compute_categorical_stats(features_df: DataFrame, categorical_features: List[str]):
-    """This function computes frequencies for categorical features. Each column must have at least one non-NULL value, 
-    all NULL columns are ignored. NULL value is ignored in frequencies (number of NULLs is reported for every 
+    """This function computes frequencies for categorical features. Each column must have at least one non-NULL value,
+    all NULL columns are ignored. NULL value is ignored in frequencies (number of NULLs is reported for every
     training/evaluation/scoring jobs).
 
     Args:
         features_df (DataFrame): Teradata DataFrame used to compute statistics metadata
         categorical_features (List): list of columns representing categorical features
 
     Returns:
         dict: Dictionary with keys corresponding to requested features, and values containing frequencies
-    """    
-    logger.debug(f"Executing this VAL {valib.Frequency(data=features_df, columns=categorical_features).show_query()}")
+    """
+    logger.debug(
+        f"Executing this VAL {valib.Frequency(data=features_df, columns=categorical_features).show_query()}"
+    )
     statistics = valib.Frequency(data=features_df, columns=categorical_features)
     statistics = statistics.result.to_pandas(all_rows=True).reset_index()
-    statistics = statistics.drop(statistics.columns.difference(["xcol", "xval", "xpct"]), axis=1)
+    statistics = statistics.drop(
+        statistics.columns.difference(["xcol", "xval", "xpct"]), axis=1
+    )
     statistics["xcol"] = statistics["xcol"].str.lower()
-    statistics = statistics.groupby('xcol').apply(lambda x: dict(zip(x['xval'], x['xpct']))).to_dict()
+    statistics = (
+        statistics.groupby("xcol")
+        .apply(lambda x: dict(zip(x["xval"], x["xpct"])))
+        .to_dict()
+    )
 
     lowered_features = list(map(str.lower, categorical_features))
     features = list(lowered_features)
     for f in features:
         values_list = list(statistics[f].keys())
         for k in values_list:
             if isinstance(k, numbers.Number):
                 if math.isnan(k):
-                    logger.warning(f"Categorical feature {f} has NULL values in reference table, NULLs will be ignored")
-                    del statistics[f][k]                
+                    logger.warning(
+                        f"Categorical feature {f} has NULL values in reference table, NULLs will be ignored"
+                    )
+                    del statistics[f][k]
         if not statistics[f]:
-            logger.warning(f"Categorical feature {f} has only NULL values in reference table, no statistics metadata generated")
+            logger.warning(
+                f"Categorical feature {f} has only NULL values in reference table, no statistics metadata generated"
+            )
             lowered_features.remove(f)
-    
-    column_stats = {f: {"categories": list(statistics[f].keys())} for f in lowered_features}
+
+    column_stats = {
+        f: {"categories": list(statistics[f].keys())} for f in lowered_features
+    }
 
     return column_stats
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/stats/stats_util.py` & `teradatamodelops-7.0.6rc2/aoa/stats/stats_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,41 +23,47 @@
             return float(obj)
         elif isinstance(obj, np.ndarray):
             return obj.tolist()
         else:
             return super(_NpEncoder, self).default(obj)
 
 
-def _compute_continuous_edges(variables: List[str], statistics: pd.DataFrame, dtypes: Dict, bins=10) -> List[float]:
+def _compute_continuous_edges(
+    variables: List[str], statistics: pd.DataFrame, dtypes: Dict, bins=10
+) -> List[float]:
     edges = []
 
     # should return what is in the feature catalog.. for now calculate linspace boundaries based on min/max
-    ranges = statistics.drop(statistics.columns.difference(["xcol", "xmin", "xmax"]), axis=1)
+    ranges = statistics.drop(
+        statistics.columns.difference(["xcol", "xmin", "xmax"]), axis=1
+    )
     ranges = ranges.set_index("xcol")
     ranges.index = ranges.index.map(str.lower)
-    ranges = ranges.to_dict(orient='index')
+    ranges = ranges.to_dict(orient="index")
 
     for var in variables:
         x_min, x_max = ranges[var]["xmin"], ranges[var]["xmax"]
 
         # if integer type and range is less than the number of bins, only use 'range' bins
         if x_max - x_min < bins and dtypes[var].startswith("int"):
-            edges.append(np.linspace(x_min, x_max, int(x_max) - int(x_min) + 1).tolist())
+            edges.append(
+                np.linspace(x_min, x_max, int(x_max) - int(x_min) + 1).tolist()
+            )
         elif dtypes[var].startswith("decimal") or dtypes[var].startswith("float"):
             # (min / max must be rounded up / down accordingly so easier to just use the vals from stats)
             vals = np.linspace(x_min, x_max, bins + 1).tolist()
 
             # Rounding all edges to the best Teradata-compatible precision
             vals = list(map(_round_to_td_float, vals))
-                
+
             dedup = []
             [dedup.append(x) for x in vals if x not in dedup]
 
             edges.append(dedup)
-        else: # Here we compute for regular int variables
+        else:  # Here we compute for regular int variables
             vals = np.linspace(x_min, x_max, bins + 1).tolist()
             for i in range(1, len(vals)):
                 vals[i] = round(vals[i], 1)
             edges.append(vals)
 
     return edges
 
@@ -69,15 +75,17 @@
     for edges in all_edges:
         edges_str = ",".join(str(edge) for edge in edges)
         boundaries.append("{{ {} }}".format(edges_str))
 
     return boundaries
 
 
-def _fill_missing_bins(bin_edges: List[float], bin_values: List[float], reference_edges: List[float]) -> List[float]:
+def _fill_missing_bins(
+    bin_edges: List[float], bin_values: List[float], reference_edges: List[float]
+) -> List[float]:
     """
     Compare the `bin_edges` returned by VAL to `reference_edges` and fill in any missing bins with `0`.
     This is required as VAL doesn't return empty bins and so if we want to ensure we always have all the bins
     represented in the `bin_values` (which we do or else indices vs reference edges mean nothing), then we must do this.
 
     """
     new_bin_values = list(bin_values)
@@ -91,19 +99,21 @@
 
         if not is_present:
             new_bin_values.insert(i, 0.0)
 
     return new_bin_values
 
 
-def _process_categorical_var(frequencies: pd.DataFrame,
-                             group_label: str,
-                             variable_name: str,
-                             feature_importance: float,
-                             reference_categories: List) -> Dict:
+def _process_categorical_var(
+    frequencies: pd.DataFrame,
+    group_label: str,
+    variable_name: str,
+    feature_importance: float,
+    reference_categories: List,
+) -> Dict:
     """
     Adds the following struct
     {
         "type": "categorical",
         "group": "<group-name>",
         "importance": "<feature-importance>",
         "statistics": {
@@ -114,71 +124,78 @@
                 "cat2": 10,
                 ...
             }
         }
     }
     """
 
-    data_struct = {
-        "type": "categorical",
-        "group": group_label,
-        "statistics": {}
-    }
+    data_struct = {"type": "categorical", "group": group_label, "statistics": {}}
 
     if feature_importance:
         data_struct["importance"] = feature_importance
 
     var_freq = frequencies[frequencies.xcol == variable_name]
 
     # if first row is nan then it is the null values in the dataset. remove from histogram
     if var_freq["xval"].isnull().values.any():
         n = var_freq[var_freq["xval"].isnull()]
         data_struct["statistics"]["nulls"] = n.xcnt.tolist()[0]
         var_freq = var_freq[var_freq["xval"].notnull()]
 
     if var_freq.empty:
         # We should probably generate all-zero histogram here?
-        logger.warning(f"Categorical feature {variable_name} has only NULL values, not computing a frequency")
+        logger.warning(
+            f"Categorical feature {variable_name} has only NULL values, not computing a frequency"
+        )
         return data_struct
-    
-    frequencies_dict = var_freq[["xval", "xcnt"]].set_index("xval").T.to_dict(orient='records')[0]
+
+    frequencies_dict = (
+        var_freq[["xval", "xcnt"]].set_index("xval").T.to_dict(orient="records")[0]
+    )
 
     if reference_categories == None:
         # No reference categories - we stop here, not reporting frequencies
         data_struct["statistics"]["unmonitored_frequency"] = frequencies_dict
         return data_struct
     else:
-        
+
         # Record the reference categories. This is so we can map based on category -> index consistently for the
         # prometheus labels. This should be removed when this mapping is removed from handling in prometheus on backend.
         data_struct["categories"] = reference_categories
 
         # Record the `statistics.frequency` for each category (using the category as key).
         # `0` is set as the frequency for any category which is in `reference_categories` but not in `frequencies_dict`
         # This approach allows for new categories to be added over time (never removed) to reference_categories and
         # for everything to remain consistent.
         data_struct["statistics"]["frequency"] = {
-            cat: frequencies_dict.get(cat, 0) if cat in reference_categories else 0 for i, cat in enumerate(reference_categories)
+            cat: frequencies_dict.get(cat, 0) if cat in reference_categories else 0
+            for i, cat in enumerate(reference_categories)
         }
         for f in frequencies_dict.keys():
             if f not in reference_categories:
-                logger.warning(f"Categorical feature {variable_name} has a new category {f} that's not listed in reference categories")
+                logger.warning(
+                    f"Categorical feature {variable_name} has a new category {f} that's not listed in reference categories"
+                )
                 if "unmonitored_frequency" not in data_struct["statistics"]:
                     data_struct["statistics"]["unmonitored_frequency"] = {}
-                data_struct["statistics"]["unmonitored_frequency"][f] = frequencies_dict.get(f)
-                
+                data_struct["statistics"]["unmonitored_frequency"][f] = (
+                    frequencies_dict.get(f)
+                )
+
         return data_struct
 
 
-def _process_continuous_var(histogram: pd.DataFrame,
-                            stats: pd.DataFrame,
-                            group_label: str,
-                            variable_name: str,
-                            feature_importance: float,
-                            reference_edges: List[float]) -> Dict:
+def _process_continuous_var(
+    histogram: pd.DataFrame,
+    stats: pd.DataFrame,
+    group_label: str,
+    variable_name: str,
+    feature_importance: float,
+    reference_edges: List[float],
+) -> Dict:
     """
     Adds the following struct
     {
         "type": "continuous",
         "group": "<group-name>",
         "importance": "<feature-importance>",
         "statistics": {
@@ -203,33 +220,39 @@
 
     if feature_importance:
         data_struct["importance"] = feature_importance
 
     def _strip_key_x(d: Dict):
         return {k[1:]: v for k, v in d.items()}
 
-    stats_values = stats[stats.xcol == variable_name].drop(["xdb", "xtbl", "xcol"], axis=1).to_dict(orient='records')[0]
+    stats_values = (
+        stats[stats.xcol == variable_name]
+        .drop(["xdb", "xtbl", "xcol"], axis=1)
+        .to_dict(orient="records")[0]
+    )
     data_struct["statistics"].update(_strip_key_x(stats_values))
 
     if histogram.empty:
         # No histogram available - we stop here, not reporting histogram
         return data_struct
 
-    var_hist = histogram[histogram.xcol == variable_name].sort_values(by=['xbin'])
+    var_hist = histogram[histogram.xcol == variable_name].sort_values(by=["xbin"])
 
     # if first row is nan then it is the null values in the dataset. remove from histogram
     if var_hist["xbin"].isnull().values.any():
         n = var_hist[var_hist["xbin"].isnull()]
         data_struct["statistics"]["nulls"] = n.xcnt.tolist()[0]
 
         var_hist = var_hist[var_hist["xbin"].notnull()]
 
     if var_hist.empty:
         # We should probably generate all-zero histogram here?
-        logger.warning(f"Continuous feature {variable_name} has only NULL values, not computing a histogram")
+        logger.warning(
+            f"Continuous feature {variable_name} has only NULL values, not computing a histogram"
+        )
         return data_struct
 
     bin_edges = [var_hist.xbeg.tolist()[0]] + var_hist.xend.tolist()
     bin_values = var_hist.xcnt.tolist()
 
     # (issue #123) VAL docs originally stated that:
     # VAL histograms will values lower than the first bin to the first bin, but values greater than the
@@ -242,48 +265,60 @@
         bin_edges = bin_edges[:-1]
     if is_left_outlier_bin:
         bin_edges = bin_edges[1:]
 
     # Add missing bin_values based on the bin_edges vs reference_edges.
     # VAL doesn't return empty bins
     if len(bin_edges) < len(reference_edges):
-        bin_values = _fill_missing_bins(bin_edges=bin_edges, bin_values=bin_values, reference_edges=reference_edges)
+        bin_values = _fill_missing_bins(
+            bin_edges=bin_edges, bin_values=bin_values, reference_edges=reference_edges
+        )
 
     right_outliers = 0
     left_outliers = 0
     if is_right_outlier_bin:
         right_outliers = int(bin_values[-1])
-        logger.warning(f"Continuous feature {variable_name} has values larger than the rightmost bin, identified {right_outliers} values")
-        bin_values[-2] += bin_values[-1] # Probably should consider removing as some point, when outliers are properly reported and visible to the user
+        logger.warning(
+            f"Continuous feature {variable_name} has values larger than the rightmost bin, identified {right_outliers} values"
+        )
+        bin_values[-2] += bin_values[
+            -1
+        ]  # Probably should consider removing as some point, when outliers are properly reported and visible to the user
         bin_values = bin_values[:-1]
     if is_left_outlier_bin:
         left_outliers = int(bin_values[0])
-        logger.warning(f"Continuous feature {variable_name} has values smaller than the leftmost bin, identified {left_outliers} values")
-        bin_values[1] += bin_values[0] # Probably should consider removing as some point, when outliers are properly reported and visible to the user
+        logger.warning(
+            f"Continuous feature {variable_name} has values smaller than the leftmost bin, identified {left_outliers} values"
+        )
+        bin_values[1] += bin_values[
+            0
+        ]  # Probably should consider removing as some point, when outliers are properly reported and visible to the user
         bin_values = bin_values[1:]
 
     data_struct["statistics"]["histogram"] = {
         "edges": reference_edges,
-        "values": bin_values
+        "values": bin_values,
     }
 
     if is_right_outlier_bin:
         data_struct["statistics"]["histogram"]["right_outliers"] = right_outliers
     if is_left_outlier_bin:
         data_struct["statistics"]["histogram"]["left_outliers"] = left_outliers
 
     return data_struct
 
 
-def _parse_scoring_stats(features_df: DataFrame,
-                         predicted_df: DataFrame,
-                         data_stats: Dict,
-                         feature_importance: Dict[str, float] = {},
-                         feature_metadata_fqtn: str = None,
-                         feature_metadata_group: str = None) -> Dict:
+def _parse_scoring_stats(
+    features_df: DataFrame,
+    predicted_df: DataFrame,
+    data_stats: Dict,
+    feature_importance: Dict[str, float] = {},
+    feature_metadata_fqtn: str = None,
+    feature_metadata_group: str = None,
+) -> Dict:
     if not isinstance(features_df, DataFrame):
         raise TypeError("We only support teradataml DataFrame for features")
 
     if not isinstance(predicted_df, DataFrame):
         raise TypeError("We only support teradataml DataFrame for predictions")
 
     features = []
@@ -303,211 +338,252 @@
                 features.append(name)
             elif var_type == "targets":
                 targets.append(name)
             if "type" in value and value["type"] == "categorical":
                 categorical.append(name)
 
     if predicted_df.shape[0] != features_df.shape[0]:
-        raise ValueError("The number of prediction rows do not match the number of features rows!")
-
-    data_stats = _capture_stats(df=features_df,
-                                features=features,
-                                targets=[],
-                                categorical=categorical,
-                                feature_importance=feature_importance,
-                                feature_metadata_fqtn=feature_metadata_fqtn,
-                                feature_metadata_group=feature_metadata_group)
-
-    targets_struct = _capture_stats(df=predicted_df,
-                                    features=[],
-                                    targets=targets,
-                                    categorical=categorical,
-                                    feature_importance=feature_importance,
-                                    feature_metadata_fqtn=feature_metadata_fqtn,
-                                    feature_metadata_group=feature_metadata_group)
+        raise ValueError(
+            "The number of prediction rows do not match the number of features rows!"
+        )
+
+    data_stats = _capture_stats(
+        df=features_df,
+        features=features,
+        targets=[],
+        categorical=categorical,
+        feature_importance=feature_importance,
+        feature_metadata_fqtn=feature_metadata_fqtn,
+        feature_metadata_group=feature_metadata_group,
+    )
+
+    targets_struct = _capture_stats(
+        df=predicted_df,
+        features=[],
+        targets=targets,
+        categorical=categorical,
+        feature_importance=feature_importance,
+        feature_metadata_fqtn=feature_metadata_fqtn,
+        feature_metadata_group=feature_metadata_group,
+    )
 
     data_stats["targets"] = targets_struct["targets"]
 
     return data_stats
 
 
-def _capture_stats(df: DataFrame,
-                   features: List,
-                   targets: List,
-                   categorical: List,
-                   feature_importance: Dict[str, float] = {},
-                   feature_metadata_fqtn: str = {},
-                   feature_metadata_group: str = "default") -> Dict:
+def _capture_stats(
+    df: DataFrame,
+    features: List,
+    targets: List,
+    categorical: List,
+    feature_importance: Dict[str, float] = {},
+    feature_metadata_fqtn: str = {},
+    feature_metadata_group: str = "default",
+) -> Dict:
     if not isinstance(df, DataFrame):
         raise TypeError("We only support teradataml DataFrame")
 
     # lowercase all keys/names to avoid mismatches between sql/dataframes case sensitivity
     features = [f.lower() for f in features]
     targets = [t.lower() for t in targets]
     categorical = [c.lower() for c in categorical]
     feature_importance = {k.lower(): v for k, v in feature_importance.items()}
     df_columns = [c.lower() for c in df.columns]
 
     # validate that the dataframe contains the features/targets provided
     if features and not set(features).issubset(df_columns):
-        raise ValueError(f"features dataframe with columns ({df.columns}) does not contain features: {features}")
+        raise ValueError(
+            f"features dataframe with columns ({df.columns}) does not contain features: {features}"
+        )
 
     if targets and not set(targets).issubset(df_columns):
-        raise ValueError(f"targets dataframe with columns ({df.columns}) does not contain targets: {targets}")
+        raise ValueError(
+            f"targets dataframe with columns ({df.columns}) does not contain targets: {targets}"
+        )
 
     if not feature_metadata_fqtn:
         raise ValueError("feature_metadata_fqtn must be defined")
 
     total_rows = df.shape[0]
     continuous_vars = list((set(features) | set(targets)) - set(categorical))
     categorical_vars = list((set(features) | set(targets)) - set(continuous_vars))
     reference_edges = []
     reference_categories = []
     available_continuous_vars = []
     available_categorical_vars = []
 
     if len(continuous_vars) > 0:
-        logger.debug(f"Executing this VAL {valib.Statistics(data=df, columns=continuous_vars, stats_options='all').show_query()}")
+        logger.debug(
+            f"Executing this VAL {valib.Statistics(data=df, columns=continuous_vars, stats_options='all').show_query()}"
+        )
         stats = valib.Statistics(data=df, columns=continuous_vars, stats_options="all")
         stats = stats.result.to_pandas().fillna(value_for_nan).reset_index()
         stats["xcol"] = stats["xcol"].str.lower()
 
         stats_metadata = store.get_feature_stats(feature_metadata_fqtn, "continuous")
 
         for v in continuous_vars:
             if v.lower() in stats_metadata.keys():
                 reference_edges.append(stats_metadata[v.lower()]["edges"])
                 available_continuous_vars.append(v)
             else:
-                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
-                               f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}")
+                logger.warning(
+                    f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
+                    f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}"
+                )
 
         if len(available_continuous_vars) > 0:
             hist_boundaries = _convert_all_edges_to_val_str(reference_edges)
-            histogram = _histogram_wrapper(data=df,columns=available_continuous_vars,boundaries=hist_boundaries)
+            histogram = _histogram_wrapper(
+                data=df, columns=available_continuous_vars, boundaries=hist_boundaries
+            )
             histogram["xcol"] = histogram["xcol"].str.lower()
 
     if len(categorical_vars) > 0:
         stats_metadata = store.get_feature_stats(feature_metadata_fqtn, "categorical")
-            
+
         for v in categorical_vars:
             if v.lower() in stats_metadata.keys():
                 reference_categories.append(stats_metadata[v.lower()]["categories"])
                 available_categorical_vars.append(v)
             else:
-                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
-                               f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}")
+                logger.warning(
+                    f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
+                    f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}"
+                )
 
         # We compute frequencies for all categorical features independent of metadata availability
         # But we only reporing number of nulls if reference categories are not available
-        logger.debug(f"Executing this VAL {valib.Frequency(data=df, columns=categorical_vars).show_query()}")
+        logger.debug(
+            f"Executing this VAL {valib.Frequency(data=df, columns=categorical_vars).show_query()}"
+        )
         frequencies = valib.Frequency(data=df, columns=categorical_vars)
         frequencies = frequencies.result.to_pandas(all_rows=True).reset_index()
         frequencies["xcol"] = frequencies["xcol"].str.lower()
 
-    data_struct = {
-        "num_rows": total_rows,
-        "features": {},
-        "targets": {}
-    }
+    data_struct = {"num_rows": total_rows, "features": {}, "targets": {}}
 
     def add_var_metadata(variable_type, group_label):
         if variable_name in continuous_vars:
             if variable_name in available_continuous_vars:
                 data_struct[variable_type][variable_name] = _process_continuous_var(
                     histogram=histogram,
                     stats=stats,
-                    reference_edges=reference_edges[available_continuous_vars.index(variable_name)],
+                    reference_edges=reference_edges[
+                        available_continuous_vars.index(variable_name)
+                    ],
                     group_label=group_label,
                     variable_name=variable_name,
-                    feature_importance=feature_importance.get(variable_name, None))
+                    feature_importance=feature_importance.get(variable_name, None),
+                )
             else:
                 data_struct[variable_type][variable_name] = _process_continuous_var(
                     histogram=pd.DataFrame(),
                     stats=stats,
                     reference_edges=None,
                     group_label=group_label,
                     variable_name=variable_name,
-                    feature_importance=feature_importance.get(variable_name, None))
+                    feature_importance=feature_importance.get(variable_name, None),
+                )
         else:
             if variable_name in available_categorical_vars:
                 data_struct[variable_type][variable_name] = _process_categorical_var(
                     frequencies=frequencies,
                     group_label=group_label,
                     variable_name=variable_name,
                     feature_importance=feature_importance.get(variable_name, None),
-                    reference_categories=reference_categories[available_categorical_vars.index(variable_name)]
+                    reference_categories=reference_categories[
+                        available_categorical_vars.index(variable_name)
+                    ],
                 )
             else:
                 data_struct[variable_type][variable_name] = _process_categorical_var(
                     frequencies=frequencies,
                     group_label=group_label,
                     variable_name=variable_name,
                     feature_importance=feature_importance.get(variable_name, None),
-                    reference_categories=None
+                    reference_categories=None,
                 )
 
     for variable_name in features:
         add_var_metadata("features", feature_metadata_group)
 
     for variable_name in targets:
         add_var_metadata("targets", feature_metadata_group)
 
-    missing_continuous = [c for c in continuous_vars if not(c.lower() in available_continuous_vars)]
-    missing_categorical = [c for c in categorical_vars if not(c.lower() in available_categorical_vars)]
+    missing_continuous = [
+        c for c in continuous_vars if not (c.lower() in available_continuous_vars)
+    ]
+    missing_categorical = [
+        c for c in categorical_vars if not (c.lower() in available_categorical_vars)
+    ]
 
     if len(missing_categorical) > 0 or len(missing_continuous) > 0:
         data_struct["missing_metadata"] = {}
         if len(missing_continuous) > 0:
             data_struct["missing_metadata"]["continuous"] = missing_continuous
         if len(missing_categorical) > 0:
             data_struct["missing_metadata"]["categorical"] = missing_categorical
 
     return data_struct
 
-def _histogram_wrapper(data,columns,boundaries):
+
+def _histogram_wrapper(data, columns, boundaries):
     working_columns = list(columns)
     working_boundaries = list(boundaries)
     result = []
 
     # Iterate over an updated list of columns while it's not empty
     while working_columns:
         tc = list(working_columns)
         tb = list(working_boundaries)
         # If the size of td_analyze parameter is bigger than the limt
         # then reduce the list of columns until it fits
         while _val_parameter_length_too_long(tc, tb):
             if len(tc) == 1:
-                raise Exception(f"VAL histogram parameters are too long even for single column {tc[0]}")
+                raise Exception(
+                    f"VAL histogram parameters are too long even for single column {tc[0]}"
+                )
             tc.pop()
             tb.pop()
-        
+
         # compute a histogram on the longest possible list of columns
-        logger.debug(f"Executing this VAL {valib.Histogram(data=data,columns=tc,boundaries=tb).show_query()}")
-        histogram = valib.Histogram(data=data,columns=tc,boundaries=tb)
+        logger.debug(
+            f"Executing this VAL {valib.Histogram(data=data,columns=tc,boundaries=tb).show_query()}"
+        )
+        histogram = valib.Histogram(data=data, columns=tc, boundaries=tb)
         result.append(histogram.result.to_pandas(all_rows=True).reset_index())
 
-        # removing columns thats already computed 
-        working_columns = working_columns[len(tc):]
-        working_boundaries = working_boundaries[len(tb):]
-    
+        # removing columns thats already computed
+        working_columns = working_columns[len(tc) :]
+        working_boundaries = working_boundaries[len(tb) :]
+
     return pd.concat(result)
 
 
-def _val_parameter_length_too_long(columns,boundaries, limit = 31000):
+def _val_parameter_length_too_long(columns, boundaries, limit=31000):
     db_tbl_string = "database=;tablename=;outputdatabase=;outputtablename=;"
     column_string = f"columns={','.join(columns)};boundaries={','.join(boundaries)};"
     # assuming maximum length for database and table names at 128
     final_length = len(db_tbl_string) + len(column_string) + 128 * 4
     if final_length > limit:
-        logger.debug(f"VAL histogram parameters are too long for these columns, trying to compute sequentially: {','.join(columns)}")
+        logger.debug(
+            f"VAL histogram parameters are too long for these columns, trying to compute sequentially: {','.join(columns)}"
+        )
     return final_length > limit
 
 
-def _round_to_td_float(x, max_digits = 15):
+def _round_to_td_float(x, max_digits=15):
     # This function is needed to cast/round decimal and float number to the maximum precision allowed by Teradata database.
     # Teradata floats allow maximum 15 digits for mantissa, so this strange logic below does exactly that.
     # Possibly at some point we may need to add a round to exponent as well.
     (sign, digits, exponent) = Decimal(x).as_tuple()
     e = len(digits) + exponent
-    (_, m, _) = Decimal(x).scaleb(-e).quantize(Decimal(f"1E-{max_digits}")).normalize().as_tuple()
-    return np.float64(Decimal((sign, m, e - len(m))))
+    (_, m, _) = (
+        Decimal(x)
+        .scaleb(-e)
+        .quantize(Decimal(f"1E-{max_digits}"))
+        .normalize()
+        .as_tuple()
+    )
+    return np.float64(Decimal((sign, m, e - len(m))))
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/stats/store.py` & `teradatamodelops-7.0.6rc2/aoa/stats/store.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,49 +44,59 @@
     execute_sql(m_query)
     logger.debug(dt_query)
     execute_sql(dt_query)
 
 
 def get_feature_stats_summary(features_table: str) -> Dict:
     try:
-      fs = DataFrame.from_query(f"SEL column_name, column_type FROM {features_table}").to_pandas(all_rows=True)
-      fs = fs.reset_index().drop(fs.columns.difference(["column_name", "column_type"]), axis=1)
-      fs = fs.set_index("column_name")
-      return pd.Series(fs.column_type).to_dict()
+        fs = DataFrame.from_query(
+            f"SEL column_name, column_type FROM {features_table}"
+        ).to_pandas(all_rows=True)
+        fs = fs.reset_index().drop(
+            fs.columns.difference(["column_name", "column_type"]), axis=1
+        )
+        fs = fs.set_index("column_name")
+        return pd.Series(fs.column_type).to_dict()
     except Exception:
-       logger.warning("Couldn't read statistics metadata, assuming it's empty")
-       return {}
-
+        logger.warning("Couldn't read statistics metadata, assuming it's empty")
+        return {}
 
 
 def get_feature_stats(features_table: str, feature_type: str) -> Dict:
     try:
-      fs = DataFrame.from_query(f"SEL * FROM {features_table} WHERE column_type='{feature_type}'").to_pandas(all_rows=True)
-      fs = fs.reset_index().drop(fs.columns.difference(["column_name", "stats"]), axis=1)
-      fs = fs.set_index("column_name")
-      fs = pd.Series(fs.stats).to_dict()
-      return {k: json.loads(fs[k]) for k in fs}
+        fs = DataFrame.from_query(
+            f"SEL * FROM {features_table} WHERE column_type='{feature_type}'"
+        ).to_pandas(all_rows=True)
+        fs = fs.reset_index().drop(
+            fs.columns.difference(["column_name", "stats"]), axis=1
+        )
+        fs = fs.set_index("column_name")
+        fs = pd.Series(fs.stats).to_dict()
+        return {k: json.loads(fs[k]) for k in fs}
     except Exception:
-       logger.warning("Couldn't read statistics metadata, assuming it's empty")
-       return {}
+        logger.warning("Couldn't read statistics metadata, assuming it's empty")
+        return {}
 
 
-def get_features_stats_metadata_ct_query(tablename: str, volatile: bool= False) -> str:
-  # It's crucial that we use column_name as a unique index here, because UI currently doesn't allow to set a feature type
-  # If the user wants the same column to play as both continuous and categorical features, she must provide a copy of the column with a different name
-  ct_query = """
+def get_features_stats_metadata_ct_query(tablename: str, volatile: bool = False) -> str:
+    # It's crucial that we use column_name as a unique index here, because UI currently doesn't allow to set a feature type
+    # If the user wants the same column to play as both continuous and categorical features, she must provide a copy of the column with a different name
+    ct_query = """
   CREATE {} (
       column_name VARCHAR(128), 
       column_type VARCHAR(128),
       stats JSON, 
       update_ts TIMESTAMP)
   UNIQUE PRIMARY INDEX ( column_name ){}
   """
-  if volatile:
-    return ct_query.format(f"VOLATILE TABLE {tablename}"," ON COMMIT PRESERVE ROWS;")
-  else:
-    return ct_query.format(f"TABLE {tablename}",";")
+    if volatile:
+        return ct_query.format(
+            f"VOLATILE TABLE {tablename}", " ON COMMIT PRESERVE ROWS;"
+        )
+    else:
+        return ct_query.format(f"TABLE {tablename}", ";")
+
 
 def create_features_stats_table(features_table: str, volatile: bool = False) -> None:
     query = get_features_stats_metadata_ct_query(features_table, volatile)
     logger.debug(query)
     execute_sql(query)
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/util/artifacts.py` & `teradatamodelops-7.0.6rc2/aoa/util/artifacts.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc1/aoa/util/byom.py` & `teradatamodelops-7.0.6rc2/aoa/util/byom.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 from teradataml import DataFrame
 from .connections import execute_sql_in_context
 
 
-def store_byom_tmp(context, table: str, model_version: str, model_bytes: bytes) -> DataFrame:
+def store_byom_tmp(
+    context, table: str, model_version: str, model_bytes: bytes
+) -> DataFrame:
     """
     Store a byom model in a temporary table so we can use it
 
     :param context: get_context()
     :param table: temp table name to use
     :param model_version: model version
     :param model_bytes: model bytes
     :return: DataFrame of model
     """
-    execute_sql_in_context(context, f"""
+    execute_sql_in_context(
+        context,
+        f"""
         CREATE VOLATILE TABLE {table}(
             model_id VARCHAR(255),
             model BLOB(2097088000)
         ) ON COMMIT PRESERVE ROWS;
-        """)
+        """,
+    )
 
-    execute_sql_in_context(context,f"INSERT INTO {table}(model_id, model) values(?,?)",
-                    (model_version, model_bytes))
+    execute_sql_in_context(
+        context,
+        f"INSERT INTO {table}(model_id, model) values(?,?)",
+        (model_version, model_bytes),
+    )
 
-    return DataFrame.from_query(f"""
+    return DataFrame.from_query(
+        f"""
         SELECT model_id, model FROM {table} 
             WHERE model_id='{model_version}'
-        """)
+        """
+    )
 
 
 def check_if_table_exists(context, database: str, name: str, table_kind: str) -> bool:
     """
     Check if the table/view/etc exists in the database
 
     :param context: sqlalchemy context/engine
     :param database: the database
     :param name: the table/view/etc name
     :param table_kind: 'V' for view, 'T' for table etc
     :return: (bool) True if exists, False otherwise
     """
-    rs = execute_sql_in_context(context,f"""
+    rs = execute_sql_in_context(
+        context,
+        f"""
     SELECT * FROM DBC.TABLES WHERE 
         TABLENAME ='{name}' AND 
         tablekind = '{table_kind}' AND 
         databasename='{database}'
-    """)
+    """,
+    )
 
     return rs.rowcount >= 1
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/util/connections.py` & `teradatamodelops-7.0.6rc2/aoa/util/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from teradataml import (
-    create_context,
-    get_context,
-    configure
-)
+from teradataml import create_context, get_context, configure
 
 import os
 import logging
 import urllib.parse
 import sqlalchemy
 
 logger = logging.getLogger(__name__)
@@ -47,55 +43,63 @@
             logger.debug(f"Configuring temp database for tables/views to {database}")
             configure.temp_table_database = database
             configure.temp_view_database = database
 
         configure.val_install_location = os.environ.get("AOA_VAL_INSTALL_DB", "VAL")
         configure.byom_install_location = os.environ.get("AOA_BYOM_INSTALL_DB", "MLDB")
 
-        logger.debug(f"Connecting to {host} on database {database} using logmech {logmech} as {username}")
-        td_sqlalchemy_engine = _aoa_create_engine(host=host,
-                                                  database=database,
-                                                  username=username,
-                                                  password=password,
-                                                  logmech=logmech)
+        logger.debug(
+            f"Connecting to {host} on database {database} using logmech {logmech} as {username}"
+        )
+        td_sqlalchemy_engine = _aoa_create_engine(
+            host=host,
+            database=database,
+            username=username,
+            password=password,
+            logmech=logmech,
+        )
 
         create_context(tdsqlengine=td_sqlalchemy_engine)
 
         from aoa import __version__
-        execute_sql(f"""
+
+        execute_sql(
+            f"""
         SET QUERY_BAND = 'appVersion={__version__};appName=VMO;appFunc=python;org=teradata-internal-telem;' FOR SESSION VOLATILE
-        """)
+        """
+        )
 
     else:
         logger.info("teradataml context already exists. Skipping create_context.")
 
 
-def _aoa_create_engine(host: str,
-                       database: str,
-                       username: str,
-                       password: str,
-                       logmech: str) -> sqlalchemy.engine.Engine:
+def _aoa_create_engine(
+    host: str, database: str, username: str, password: str, logmech: str
+) -> sqlalchemy.engine.Engine:
     """
     Custom create_engine which works around teradataml bug wrt to password encoding. Will be removed when
     teradataml patch is released.
     """
 
     from sqlalchemy import create_engine
     from teradataml.common.exceptions import TeradataMlException
     from teradataml.common.messages import Messages
     from teradataml.common.messagecodes import MessageCodes
 
-    username = '' if username is None else username
-    host_value = '{}:{}@{}'.format(username, password, host)
-    other_connection_parameters = _format_connection_parameters(logmech=logmech,
-                                                                   database=database)
-    
+    username = "" if username is None else username
+    host_value = "{}:{}@{}".format(username, password, host)
+    other_connection_parameters = _format_connection_parameters(
+        logmech=logmech, database=database
+    )
+
     try:
         engine_url = "teradatasql://{}{}"
-        td_sqlalchemy_engine = create_engine(engine_url.format(host_value, other_connection_parameters))
+        td_sqlalchemy_engine = create_engine(
+            engine_url.format(host_value, other_connection_parameters)
+        )
 
         # Masking senstive information - password, logmech and logdata.
         try:
             # Below statement raises an AttributeError with SQLAlchemy
             # version 1.4.x
             td_sqlalchemy_engine.url.password = "***"
         except AttributeError:
@@ -103,54 +107,60 @@
             # converted _URL object to immutable object from version 1.4.x.
             new_url = td_sqlalchemy_engine.url.set(password="***")
             td_sqlalchemy_engine.url = new_url
         except Exception:
             pass
 
         try:
-            if ('LOGMECH' in td_sqlalchemy_engine.url.query):
-                td_sqlalchemy_engine.url.query['LOGMECH'] = "***"
+            if "LOGMECH" in td_sqlalchemy_engine.url.query:
+                td_sqlalchemy_engine.url.query["LOGMECH"] = "***"
         except Exception:
             pass
 
     except TeradataMlException:
         raise
     except Exception as err:
-        raise TeradataMlException(Messages.get_message(MessageCodes.CONNECTION_FAILURE),
-                                  MessageCodes.CONNECTION_FAILURE) from err
+        raise TeradataMlException(
+            Messages.get_message(MessageCodes.CONNECTION_FAILURE),
+            MessageCodes.CONNECTION_FAILURE,
+        ) from err
 
     return td_sqlalchemy_engine
 
 
-def _format_connection_parameters(logmech,database):
+def _format_connection_parameters(logmech, database):
     if not logmech and not database:
         return ""
     result = []
     if logmech:
         result.append(f"LOGMECH={logmech.upper()}")
     if database:
         result.append(f"DATABASE={database.upper()}")
     return "/?{}".format("&".join(result))
 
 
-def execute_sql_in_context(context, statement, parameters = None):
+def execute_sql_in_context(context, statement, parameters=None):
     from teradataml.common.exceptions import TeradataMlException
     from teradataml.common.messages import Messages
     from teradataml.common.messagecodes import MessageCodes
 
     if context is not None:
         tdsql_con = context.raw_connection().driver_connection
         cursor = tdsql_con.cursor()
         return cursor.execute(statement, parameters)
     else:
-        raise TeradataMlException(Messages.get_message(MessageCodes.INVALID_CONTEXT_CONNECTION),
-                                  MessageCodes.INVALID_CONTEXT_CONNECTION)
+        raise TeradataMlException(
+            Messages.get_message(MessageCodes.INVALID_CONTEXT_CONNECTION),
+            MessageCodes.INVALID_CONTEXT_CONNECTION,
+        )
+
+
+def execute_sql(statement, parameters=None):
+    return execute_sql_in_context(get_context(), statement, parameters)
 
-def execute_sql(statement, parameters = None):
-    return execute_sql_in_context(get_context(),statement,parameters)
 
 def tmo_create_context(database: str = None) -> sqlalchemy.engine.Engine:
     """
     Creates a teradataml context if one does not already exist.
     Most users should not need to understand how we pass the environment variables etc for dataset connections. This
     provides a way to achieve that and also allow them to work within a notebook for example where a context is already
     present.
```

### Comparing `teradatamodelops-7.0.6rc1/aoa/util/sto.py` & `teradatamodelops-7.0.6rc2/aoa/util/sto.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,35 @@
 from .connections import execute_sql
 
 import json
 import sys
 
 DEFAULT_STO_MODELS_TABLE = "vmo_sto_models"
 
+
 def save_evaluation_metrics(partition_df: DataFrame, metrics: List):
     """
     :param partition_df: teradata dataframe containing at least ["partition_id", "partition_metadata", "num_rows"]
     :param metrics: list of metrics to normalize and report
     :return: None
     """
     total_rows = int(partition_df.select(["num_rows"]).sum().to_pandas().iloc[0])
 
     metrics_sql = [
         f"SUM(CAST(partition_metadata AS JSON).JSONExtractValue('$.metrics.{metric}') * num_rows/{total_rows}) AS {metric}"
-        for metric in metrics]
-    joined_metrics_sql = ','.join(metrics_sql)
-    metrics = DataFrame.from_query(f"SELECT {joined_metrics_sql} FROM {partition_df._table_name}").to_pandas()
+        for metric in metrics
+    ]
+    joined_metrics_sql = ",".join(metrics_sql)
+    metrics = DataFrame.from_query(
+        f"SELECT {joined_metrics_sql} FROM {partition_df._table_name}"
+    ).to_pandas()
 
     metrics = {metric: "{:.2f}".format(metrics.iloc[0][metric]) for metric in metrics}
 
-    with open("artifacts/output/metrics.json", 'w+') as f:
+    with open("artifacts/output/metrics.json", "w+") as f:
         json.dump(metrics, f, indent=2)
 
 
 def save_metadata(partition_df: DataFrame):
     """
     create statistic summaries based on the provided dataframe produced via training or evaluation
 
@@ -44,42 +48,48 @@
 
     :param partition_df: teradata dataframe containing at least ["partition_id", "partition_metadata", "num_rows"]
     :return: None
     """
 
     total_rows = int(partition_df.select(["num_rows"]).sum().to_pandas().iloc[0])
 
-    metadata_df = partition_df.select(["partition_id", "partition_metadata", "num_rows"]).to_pandas()
-
-    metadata_dict = {r["partition_id"]: json.loads(r["partition_metadata"])
-                     for r in metadata_df.to_dict(orient='records')}
+    metadata_df = partition_df.select(
+        ["partition_id", "partition_metadata", "num_rows"]
+    ).to_pandas()
+
+    metadata_dict = {
+        r["partition_id"]: json.loads(r["partition_metadata"])
+        for r in metadata_df.to_dict(orient="records")
+    }
 
-    with open("artifacts/output/partitions.json", 'w+') as f:
+    with open("artifacts/output/partitions.json", "w+") as f:
         json.dump(metadata_dict, f, indent=2)
 
     data_metadata = {
         "num_rows": total_rows,
-        "num_partitions": int(metadata_df.shape[0])
+        "num_partitions": int(metadata_df.shape[0]),
     }
 
-    with open("artifacts/output/data_stats.json", 'w+') as f:
+    with open("artifacts/output/data_stats.json", "w+") as f:
         json.dump(data_metadata, f, indent=2)
 
 
 def cleanup_cli(model_version: str, models_table: str = DEFAULT_STO_MODELS_TABLE):
     """
     cli uses model version of "cli" always. We need to cleanup models table between runs.
     A better solution would be for the cli to write to a different table completely and just "recreate" on each run
 
     :param model_version: the model version being executed
     :param models_table: the models table for cleanup (default is vmo_sto_models)
     :return: None
     """
     if model_version == "cli":
-        execute_sql("DELETE FROM {table} WHERE model_version='cli'".format(table=models_table))
+        execute_sql(
+            "DELETE FROM {table} WHERE model_version='cli'".format(table=models_table)
+        )
 
 
 def check_sto_version(python_interpreter="tdpython3"):
     """
     Check Python version In-Vantage against the version where this function is running,
     if it's incompatible raise an exception
 
@@ -89,30 +99,39 @@
     version_query = f"""
     SEL DISTINCT ver
     FROM SCRIPT(
         SCRIPT_COMMAND('{python_interpreter} -c "import sys; print(\\".\\".join(map(str, sys.version_info[0:2])))"')
         RETURNS('ver VARCHAR(10)') 
     );
     """
-    local_version = '.'.join(map(str, sys.version_info[0:2]))
+    local_version = ".".join(map(str, sys.version_info[0:2]))
     result = execute_sql(version_query)
     if result.rowcount != 1:
-        raise Exception('Different STO configuration on different nodes, please contact your system administrator')
+        raise Exception(
+            "Different STO configuration on different nodes, please contact your system administrator"
+        )
     try:
         remote_version = next(iter(result))[0]
     except Exception as err:
-        raise Exception(f"Different STO configuration on different nodes, please contact your system administrator. "
-                        f"\nError: {err}")
+        raise Exception(
+            f"Different STO configuration on different nodes, please contact your system administrator. "
+            f"\nError: {err}"
+        )
 
     if local_version != remote_version:
-        raise Exception('Python versions not matching, local: {local}, In-Vantage: {remote}'.format(local=local_version,
-                                                                                                    remote=remote_version))
+        raise Exception(
+            "Python versions not matching, local: {local}, In-Vantage: {remote}".format(
+                local=local_version, remote=remote_version
+            )
+        )
 
 
-def collect_sto_versions(raise_diff_config_exception=True,python_interpreter="tdpython3"):
+def collect_sto_versions(
+    raise_diff_config_exception=True, python_interpreter="tdpython3"
+):
     """
     Collects Python and packages information from In-Vantage installation
 
     :param python_interpreter: path to python interpreter on Vantage node (default is tdpython3)
     :param raise_diff_config_exception: whether raise an exception if different Python versions are detected on different AMPs of Vantage system
     :return: Dict with python_version and packages versions
     """
@@ -121,41 +140,47 @@
     FROM SCRIPT(
         SCRIPT_COMMAND('{python_interpreter} -c "import sys; print(sys.version.replace(\\"\\n\\",\\" \\"))"')
         RETURNS('ver VARCHAR(100)') 
     );
     """
     result = execute_sql(python_version_query)
     if result.rowcount != 1 and raise_diff_config_exception:
-        raise Exception('Different STO configuration on different nodes, please contact your system administrator')
+        raise Exception(
+            "Different STO configuration on different nodes, please contact your system administrator"
+        )
     try:
         python_version = next(iter(result))[0]
     except Exception as err:
-        raise Exception(f"Different STO configuration on different nodes, please contact your system administrator. "
-                        f"\nError: {err}")
+        raise Exception(
+            f"Different STO configuration on different nodes, please contact your system administrator. "
+            f"\nError: {err}"
+        )
 
     packages_version_query = f"""
     SEL DISTINCT pkg
     FROM SCRIPT(
         SCRIPT_COMMAND('{python_interpreter} -c "import pkg_resources; [print(pkg) for pkg in pkg_resources.working_set]"')
         RETURNS('pkg VARCHAR(100)') 
     );
     """
     result = execute_sql(packages_version_query)
     packages = {}
     for row in result:
         pair = row[0].split(" ")
         packages[pair[0]] = pair[1]
 
-    return {'python_version': python_version, 'packages': packages}
+    return {"python_version": python_version, "packages": packages}
 
 
-def get_joined_models_df(data_table: str,
-                         model_artefacts_table: str,
-                         model_version: str,
-                         partition_id: str = "partition_id"):
+def get_joined_models_df(
+    data_table: str,
+    model_artefacts_table: str,
+    model_version: str,
+    partition_id: str = "partition_id",
+):
     """
     Joins the dataset which is to be used for scoring/evaluation with the model artefacts and appends the model_artefact
     to the first row with the column name 'model'.
 
     Args:
         data_table: the table/view of the dataset to join
         model_artefacts_table: the model artefacts table where the model artefacts are stored
@@ -172,18 +197,20 @@
         ON d.{partition_id} = m.partition_id
         WHERE m.model_version = '{model_version}'
     """
 
     return DataFrame.from_query(query)
 
 
-def get_joined_single_model_df(data_table: str,
-                               model_version: str,
-                               model_artefacts_table: str = DEFAULT_STO_MODELS_TABLE,
-                               partition_id: str = "partition_id"):
+def get_joined_single_model_df(
+    data_table: str,
+    model_version: str,
+    model_artefacts_table: str = DEFAULT_STO_MODELS_TABLE,
+    partition_id: str = "partition_id",
+):
     """
     Joins the dataset which is to be used for scoring/evaluation with a single model artefact and appends that artefact
     to the first row of each partition with the column name 'model'.
     If there's more than one artefact corresponding to 'model_version' then the random first one is taken.
 
 
     Args:
@@ -199,25 +226,30 @@
     SELECT d.*, CASE WHEN n_row=1 THEN m.model ELSE null END AS model 
         FROM (SEL x.*, ROW_NUMBER() OVER (PARTITION BY x.{partition_id} ORDER BY x.{partition_id}) AS n_row FROM {data_table} x) AS d
         CROSS JOIN (SEL * FROM {model_artefacts_table} WHERE model_version = '{model_version}' QUALIFY CSUM(1,1) = 1) m
     """
 
     return DataFrame.from_query(query)
 
-def get_joined_partitioned_models_df(data_table: str,
-                               model_version: str,
-                               model_artefacts_table: str = DEFAULT_STO_MODELS_TABLE,
-                               partition_id: str = "partition_id"):
+
+def get_joined_partitioned_models_df(
+    data_table: str,
+    model_version: str,
+    model_artefacts_table: str = DEFAULT_STO_MODELS_TABLE,
+    partition_id: str = "partition_id",
+):
     """
     Joins the dataset which is to be used for scoring/evaluation with the model artefacts and appends the artefact
     to the first row with the column name 'model'.
 
     Args:
         data_table: the table/view of the dataset to join
         model_version: the model version to use from the model artefacts
         model_artefacts_table: the model artefacts table where the model artefacts are stored (defaults to vmo_sto_models)
         partition_id: the dataset partition_id
 
     Returns:
         DataFrame
     """
-    return get_joined_models_df(data_table, model_artefacts_table, model_version, partition_id)
+    return get_joined_models_df(
+        data_table, model_artefacts_table, model_version, partition_id
+    )
```

### Comparing `teradatamodelops-7.0.6rc1/scripts/tmo` & `teradatamodelops-7.0.6rc2/scripts/tmo`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import yaml
 
 from pathlib import Path
 from aoa.crypto import crypto
 
 base_path = os.path.abspath(os.getcwd())
 model_catalog = os.path.join(base_path, "model_definitions/")
-available_modes = ['Train', 'Evaluate', 'Score']
+available_modes = ["Train", "Evaluate", "Score"]
 config_dir = f"{Path.home()}/.aoa"
 
 
 def validate_cwd_valid():
     return os.path.exists(model_catalog)
 
 
@@ -27,109 +27,130 @@
 
     repo_manager.init_model_directory()
 
     if not repo_manager.repo_config_exists():
         link_repo(repo_manager=repo_manager, aoa_client=aoa_client)
 
 
-def input_string(name, required=False, tooltip='', password=False, called_from_test=False):
+def input_string(
+    name, required=False, tooltip="", password=False, called_from_test=False
+):
     from getpass import getpass
 
-    if tooltip != '':
+    if tooltip != "":
         print(tooltip)
 
-    value = getpass("Enter {}: ".format(name)) if password and not called_from_test else input(
-        "Enter {}: ".format(name))
+    value = (
+        getpass("Enter {}: ".format(name))
+        if password and not called_from_test
+        else input("Enter {}: ".format(name))
+    )
 
-    if value == '' and required:
-        print('Value required. Please try again.')
-        print('You may cancel at anytime by pressing Ctrl+C')
+    if value == "" and required:
+        print("Value required. Please try again.")
+        print("You may cancel at anytime by pressing Ctrl+C")
         print("")
         return input_string(name, required, tooltip)
 
     return value
 
 
-def input_select(name, values, label='', default=None):
+def input_select(name, values, label="", default=None):
     if len(values) == 0:
         return
 
-    if label != '':
+    if label != "":
         print_underscored(label)
 
     for ix, item in enumerate(values):
-        default_text = " (default)" if default and default == item else ''
+        default_text = " (default)" if default and default == item else ""
         print("[{}] {}".format(ix, item) + default_text)
 
-    tmp_index = input("Select {} by index (or leave blank for the default one): ".format(name)) if default else input(
-        "Select {} by index: ".format(name))
+    tmp_index = (
+        input("Select {} by index (or leave blank for the default one): ".format(name))
+        if default
+        else input("Select {} by index: ".format(name))
+    )
 
-    if default and default in values and tmp_index == '':
+    if default and default in values and tmp_index == "":
         tmp_index = values.index(default)
-    elif (tmp_index == '' and not default) or (not tmp_index.isnumeric() or int(tmp_index) >= len(values)):
-        print('Wrong selection, please try again by selecting the index number on the first column.')
-        print('You may cancel at anytime by pressing Ctrl+C.')
+    elif (tmp_index == "" and not default) or (
+        not tmp_index.isnumeric() or int(tmp_index) >= len(values)
+    ):
+        print(
+            "Wrong selection, please try again by selecting the index number on the first column."
+        )
+        print("You may cancel at anytime by pressing Ctrl+C.")
         print("")
         return input_select(name, values, label, default)
 
     return values[int(tmp_index)]
 
 
 def yes_or_no(question):
     while "the answer is invalid":
-        reply = str(input(question + ' (y/n): ')).lower().strip()
-        if reply[:1] == 'y':
+        reply = str(input(question + " (y/n): ")).lower().strip()
+        if reply[:1] == "y":
             return True
-        if reply[:1] == 'n':
+        if reply[:1] == "n":
             return False
 
 
 def bash_escape(string):
-    return string.replace('\\', '\\\\')
+    return string.replace("\\", "\\\\")
 
 
 def add_model(args, repo_manager, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     if not validate_cwd_valid():
-        logging.error("Current working directory must the root of a model repository to execute this command")
+        logging.error(
+            "Current working directory must the root of a model repository to execute this command"
+        )
         exit(1)
 
     import tempfile
+
     temp_path = tempfile.TemporaryDirectory()
     logging.info("Using this model catalog from Git repo {}".format(args.template_url))
     repo_manager.clone_repository(args.template_url, temp_path.name, args.branch)
 
     templates = repo_manager.get_templates(source_path=temp_path.name)
     if len(templates) == 0:
         logging.error(
-            "Repo doesn't contain any models to use as templates, use different repo as a model catalog")
+            "Repo doesn't contain any models to use as templates, use different repo as a model catalog"
+        )
         exit(1)
 
     print("")
-    model_lang = input_select("model language", list(templates.keys()), "Available languages:")
+    model_lang = input_select(
+        "model language", list(templates.keys()), "Available languages:"
+    )
 
     print("")
     models = {f"{v[0]} ({k})": k for k, v in templates[model_lang].items()}
-    model_template = input_select("template type", list(models.keys()), "Available models:")
+    model_template = input_select(
+        "template type", list(models.keys()), "Available models:"
+    )
     model_template_dir = templates[model_lang][models[model_template]][1]
 
-    model_name = input_string('model name', True)
-    model_desc = input_string('model description', False)
+    model_name = input_string("model name", True)
+    model_desc = input_string("model description", False)
 
     import uuid
+
     model_id = str(uuid.uuid4())
 
     repo_manager.add_model(
         model_id=model_id,
         model_name=model_name,
         model_desc=model_desc,
         template=model_template_dir,
-        base_path=base_path
+        base_path=base_path,
     )
     print("Creating model structure for model: ({}) {}".format(model_id, model_name))
 
 
 def run_model(args, repo_manager, aoa_client, **kwargs):
     from aoa import TrainModel
     from aoa import EvaluateModel
@@ -139,157 +160,228 @@
     import json
 
     if args.cwd:
         set_cwd(args.cwd)
 
     current_project = get_current_project(repo_manager, aoa_client, True)
     if not current_project:
-        logging.error("Current working directory must the root of a model repository to execute this command")
+        logging.error(
+            "Current working directory must the root of a model repository to execute this command"
+        )
         exit(1)
 
     aoa_client.set_project_id(current_project["id"])
 
     def _select_model_id(catalog):
-        catalog_values = [catalog[i]['name'] for i in catalog]
-        selected_model_value = input_select('model', catalog_values, 'Available models:')
-        selected_model = next((catalog[i] for i in catalog if catalog[i]['name'] == selected_model_value), None)
+        catalog_values = [catalog[i]["name"] for i in catalog]
+        selected_model_value = input_select(
+            "model", catalog_values, "Available models:"
+        )
+        selected_model = next(
+            (catalog[i] for i in catalog if catalog[i]["name"] == selected_model_value),
+            None,
+        )
         print("")
-        return selected_model['id'] if 'id' in selected_model else None
+        return selected_model["id"] if "id" in selected_model else None
 
     def _select_mode():
-        selected_mode = input_select('mode', available_modes, 'Available modes:').lower()
+        selected_mode = input_select(
+            "mode", available_modes, "Available modes:"
+        ).lower()
         print("")
         return selected_mode
 
     def _select_dataset(dataset_list):
         dataset_values = [i["name"] for i in dataset_list]
-        selected_dataset_value = input_select('dataset', dataset_values, 'Available datasets:')
-        selected_dataset = next((i for i in dataset_list if i['name'] == selected_dataset_value), None)
+        selected_dataset_value = input_select(
+            "dataset", dataset_values, "Available datasets:"
+        )
+        selected_dataset = next(
+            (i for i in dataset_list if i["name"] == selected_dataset_value), None
+        )
         print("")
         return selected_dataset
 
     def _select_dataset_template(template_list):
         template_values = [i["name"] for i in template_list]
-        selected_template_value = input_select('dataset template', template_values, 'Available dataset templates:')
-        selected_template = next((i for i in template_list if i['name'] == selected_template_value), None)
+        selected_template_value = input_select(
+            "dataset template", template_values, "Available dataset templates:"
+        )
+        selected_template = next(
+            (i for i in template_list if i["name"] == selected_template_value), None
+        )
         print("")
         return selected_template
 
     def _select_connection(connection=None):
         from argparse import Namespace
+
         return activate_connection(Namespace(cwd=None, connection=connection))
 
     available_models = TrainModel.get_model_ids(model_catalog, True)
 
     if not args.model_id:
         model_id = _select_model_id(available_models)
     else:
         model_id_exists = next(
-            (available_models[i] for i in available_models if available_models[i]['id'] == args.model_id), False)
+            (
+                available_models[i]
+                for i in available_models
+                if available_models[i]["id"] == args.model_id
+            ),
+            False,
+        )
         if not model_id_exists:
-            print('Model not found. Please select one from the list below or press Ctrl+C to quit.')
-        model_id = args.model_id if model_id_exists else _select_model_id(available_models)
+            print(
+                "Model not found. Please select one from the list below or press Ctrl+C to quit."
+            )
+        model_id = (
+            args.model_id if model_id_exists else _select_model_id(available_models)
+        )
 
     if not args.mode:
         mode = _select_mode()
 
     else:
-        mode_exists = True if args.mode in [x.lower() for x in available_modes] else False
+        mode_exists = (
+            True if args.mode in [x.lower() for x in available_modes] else False
+        )
         if not mode_exists:
-            print('Mode not found. Please select one from the list below or press Ctrl+C to quit.')
+            print(
+                "Mode not found. Please select one from the list below or press Ctrl+C to quit."
+            )
         mode = args.mode if mode_exists else _select_mode()
 
     if args.local_dataset:
-        with open(args.local_dataset, 'r') as f:
+        with open(args.local_dataset, "r") as f:
             rendered_dataset = json.load(f)
 
     elif args.local_dataset_template:
-        with open(args.local_dataset_template, 'r') as f:
+        with open(args.local_dataset_template, "r") as f:
             rendered_dataset = json.load(f)
 
     else:
         if mode == "score":
-            dataset_template_api = DatasetTemplateApi(aoa_client=aoa_client, show_archived=False)
+            dataset_template_api = DatasetTemplateApi(
+                aoa_client=aoa_client, show_archived=False
+            )
 
             available_templates = list(dataset_template_api)
             if not args.local_dataset_template and not args.dataset_template_id:
                 template = _select_dataset_template(available_templates)
                 if not template:
                     logging.error("No dataset templates found in project")
                     exit(1)
 
             elif args.dataset_template_id:
-                template_exists = next((True for i in available_templates if i['id'] == args.dataset_template_id),
-                                       False)
+                template_exists = next(
+                    (
+                        True
+                        for i in available_templates
+                        if i["id"] == args.dataset_template_id
+                    ),
+                    False,
+                )
                 if not template_exists:
-                    print('Dataset template not found. Please select one from the list below or press Ctrl+C to quit.')
-                template = dataset_template_api.find_by_id(
-                    args.dataset_template_id) if template_exists else _select_dataset_template(available_templates)
+                    print(
+                        "Dataset template not found. Please select one from the list below or press Ctrl+C to quit."
+                    )
+                template = (
+                    dataset_template_api.find_by_id(args.dataset_template_id)
+                    if template_exists
+                    else _select_dataset_template(available_templates)
+                )
 
             dataset_template_id = template["id"]
 
             rendered_dataset = dataset_template_api.render(id=dataset_template_id)
 
         else:
-            template_api = DatasetTemplateApi(aoa_client=aoa_client, show_archived=False)
+            template_api = DatasetTemplateApi(
+                aoa_client=aoa_client, show_archived=False
+            )
             dataset_api = DatasetApi(aoa_client=aoa_client, show_archived=False)
 
             if not args.local_dataset and not args.dataset_id:
                 available_templates = list(template_api)
                 template = _select_dataset_template(available_templates)
                 if not template:
                     logging.error("No dataset template found in project")
                     exit(1)
 
                 from aoa.api.api_iterator import ApiIterator
                 from functools import partial
-                available_datasets = list(ApiIterator(
-                    api_func=partial(dataset_api.find_by_dataset_template_id, template["id"], archived=False),
-                    entities="datasets"))
+
+                available_datasets = list(
+                    ApiIterator(
+                        api_func=partial(
+                            dataset_api.find_by_dataset_template_id,
+                            template["id"],
+                            archived=False,
+                        ),
+                        entities="datasets",
+                    )
+                )
                 dataset = _select_dataset(available_datasets)
                 if not dataset:
                     logging.error("No datasets found in project")
                     exit(1)
 
             elif args.dataset_id:
                 dataset = dataset_api.find_by_id(args.dataset_id)
                 if not dataset:
-                    print('Dataset not found. Please select one from the list below or press Ctrl+C to quit.')
+                    print(
+                        "Dataset not found. Please select one from the list below or press Ctrl+C to quit."
+                    )
                     exit(1)
 
             dataset_id = dataset["id"]
 
             rendered_dataset = dataset_api.render(dataset_id)
 
     connection_id = _select_connection(args.connection if args.connection else None)
 
     print("")
     print("To execute the same command again run:")
     if mode != "score":
         if args.local_dataset:
-            print(f"tmo run -m {mode} -id {model_id} -c {connection_id} -ld {args.local_dataset}")
+            print(
+                f"tmo run -m {mode} -id {model_id} -c {connection_id} -ld {args.local_dataset}"
+            )
         else:
-            print(f"tmo run -m {mode} -id {model_id} -d {dataset_id} -c {connection_id}")
+            print(
+                f"tmo run -m {mode} -id {model_id} -d {dataset_id} -c {connection_id}"
+            )
     else:
         if args.local_dataset_template:
-            print(f"tmo run -m {mode} -id {model_id} -c {connection_id} -lt {args.local_dataset_template}")
+            print(
+                f"tmo run -m {mode} -id {model_id} -c {connection_id} -lt {args.local_dataset_template}"
+            )
         else:
-            print(f"tmo run -m {mode} -id {model_id} -t {dataset_template_id} -c {connection_id}")
+            print(
+                f"tmo run -m {mode} -id {model_id} -t {dataset_template_id} -c {connection_id}"
+            )
     print("")
     print("")
 
     if mode == "train":
         trainer = TrainModel(repo_manager)
-        trainer.train_model_local(model_id, rendered_dataset=rendered_dataset, base_path=base_path)
+        trainer.train_model_local(
+            model_id, rendered_dataset=rendered_dataset, base_path=base_path
+        )
     elif mode == "evaluate":
         evaluator = EvaluateModel(repo_manager)
-        evaluator.evaluate_model_local(model_id, rendered_dataset=rendered_dataset, base_path=base_path)
+        evaluator.evaluate_model_local(
+            model_id, rendered_dataset=rendered_dataset, base_path=base_path
+        )
     elif mode == "score":
         scorer = ScoreModel(repo_manager)
-        scorer.batch_score_model_local(model_id, rendered_dataset=rendered_dataset, base_path=base_path)
+        scorer.batch_score_model_local(
+            model_id, rendered_dataset=rendered_dataset, base_path=base_path
+        )
     else:
         logging.error("Unsupported mode used: " + mode)
         exit(1)
 
 
 def list_resources(args, repo_manager, aoa_client, **kwargs):
     from aoa import TrainModel
@@ -312,34 +404,45 @@
             project = list_and_select_projects(repo_manager, aoa_client, False, True)
 
         model_api = ModelApi(aoa_client, show_archived=False)
         print_underscored("List of models for project {}:".format(project["name"]))
         if not len(model_api) > 0:
             print("No models were found")
         for i, model in enumerate(model_api):
-            print("[{}] Id: ({}) Type: ({}) {}".format(i, model["id"], model["source"], model["name"]))
+            print(
+                "[{}] Id: ({}) Type: ({}) {}".format(
+                    i, model["id"], model["source"], model["name"]
+                )
+            )
 
     if args.local_models:
         local_models = TrainModel.get_model_folders(model_catalog, True)
         print_underscored("List of local models:")
         if not len(local_models) > 0:
             print("No local models were found")
         for local_model in local_models:
-            print("[{}] {} (Git: {})".format(local_model, local_models[local_model]["name"],
-                                             local_models[local_model]["id"]))
+            print(
+                "[{}] {} (Git: {})".format(
+                    local_model,
+                    local_models[local_model]["name"],
+                    local_models[local_model]["id"],
+                )
+            )
 
     if args.templates:
         project = get_current_project(repo_manager, aoa_client)
         if project:
             aoa_client.set_project_id(project["id"])
         else:
             project = list_and_select_projects(repo_manager, aoa_client, False, True)
 
         template_api = DatasetTemplateApi(aoa_client=aoa_client, show_archived=False)
-        print_underscored("List of dataset templates for project {}:".format(project["name"]))
+        print_underscored(
+            "List of dataset templates for project {}:".format(project["name"])
+        )
         if not len(template_api) > 0:
             print("No dataset templates were found")
         for i, template in enumerate(template_api):
             print("[{}] ({}) {}".format(i, template["id"], template["name"]))
 
     if args.datasets:
         project = get_current_project(repo_manager, aoa_client)
@@ -353,17 +456,25 @@
         if not len(dataset_api) > 0:
             print("No datasets were found")
         for i, dataset in enumerate(dataset_api):
             print("[{}] ({}) {}".format(i, dataset["id"], dataset["name"]))
 
     if args.connections:
         from argparse import Namespace
+
         list_connections(Namespace(cwd=None, connections=None))
 
-    elif not args.projects and not args.models and not args.local_models and not args.templates and not args.datasets and not args.connections:
+    elif (
+        not args.projects
+        and not args.models
+        and not args.local_models
+        and not args.templates
+        and not args.datasets
+        and not args.connections
+    ):
         logging.error("Invalid object selection...")
         kwargs.get("parent_parser").print_help()
         exit(1)
 
 
 def clone(args, repo_manager, aoa_client, **kwargs):
     if args.cwd:
@@ -376,311 +487,397 @@
 
         project_api = ProjectApi(aoa_client=aoa_client, show_archived=False)
         try:
             project = project_api.find_by_id(args.project_id)
         except Exception:
             project = None
         if not project:
-            print('Project not found. Please select one from the list below or press Ctrl+C to quit.')
+            print(
+                "Project not found. Please select one from the list below or press Ctrl+C to quit."
+            )
             project = list_and_select_projects(repo_manager, aoa_client, False, True)
 
     if args.path:
         path = args.path
     else:
         path = os.path.join(base_path, project["name"])
 
     project_git = project["gitRepositoryUrl"]
 
     repo_manager.clone_repository(project_git, path, project.get("branch", "master"))
 
-    config = {
-        "project_id": project['id']
-    }
+    config = {"project_id": project["id"]}
     repo_manager.write_repo_config(config, path)
     print("Project cloned at {}".format(path))
 
 
 def list_connections(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     try:
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'r') as f:
+        with open(connections_file, "r") as f:
             connections = yaml.safe_load(f)
     except:
         logging.error("No connections file found. Please add them first.")
         exit(1)
 
-    if 'connections' in connections and len(connections['connections']) > 0:
+    if "connections" in connections and len(connections["connections"]) > 0:
         print_underscored("List of local connections:")
-        for i, connection in enumerate(connections['connections']):
+        for i, connection in enumerate(connections["connections"]):
             print(
-                "[{}] ({}) Name: {} Username: {} Host: {} Database: {}".format(i, connection["id"], connection["name"],
-                                                                               connection["username"],
-                                                                               connection["host"],
-                                                                               connection.get("database", "")))
+                "[{}] ({}) Name: {} Username: {} Host: {} Database: {}".format(
+                    i,
+                    connection["id"],
+                    connection["name"],
+                    connection["username"],
+                    connection["host"],
+                    connection.get("database", ""),
+                )
+            )
     else:
         logging.error("No connections found in file. Please add them first.")
 
 
 def add_connections(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     try:
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'r') as f:
+        with open(connections_file, "r") as f:
             connections_dict = yaml.safe_load(f)
             if connections_dict is None:
                 connections_dict = {}
     except:
         logging.info("No connections file found, creating new one...")
         connections_dict = {}
 
-    connections = connections_dict['connections'] if connections_dict and 'connections' in connections_dict and len(
-        connections_dict['connections']) > 0 else []
+    connections = (
+        connections_dict["connections"]
+        if connections_dict
+        and "connections" in connections_dict
+        and len(connections_dict["connections"]) > 0
+        else []
+    )
 
     if args.name and args.username and args.password and args.host:
         name = args.name
         username = args.username
         password = args.password
         host = args.host
         database = args.database
         val_db = args.val_db
         byom_db = args.byom_db
 
     elif not (args.username or args.password or args.name or args.host):
-        name = input_string(name='name', tooltip='Type the connection name')
-        username = input_string(name='username', tooltip='Type the connection username')
-        password = input_string(name='password', tooltip='Type the connection password (will not show)', password=True)
-        host = input_string(name='host', tooltip='Type the connection host')
-        byom_db = input_string(name='BYOM database',
-                               required=True,
-                               tooltip='The BYOM installation to use')
-        val_db = input_string(name='VAL database ',
-                              required=True,
-                              tooltip='The VAL installation to use')
-        database = input_string(name='database',
-                                required=False,
-                                tooltip='Type the default database (optional)')
+        name = input_string(name="name", tooltip="Type the connection name")
+        username = input_string(name="username", tooltip="Type the connection username")
+        password = input_string(
+            name="password",
+            tooltip="Type the connection password (will not show)",
+            password=True,
+        )
+        host = input_string(name="host", tooltip="Type the connection host")
+        byom_db = input_string(
+            name="BYOM database", required=True, tooltip="The BYOM installation to use"
+        )
+        val_db = input_string(
+            name="VAL database ", required=True, tooltip="The VAL installation to use"
+        )
+        database = input_string(
+            name="database",
+            required=False,
+            tooltip="Type the default database (optional)",
+        )
 
     else:
         logging.error("Invalid arguments...")
         args.parent_parser.print_help()
         exit(1)
 
     import uuid
+
     connection_id = str(uuid.uuid4())
     encrypted_password = crypto.td_encrypt_password(
         password=password,
         pass_key_filename="{}/{}.key".format(config_dir, connection_id),
-        enc_pass_filename="{}/{}.pass".format(config_dir, connection_id))
+        enc_pass_filename="{}/{}.pass".format(config_dir, connection_id),
+    )
 
-    connections.append({
-        'id': connection_id,
-        'name': name,
-        'username': username,
-        'password': encrypted_password,
-        'host': host,
-        'logmech': 'TDNEGO',
-        'database': database,
-        'val_db': val_db,
-        'byom_db': byom_db
-    })
-    connections_dict['connections'] = connections
+    connections.append(
+        {
+            "id": connection_id,
+            "name": name,
+            "username": username,
+            "password": encrypted_password,
+            "host": host,
+            "logmech": "TDNEGO",
+            "database": database,
+            "val_db": val_db,
+            "byom_db": byom_db,
+        }
+    )
+    connections_dict["connections"] = connections
 
     try:
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'w+') as f:
+        with open(connections_file, "w+") as f:
             yaml.safe_dump(connections_dict, f, default_flow_style=False)
     except Exception as ex:
         logging.error("Can't save connections file: {}".format(ex))
         exit(1)
 
 
 def remove_connections(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     def _check_connection_exists(id, obj):
         for connection in obj:
-            if 'id' in connection and connection['id'] == id:
+            if "id" in connection and connection["id"] == id:
                 return True
         return False
 
     def _remove_connection(id, obj):
         if os.path.exists("{}/{}.key".format(config_dir, id)):
             os.remove("{}/{}.key".format(config_dir, id))
         if os.path.exists("{}/{}.pass".format(config_dir, id)):
             os.remove("{}/{}.pass".format(config_dir, id))
         result = []
         for item in obj:
-            if item['id'] != id:
+            if item["id"] != id:
                 result.append(item)
         return result
 
     try:
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'r') as f:
+        with open(connections_file, "r") as f:
             connections_dict = yaml.safe_load(f)
             if connections_dict is None or not (
-                    'connections' in connections_dict and len(connections_dict['connections']) > 0):
+                "connections" in connections_dict
+                and len(connections_dict["connections"]) > 0
+            ):
                 logging.info("No connections defined, nothing to remove.")
     except:
         logging.info("No connections file found, nothing to remove.")
         exit(0)
 
-    connections = connections_dict['connections'] if 'connections' in connections_dict and len(
-        connections_dict['connections']) > 0 else []
+    connections = (
+        connections_dict["connections"]
+        if "connections" in connections_dict
+        and len(connections_dict["connections"]) > 0
+        else []
+    )
     if args.connection:
         id = args.connection
         if not _check_connection_exists(id, connections):
-            logging.info('Connection does not exists, exiting.')
+            logging.info("Connection does not exists, exiting.")
             exit(1)
     else:
-        name = input_select('connection', [item['name'] for item in connections], 'List of local connections')
+        name = input_select(
+            "connection",
+            [item["name"] for item in connections],
+            "List of local connections",
+        )
         connection = next(
-            (connections[i]['id'] for i, item in enumerate(connections) if connections[i]['name'] == name), None)
+            (
+                connections[i]["id"]
+                for i, item in enumerate(connections)
+                if connections[i]["name"] == name
+            ),
+            None,
+        )
 
     connections = _remove_connection(connection, connections)
-    connections_dict['connections'] = connections
+    connections_dict["connections"] = connections
 
     try:
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'w+') as f:
+        with open(connections_file, "w+") as f:
             yaml.safe_dump(connections_dict, f, default_flow_style=False)
     except Exception as ex:
         logging.error("Can't save connections file: {}".format(ex))
         exit(1)
 
 
 def export_connection(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     def _check_connection_exists(id, obj):
         for connection in obj:
-            if 'id' in connection and connection['id'] == id:
+            if "id" in connection and connection["id"] == id:
                 return True
         return False
 
     try:
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'r') as f:
+        with open(connections_file, "r") as f:
             connections_dict = yaml.safe_load(f)
             if connections_dict is None or not (
-                    'connections' in connections_dict and len(connections_dict['connections']) > 0):
+                "connections" in connections_dict
+                and len(connections_dict["connections"]) > 0
+            ):
                 logging.info("No connections defined, Please add them first.")
     except:
         logging.info("No connections file found, Please add them first.")
         exit(0)
 
-    connections = connections_dict['connections'] if 'connections' in connections_dict and len(
-        connections_dict['connections']) > 0 else []
+    connections = (
+        connections_dict["connections"]
+        if "connections" in connections_dict
+        and len(connections_dict["connections"]) > 0
+        else []
+    )
     if args.connection:
         id = args.connection
         if not _check_connection_exists(id, connections):
-            logging.info('Connection does not exists, exiting.')
+            logging.info("Connection does not exists, exiting.")
             exit(1)
     else:
-        name = input_select('connection', [item['name'] for item in connections], 'List of local connections')
-        connection = next((connections[i] for i, item in enumerate(connections) if connections[i]['name'] == name),
-                          None)
+        name = input_select(
+            "connection",
+            [item["name"] for item in connections],
+            "List of local connections",
+        )
+        connection = next(
+            (
+                connections[i]
+                for i, item in enumerate(connections)
+                if connections[i]["name"] == name
+            ),
+            None,
+        )
 
     print("\nCopy the below command and execute in your terminal: \n")
-    print("export AOA_CONN_USERNAME=\"{}\" && \\\n".format(bash_escape(connection['username'])) +
-          "export AOA_CONN_PASSWORD=\"{}\" && \\\n".format(bash_escape(connection['password'])) +
-          "export AOA_CONN_HOST=\"{}\" && \\\n".format(bash_escape(connection['host'])) +
-          "export AOA_CONN_LOG_MECH=\"{}\" && \\\n".format(bash_escape(connection['logmech'])) +
-          "export AOA_CONN_DATABASE=\"{}\" && \\\n".format(bash_escape(connection.get('database', ""))) +
-          "export AOA_VAL_INSTALL_DB=\"{}\" && \\\n".format(bash_escape(connection.get('val_db', "VAL"))) +
-          "export AOA_BYOM_INSTALL_DB=\"{}\" && \\\n".format(bash_escape(connection.get('byom_db', "BYOM")))
-          )
+    print(
+        'export AOA_CONN_USERNAME="{}" && \\\n'.format(
+            bash_escape(connection["username"])
+        )
+        + 'export AOA_CONN_PASSWORD="{}" && \\\n'.format(
+            bash_escape(connection["password"])
+        )
+        + 'export AOA_CONN_HOST="{}" && \\\n'.format(bash_escape(connection["host"]))
+        + 'export AOA_CONN_LOG_MECH="{}" && \\\n'.format(
+            bash_escape(connection["logmech"])
+        )
+        + 'export AOA_CONN_DATABASE="{}" && \\\n'.format(
+            bash_escape(connection.get("database", ""))
+        )
+        + 'export AOA_VAL_INSTALL_DB="{}" && \\\n'.format(
+            bash_escape(connection.get("val_db", "VAL"))
+        )
+        + 'export AOA_BYOM_INSTALL_DB="{}" && \\\n'.format(
+            bash_escape(connection.get("byom_db", "BYOM"))
+        )
+    )
 
 
 def activate_connection(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     def _check_connection_exists(id, obj):
         for connection in obj:
-            if 'id' in connection and connection['id'] == id:
+            if "id" in connection and connection["id"] == id:
                 return True
         return False
 
     def _activate_connection(id, obj):
         for connx in obj:
-            if 'id' in connx and connx['id'] == id:
-                os.environ['AOA_CONN_USERNAME'] = connx['username']
-                os.environ['AOA_CONN_PASSWORD'] = connx['password']
-                os.environ['AOA_CONN_HOST'] = connx['host']
-                os.environ['AOA_CONN_LOG_MECH'] = connx['logmech']
-                os.environ['AOA_CONN_DATABASE'] = connx.get('database', "")
-                os.environ['AOA_VAL_INSTALL_DB'] = connx.get("val_db", "VAL")
-                os.environ['AOA_BYOM_INSTALL_DB'] = connx.get("ml_db", "MLDB")
+            if "id" in connx and connx["id"] == id:
+                os.environ["AOA_CONN_USERNAME"] = connx["username"]
+                os.environ["AOA_CONN_PASSWORD"] = connx["password"]
+                os.environ["AOA_CONN_HOST"] = connx["host"]
+                os.environ["AOA_CONN_LOG_MECH"] = connx["logmech"]
+                os.environ["AOA_CONN_DATABASE"] = connx.get("database", "")
+                os.environ["AOA_VAL_INSTALL_DB"] = connx.get("val_db", "VAL")
+                os.environ["AOA_BYOM_INSTALL_DB"] = connx.get("ml_db", "MLDB")
 
                 return True
         return False
 
     try:
         Path(config_dir).mkdir(parents=True, exist_ok=True)
         connections_file = "{}/connections.yaml".format(config_dir)
-        with open(connections_file, 'r') as f:
+        with open(connections_file, "r") as f:
             connections_dict = yaml.safe_load(f)
             if connections_dict is None:
                 connections_dict = {}
     except:
         logging.info("No connections file found, you must create a connection first")
         exit(1)
 
-    connections = connections_dict['connections'] if 'connections' in connections_dict and len(
-        connections_dict['connections']) > 0 else []
+    connections = (
+        connections_dict["connections"]
+        if "connections" in connections_dict
+        and len(connections_dict["connections"]) > 0
+        else []
+    )
     if args.connection:
         connection = args.connection
-    elif kwargs.get('connection'):
-        connection = kwargs.get('connection')
+    elif kwargs.get("connection"):
+        connection = kwargs.get("connection")
     else:
         if len(connections) == 1:
-            print("Automatic connection selection as only one available: {}".format(connections[0]["name"]))
+            print(
+                "Automatic connection selection as only one available: {}".format(
+                    connections[0]["name"]
+                )
+            )
             connection = connections[0]["id"]
         else:
-            selected_connection_value = input_select('connection', [item['name'] for item in connections],
-                                                     'Available connections:')
-            connection = next((connections[i]['id'] for i, item in enumerate(connections) if
-                               connections[i]['name'] == selected_connection_value), None)
+            selected_connection_value = input_select(
+                "connection",
+                [item["name"] for item in connections],
+                "Available connections:",
+            )
+            connection = next(
+                (
+                    connections[i]["id"]
+                    for i, item in enumerate(connections)
+                    if connections[i]["name"] == selected_connection_value
+                ),
+                None,
+            )
 
     if _check_connection_exists(connection, connections):
         _activate_connection(connection, connections)
     else:
-        logging.error('The specified connection was not found.')
+        logging.error("The specified connection was not found.")
         exit(1)
 
     return connection
 
 
 def test_connection(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     def _test_connection():
         from aoa.util import aoa_create_context
         from aoa.util.connections import execute_sql
+
         aoa_create_context()
         test_query = "SEL infodata FROM dbc.dbcinfo WHERE infokey = 'VERSION'"
         logging.debug(test_query)
         result = execute_sql(test_query).fetchall()
         return result[0][0]
 
     from argparse import Namespace
-    activate_connection(Namespace(cwd=None, connection=args.connection if args.connection else None))
+
+    activate_connection(
+        Namespace(cwd=None, connection=args.connection if args.connection else None)
+    )
 
     try:
         ver = _test_connection()
         print("Connection successful, Vantage version: {}".format(ver))
     except Exception as ex:
         logging.error("Failed to test connecton: {}".format(ex))
         logging.error("Please use 'tmo connection add' to add working connection")
@@ -689,38 +886,44 @@
 
 def create_byom_table(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     from aoa.stats import store
     from aoa.util.connections import execute_sql
+
     ct_query = store.byom_query.format(args.name)
     print(ct_query)
 
     if args.execute_ddl:
         from argparse import Namespace
+
         activate_connection(Namespace(cwd=None, connection=None))
         from aoa.util import aoa_create_context
+
         try:
             aoa_create_context()
             logging.debug(ct_query)
             execute_sql(ct_query)
         except Exception as ex:
             raise Exception("Could not create BYOM table: {}".format(ex)) from ex
 
         print("BYOM table {} created successfully".format(args.metadata_table))
     else:
-        print("Execution not requested, just showing DDL. To execute this DDL, add -e to the command.")
+        print(
+            "Execution not requested, just showing DDL. To execute this DDL, add -e to the command."
+        )
 
 
 def compute_stats(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     from argparse import Namespace
+
     activate_connection(Namespace(cwd=None, connection=None))
 
     from aoa.util import aoa_create_context
     from aoa.stats import stats, store
     from teradataml import DataFrame
 
     try:
@@ -728,106 +931,128 @@
 
         df = DataFrame.from_query(f"SEL * FROM {args.source_table}")
 
         columns = list(map(str.strip, map(str.lower, args.columns.split(","))))
 
         if args.feature_type == "categorical":
             fs = stats.compute_categorical_stats(df, columns)
-            store.save_feature_stats(features_table=args.metadata_table, feature_type="categorical", stats=fs)
+            store.save_feature_stats(
+                features_table=args.metadata_table, feature_type="categorical", stats=fs
+            )
 
         elif args.feature_type == "continuous":
             fs = stats.compute_continuous_stats(df, columns)
-            store.save_feature_stats(features_table=args.metadata_table, feature_type="continuous", stats=fs)
+            store.save_feature_stats(
+                features_table=args.metadata_table, feature_type="continuous", stats=fs
+            )
     except Exception as ex:
         raise Exception("Could not compute feature stats: {}".format(ex)) from ex
 
     logging.info("Statistics computed successfully")
 
 
 def list_stats(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     from argparse import Namespace
+
     activate_connection(Namespace(cwd=None, connection=None))
     from aoa.util import aoa_create_context
     from aoa.stats import store
 
     try:
         aoa_create_context()
         stats_summary = store.get_feature_stats_summary(args.metadata_table)
         logging.debug(stats_summary)
 
         if len(stats_summary) < 0:
-            raise Exception("No statistics stored in the table {}".format(args.metadata_table))
+            raise Exception(
+                "No statistics stored in the table {}".format(args.metadata_table)
+            )
 
         width = len(max(list(stats_summary.keys()), key=len))
         print_underscored("List of stored feature stats:")
         for v in stats_summary:
-            print("{feature: <{width}} | {type}".format(feature=v, width=width, type=stats_summary[v]))
+            print(
+                "{feature: <{width}} | {type}".format(
+                    feature=v, width=width, type=stats_summary[v]
+                )
+            )
     except Exception as ex:
         raise Exception("Could not list feature stats: {}".format(ex)) from ex
 
 
 def create_stats_table(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
 
     from aoa.stats.store import get_features_stats_metadata_ct_query
     from aoa.util.connections import execute_sql
+
     ct_query = get_features_stats_metadata_ct_query(args.metadata_table)
     print(ct_query)
 
     if args.execute_ddl:
         from argparse import Namespace
+
         activate_connection(Namespace(cwd=None, connection=None))
         from aoa.util import aoa_create_context
+
         try:
             aoa_create_context()
             logging.debug(ct_query)
             execute_sql(ct_query)
         except Exception as ex:
             raise Exception("Could not create statistics: {}".format(ex)) from ex
 
         print("Statistics table {} created successfully".format(args.metadata_table))
     else:
-        print("Execution not requested, just showing DDL. To execute this DDL, add -e to the command.")
+        print(
+            "Execution not requested, just showing DDL. To execute this DDL, add -e to the command."
+        )
 
 
 def import_stats(args, **kwargs):
     if args.cwd:
         set_cwd(args.cwd)
     if args.show_example:
-        print("""
+        print(
+            """
             {
                 "age": {
                     "edges": [21.0, 27.0, 33.0, 39.0, 45.0, 51.0, 57.0, 63.0, 69.0, 75.0, 81.0]
                 }, 
                 "hasdiabetes": {
                     "frequencies": ["0", "1"
                     ]
                 }
             }
-        """)
+        """
+        )
         exit(0)
 
     from argparse import Namespace
+
     activate_connection(Namespace(cwd=None, connection=None))
     from aoa.util import aoa_create_context
     from aoa.stats import store
     import json
+
     try:
         aoa_create_context()
         json_file = open(args.statistics_file)
         stats = json.load(json_file)
         store.save_feature_stats(args.metadata_table, stats)
     except Exception as ex:
         raise Exception("Could not list feature stats: {}".format(ex)) from ex
 
-    print("Successfully saved statistics in {} features table".format(args.metadata_table))
+    print(
+        "Successfully saved statistics in {} features table".format(args.metadata_table)
+    )
 
 
 def doctor(args, repo_manager, aoa_client, **kwargs):
     print("Testing ModelOps service configuration")
 
     from aoa import ProjectApi
 
@@ -835,26 +1060,29 @@
         project_api = ProjectApi(aoa_client=aoa_client, show_archived=False)
         projects = list(project_api)
         if len(projects) > 0:
             print(f"ModelOps service configured, number of projects: {len(projects)}")
         else:
             raise
     except Exception as ex:
-        logging.error("Failed to connect to ModelOps or find any project. \n" +
-                      "Please (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config")
+        logging.error(
+            "Failed to connect to ModelOps or find any project. \n"
+            + "Please (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config"
+        )
 
     print("")
 
     print("Testing Vantage connections")
     args.connection = None
     test_connection(args)
 
 
 def set_cwd(path):
     import os
+
     if not os.path.exists(path):
         logging.error("The specified path does not exist... exiting")
         exit(1)
     os.chdir(path)
     global base_path, model_catalog
     base_path = os.path.abspath(os.getcwd())
     model_catalog = os.path.join(base_path, "model_definitions/")
@@ -867,47 +1095,55 @@
         print("{}".format(__version__))
     else:
         kwargs.get("parent_parser").print_help()
 
 
 def print_underscored(message):
     print(message)
-    print('-' * len(message))
+    print("-" * len(message))
 
 
-def list_and_select_projects(repo_manager, aoa_client, as_list=False, check_config=False):
+def list_and_select_projects(
+    repo_manager, aoa_client, as_list=False, check_config=False
+):
     from aoa import ProjectApi
 
     project_api = ProjectApi(aoa_client=aoa_client, show_archived=False)
     projects = list(project_api)
 
-    print_underscored('List of projects:' if as_list else 'Available projects:')
+    print_underscored("List of projects:" if as_list else "Available projects:")
     if not len(projects) > 0:
-        print('No projects were found')
+        print("No projects were found")
     for ix, item in enumerate(projects):
         print("[{}] ({}) {}".format(ix, item["id"], item["name"]))
     if as_list:
         return
 
     current_project = get_current_project(repo_manager, aoa_client, check_config)
     current_project = current_project if current_project else ""
     current_index = "none"
     for ix, item in enumerate(projects):
-        if 'id' in current_project and current_project["id"] == item["id"]:
+        if "id" in current_project and current_project["id"] == item["id"]:
             current_index = ix
-    tmp_index = input("Select project by index (current selection: {}): ".format(current_index))
+    tmp_index = input(
+        "Select project by index (current selection: {}): ".format(current_index)
+    )
     print("")
 
-    if ((not tmp_index.isnumeric() or int(tmp_index) >= len(projects)) and not tmp_index == '') or (
-            tmp_index == '' and current_index == "none"):
-        print('Wrong selection, please try again by selecting the index number on the first column.')
+    if (
+        (not tmp_index.isnumeric() or int(tmp_index) >= len(projects))
+        and not tmp_index == ""
+    ) or (tmp_index == "" and current_index == "none"):
+        print(
+            "Wrong selection, please try again by selecting the index number on the first column."
+        )
         print("")
         return list_and_select_projects(repo_manager, aoa_client, as_list, check_config)
 
-    if tmp_index == '':
+    if tmp_index == "":
         tmp_index = current_index
 
     selected_project = projects[int(tmp_index)]
 
     if aoa_client:
         aoa_client.set_project_id(selected_project["id"])
 
@@ -917,227 +1153,433 @@
 def get_current_project(repo_manager, aoa_client, check_repo_conf=False):
     from aoa import ProjectApi
 
     if not validate_cwd_valid():
         return
 
     repo_conf = repo_manager.read_repo_config()
-    current_project_id = repo_conf["project_id"] if repo_conf and "project_id" in repo_conf else ""
+    current_project_id = (
+        repo_conf["project_id"] if repo_conf and "project_id" in repo_conf else ""
+    )
     project_api = ProjectApi(aoa_client=aoa_client, show_archived=False)
     current_project = project_api.find_by_id(current_project_id)
 
     if current_project:
         return current_project
     elif not current_project and check_repo_conf:
-        print('The repository is not linked to a ModelOps project.')
-        print('Please execute \'tmo link\'')
+        print("The repository is not linked to a ModelOps project.")
+        print("Please execute 'tmo link'")
         print("")
 
     return
 
 
 def link_repo(repo_manager, aoa_client, **kwargs):
     current_project = list_and_select_projects(repo_manager, aoa_client, False, False)
-    config = {
-        "project_id": current_project['id']
-    }
+    config = {"project_id": current_project["id"]}
     repo_manager.write_repo_config(config)
     print("Repo linked to Project.")
 
 
 def handle_generic_error(ex: Exception, debug: bool):
     if debug:
         logging.exception("An error occurred, printing stack trace output.")
     else:
         logging.error("An error occurred: {}".format(ex))
         exit(1)
 
 
 def main():
     try:
-        parent_parser = argparse.ArgumentParser(description='TMO CLI')
-        parent_parser.add_argument('--debug', action='store_true', help='Enable debug logging')
-        parent_parser.add_argument('--version', action='store_true', help='Display the version of this tool')
+        parent_parser = argparse.ArgumentParser(description="TMO CLI")
+        parent_parser.add_argument(
+            "--debug", action="store_true", help="Enable debug logging"
+        )
+        parent_parser.add_argument(
+            "--version", action="store_true", help="Display the version of this tool"
+        )
         parent_parser.set_defaults(func=print_help)
 
-        subparsers = parent_parser.add_subparsers(title="actions", description="valid actions", dest="command")
+        subparsers = parent_parser.add_subparsers(
+            title="actions", description="valid actions", dest="command"
+        )
 
         common_parser = argparse.ArgumentParser(add_help=False)
-        common_parser.add_argument('--debug', action='store_true', help='Enable debug logging')
-        common_parser.add_argument('-cwd', '--cwd', type=str, help=argparse.SUPPRESS)
-        common_parser.add_argument('--test', action='store_true', help=argparse.SUPPRESS)
-
-        parser_list = subparsers.add_parser("list", help="List projects, models, local models or datasets",
-                                            parents=[common_parser])
-        parser_list.add_argument('-p', '--projects', action='store_true', help='List projects')
-        parser_list.add_argument('-m', '--models', action='store_true',
-                                 help='List registered models (committed / pushed)')
-        parser_list.add_argument('-lm', '--local-models', action='store_true',
-                                 help='List local models. Includes registered and non-registered (non-committed / non-pushed)')
-        parser_list.add_argument('-t', '--templates', action='store_true', help='List dataset templates')
-        parser_list.add_argument('-d', '--datasets', action='store_true', help='List datasets')
-        parser_list.add_argument('-c', '--connections', action='store_true', help='List local connections')
+        common_parser.add_argument(
+            "--debug", action="store_true", help="Enable debug logging"
+        )
+        common_parser.add_argument("-cwd", "--cwd", type=str, help=argparse.SUPPRESS)
+        common_parser.add_argument(
+            "--test", action="store_true", help=argparse.SUPPRESS
+        )
+
+        parser_list = subparsers.add_parser(
+            "list",
+            help="List projects, models, local models or datasets",
+            parents=[common_parser],
+        )
+        parser_list.add_argument(
+            "-p", "--projects", action="store_true", help="List projects"
+        )
+        parser_list.add_argument(
+            "-m",
+            "--models",
+            action="store_true",
+            help="List registered models (committed / pushed)",
+        )
+        parser_list.add_argument(
+            "-lm",
+            "--local-models",
+            action="store_true",
+            help="List local models. Includes registered and non-registered (non-committed / non-pushed)",
+        )
+        parser_list.add_argument(
+            "-t", "--templates", action="store_true", help="List dataset templates"
+        )
+        parser_list.add_argument(
+            "-d", "--datasets", action="store_true", help="List datasets"
+        )
+        parser_list.add_argument(
+            "-c", "--connections", action="store_true", help="List local connections"
+        )
         parser_list.set_defaults(func=list_resources)
 
-        parser_add = subparsers.add_parser("add", help="Add model to working dir", parents=[common_parser])
-        parser_add.add_argument('-t', '--template-url', type=str, help='Git URL for template repository', required=True)
-        parser_add.add_argument('-b', '--branch', type=str, default='main', help='Git branch to pull templates (default is main)', required=True)
+        parser_add = subparsers.add_parser(
+            "add", help="Add model to working dir", parents=[common_parser]
+        )
+        parser_add.add_argument(
+            "-t",
+            "--template-url",
+            type=str,
+            help="Git URL for template repository",
+            required=True,
+        )
+        parser_add.add_argument(
+            "-b",
+            "--branch",
+            type=str,
+            default="main",
+            help="Git branch to pull templates (default is main)",
+            required=True,
+        )
         parser_add.set_defaults(func=add_model)
 
-        parser_run = subparsers.add_parser("run", help="Train and Evaluate model locally", parents=[common_parser])
-        parser_run.add_argument('-id', '--model-id', type=str, help='Id of model')
-        parser_run.add_argument('-m', '--mode', type=str, help='Mode (train or evaluate)')
-        parser_run.add_argument('-d', '--dataset-id', type=str, help='Remote datasetId')
-        parser_run.add_argument('-t', '--dataset-template-id', type=str, help='Remote datasetTemplateId')
-        parser_run.add_argument('-ld', '--local-dataset', type=str, help='Path to local dataset metadata file')
-        parser_run.add_argument('-lt', '--local-dataset-template', type=str,
-                                help='Path to local dataset template metadata file')
-        parser_run.add_argument('-c', '--connection', type=str, help='Local connection id')
+        parser_run = subparsers.add_parser(
+            "run", help="Train and Evaluate model locally", parents=[common_parser]
+        )
+        parser_run.add_argument("-id", "--model-id", type=str, help="Id of model")
+        parser_run.add_argument(
+            "-m", "--mode", type=str, help="Mode (train or evaluate)"
+        )
+        parser_run.add_argument("-d", "--dataset-id", type=str, help="Remote datasetId")
+        parser_run.add_argument(
+            "-t", "--dataset-template-id", type=str, help="Remote datasetTemplateId"
+        )
+        parser_run.add_argument(
+            "-ld",
+            "--local-dataset",
+            type=str,
+            help="Path to local dataset metadata file",
+        )
+        parser_run.add_argument(
+            "-lt",
+            "--local-dataset-template",
+            type=str,
+            help="Path to local dataset template metadata file",
+        )
+        parser_run.add_argument(
+            "-c", "--connection", type=str, help="Local connection id"
+        )
         parser_run.set_defaults(func=run_model)
 
-        parser_init = subparsers.add_parser("init", help="Initialize model directory with basic structure",
-                                            parents=[common_parser])
+        parser_init = subparsers.add_parser(
+            "init",
+            help="Initialize model directory with basic structure",
+            parents=[common_parser],
+        )
         parser_init.set_defaults(func=init_model_directory)
 
-        parser_clone = subparsers.add_parser("clone", help="Clone Project Repository", parents=[common_parser])
-        parser_clone.add_argument('-id', '--project-id', type=str, help='Id of Project to clone')
-        parser_clone.add_argument('-p', '--path', type=str, help='Path to clone repository to')
+        parser_clone = subparsers.add_parser(
+            "clone", help="Clone Project Repository", parents=[common_parser]
+        )
+        parser_clone.add_argument(
+            "-id", "--project-id", type=str, help="Id of Project to clone"
+        )
+        parser_clone.add_argument(
+            "-p", "--path", type=str, help="Path to clone repository to"
+        )
         parser_clone.set_defaults(func=clone)
 
-        parser_configure = subparsers.add_parser("link", help="Link local repo to project", parents=[common_parser])
+        parser_configure = subparsers.add_parser(
+            "link", help="Link local repo to project", parents=[common_parser]
+        )
         parser_configure.set_defaults(func=link_repo)
 
-        parser_connections = subparsers.add_parser("connection", help="Manage local connections")
-        subparser_connections = parser_connections.add_subparsers(title="actions", description="valid actions",
-                                                                  dest="command")
-        subparser_list_connections = subparser_connections.add_parser("list", help="List all local connections",
-                                                                      parents=[common_parser])
+        parser_connections = subparsers.add_parser(
+            "connection", help="Manage local connections"
+        )
+        subparser_connections = parser_connections.add_subparsers(
+            title="actions", description="valid actions", dest="command"
+        )
+        subparser_list_connections = subparser_connections.add_parser(
+            "list", help="List all local connections", parents=[common_parser]
+        )
         subparser_list_connections.set_defaults(func=list_connections)
-        subparser_add_connections = subparser_connections.add_parser("add", help="Add a local connection",
-                                                                     parents=[common_parser])
-        subparser_add_connections.add_argument('-n', '--name', type=str, help='Connection name')
-        subparser_add_connections.add_argument('-H', '--host', type=str, help='Connection host')
-        subparser_add_connections.add_argument('-u', '--username', type=str, help='Connection username')
-        subparser_add_connections.add_argument('-p', '--password', type=str, help='Connection password')
-        subparser_add_connections.add_argument('-d', '--database', type=str, help='Connection default database')
-        subparser_add_connections.add_argument('--val-db', type=str, default='val', help='Configure VAL installation db (default is val)')
-        subparser_add_connections.add_argument('--byom-db', type=str, default='mldb', help='Configure BYOM installation db (default is mldb)')
-        subparser_add_connections.set_defaults(func=add_connections, parent_parser=subparser_add_connections)
-        subparser_remove_connections = subparser_connections.add_parser("remove", help="Remove a local connection",
-                                                                        parents=[common_parser])
-        subparser_remove_connections.add_argument('-c', '--connection', type=str, help='Local connection id')
+        subparser_add_connections = subparser_connections.add_parser(
+            "add", help="Add a local connection", parents=[common_parser]
+        )
+        subparser_add_connections.add_argument(
+            "-n", "--name", type=str, help="Connection name"
+        )
+        subparser_add_connections.add_argument(
+            "-H", "--host", type=str, help="Connection host"
+        )
+        subparser_add_connections.add_argument(
+            "-u", "--username", type=str, help="Connection username"
+        )
+        subparser_add_connections.add_argument(
+            "-p", "--password", type=str, help="Connection password"
+        )
+        subparser_add_connections.add_argument(
+            "-d", "--database", type=str, help="Connection default database"
+        )
+        subparser_add_connections.add_argument(
+            "--val-db",
+            type=str,
+            default="val",
+            help="Configure VAL installation db (default is val)",
+        )
+        subparser_add_connections.add_argument(
+            "--byom-db",
+            type=str,
+            default="mldb",
+            help="Configure BYOM installation db (default is mldb)",
+        )
+        subparser_add_connections.set_defaults(
+            func=add_connections, parent_parser=subparser_add_connections
+        )
+        subparser_remove_connections = subparser_connections.add_parser(
+            "remove", help="Remove a local connection", parents=[common_parser]
+        )
+        subparser_remove_connections.add_argument(
+            "-c", "--connection", type=str, help="Local connection id"
+        )
         subparser_remove_connections.set_defaults(func=remove_connections)
-        subparser_export_connections = subparser_connections.add_parser("export",
-                                                                        help="Export a local connection to be used as a shell script",
-                                                                        parents=[common_parser])
-        subparser_export_connections.add_argument('-c', '--connection', type=str, help='Local connection id')
+        subparser_export_connections = subparser_connections.add_parser(
+            "export",
+            help="Export a local connection to be used as a shell script",
+            parents=[common_parser],
+        )
+        subparser_export_connections.add_argument(
+            "-c", "--connection", type=str, help="Local connection id"
+        )
         subparser_export_connections.set_defaults(func=export_connection)
-        subparser_test_connections = subparser_connections.add_parser("test", help="Test a local connection",
-                                                                      parents=[common_parser])
-        subparser_test_connections.add_argument('-c', '--connection', type=str, help='Local connection id')
+        subparser_test_connections = subparser_connections.add_parser(
+            "test", help="Test a local connection", parents=[common_parser]
+        )
+        subparser_test_connections.add_argument(
+            "-c", "--connection", type=str, help="Local connection id"
+        )
         subparser_test_connections.set_defaults(func=test_connection)
 
-        subparser_create_byom_table = subparser_connections.add_parser("create-byom-table",
-                                                                       help="Create a table to store BYOM models",
-                                                                       parents=[common_parser])
-        subparser_create_byom_table.add_argument('-n', '--name', type=str, default='tmo_byom_models',
-                                                 help='Name of BYOM table (default is tmo_byom_models)')
-        subparser_create_byom_table.add_argument('-e', '--execute-ddl', action='store_true',
-                                                 help='Execute CREATE TABLE DDL, not just generate it')
+        subparser_create_byom_table = subparser_connections.add_parser(
+            "create-byom-table",
+            help="Create a table to store BYOM models",
+            parents=[common_parser],
+        )
+        subparser_create_byom_table.add_argument(
+            "-n",
+            "--name",
+            type=str,
+            default="tmo_byom_models",
+            help="Name of BYOM table (default is tmo_byom_models)",
+        )
+        subparser_create_byom_table.add_argument(
+            "-e",
+            "--execute-ddl",
+            action="store_true",
+            help="Execute CREATE TABLE DDL, not just generate it",
+        )
         subparser_create_byom_table.set_defaults(func=create_byom_table)
 
-        parser_features = subparsers.add_parser("feature", help="Manage feature statistics")
-        subparser_feature = parser_features.add_subparsers(title="action", description="valid actions", dest="command")
-        subparser_compute_stats = subparser_feature.add_parser("compute-stats", help="Compute feature statistics",
-                                                               parents=[common_parser])
-        subparser_compute_stats.add_argument('-s', '--source-table', type=str, help='Feature source table/view',
-                                             required=True)
-        subparser_compute_stats.add_argument('-m', '--metadata-table', type=str,
-                                             help='Metadata table for feature stats, including database name',
-                                             required=True)
-        subparser_compute_stats.add_argument('-t', '--feature-type', choices=['continuous', 'categorical'],
-                                             default='continuous', help='Feature type: continuous or categorical (default is continuous)')
-        subparser_compute_stats.add_argument('-c', '--columns', type=str, help='List of feature columns', required=True)
-        subparser_compute_stats.set_defaults(func=compute_stats, parent_parser=subparser_compute_stats)
-        subparser_list_stats = subparser_feature.add_parser("list-stats", help="List available statistics",
-                                                            parents=[common_parser])
-        subparser_list_stats.add_argument('-m', '--metadata-table', type=str,
-                                          help='Metadata table for feature stats, including database name',
-                                          required=True)
-        subparser_list_stats.set_defaults(func=list_stats, parent_parser=subparser_list_stats)
-        subparser_create_stats_table = subparser_feature.add_parser("create-stats-table",
-                                                                    help="Create statistics table",
-                                                                    parents=[common_parser])
-        subparser_create_stats_table.add_argument('-m', '--metadata-table', type=str,
-                                                  help='Metadata table for feature stats, including database name',
-                                                  required=True)
-        subparser_create_stats_table.add_argument('-e', '--execute-ddl', action='store_true',
-                                                  help='Execute CREATE TABLE DDL, not just generate it')
-        subparser_create_stats_table.set_defaults(func=create_stats_table, parent_parser=subparser_create_stats_table)
-        subparser_import_stats = subparser_feature.add_parser("import-stats",
-                                                              help="Import column statistics from local JSON file",
-                                                              parents=[common_parser])
-        subparser_import_stats.add_argument('-m', '--metadata-table', type=str,
-                                            help='Metadata table for feature stats, including database name',
-                                            required=True)
-        subparser_import_stats.add_argument('-f', '--statistics-file', type=str, help='Name of statistics JSON file',
-                                            required=True)
-        subparser_import_stats.add_argument('-s', '--show-example', action='store_true',
-                                            help='Show file structure example and exit')
-        subparser_import_stats.set_defaults(func=import_stats, parent_parser=subparser_import_stats)
-
-        parser_doctor = subparsers.add_parser("doctor", help="Diagnose configuration issues", parents=[common_parser])
+        parser_features = subparsers.add_parser(
+            "feature", help="Manage feature statistics"
+        )
+        subparser_feature = parser_features.add_subparsers(
+            title="action", description="valid actions", dest="command"
+        )
+        subparser_compute_stats = subparser_feature.add_parser(
+            "compute-stats", help="Compute feature statistics", parents=[common_parser]
+        )
+        subparser_compute_stats.add_argument(
+            "-s",
+            "--source-table",
+            type=str,
+            help="Feature source table/view",
+            required=True,
+        )
+        subparser_compute_stats.add_argument(
+            "-m",
+            "--metadata-table",
+            type=str,
+            help="Metadata table for feature stats, including database name",
+            required=True,
+        )
+        subparser_compute_stats.add_argument(
+            "-t",
+            "--feature-type",
+            choices=["continuous", "categorical"],
+            default="continuous",
+            help="Feature type: continuous or categorical (default is continuous)",
+        )
+        subparser_compute_stats.add_argument(
+            "-c", "--columns", type=str, help="List of feature columns", required=True
+        )
+        subparser_compute_stats.set_defaults(
+            func=compute_stats, parent_parser=subparser_compute_stats
+        )
+        subparser_list_stats = subparser_feature.add_parser(
+            "list-stats", help="List available statistics", parents=[common_parser]
+        )
+        subparser_list_stats.add_argument(
+            "-m",
+            "--metadata-table",
+            type=str,
+            help="Metadata table for feature stats, including database name",
+            required=True,
+        )
+        subparser_list_stats.set_defaults(
+            func=list_stats, parent_parser=subparser_list_stats
+        )
+        subparser_create_stats_table = subparser_feature.add_parser(
+            "create-stats-table",
+            help="Create statistics table",
+            parents=[common_parser],
+        )
+        subparser_create_stats_table.add_argument(
+            "-m",
+            "--metadata-table",
+            type=str,
+            help="Metadata table for feature stats, including database name",
+            required=True,
+        )
+        subparser_create_stats_table.add_argument(
+            "-e",
+            "--execute-ddl",
+            action="store_true",
+            help="Execute CREATE TABLE DDL, not just generate it",
+        )
+        subparser_create_stats_table.set_defaults(
+            func=create_stats_table, parent_parser=subparser_create_stats_table
+        )
+        subparser_import_stats = subparser_feature.add_parser(
+            "import-stats",
+            help="Import column statistics from local JSON file",
+            parents=[common_parser],
+        )
+        subparser_import_stats.add_argument(
+            "-m",
+            "--metadata-table",
+            type=str,
+            help="Metadata table for feature stats, including database name",
+            required=True,
+        )
+        subparser_import_stats.add_argument(
+            "-f",
+            "--statistics-file",
+            type=str,
+            help="Name of statistics JSON file",
+            required=True,
+        )
+        subparser_import_stats.add_argument(
+            "-s",
+            "--show-example",
+            action="store_true",
+            help="Show file structure example and exit",
+        )
+        subparser_import_stats.set_defaults(
+            func=import_stats, parent_parser=subparser_import_stats
+        )
+
+        parser_doctor = subparsers.add_parser(
+            "doctor", help="Diagnose configuration issues", parents=[common_parser]
+        )
         parser_doctor.set_defaults(func=doctor)
 
         args = parent_parser.parse_args()
 
         logging_level = logging.DEBUG if args.debug else logging.INFO
-        logging.basicConfig(format="%(message)s", stream=sys.stdout, level=logging_level)
+        logging.basicConfig(
+            format="%(message)s", stream=sys.stdout, level=logging_level
+        )
         print("")
 
         # certain functions don't need an API connection, we can call them without initializing a client and repo manager
-        local_functions = [print_help, list_connections, remove_connections, add_connections, test_connection,
-                             export_connection, create_byom_table, create_stats_table, import_stats, list_stats,
-                             compute_stats]
+        local_functions = [
+            print_help,
+            list_connections,
+            remove_connections,
+            add_connections,
+            test_connection,
+            export_connection,
+            create_byom_table,
+            create_stats_table,
+            import_stats,
+            list_stats,
+            compute_stats,
+        ]
         if args.command and args.func not in local_functions:
             from aoa import RepoManager
             from aoa import AoaClient
 
             repo_manager = RepoManager(base_path)
             aoa_client = AoaClient()
 
-            args.func(repo_manager=repo_manager, aoa_client=aoa_client, args=args, parent_parser=parent_parser)
+            args.func(
+                repo_manager=repo_manager,
+                aoa_client=aoa_client,
+                args=args,
+                parent_parser=parent_parser,
+            )
         else:
             args.func(args=args, parent_parser=parent_parser)
 
     except requests.exceptions.ConnectionError as ce:
-        logging.error("Could not connect to ModelOps API. \n" +
-                      "Please verify you are connected to network and have access to ModelOps UI.\n" +
-                      "If you are connected and have access, " +
-                      "try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config.\n\n" +
-                      "For more details, run with --debug.\n")
+        logging.error(
+            "Could not connect to ModelOps API. \n"
+            + "Please verify you are connected to network and have access to ModelOps UI.\n"
+            + "If you are connected and have access, "
+            + "try (re)copy the CLI configuration from ModelOps UI -> Session Details -> CLI Config.\n\n"
+            + "For more details, run with --debug.\n"
+        )
 
         if args.debug:
             logging.exception("An error occurred, printing stack trace output.")
 
         exit(1)
 
     except oauthlib.oauth2.rfc6749.errors.InvalidGrantError as ge:
         if ge.description in ["Token is not active", "Session not active"]:
-            logging.error(ge.description + "\nClearing the token cache. Please re-run cmd and login again.\n")
+            logging.error(
+                ge.description
+                + "\nClearing the token cache. Please re-run cmd and login again.\n"
+            )
 
             if os.path.exists(AoaClient.DEFAULT_TOKEN_CACHE_FILE_PATH):
                 os.remove(AoaClient.DEFAULT_TOKEN_CACHE_FILE_PATH)
 
             exit(1)
         else:
             handle_generic_error(ge, args.debug)
 
     except oauthlib.oauth2.rfc6749.errors.InvalidTokenError as ge:
-        logging.error(ge.description + "\nClearing the token cache. Please re-run cmd and login again.\n")
+        logging.error(
+            ge.description
+            + "\nClearing the token cache. Please re-run cmd and login again.\n"
+        )
 
         if os.path.exists(AoaClient.DEFAULT_TOKEN_CACHE_FILE_PATH):
             os.remove(AoaClient.DEFAULT_TOKEN_CACHE_FILE_PATH)
 
         exit(1)
 
     except KeyboardInterrupt:
```

### Comparing `teradatamodelops-7.0.6rc1/setup.py` & `teradatamodelops-7.0.6rc2/setup.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/PKG-INFO` & `teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.6rc1
+Version: 7.0.6rc2
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/SOURCES.txt` & `teradatamodelops-7.0.6rc2/teradatamodelops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

