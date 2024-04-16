# Comparing `tmp/teradatamodelops-7.0.5b5.tar.gz` & `tmp/teradatamodelops-7.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teradatamodelops-7.0.5b5.tar", last modified: Fri Feb 23 10:05:08 2024, max compression
+gzip compressed data, was "teradatamodelops-7.0.6rc1.tar", last modified: Tue Apr 16 09:43:51 2024, max compression
```

## Comparing `teradatamodelops-7.0.5b5.tar` & `teradatamodelops-7.0.6rc1.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.342942 teradatamodelops-7.0.5b5/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/LICENSE.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/MANIFEST.in
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22889 2024-02-23 10:05:08.342370 teradatamodelops-7.0.5b5/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2072 2024-02-15 07:15:39.000000 teradatamodelops-7.0.5b5/README.md
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.226599 teradatamodelops-7.0.5b5/aoa/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1146 2024-02-23 10:04:54.000000 teradatamodelops-7.0.5b5/aoa/__init__.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.244001 teradatamodelops-7.0.5b5/aoa/api/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/api/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1478 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/api/api_iterator.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4632 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/api/base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3608 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/dataset_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1501 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/dataset_connection_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2350 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/dataset_template_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3048 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/deployment_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      781 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/api/iterator_base_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4717 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/job_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3288 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/job_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1000 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/api/message_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4397 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2727 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/project_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6328 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/trained_model_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     5296 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/trained_model_artefacts_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4543 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api/trained_model_event_api.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    17659 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/api_client.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.269966 teradatamodelops-7.0.5b5/aoa/cli/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/cli/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4345 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/cli/base_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6371 2024-02-15 07:15:39.000000 teradatamodelops-7.0.5b5/aoa/cli/evaluate_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.272533 teradatamodelops-7.0.5b5/aoa/cli/metadata_files/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/cli/metadata_files/.gitignore
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/cli/metadata_files/readme.md
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4887 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/cli/repo_manager.py
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/cli/run_model.R
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3896 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/cli/score_model.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4658 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/cli/train_model.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.274546 teradatamodelops-7.0.5b5/aoa/context/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/context/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3709 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/context/model_context.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.278325 teradatamodelops-7.0.5b5/aoa/crypto/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29020 2024-01-30 10:50:35.000000 teradatamodelops-7.0.5b5/aoa/crypto/TJEncryptPassword.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/crypto/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6543 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/crypto/crypto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.283912 teradatamodelops-7.0.5b5/aoa/stats/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/stats/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16972 2024-02-23 09:50:56.000000 teradatamodelops-7.0.5b5/aoa/stats/stats.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22134 2024-02-19 13:23:38.000000 teradatamodelops-7.0.5b5/aoa/stats/stats_util.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3494 2024-02-15 07:15:39.000000 teradatamodelops-7.0.5b5/aoa/stats/store.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.290851 teradatamodelops-7.0.5b5/aoa/util/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/util/__init__.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.5b5/aoa/util/artifacts.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1531 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/aoa/util/byom.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6282 2024-02-15 07:15:39.000000 teradatamodelops-7.0.5b5/aoa/util/connections.py
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9150 2024-02-15 07:15:39.000000 teradatamodelops-7.0.5b5/aoa/util/sto.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.293899 teradatamodelops-7.0.5b5/scripts/
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      239 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/scripts/aoa
--rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    50274 2024-02-23 09:38:11.000000 teradatamodelops-7.0.5b5/scripts/tmo
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      441 2024-02-23 10:05:08.362322 teradatamodelops-7.0.5b5/setup.cfg
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      881 2023-09-28 18:54:04.000000 teradatamodelops-7.0.5b5/setup.py
-drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-02-23 10:05:08.340683 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22889 2024-02-23 10:05:08.000000 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/PKG-INFO
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1291 2024-02-23 10:05:08.000000 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/SOURCES.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-02-23 10:05:08.000000 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/dependency_links.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-02-23 10:05:08.000000 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/requires.txt
--rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-02-23 10:05:08.000000 teradatamodelops-7.0.5b5/teradatamodelops.egg-info/top_level.txt
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.839447 teradatamodelops-7.0.6rc1/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9081 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    13324 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/LICENSE.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)       70 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/MANIFEST.in
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 09:43:51.838994 teradatamodelops-7.0.6rc1/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2072 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/README.md
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.420981 teradatamodelops-7.0.6rc1/aoa/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1205 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/aoa/__init__.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.582659 teradatamodelops-7.0.6rc1/aoa/api/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1478 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/api_iterator.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4632 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3608 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1501 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_connection_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2350 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/dataset_template_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3048 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/deployment_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      781 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/iterator_base_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4717 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/job_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3288 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/job_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1000 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/api/message_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4397 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     2727 2024-04-11 11:19:05.000000 teradatamodelops-7.0.6rc1/aoa/api/project_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6237 2024-04-16 09:16:52.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6015 2024-04-16 09:23:37.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_artefacts_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4543 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/api/trained_model_event_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      893 2024-04-16 08:05:32.000000 teradatamodelops-7.0.6rc1/aoa/api/user_attributes_api.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    17659 2024-04-16 09:23:24.000000 teradatamodelops-7.0.6rc1/aoa/api_client.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.638198 teradatamodelops-7.0.6rc1/aoa/cli/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4345 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/base_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6371 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/cli/evaluate_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.651820 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      143 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/.gitignore
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      179 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/metadata_files/readme.md
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4887 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/repo_manager.py
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)     2017 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/cli/run_model.R
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3896 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/score_model.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     4658 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/cli/train_model.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.660198 teradatamodelops-7.0.6rc1/aoa/context/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/context/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3709 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/context/model_context.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.681194 teradatamodelops-7.0.6rc1/aoa/crypto/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    29020 2024-01-30 10:50:35.000000 teradatamodelops-7.0.6rc1/aoa/crypto/TJEncryptPassword.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/crypto/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6543 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/crypto/crypto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.760563 teradatamodelops-7.0.6rc1/aoa/stats/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        0 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/stats/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    16963 2024-02-27 13:24:56.000000 teradatamodelops-7.0.6rc1/aoa/stats/stats.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    22431 2024-04-09 08:50:48.000000 teradatamodelops-7.0.6rc1/aoa/stats/stats_util.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     3494 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/stats/store.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.797357 teradatamodelops-7.0.6rc1/aoa/util/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      123 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/util/__init__.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      685 2023-03-02 09:03:18.000000 teradatamodelops-7.0.6rc1/aoa/util/artifacts.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1531 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/aoa/util/byom.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     6564 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/aoa/util/connections.py
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     9150 2024-02-27 13:22:27.000000 teradatamodelops-7.0.6rc1/aoa/util/sto.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.813822 teradatamodelops-7.0.6rc1/scripts/
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)      239 2023-09-28 18:54:04.000000 teradatamodelops-7.0.6rc1/scripts/aoa
+-rwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)    50274 2024-04-09 08:50:48.000000 teradatamodelops-7.0.6rc1/scripts/tmo
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      442 2024-04-16 09:43:51.843065 teradatamodelops-7.0.6rc1/setup.cfg
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      986 2024-04-16 08:05:35.000000 teradatamodelops-7.0.6rc1/setup.py
+drwxr-xr-x   0 anton.zadorozhniy   (502) staff       (20)        0 2024-04-16 09:43:51.837871 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)    23651 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/PKG-INFO
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)     1322 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/SOURCES.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        1 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/dependency_links.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)      210 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/requires.txt
+-rw-r--r--   0 anton.zadorozhniy   (502) staff       (20)        4 2024-04-16 09:43:51.000000 teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/top_level.txt
```

### Comparing `teradatamodelops-7.0.5b5/LICENSE-3RD-PARTY.txt` & `teradatamodelops-7.0.6rc1/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/LICENSE.txt` & `teradatamodelops-7.0.6rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/PKG-INFO` & `teradatamodelops-7.0.6rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.5b5
+Version: 7.0.6rc1
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSE-3RD-PARTY.txt
 Requires-Dist: jinja2>=3.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib>=1.3.1
 Requires-Dist: oauthlib>=3.2.2
@@ -22,14 +22,15 @@
 Requires-Dist: pycryptodome>=3.19.1
 Requires-Dist: httpx>=0.23.0
 
 # Teradata ModelOps Client
 
 - [Installation](#installation)
 - [CLI](#cli)
+- [Authentication](#authentication)
 - [SDK](#sdk)
 - [Release Notes](#release-notes)
 
 
 # Installation
 
 The teradatamodelops is available from [pypi](https://pypi.org/project/teradatamodelops/)
@@ -374,39 +375,53 @@
 Let's assume we have a PMML model which we have trained in another data science platform. We want to import the artefacts for this version (model.pmml and data_stats.json) against a BYOM model `f937b5d8-02c6-5150-80c7-1e4ff07fea31`.
 
 ```python
 from aoa import (
     AoaClient, 
     ModelApi,
     TrainedModelApi, 
-    TrainedModelArtefactsApi, 
+    TrainedModelArtefactsApi,
+    UserAttributesApi, 
     JobApi
 )
 import uuid
 
 client = AoaClient(project_id="23e1df4b-b630-47a1-ab80-7ad5385fcd8d")
 model_api = ModelApi(aoa_client=client)
 trained_model_api = TrainedModelApi(aoa_client=client)
 trained_model_artefacts_api = TrainedModelArtefactsApi(aoa_client=client)
+user_attributes_api = UserAttributesApi(aoa_client=client)
+
 job_api = JobApi(aoa_client=client)
 
-artefacts_import_id = uuid.uuid4()
-artefacts = ["model.pmml", "data_stats.json"]
+# set metadata for your import request
+model_id = '<model-uuid>'
+filename = './pima.pmml'
+language = 'PMML'
+dataset_connection_id = '<dataset-connection-uuid>'
+train_dataset_id = 'train-dataset-uuid'
 
 # first, upload the artefacts which we want to associate with the BYOM model version
-trained_model_artefacts_api.upload_artefacts(artefacts_import_id, artefacts)
+import_id = trained_model_artefacts_api.upload_byom_model(language,filename)
 
 import_request = {
-   "artefactImportId": str(artefacts_import_id),
-   "externalId": "my-byom-version-id"
+    "artefactImportId": import_id,
+    "externalId": "my_model_external_id",
+    "modelMonitoring": {
+        "language": language,
+        "useDefaultEvaluation": True,
+        "evaluationEnabled": True,
+        "modelType": "CLASSIFICATION",
+        "byomColumnExpression": "CAST(CAST(json_report AS JSON).JSONExtractValue('$.predicted_HasDiabetes') AS INT)",
+        "driftMonitoringEnabled": True,
+        "datasetId": train_dataset_id,
+        "datasetConnectionId": default_connection_id,
+    },
 }
 
-# update with id of your model 
-model_id = "<model-uuid>"
-
 job = model_api.import_byom(model_id, import_request)
 
 # wait until the job completes (if the job fails it will raise an exception)
 job_api.wait(job["id"])
 
 # now you can list the artefacts which were uploaded and linked to the model version
 trained_model_id = job["metadata"]["trainedModel"]["id"]
@@ -414,14 +429,21 @@
 ```
 
 
 ## Release Notes
 
 ### current
 
+- Fixed compatibility issue with `teradataml>=20.0.0.0`
+- Minor formatting updates
+- Added user attributes API
+- Updated programmatic BYOM import examples
+
+### 7.0.5
+
 **WARNING** Please recreate statistics metadata if you are using this version. It will produce more accurate results and correct behaviour.
 
 - Fixed computing statistics metadata for continuous features with all NULLs
 - Fixed training/eval/scoring statistics on columns with all NULLs
 - Added a workaround for VAL Histograms failure due to SP argument being longer than 31000 characters
 - Rounding all Decimal and Float bin edges to Teradata-supported FLOAT literals (15 digits max)
 - Fixed CLI error computing continuous statistics metadata related to mixed case column names
```

### Comparing `teradatamodelops-7.0.5b5/README.md` & `teradatamodelops-7.0.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/__init__.py` & `teradatamodelops-7.0.6rc1/aoa/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "7.0.5b5"
+__version__ = "7.0.6rc1"
 
 # import client
 from aoa.api_client import AoaClient
 
 # import APIs into api package
 from aoa.api.dataset_api import DatasetApi
 from aoa.api.dataset_template_api import DatasetTemplateApi
@@ -13,14 +13,15 @@
 from aoa.api.trained_model_event_api import TrainedModelEventApi
 from aoa.api.trained_model_artefacts_api import TrainedModelArtefactsApi
 from aoa.api.job_api import JobApi
 from aoa.api.job_event_api import JobEventApi
 from aoa.api.deployment_api import DeploymentApi
 from aoa.api.api_iterator import ApiIterator
 from aoa.api.message_api import MessageApi
+from aoa.api.user_attributes_api import UserAttributesApi
 
 # import repo into api package
 from aoa.cli.repo_manager import RepoManager
 from aoa.cli.evaluate_model import EvaluateModel
 from aoa.cli.score_model import ScoreModel
 from aoa.cli.train_model import TrainModel
 from aoa.cli.base_model import BaseModel
```

### Comparing `teradatamodelops-7.0.5b5/aoa/api/api_iterator.py` & `teradatamodelops-7.0.6rc1/aoa/api/api_iterator.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/base_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/base_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/dataset_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/dataset_connection_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/dataset_connection_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/dataset_template_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/dataset_template_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/deployment_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/iterator_base_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/iterator_base_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/job_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/job_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/job_event_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/job_event_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/message_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/message_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/model_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/model_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/project_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/project_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api/trained_model_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/trained_model_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import absolute_import
-from typing import Dict, List
+from typing import Dict
 
 from aoa.api.iterator_base_api import IteratorBaseApi
-from aoa.api.trained_model_artefacts_api import TrainedModelArtefactsApi
-
-import uuid
 
 
 class TrainedModelApi(IteratorBaseApi):
 
     path = "/api/trainedModels/"
     type = "TRAINED_MODEL"
 
@@ -183,7 +180,8 @@
         self.required_params(['deploymentId'], retire_request)
 
         return self.aoa_client.post_request(
             path=self.path + trained_model_id + '/retire',
             header_params=self._get_header_params(),
             query_params={},
             body=retire_request)
+
```

### Comparing `teradatamodelops-7.0.5b5/aoa/api/trained_model_artefacts_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/trained_model_artefacts_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List
 from aoa.api.base_api import BaseApi
 
 import requests
 import uuid
 import os
 
+SUPPORTED_BYOM_FORMATS = ["PMML","ONNX","H2O","H2O_DAI","DATAROBOT","DATAIKU"]
 
 class TrainedModelArtefactsApi(BaseApi):
 
     def _get_header_params(self):
         header_vars = ['AOA-Project-ID', 'VMO-Project-ID', 'Content-Type', 'Accept']  # AOA-Project-ID kept for backwards compatibility
         header_vals = [
             self.aoa_client.project_id,
@@ -69,15 +70,15 @@
         query_params = self.generate_params(['objectKey'], [artefact])
 
         response = self.aoa_client.get_request(
             path="/api/trainedModels/{}/artefacts/signedUploadUrl".format(trained_model_id),
             header_params=self._get_header_params(),
             query_params=query_params)
 
-        return response["url"]
+        return response["endpoint"]
 
     def download_artefacts(self, trained_model_id: uuid, path: str = "."):
         """
         downloads all artefacts for the given trained model
 
         Parameters:
            trained_model_id (uuid): Trained Model Id
@@ -120,22 +121,38 @@
 
         else:
             for root, d, files in os.walk(artefacts_folder):
                 for file in files:
                     object_key = os.path.relpath(os.path.join(root, file), artefacts_folder)
                     self.__upload_artefact(os.path.join(root, file), object_key, import_id)
 
+    def upload_byom_model(self, format: str, file_path: str, import_id: str = None):
+        """Simplified method to upload just a single file as BYOM model version. 
+        File is renamed during upload, so any local filename could be used.
+
+        Args:
+            format (str): One of supported formats, e.g. PMML, ONNX, H2O
+            file_path (str): local file path to a model artefact
+            import_id (str, optional): by default import_id is randomly generated. If required, specific import_id could be provided.
+
+        Raises:
+            ValueError: if format string is not one of supported formats
+
+        Returns:
+            str: import_id that could be used by import_byom method
+        """        
+        if format not in SUPPORTED_BYOM_FORMATS:
+            raise ValueError(f"The format {format} is not supported for simplified BYOM import, use `import_file` instead")
+
+        if not import_id:
+            import_id = str(uuid.uuid4())
+
+        self.__upload_artefact(file_path,f"model.{format.lower()}",import_id)
+        return import_id
+
     def __upload_artefact(self, artefact, object_key, import_id):
-        query_params = {
-            'objectKey': object_key
-        }
-        header_params = {
-            'AOA-Project-ID': "{}".format(self.aoa_client.project_id),  # AOA-Project-ID kept for backwards compatibility
-            'VMO-Project-ID': "{}".format(self.aoa_client.project_id)
-        }
-        signed_url = self.aoa_client.get_request("/api/trainedModels/{}/artefacts/signedUploadUrl"
-                                                 .format(import_id), header_params, query_params)
+        signed_url = self.get_signed_upload_url(import_id,object_key)
         # don't use aoa_client.session here as we don't want to send auth info.
-        upload_resp = requests.put(signed_url['endpoint'],
+        upload_resp = requests.put(signed_url,
                                    data=open(artefact, 'rb'),
                                    verify=self.aoa_client.session.verify)
         upload_resp.raise_for_status()
```

### Comparing `teradatamodelops-7.0.5b5/aoa/api/trained_model_event_api.py` & `teradatamodelops-7.0.6rc1/aoa/api/trained_model_event_api.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/api_client.py` & `teradatamodelops-7.0.6rc1/aoa/api_client.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/base_model.py` & `teradatamodelops-7.0.6rc1/aoa/cli/base_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/evaluate_model.py` & `teradatamodelops-7.0.6rc1/aoa/cli/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/repo_manager.py` & `teradatamodelops-7.0.6rc1/aoa/cli/repo_manager.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/run_model.R` & `teradatamodelops-7.0.6rc1/aoa/cli/run_model.R`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/score_model.py` & `teradatamodelops-7.0.6rc1/aoa/cli/score_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/cli/train_model.py` & `teradatamodelops-7.0.6rc1/aoa/cli/train_model.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/context/model_context.py` & `teradatamodelops-7.0.6rc1/aoa/context/model_context.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/crypto/TJEncryptPassword.py` & `teradatamodelops-7.0.6rc1/aoa/crypto/TJEncryptPassword.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/crypto/crypto.py` & `teradatamodelops-7.0.6rc1/aoa/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/stats/stats.py` & `teradatamodelops-7.0.6rc1/aoa/stats/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     features = []
     for f in lowered_features:
         if dtypes[f].startswith("decimal") or dtypes[f].startswith("float") or dtypes[f].startswith("int"):
             features.append(f)
         else:
             logger.warning(f"Column {f} has a type {dtypes[f]} which is not compatible with continuous feature types. This column will be ignored.")
 
-    logger.debug(f"Executing this VAL call {valib.Statistics(data=features_df, columns=features, stats_options='all').show_query()}")
+    logger.debug(f"Executing this VAL {valib.Statistics(data=features_df, columns=features, stats_options='all').show_query()}")
     stats = valib.Statistics(data=features_df, columns=features, stats_options="all")
     stats = stats.result.to_pandas(all_rows=True).reset_index()
     stats["xcol"] = stats["xcol"].str.lower()
     stats = stats.set_index("xcol",drop=False)
 
     non_trivial_features = []
     for f in features:
@@ -332,15 +332,15 @@
     Args:
         features_df (DataFrame): Teradata DataFrame used to compute statistics metadata
         categorical_features (List): list of columns representing categorical features
 
     Returns:
         dict: Dictionary with keys corresponding to requested features, and values containing frequencies
     """    
-    logger.debug(f"Executing this VAL call {valib.Frequency(data=features_df, columns=categorical_features).show_query()}")
+    logger.debug(f"Executing this VAL {valib.Frequency(data=features_df, columns=categorical_features).show_query()}")
     statistics = valib.Frequency(data=features_df, columns=categorical_features)
     statistics = statistics.result.to_pandas(all_rows=True).reset_index()
     statistics = statistics.drop(statistics.columns.difference(["xcol", "xval", "xpct"]), axis=1)
     statistics["xcol"] = statistics["xcol"].str.lower()
     statistics = statistics.groupby('xcol').apply(lambda x: dict(zip(x['xval'], x['xpct']))).to_dict()
 
     lowered_features = list(map(str.lower, categorical_features))
@@ -349,13 +349,13 @@
         values_list = list(statistics[f].keys())
         for k in values_list:
             if isinstance(k, numbers.Number):
                 if math.isnan(k):
                     logger.warning(f"Categorical feature {f} has NULL values in reference table, NULLs will be ignored")
                     del statistics[f][k]                
         if not statistics[f]:
-            logger.warning(f"Categorical feaure {f} has only NULL values in reference table, no statistics metadata generated")
+            logger.warning(f"Categorical feature {f} has only NULL values in reference table, no statistics metadata generated")
             lowered_features.remove(f)
     
     column_stats = {f: {"categories": list(statistics[f].keys())} for f in lowered_features}
 
     return column_stats
```

### Comparing `teradatamodelops-7.0.5b5/aoa/stats/stats_util.py` & `teradatamodelops-7.0.6rc1/aoa/stats/stats_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,27 +362,27 @@
     categorical_vars = list((set(features) | set(targets)) - set(continuous_vars))
     reference_edges = []
     reference_categories = []
     available_continuous_vars = []
     available_categorical_vars = []
 
     if len(continuous_vars) > 0:
-        logger.debug(f"Executing this VAL call {valib.Statistics(data=df, columns=continuous_vars, stats_options='all').show_query()}")
+        logger.debug(f"Executing this VAL {valib.Statistics(data=df, columns=continuous_vars, stats_options='all').show_query()}")
         stats = valib.Statistics(data=df, columns=continuous_vars, stats_options="all")
         stats = stats.result.to_pandas().fillna(value_for_nan).reset_index()
         stats["xcol"] = stats["xcol"].str.lower()
 
         stats_metadata = store.get_feature_stats(feature_metadata_fqtn, "continuous")
 
         for v in continuous_vars:
             if v.lower() in stats_metadata.keys():
                 reference_edges.append(stats_metadata[v.lower()]["edges"])
                 available_continuous_vars.append(v)
             else:
-                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored."
+                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
                                f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}")
 
         if len(available_continuous_vars) > 0:
             hist_boundaries = _convert_all_edges_to_val_str(reference_edges)
             histogram = _histogram_wrapper(data=df,columns=available_continuous_vars,boundaries=hist_boundaries)
             histogram["xcol"] = histogram["xcol"].str.lower()
 
@@ -390,20 +390,20 @@
         stats_metadata = store.get_feature_stats(feature_metadata_fqtn, "categorical")
             
         for v in categorical_vars:
             if v.lower() in stats_metadata.keys():
                 reference_categories.append(stats_metadata[v.lower()]["categories"])
                 available_categorical_vars.append(v)
             else:
-                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored."
+                logger.warning(f"Feature {v} doesn't have statistics metadata defined, and will not be monitored.\n"
                                f"In order to enable monitoring for this feature, make sure that statistics metadata is availabe in {feature_metadata_fqtn}")
 
         # We compute frequencies for all categorical features independent of metadata availability
         # But we only reporing number of nulls if reference categories are not available
-        logger.debug(f"Executing this VAL call {valib.Frequency(data=df, columns=categorical_vars).show_query()}")
+        logger.debug(f"Executing this VAL {valib.Frequency(data=df, columns=categorical_vars).show_query()}")
         frequencies = valib.Frequency(data=df, columns=categorical_vars)
         frequencies = frequencies.result.to_pandas(all_rows=True).reset_index()
         frequencies["xcol"] = frequencies["xcol"].str.lower()
 
     data_struct = {
         "num_rows": total_rows,
         "features": {},
@@ -478,15 +478,15 @@
         while _val_parameter_length_too_long(tc, tb):
             if len(tc) == 1:
                 raise Exception(f"VAL histogram parameters are too long even for single column {tc[0]}")
             tc.pop()
             tb.pop()
         
         # compute a histogram on the longest possible list of columns
-        logger.debug(f"Executing this VAL call {valib.Histogram(data=data,columns=tc,boundaries=tb).show_query()}")
+        logger.debug(f"Executing this VAL {valib.Histogram(data=data,columns=tc,boundaries=tb).show_query()}")
         histogram = valib.Histogram(data=data,columns=tc,boundaries=tb)
         result.append(histogram.result.to_pandas(all_rows=True).reset_index())
 
         # removing columns thats already computed 
         working_columns = working_columns[len(tc):]
         working_boundaries = working_boundaries[len(tb):]
     
@@ -500,11 +500,14 @@
     final_length = len(db_tbl_string) + len(column_string) + 128 * 4
     if final_length > limit:
         logger.debug(f"VAL histogram parameters are too long for these columns, trying to compute sequentially: {','.join(columns)}")
     return final_length > limit
 
 
 def _round_to_td_float(x, max_digits = 15):
+    # This function is needed to cast/round decimal and float number to the maximum precision allowed by Teradata database.
+    # Teradata floats allow maximum 15 digits for mantissa, so this strange logic below does exactly that.
+    # Possibly at some point we may need to add a round to exponent as well.
     (sign, digits, exponent) = Decimal(x).as_tuple()
     e = len(digits) + exponent
     (_, m, _) = Decimal(x).scaleb(-e).quantize(Decimal(f"1E-{max_digits}")).normalize().as_tuple()
     return np.float64(Decimal((sign, m, e - len(m))))
```

### Comparing `teradatamodelops-7.0.5b5/aoa/stats/store.py` & `teradatamodelops-7.0.6rc1/aoa/stats/store.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/util/artifacts.py` & `teradatamodelops-7.0.6rc1/aoa/util/artifacts.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/util/byom.py` & `teradatamodelops-7.0.6rc1/aoa/util/byom.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/aoa/util/connections.py` & `teradatamodelops-7.0.6rc1/aoa/util/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,22 +79,20 @@
     teradataml patch is released.
     """
 
     from sqlalchemy import create_engine
     from teradataml.common.exceptions import TeradataMlException
     from teradataml.common.messages import Messages
     from teradataml.common.messagecodes import MessageCodes
-    from teradataml.context.context import _mask_logmech_logdata, _get_other_connection_parameters
 
     username = '' if username is None else username
     host_value = '{}:{}@{}'.format(username, password, host)
-    other_connection_parameters = _get_other_connection_parameters(logmech=logmech,
-                                                                   logdata=None,
+    other_connection_parameters = _format_connection_parameters(logmech=logmech,
                                                                    database=database)
-
+    
     try:
         engine_url = "teradatasql://{}{}"
         td_sqlalchemy_engine = create_engine(engine_url.format(host_value, other_connection_parameters))
 
         # Masking senstive information - password, logmech and logdata.
         try:
             # Below statement raises an AttributeError with SQLAlchemy
@@ -103,25 +101,41 @@
         except AttributeError:
             # Masking the password should be different from above as SQLAlchemy
             # converted _URL object to immutable object from version 1.4.x.
             new_url = td_sqlalchemy_engine.url.set(password="***")
             td_sqlalchemy_engine.url = new_url
         except Exception:
             pass
-        _mask_logmech_logdata()
+
+        try:
+            if ('LOGMECH' in td_sqlalchemy_engine.url.query):
+                td_sqlalchemy_engine.url.query['LOGMECH'] = "***"
+        except Exception:
+            pass
 
     except TeradataMlException:
         raise
     except Exception as err:
         raise TeradataMlException(Messages.get_message(MessageCodes.CONNECTION_FAILURE),
                                   MessageCodes.CONNECTION_FAILURE) from err
 
     return td_sqlalchemy_engine
 
 
+def _format_connection_parameters(logmech,database):
+    if not logmech and not database:
+        return ""
+    result = []
+    if logmech:
+        result.append(f"LOGMECH={logmech.upper()}")
+    if database:
+        result.append(f"DATABASE={database.upper()}")
+    return "/?{}".format("&".join(result))
+
+
 def execute_sql_in_context(context, statement, parameters = None):
     from teradataml.common.exceptions import TeradataMlException
     from teradataml.common.messages import Messages
     from teradataml.common.messagecodes import MessageCodes
 
     if context is not None:
         tdsql_con = context.raw_connection().driver_connection
```

### Comparing `teradatamodelops-7.0.5b5/aoa/util/sto.py` & `teradatamodelops-7.0.6rc1/aoa/util/sto.py`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/scripts/tmo` & `teradatamodelops-7.0.6rc1/scripts/tmo`

 * *Files identical despite different names*

### Comparing `teradatamodelops-7.0.5b5/setup.py` & `teradatamodelops-7.0.6rc1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from aoa import __version__
 
 NAME = "teradatamodelops"
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
+# relative links in pypi.md depend on this PyPi issue https://github.com/pypa/readme_renderer/issues/163
 with open("docs/pypi.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name=NAME,
     version=__version__,
     description="Python client for Teradata ModelOps (TMO)",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     license_files=['LICENSE.txt', 'LICENSE-3RD-PARTY.txt'],
     author="Teradata",
     author_email="teradata.corporation@teradatacorporation.com",
     url="",
     install_requires=required,
     tests_require=['pytest', 'pytest-console-scripts'],
     setup_requires=['pytest-runner'],
```

### Comparing `teradatamodelops-7.0.5b5/teradatamodelops.egg-info/PKG-INFO` & `teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: teradatamodelops
-Version: 7.0.5b5
+Version: 7.0.6rc1
 Summary: Python client for Teradata ModelOps (TMO)
 Home-page: 
 Author: Teradata
 Author-email: teradata.corporation@teradatacorporation.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: LICENSE-3RD-PARTY.txt
 Requires-Dist: jinja2>=3.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: requests-oauthlib>=1.3.1
 Requires-Dist: oauthlib>=3.2.2
@@ -22,14 +22,15 @@
 Requires-Dist: pycryptodome>=3.19.1
 Requires-Dist: httpx>=0.23.0
 
 # Teradata ModelOps Client
 
 - [Installation](#installation)
 - [CLI](#cli)
+- [Authentication](#authentication)
 - [SDK](#sdk)
 - [Release Notes](#release-notes)
 
 
 # Installation
 
 The teradatamodelops is available from [pypi](https://pypi.org/project/teradatamodelops/)
@@ -374,39 +375,53 @@
 Let's assume we have a PMML model which we have trained in another data science platform. We want to import the artefacts for this version (model.pmml and data_stats.json) against a BYOM model `f937b5d8-02c6-5150-80c7-1e4ff07fea31`.
 
 ```python
 from aoa import (
     AoaClient, 
     ModelApi,
     TrainedModelApi, 
-    TrainedModelArtefactsApi, 
+    TrainedModelArtefactsApi,
+    UserAttributesApi, 
     JobApi
 )
 import uuid
 
 client = AoaClient(project_id="23e1df4b-b630-47a1-ab80-7ad5385fcd8d")
 model_api = ModelApi(aoa_client=client)
 trained_model_api = TrainedModelApi(aoa_client=client)
 trained_model_artefacts_api = TrainedModelArtefactsApi(aoa_client=client)
+user_attributes_api = UserAttributesApi(aoa_client=client)
+
 job_api = JobApi(aoa_client=client)
 
-artefacts_import_id = uuid.uuid4()
-artefacts = ["model.pmml", "data_stats.json"]
+# set metadata for your import request
+model_id = '<model-uuid>'
+filename = './pima.pmml'
+language = 'PMML'
+dataset_connection_id = '<dataset-connection-uuid>'
+train_dataset_id = 'train-dataset-uuid'
 
 # first, upload the artefacts which we want to associate with the BYOM model version
-trained_model_artefacts_api.upload_artefacts(artefacts_import_id, artefacts)
+import_id = trained_model_artefacts_api.upload_byom_model(language,filename)
 
 import_request = {
-   "artefactImportId": str(artefacts_import_id),
-   "externalId": "my-byom-version-id"
+    "artefactImportId": import_id,
+    "externalId": "my_model_external_id",
+    "modelMonitoring": {
+        "language": language,
+        "useDefaultEvaluation": True,
+        "evaluationEnabled": True,
+        "modelType": "CLASSIFICATION",
+        "byomColumnExpression": "CAST(CAST(json_report AS JSON).JSONExtractValue('$.predicted_HasDiabetes') AS INT)",
+        "driftMonitoringEnabled": True,
+        "datasetId": train_dataset_id,
+        "datasetConnectionId": default_connection_id,
+    },
 }
 
-# update with id of your model 
-model_id = "<model-uuid>"
-
 job = model_api.import_byom(model_id, import_request)
 
 # wait until the job completes (if the job fails it will raise an exception)
 job_api.wait(job["id"])
 
 # now you can list the artefacts which were uploaded and linked to the model version
 trained_model_id = job["metadata"]["trainedModel"]["id"]
@@ -414,14 +429,21 @@
 ```
 
 
 ## Release Notes
 
 ### current
 
+- Fixed compatibility issue with `teradataml>=20.0.0.0`
+- Minor formatting updates
+- Added user attributes API
+- Updated programmatic BYOM import examples
+
+### 7.0.5
+
 **WARNING** Please recreate statistics metadata if you are using this version. It will produce more accurate results and correct behaviour.
 
 - Fixed computing statistics metadata for continuous features with all NULLs
 - Fixed training/eval/scoring statistics on columns with all NULLs
 - Added a workaround for VAL Histograms failure due to SP argument being longer than 31000 characters
 - Rounding all Decimal and Float bin edges to Teradata-supported FLOAT literals (15 digits max)
 - Fixed CLI error computing continuous statistics metadata related to mixed case column names
```

### Comparing `teradatamodelops-7.0.5b5/teradatamodelops.egg-info/SOURCES.txt` & `teradatamodelops-7.0.6rc1/teradatamodelops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 aoa/api/job_event_api.py
 aoa/api/message_api.py
 aoa/api/model_api.py
 aoa/api/project_api.py
 aoa/api/trained_model_api.py
 aoa/api/trained_model_artefacts_api.py
 aoa/api/trained_model_event_api.py
+aoa/api/user_attributes_api.py
 aoa/cli/__init__.py
 aoa/cli/base_model.py
 aoa/cli/evaluate_model.py
 aoa/cli/repo_manager.py
 aoa/cli/run_model.R
 aoa/cli/score_model.py
 aoa/cli/train_model.py
```

