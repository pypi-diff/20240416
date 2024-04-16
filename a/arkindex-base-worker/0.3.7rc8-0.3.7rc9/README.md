# Comparing `tmp/arkindex-base-worker-0.3.7rc8.tar.gz` & `tmp/arkindex-base-worker-0.3.7rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkindex-base-worker-0.3.7rc8.tar", last modified: Fri Apr  5 10:26:55 2024, max compression
+gzip compressed data, was "arkindex-base-worker-0.3.7rc9.tar", last modified: Wed Apr 10 16:44:30 2024, max compression
```

## Comparing `arkindex-base-worker-0.3.7rc8.tar` & `arkindex-base-worker-0.3.7rc9.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3359 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3359 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1633 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-05 10:26:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/arkindex_worker/
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/cache.py
--rw-rw-rw-   0 root         (0) root         (0)    14267 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/image.py
--rw-rw-rw-   0 root         (0) root         (0)     9844 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6900 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/
--rw-rw-rw-   0 root         (0) root         (0)    18806 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19585 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10328 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    33848 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/element.py
--rw-rw-rw-   0 root         (0) root         (0)    14714 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/entity.py
--rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/task.py
--rw-rw-rw-   0 root         (0) root         (0)    10235 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/training.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/transcription.py
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/version.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/docs-requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.417494 arkindex-base-worker-0.3.7rc8/hooks/
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/hooks/pre_gen_project.py
--rw-rw-rw-   0 root         (0) root         (0)     2405 2024-04-05 10:25:44.000000 arkindex-base-worker-0.3.7rc8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-05 10:26:55.425494 arkindex-base-worker-0.3.7rc8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-05 10:26:37.000000 arkindex-base-worker-0.3.7rc8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22134 2024-04-05 10:07:55.000000 arkindex-base-worker-0.3.7rc8/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    24512 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_base_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    10640 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    23848 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_dataset_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    13181 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_element.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    26417 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_classifications.py
--rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11777 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)    84971 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_elements.py
--rw-rw-rw-   0 root         (0) root         (0)    34557 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_entities.py
--rw-rw-rw-   0 root         (0) root         (0)    18756 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     8414 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_training.py
--rw-rw-rw-   0 root         (0) root         (0)    73468 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_transcriptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17163 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_worker.py
--rw-rw-rw-   0 root         (0) root         (0)    16262 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_image.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     1236 2024-04-05 10:07:56.000000 arkindex-base-worker-0.3.7rc8/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.413494 arkindex-base-worker-0.3.7rc8/worker-demo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/worker-demo/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/tests/test_worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-05 10:26:55.421494 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-05 10:23:38.000000 arkindex-base-worker-0.3.7rc8/worker-demo/worker_demo/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.905453 arkindex-base-worker-0.3.7rc9/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-10 16:44:30.905453 arkindex-base-worker-0.3.7rc9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.901453 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3538 2024-04-10 16:44:30.000000 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-10 16:44:30.000000 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 16:44:30.000000 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      340 2024-04-10 16:44:30.000000 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-10 16:44:30.000000 arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.897453 arkindex-base-worker-0.3.7rc9/arkindex_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11248 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    14267 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     9844 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     7243 2024-04-10 11:08:05.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.897453 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/
+-rw-rw-rw-   0 root         (0) root         (0)    18806 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19585 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10328 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    33848 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/element.py
+-rw-rw-rw-   0 root         (0) root         (0)    14714 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/task.py
+-rw-rw-rw-   0 root         (0) root         (0)    10235 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/training.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/transcription.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.897453 arkindex-base-worker-0.3.7rc9/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/hooks/pre_gen_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     2724 2024-04-10 16:41:25.000000 arkindex-base-worker-0.3.7rc9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 16:44:30.905453 arkindex-base-worker-0.3.7rc9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.897453 arkindex-base-worker-0.3.7rc9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:44:11.000000 arkindex-base-worker-0.3.7rc9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22134 2024-04-10 11:03:07.000000 arkindex-base-worker-0.3.7rc9/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    24512 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_base_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    10640 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    23848 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_dataset_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    13181 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_element.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.901453 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    26417 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_classifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11777 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)    84971 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_elements.py
+-rw-rw-rw-   0 root         (0) root         (0)    34557 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)    18756 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     8414 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_training.py
+-rw-rw-rw-   0 root         (0) root         (0)    73468 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_transcriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17163 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)    16262 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_image.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2024-04-10 11:03:08.000000 arkindex-base-worker-0.3.7rc9/tests/test_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-04-10 11:08:05.000000 arkindex-base-worker-0.3.7rc9/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.893453 arkindex-base-worker-0.3.7rc9/worker-demo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.901453 arkindex-base-worker-0.3.7rc9/worker-demo/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 16:41:47.000000 arkindex-base-worker-0.3.7rc9/worker-demo/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-10 16:41:47.000000 arkindex-base-worker-0.3.7rc9/worker-demo/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-10 16:41:47.000000 arkindex-base-worker-0.3.7rc9/worker-demo/tests/test_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 16:44:30.901453 arkindex-base-worker-0.3.7rc9/worker-demo/worker_demo/
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-04-10 16:41:47.000000 arkindex-base-worker-0.3.7rc9/worker-demo/worker_demo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-10 16:41:47.000000 arkindex-base-worker-0.3.7rc9/worker-demo/worker_demo/worker.py
```

### Comparing `arkindex-base-worker-0.3.7rc8/LICENSE` & `arkindex-base-worker-0.3.7rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/PKG-INFO` & `arkindex-base-worker-0.3.7rc9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc8
+Version: 0.3.7rc9
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
         
@@ -52,14 +52,18 @@
 Requires-Dist: black==24.2.0; extra == "docs"
 Requires-Dist: doc8==1.1.1; extra == "docs"
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.10; extra == "docs"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs"
 Requires-Dist: recommonmark==0.7.1; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest==8.0.1; extra == "tests"
+Requires-Dist: pytest-mock==3.12.0; extra == "tests"
+Requires-Dist: pytest-responses==0.5.1; extra == "tests"
 
 # Arkindex base Worker
 
 An easy to use Python 3 high level API client, to build ML tasks.
 
 This is an open-source project, licensed using [the MIT license](https://opensource.org/license/mit/).
```

### Comparing `arkindex-base-worker-0.3.7rc8/README.md` & `arkindex-base-worker-0.3.7rc9/README.md`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/PKG-INFO` & `arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkindex-base-worker
-Version: 0.3.7rc8
+Version: 0.3.7rc9
 Summary: Base Worker to easily build Arkindex ML workflows
 Author-email: Teklia <contact@teklia.com>
 Maintainer-email: Teklia <contact@teklia.com>
 License: MIT License
         
         Copyright (c) 2023 Teklia
         
@@ -52,14 +52,18 @@
 Requires-Dist: black==24.2.0; extra == "docs"
 Requires-Dist: doc8==1.1.1; extra == "docs"
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.10; extra == "docs"
 Requires-Dist: mkdocstrings==0.24.0; extra == "docs"
 Requires-Dist: mkdocstrings-python==1.8.0; extra == "docs"
 Requires-Dist: recommonmark==0.7.1; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: pytest==8.0.1; extra == "tests"
+Requires-Dist: pytest-mock==3.12.0; extra == "tests"
+Requires-Dist: pytest-responses==0.5.1; extra == "tests"
 
 # Arkindex base Worker
 
 An easy to use Python 3 high level API client, to build ML tasks.
 
 This is an open-source project, licensed using [the MIT license](https://opensource.org/license/mit/).
```

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_base_worker.egg-info/SOURCES.txt` & `arkindex-base-worker-0.3.7rc9/arkindex_base_worker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE
 README.md
-docs-requirements.txt
 pyproject.toml
-requirements.txt
 arkindex_base_worker.egg-info/PKG-INFO
 arkindex_base_worker.egg-info/SOURCES.txt
 arkindex_base_worker.egg-info/dependency_links.txt
 arkindex_base_worker.egg-info/requires.txt
 arkindex_base_worker.egg-info/top_level.txt
 arkindex_worker/__init__.py
 arkindex_worker/cache.py
@@ -41,11 +39,12 @@
 tests/test_elements_worker/test_elements.py
 tests/test_elements_worker/test_entities.py
 tests/test_elements_worker/test_metadata.py
 tests/test_elements_worker/test_task.py
 tests/test_elements_worker/test_training.py
 tests/test_elements_worker/test_transcriptions.py
 tests/test_elements_worker/test_worker.py
+worker-demo/tests/__init__.py
 worker-demo/tests/conftest.py
 worker-demo/tests/test_worker.py
 worker-demo/worker_demo/__init__.py
 worker-demo/worker_demo/worker.py
```

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/cache.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/image.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/models.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/models.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/utils.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 from pathlib import Path
 
 import zstandard
 import zstandard as zstd
 
 logger = logging.getLogger(__name__)
 
+MANUAL_SOURCE = "manual"
+
+
+def parse_source_id(value: str) -> bool | str | None:
+    """
+    Parse a UUID argument (Worker Version, Worker Run, ...) to use it directly in the API.
+    Arkindex API filters generally expect `False` to filter manual sources.
+    """
+    if value == MANUAL_SOURCE:
+        return False
+    return value or None
+
+
 CHUNK_SIZE = 1024
 """Chunk Size used for ZSTD compression"""
 
 
 def decompress_zst_archive(compressed_archive: Path) -> tuple[int, Path]:
     """
     Decompress a ZST-compressed tar archive in data dir. The tar archive is not extracted.
```

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/__init__.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/base.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/base.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/classification.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/classification.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/dataset.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/dataset.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/element.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/entity.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/entity.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/metadata.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/task.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/training.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/transcription.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/transcription.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/arkindex_worker/worker/version.py` & `arkindex-base-worker-0.3.7rc9/arkindex_worker/worker/version.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/pyproject.toml` & `arkindex-base-worker-0.3.7rc9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arkindex-base-worker"
-version = "0.3.7rc8"
+version = "0.3.7rc9"
 description = "Base Worker to easily build Arkindex ML workflows"
 license = { file = "LICENSE" }
-dynamic = ["dependencies", "optional-dependencies"]
+dependencies = [
+    "peewee==3.17.0",
+    "Pillow==10.2.0",
+    "pymdown-extensions==10.7",
+    "python-gnupg==0.5.2",
+    "shapely==2.0.3",
+    "teklia-toolbox==0.1.4rc3",
+    "zstandard==0.22.0",
+]
 authors = [
     { name = "Teklia", email = "contact@teklia.com" },
 ]
 maintainers = [
     { name = "Teklia", email = "contact@teklia.com" },
 ]
 requires-python = ">=3.10"
@@ -31,21 +39,33 @@
 [project.urls]
 Homepage = "https://workers.arkindex.org"
 Documentation = "https://workers.arkindex.org"
 Repository = "https://gitlab.teklia.com/workers/base-worker"
 "Bug Tracker" = "https://gitlab.teklia.com/workers/base-worker/issues"
 Authors = "https://teklia.com"
 
+[project.optional-dependencies]
+docs = [
+    "black==24.2.0",
+    "doc8==1.1.1",
+    "mkdocs==1.5.3",
+    "mkdocs-material==9.5.10",
+    "mkdocstrings==0.24.0",
+    "mkdocstrings-python==1.8.0",
+    "recommonmark==0.7.1",
+]
+tests = [
+    "pytest==8.0.1",
+    "pytest-mock==3.12.0",
+    "pytest-responses==0.5.1",
+]
+
 [tool.setuptools.packages]
 find = {}
 
-[tool.setuptools.dynamic]
-dependencies = { file = ["requirements.txt"] }
-optional-dependencies = { docs = { file = ["docs-requirements.txt"] } }
-
 [tool.ruff]
 exclude = [".git", "__pycache__"]
 
 [tool.ruff.lint]
 ignore = ["E501"]
 select = [
     # pycodestyle
```

### Comparing `arkindex-base-worker-0.3.7rc8/tests/conftest.py` & `arkindex-base-worker-0.3.7rc9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_base_worker.py` & `arkindex-base-worker-0.3.7rc9/tests/test_base_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_cache.py` & `arkindex-base-worker-0.3.7rc9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_dataset_worker.py` & `arkindex-base-worker-0.3.7rc9/tests/test_dataset_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_element.py` & `arkindex-base-worker-0.3.7rc9/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_classifications.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_classifications.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_cli.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_cli.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_dataset.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_dataset.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_elements.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_elements.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_entities.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_entities.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_metadata.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_metadata.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_task.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_task.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_training.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_training.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_transcriptions.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_transcriptions.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_elements_worker/test_worker.py` & `arkindex-base-worker-0.3.7rc9/tests/test_elements_worker/test_worker.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_image.py` & `arkindex-base-worker-0.3.7rc9/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/tests/test_merge.py` & `arkindex-base-worker-0.3.7rc9/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `arkindex-base-worker-0.3.7rc8/worker-demo/tests/conftest.py` & `arkindex-base-worker-0.3.7rc9/worker-demo/tests/conftest.py`

 * *Files identical despite different names*

