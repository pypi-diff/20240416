# Comparing `tmp/swebench-1.0.9.tar.gz` & `tmp/swebench-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.9.tar", last modified: Wed Apr 10 04:33:17 2024, max compression
+gzip compressed data, was "swebench-1.1.0.tar", last modified: Mon Apr 15 22:20:59 2024, max compression
```

## Comparing `swebench-1.0.9.tar` & `swebench-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.731325 swebench-1.0.9/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.9/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-10 04:33:17.731245 swebench-1.0.9/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.9/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.720539 swebench-1.0.9/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.721254 swebench-1.0.9/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.723521 swebench-1.0.9/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.9/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.9/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.9/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.9/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.9/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-10 04:33:17.731522 swebench-1.0.9/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.9/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.723817 swebench-1.0.9/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-10 04:32:33.000000 swebench-1.0.9/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.726066 swebench-1.0.9/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.727885 swebench-1.0.9/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    22538 2024-04-10 04:30:31.000000 swebench-1.0.9/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    31223 2024-04-09 19:56:34.000000 swebench-1.0.9/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.9/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.729936 swebench-1.0.9/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.0.9/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.9/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.730793 swebench-1.0.9/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.9/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-10 04:33:17.730973 swebench-1.0.9/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-10 04:33:17.000000 swebench-1.0.9/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592880 swebench-1.1.0/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.1.0/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7060 2024-04-15 22:20:59.592808 swebench-1.1.0/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5984 2024-04-15 22:20:09.000000 swebench-1.1.0/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.585261 swebench-1.1.0/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.585907 swebench-1.1.0/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.587150 swebench-1.1.0/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.1.0/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.1.0/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.1.0/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.1.0/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.1.0/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-15 22:20:59.593083 swebench-1.1.0/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1345 2024-04-11 15:11:14.000000 swebench-1.1.0/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.587362 swebench-1.1.0/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-15 19:56:17.000000 swebench-1.1.0/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.588886 swebench-1.1.0/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.590151 swebench-1.1.0/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    22114 2024-04-15 16:06:14.000000 swebench-1.1.0/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    31433 2024-04-12 18:56:31.000000 swebench-1.1.0/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7725 2024-04-12 18:56:55.000000 swebench-1.1.0/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6420 2024-04-12 18:57:04.000000 swebench-1.1.0/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10412 2024-04-10 19:23:48.000000 swebench-1.1.0/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.1.0/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.591473 swebench-1.1.0/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      430 2024-04-11 01:17:37.000000 swebench-1.1.0/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4504 2024-04-11 01:17:58.000000 swebench-1.1.0/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7102 2024-04-09 15:26:32.000000 swebench-1.1.0/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4339 2024-04-11 01:18:16.000000 swebench-1.1.0/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    12244 2024-04-12 18:57:17.000000 swebench-1.1.0/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592347 swebench-1.1.0/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.1.0/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-15 22:20:59.592542 swebench-1.1.0/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7060 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       81 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-15 22:20:59.000000 swebench-1.1.0/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.9/LICENSE` & `swebench-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/PKG-INFO` & `swebench-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.9
+Version: 1.1.0
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -22,14 +22,15 @@
 Requires-Dist: chardet
 Requires-Dist: datasets
 Requires-Dist: ghapi
 Requires-Dist: GitPython
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: rich
+Requires-Dist: tqdm
 
 <p align="center">
   <a href="https://github.com/princeton-nlp/Llamao">
     <img src="assets/swellama_banner.png" width="50%" alt="Kawi the SWE-Llama" />
   </a>
 </p>
 
@@ -54,14 +55,19 @@
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
+## 📰 News
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
+* **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
+
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
 ## 🚀 Set Up
```

#### html2text {}

```diff
@@ -1,41 +1,49 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.9 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.0 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: chardet Requires-Dist:
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
-dotenv Requires-Dist: requests Requires-Dist: rich
+dotenv Requires-Dist: requests Requires-Dist: rich Requires-Dist: tqdm
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
      SWE-bench) | [ä¸­æç®ä½](docs/README_CN.md) | [ä¸­æç¹é«](docs/
                                 README_TW.md) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
-benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
-language models on real world software issues collected from GitHub. Given a
-*codebase* and an *issue*, a language model is tasked with generating a *patch*
-that resolves the described problem. [assets/teaser.png]## ð Set Up To build
-SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
-`cd` into the repository. 3. Run `conda env create -f environment.yml` to
-created a conda environment named `swe-bench` 4. Activate the environment with
-`conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
-directly ([dev](https://drive.google.com/
+benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
+improvements to resolve issues with the evaluation harness. Read more in our
+[report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
+20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
+the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
+jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
+been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
+openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
+for evaluating large language models on real world software issues collected
+from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
+generating a *patch* that resolves the described problem. [assets/teaser.png]##
+ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
+repository locally 2. `cd` into the repository. 3. Run `conda env create -
+f environment.yml` to created a conda environment named `swe-bench` 4. Activate
+the environment with `conda activate swe-bench` ## ð½ Usage You can download
+the SWE-bench dataset directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
 main/inference/) on existing models (either models you have on-disk like LLaMA,
 or models you have access to through an API like GPT-4). The inference step is
```

### Comparing `swebench-1.0.9/README.md` & `swebench-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -25,14 +25,19 @@
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
+## 📰 News
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
+* **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
+
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
 ## 🚀 Set Up
```

#### html2text {}

```diff
@@ -5,23 +5,31 @@
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
-benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
-language models on real world software issues collected from GitHub. Given a
-*codebase* and an *issue*, a language model is tasked with generating a *patch*
-that resolves the described problem. [assets/teaser.png]## ð Set Up To build
-SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
-`cd` into the repository. 3. Run `conda env create -f environment.yml` to
-created a conda environment named `swe-bench` 4. Activate the environment with
-`conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
-directly ([dev](https://drive.google.com/
+benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
+improvements to resolve issues with the evaluation harness. Read more in our
+[report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
+20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
+the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
+jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
+been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
+openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
+for evaluating large language models on real world software issues collected
+from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
+generating a *patch* that resolves the described problem. [assets/teaser.png]##
+ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
+repository locally 2. `cd` into the repository. 3. Run `conda env create -
+f environment.yml` to created a conda environment named `swe-bench` 4. Activate
+the environment with `conda activate swe-bench` ## ð½ Usage You can download
+the SWE-bench dataset directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
 main/inference/) on existing models (either models you have on-disk like LLaMA,
 or models you have access to through an API like GPT-4). The inference step is
```

### Comparing `swebench-1.0.9/inference/llamao/distributed_attention.py` & `swebench-1.1.0/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/llamao/modeling_flash_llama.py` & `swebench-1.1.0/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/bm25_retrieval.py` & `swebench-1.1.0/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/create_instance.py` & `swebench-1.1.0/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/create_text_dataset.py` & `swebench-1.1.0/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/eval_retrieval.py` & `swebench-1.1.0/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/tokenize_dataset.py` & `swebench-1.1.0/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/make_datasets/utils.py` & `swebench-1.1.0/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/run_api.py` & `swebench-1.1.0/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/run_live.py` & `swebench-1.1.0/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/inference/run_llama.py` & `swebench-1.1.0/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/setup.py` & `swebench-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,10 +32,11 @@
         'chardet',
         'datasets',
         'ghapi',
         'GitPython',
         'python-dotenv',
         'requests',
         'rich',
+        'tqdm',
     ],
     include_package_data=True,
 )
```

### Comparing `swebench-1.0.9/swebench/__init__.py` & `swebench-1.1.0/swebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.9/swebench/collect/build_dataset.py` & `swebench-1.1.0/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/collect/build_dataset_ft.py` & `swebench-1.1.0/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/collect/get_tasks_pipeline.py` & `swebench-1.1.0/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/collect/get_top_pypi.py` & `swebench-1.1.0/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/collect/print_pulls.py` & `swebench-1.1.0/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/collect/utils.py` & `swebench-1.1.0/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/harness/constants.py` & `swebench-1.1.0/swebench/harness/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from enum import Enum
+
 MAP_VERSION_TO_INSTALL_SKLEARN = {
     k: {
         "python": "3.6",
         "packages": "numpy scipy cython pytest pandas matplotlib",
         "install": "pip install -v --no-use-pep517 --no-build-isolation -e .",
         "arch_specific_packages": {
             "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
@@ -18,20 +20,14 @@
         k: {
             "python": "3.9",
             "packages": "numpy scipy cython pytest pandas matplotlib joblib threadpoolctl",
             "install": "pip install -v --no-use-pep517 --no-build-isolation -e .",
             "arch_specific_packages": {
                 "aarch64": "gxx_linux-aarch64 gcc_linux-aarch64 make",
             },
-            "pip_packages": [
-                "numpy==1.25.2",
-                "scipy==1.11.1",
-                "joblib==1.2.0",
-                "threadpoolctl==2.2.0",
-            ]
         }
         for k in ["1.3", "1.4"]
     }
 )
 
 MAP_VERSION_TO_INSTALL_FLASK = {
     "2.0": {
@@ -205,18 +201,18 @@
         "install": "pip install -e ."
     } for k in [
         '4.4','4.5','4.6','5.0','5.1','5.2','5.3','5.4',
         '6.0','6.2','6.3','7.0','7.1','7.2','7.4','8.0'
     ]
 }
 MAP_VERSION_TO_INSTALL_PYTEST["4.4"]["pip_packages"] = [
-    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0"
+    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
     "pluggy==0.13.1", "py==1.11.0", "setuptools==68.0.0", "six==1.16.0",]
 MAP_VERSION_TO_INSTALL_PYTEST["4.5"]["pip_packages"] = [
-    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0"
+    "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
     "pluggy==0.11.0", "py==1.11.0", "setuptools==68.0.0", "six==1.16.0", "wcwidth==0.2.6"]
 MAP_VERSION_TO_INSTALL_PYTEST["4.6"]["pip_packages"] = [
     "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
     "packaging==23.1", "pluggy==0.13.1", "py==1.11.0", "six==1.16.0", "wcwidth==0.2.6"]
 for k in ["5.0", "5.1", "5.2"]:
     MAP_VERSION_TO_INSTALL_PYTEST[k]["pip_packages"] = [
         "atomicwrites==1.4.1", "attrs==23.1.0", "more-itertools==10.1.0",
@@ -419,15 +415,15 @@
         "python": "3.10",
         "packages": "environment.yml",
         "install": "pip install -e .",
         "pip_packages": [
             "numpy==1.25.2",
             "packaging==23.1",
             "pandas==1.5.3",
-            "pytest==7.4.0",
+            "pytest==8.1.1",
             "python-dateutil==2.8.2",
             "pytz==2023.3",
             "six==1.16.0",
         ],
         "no_use_env": True,
     }
     for k in ["0.12", "0.18", "0.19", "0.20", "2022.03", "2022.06", "2022.09"]
@@ -521,17 +517,14 @@
     for k in ['1.4', '2.0']})
 MAP_VERSION_TO_INSTALL_PYDICOM.update({
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.9"}
     for k in ['2.1', '2.2']})
 MAP_VERSION_TO_INSTALL_PYDICOM.update({
     k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.10"}
     for k in ['2.3']})
-MAP_VERSION_TO_INSTALL_PYDICOM.update({
-    k: {**MAP_VERSION_TO_INSTALL_PYDICOM[k], "python": "3.11"}
-    for k in ['2.4', '3.0']})
 
 MAP_VERSION_TO_INSTALL_HUMANEVAL= {k: { "python": "3.9" } for k in ['1.0']}
 
 # Constants - Task Instance Instllation Environment
 MAP_VERSION_TO_INSTALL = {
     "astropy/astropy": MAP_VERSION_TO_INSTALL_ASTROPY,
     "django/django": MAP_VERSION_TO_INSTALL_DJANGO,
@@ -557,17 +550,15 @@
 # Constants - Repository Specific Installation Instructions
 MAP_REPO_TO_INSTALL = {}
 
 # Constants - Task Instance Test Frameworks
 TEST_PYTEST = "pytest --no-header -rA --tb=no -p no:cacheprovider"
 MAP_REPO_TO_TEST_FRAMEWORK = {
     "astropy/astropy": TEST_PYTEST,
-    "dbt-labs/dbt-core": TEST_PYTEST,
     "django/django": "./tests/runtests.py --verbosity 2",
-    "huggingface/transformers": TEST_PYTEST,
     "marshmallow-code/marshmallow": TEST_PYTEST,
     "matplotlib/matplotlib": TEST_PYTEST,
     "mwaskom/seaborn": "pytest --no-header -rA",
     "pallets/flask": TEST_PYTEST,
     "psf/requests": TEST_PYTEST,
     "pvlib/pvlib-python": TEST_PYTEST,
     "pydata/xarray": TEST_PYTEST,
@@ -581,15 +572,14 @@
     "sqlfluff/sqlfluff": TEST_PYTEST,
     "swe-bench/humaneval": "python",
     "sympy/sympy": "bin/test -C --verbose",
 }
 
 # Constants - Task Instance Requirements File Paths
 MAP_REPO_TO_REQS_PATHS = {
-    "dbt-labs/dbt-core": ["dev-requirements.txt", "dev_requirements.txt"],
     "django/django": ["tests/requirements/py3.txt"],
     "matplotlib/matplotlib": ["requirements/dev/dev-requirements.txt", "requirements/testing/travis_all.txt"],
     "pallets/flask": ["requirements/dev.txt"],
     "pylint-dev/pylint": ["requirements_test.txt"],
     "pyvista/pyvista": ["requirements_test.txt", 'requirements.txt'],
     "sqlfluff/sqlfluff": ["requirements_dev.txt"],
     "sympy/sympy": ["requirements-dev.txt"],
@@ -614,29 +604,31 @@
 INSTALL_TIMEOUT = ">>>>> Init Timed Out"
 RESET_FAILED = ">>>>> Reset Failed"
 TESTS_ERROR = ">>>>> Tests Errored"
 TESTS_FAILED = ">>>>> Some Tests Failed"
 TESTS_PASSED = ">>>>> All Tests Passed"
 TESTS_TIMEOUT = ">>>>> Tests Timed Out"
 
+# Constants - Patch Types
+class PatchType(Enum):
+    PATCH_GOLD = "gold"
+    PATCH_PRED = "pred"
+    PATCH_PRED_TRY = "pred_try"
+    PATCH_PRED_MINIMAL = "pred_minimal"
+    PATCH_PRED_MINIMAL_TRY = "pred_minimal_try"
+    PATCH_TEST = "test"
+
+    def __str__(self):
+        return self.value
+
 # Constants - Miscellaneous
 NON_TEST_EXTS = [".json", ".png", "csv", ".txt", ".md", ".jpg", ".jpeg", ".pkl", ".yml", ".yaml", ".toml"]
 SWE_BENCH_URL_RAW = "https://raw.githubusercontent.com/"
 
 # Constants - Repo/Version Mapped to Appropriate Conda Link
 MAP_REPO_VERSION_TO_CONDA_LINK = {
-    "django/django": {
-        "1.11": "py311_23.9.0-0",
-    },
-    "matplotlib/matplotlib": {
-        "3.1": "py311_23.9.0-0",
-        "3.2": "py311_23.9.0-0",
-        "3.3": "py311_23.9.0-0",
-        "3.4": "py311_23.9.0-0",
-        "3.0": "py311_23.10.0-1",
-    },
-    "sympy/sympy": {
-        "1.0": "py39_23.9.0-0",
+    "psf/requests": {
+        "2.4": "py39_23.9.0-0",
     },
 }
 
 DEFAULT_CONDA_LINK = "py39_23.10.0-1"
```

### Comparing `swebench-1.0.9/swebench/harness/context_manager.py` & `swebench-1.1.0/swebench/harness/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,27 +15,28 @@
     MAP_REPO_VERSION_TO_CONDA_LINK,
     MAP_VERSION_TO_INSTALL,
     RESET_FAILED,
     TESTS_FAILED,
     TESTS_PASSED,
     TESTS_TIMEOUT,
     TESTS_ERROR,
+    PatchType,
 )
 from swebench.harness.utils import (
     clone_repo,
     get_conda_env_names,
     get_environment_yml,
     get_requirements,
     get_test_directives,
 )
 from tempfile import TemporaryDirectory
 from traceback import format_exc
 
 logging.basicConfig(format="%(asctime)s - %(levelname)s - %(message)s")
-logger_testbed = logging.getLogger("testbed_context_manager")
+logger_testbed = logging.getLogger("testbed")
 
 
 class LogWrapper:
     def __init__(
         self,
         log_file: str,
         logger: logging.Logger = None,
@@ -78,20 +79,22 @@
                 self.logger.write(f"Command: {cmd}", level=DEBUG)
             combined_args = {**self.subprocess_args, **kwargs}
             self.logger.write(f"Subprocess args: {json.dumps(combined_args)}", level=DEBUG)
             output = subprocess.run(cmd, **combined_args)
             self.logger.write(f"Std. Output:\n{output.stdout}", level=DEBUG)
             if output.stderr:
                 self.logger.write(f"Std. Error:\n{output.stderr}", level=DEBUG)
+            self.logger.write(f"Return Code: {output.returncode}", level=DEBUG)
             return output
         except subprocess.CalledProcessError as e:
             if raise_error and self.logger is not None:
                 self.logger.write(f"Error: {e}", level=ERROR)
                 self.logger.write(f"Error stdout: {e.stdout}", level=ERROR)
-                self.logger.write(f"Error stderr: {e.stderr}", level=ERROR)
+                if e.stderr:
+                    self.logger.write(f"Error stderr: {e.stderr}", level=ERROR)
                 self.logger.write(f"Error traceback: {format_exc()}", level=ERROR)
                 raise e
 
 
 class TestbedContextManager:
     def __init__(
         self,
@@ -125,16 +128,18 @@
         self.old_dir = os.getcwd()
         self.timeout = timeout
         self.verbose = verbose
         self.exec = ExecWrapper(
             subprocess_args={
                 "check": True,
                 "shell": False,
-                "capture_output": True,
+                "capture_output": False,
                 "text": True,
+                "stdout": subprocess.PIPE,
+                "stderr": subprocess.STDOUT,
             },
         )
 
         # Create log, temp directories if they don't exist
         if not os.path.exists(self.log_dir):
             logger_testbed.info(f"[Testbed] Creating log directory {self.log_dir}")
             os.makedirs(self.log_dir, exist_ok=True)
@@ -149,16 +154,16 @@
         )
 
         # Group repos by repo, then version
         self.task_instances_grouped = {}
         for instance in self.task_instances:
             # Create test command from framework + directives
             test_type = MAP_REPO_TO_TEST_FRAMEWORK[instance["repo"]]
-            test_directives = get_test_directives(instance)
-            instance["test_cmd"] = f"{test_type} {' '.join(test_directives)}"
+            instance["test_directives"] = get_test_directives(instance)
+            instance["test_cmd"] = f"{test_type} {' '.join(instance['test_directives'])}"
 
             # Group task instances by repo, version
             repo = instance["repo"]
             version = instance["version"] if "version" in instance else None
             if repo not in self.task_instances_grouped:
                 self.task_instances_grouped[repo] = {}
             if version not in self.task_instances_grouped[repo]:
@@ -332,15 +337,15 @@
                 # Create conda environment according to install instructinos
                 pkgs = install["packages"] if "packages" in install else ""
                 if pkgs == "requirements.txt":
                     # Create environment
                     cmd = (
                         f"{exec_cmd} create -n {env_name} python={install['python']} -y"
                     )
-                    self.log.write(f"Creating environment {env_name}; Command: {cmd}")
+                    self.log.write(f"Creating environment {env_name}")
                     self.exec(cmd.split(" "))
 
                     # Install dependencies
                     path_to_reqs = get_requirements(setup_ref_instance, self.testbed)
                     cmd = f". {path_activate} {env_name} && echo 'activate successful' && pip install -r {path_to_reqs}"
                     self.log.write(f"Installing dependencies for {env_name}; Command: {cmd}")
                     self.exec(cmd, shell=True)
@@ -351,15 +356,15 @@
                         path_to_reqs = get_environment_yml(
                             setup_ref_instance, env_name,
                             save_path=self.testbed
                         )
 
                         # `conda create` based installation
                         cmd = f"{exec_cmd} create -c conda-forge -n {env_name} python={install['python']} -y"
-                        self.log.write(f"Creating environment {env_name}; Command: {cmd}")
+                        self.log.write(f"Creating environment {env_name}")
                         self.exec(cmd.split(" "))
 
                         # Install dependencies
                         cmd = f"{exec_cmd} env update -f {path_to_reqs}"
                         self.log.write(f"Installing dependencies for {env_name}; Command: {cmd}")
                         self.exec(cmd.split(" "))
                     else:
@@ -368,23 +373,23 @@
                             setup_ref_instance, env_name,
                             save_path=self.testbed,
                             python_version=install["python"]
                         )
 
                         # `conda env create` based installation
                         cmd = f"{exec_cmd} env create --file {path_to_reqs}"
-                        self.log.write(f"Creating environment {env_name}; Command: {cmd}")
+                        self.log.write(f"Creating environment {env_name}")
                         self.exec(cmd.split(" "))
 
                     # Remove environment.yml
                     os.remove(path_to_reqs)
                 else:
                     # Create environment + install dependencies
                     cmd = f"{exec_cmd} create -n {env_name} python={install['python']} {pkgs} -y"
-                    self.log.write(f"Creating environment {env_name}; Command: {cmd}")
+                    self.log.write(f"Creating environment {env_name}")
                     self.exec(cmd.split(" "))
                 
                 arch = platform.machine()
                 arch_specific_packages = install.get("arch_specific_packages", {}).get(arch, "")
                 if arch_specific_packages:
                     cmd = f". {path_activate} {env_name} && conda install {arch_specific_packages} -y"
                     self.log.write(f"Installing arch-specific packages for {env_name}; Command: {cmd}")
@@ -445,15 +450,15 @@
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if self.temp_dir_work is not None:
             self.temp_dir_work.cleanup()
         if self.temp_dir_conda is not None:
             self.temp_dir_conda.cleanup()
 
 
-logger_taskenv = logging.getLogger("taskenv_context_manager")
+logger_taskenv = logging.getLogger("taskenv")
 
 
 class TaskEnvContextManager:
     def __init__(
         self,
         instance: dict,
         testbed: str,
@@ -513,17 +518,19 @@
         )
         self.timeout = timeout
 
         self.exec = ExecWrapper(
             subprocess_args={
                 "check": True,
                 "shell": False,
-                "capture_output": True,
+                "capture_output": False,
                 "text": True,
                 "env": {"CONDA_PKGS_DIRS": self.conda_cache_dir},
+                "stdout": subprocess.PIPE,
+                "stderr": subprocess.STDOUT,
             },
             logger=self.log,
         )
 
     def __enter__(self):
         """
         Enter task environment, set up log file
@@ -594,15 +601,16 @@
                 self.log.write(f"Running pre-install setup command: {cmd_pre_install}")
                 out_pre_install = self.exec(
                     cmd_pre_install, timeout=self.timeout, shell=True
                 )
                 with open(self.log_file, "a") as f:
                     f.write(f"Pre-installation Command: {cmd_pre_install}\n")
                     f.write(f"Std. Output: {out_pre_install.stdout}\n")
-                    f.write(f"Std. Error: {out_pre_install.stderr}\n")
+                    if out_pre_install.stderr:
+                        f.write(f"Std. Error: {out_pre_install.stderr}\n")
                 if out_pre_install.returncode != 0:
                     self.log.write(f"Pre-install setup failed", level=ERROR)
                     with open(self.log_file, "a") as f:
                         f.write(f"\n{INSTALL_FAIL}\n")
                     return False
 
         # Skip installation if no instructions provided
@@ -611,20 +619,14 @@
 
         cmd_install = f"{self.cmd_activate} && {specifications['install']}"
         self.log.write(f"Running installation command: {cmd_install}")
         try:
             # Run installation command
             out_install = self.exec(cmd_install, timeout=self.timeout, shell=True)
 
-            # Write installation logs to log file
-            with open(self.log_file, "a") as f:
-                f.write(f"Installation Command: {cmd_install}\n")
-                f.write(f"Std. Output: {out_install.stdout}\n")
-                f.write(f"Std. Error: {out_install.stderr}\n")
-
             if out_install.returncode != 0:
                 # Installation failed
                 self.log.write(f"Installation failed", level=ERROR)
                 with open(self.log_file, "a") as f:
                     f.write(f"\n{INSTALL_FAIL}\n")
                 return False
 
@@ -643,15 +645,15 @@
             # Installation failed
             self.log.write(f"Installation failed", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"\n{INSTALL_FAIL}: {e}\n")
             return False
 
     def apply_patch(
-        self, patch: str, patch_type: str = "", revert: bool = False
+        self, patch: str, patch_type: PatchType = "", revert: bool = False
     ) -> bool:
         """
         Apply patch to task environment
 
         Args:
             patch (str): Plaintext of patch to apply
             patch_type (str): Type of patch (e.g. "eval", "test")
@@ -669,29 +671,36 @@
         patch_path = os.path.join(
             os.path.dirname(self.testbed.rstrip("/")),
             f"temp_{self.instance[KEY_INSTANCE_ID]}_{patch_type}.patch",
         )
         with open(patch_path, "w") as f:
             f.write(patch)
 
+        # Restore test files before applying if patch_type is 'test'
+        if patch_type == PatchType.PATCH_TEST.value:
+            for test in self.instance["test_directives"]:
+                if os.path.exists(test):
+                    self.exec(f"git restore {test}".split(" "))
+
         # Apply patch to testbed directory
         apply_cmd = (
             f"git apply -v -R {patch_path}" if revert else f"git apply -v {patch_path}"
         )
         out_patch = self.exec(apply_cmd.split(" "), raise_error=False, check=False)
         os.remove(patch_path)
 
         log_cmd = "Revert" if revert else "Apply"
         if out_patch.returncode != 0:
             # Patch apply failed
             self.log.write(f"{log_cmd} patch failed ({patch_type})", level=ERROR)
             with open(self.log_file, "a") as f:
                 f.write(f"{APPLY_PATCH_FAIL}; ({patch_type})\nOutput:\n")
                 f.write(out_patch.stdout)
-                f.write(out_patch.stderr)
+                if out_patch.stderr:
+                    f.write(out_patch.stderr)
             return False
 
         # Patch apply succeeded
         self.log.write(f"{log_cmd} patch successful ({patch_type})")
         with open(self.log_file, "a") as f:
             f.write(f"{APPLY_PATCH_PASS} ({patch_type})\n")
         return True
@@ -721,19 +730,16 @@
             )
 
             # Unset environment variables if provided
             if "env_vars_test" in specifications:
                 for key in specifications["env_vars_test"]:
                     del self.exec.subprocess_args["env"][key]
 
-            # Write test results to log file
+            # Write pass/fail status to log file
             with open(self.log_file, "a") as f:
-                f.write(f"Output:\n")
-                f.write(out_test.stdout)
-                f.write(out_test.stderr)
                 if out_test.returncode != 0:
                     f.write(f"\n{TESTS_FAILED}\n")
                 else:
                     f.write(f"\n{TESTS_PASSED}\n")
 
             self.log.write(f"Test script run successful")
             return True
```

### Comparing `swebench-1.0.9/swebench/harness/engine_evaluation.py` & `swebench-1.1.0/swebench/harness/engine_evaluation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from multiprocessing import Pool, cpu_count
 from swebench.harness.constants import (
     APPLY_PATCH_FAIL,
     KEY_INSTANCE_ID,
     KEY_MODEL,
     KEY_PREDICTION,
+    PatchType,
 )
 from swebench.harness.context_manager import TaskEnvContextManager
 from swebench.harness.engine_validation import setup_testbed
 from swebench.harness.utils import (
     extract_minimal_patch,
     get_instances,
     split_instances,
@@ -42,15 +43,15 @@
     if not tcm.reset_task_env(task_instance):
         return
     
     filename_pat = re.compile(r'\[start of ([\w\.\-\/]+)\]\n(.+?)\n\[end of \1\]', re.DOTALL)
     # Run installation
     if (
         not tcm.run_install_task(task_instance)
-        or not tcm.apply_patch(task_instance["test_patch"], patch_type="test")
+        or not tcm.apply_patch(task_instance["test_patch"], patch_type=PatchType.PATCH_TEST.value)
     ):
         return
     
     # overwrite files
     for filename, contents in filename_pat.findall(task_instance['full_output']):
         correct_filename = './' + filename.lstrip('/')
         correct_filename = os.path.abspath(correct_filename)
@@ -103,29 +104,33 @@
             log_suffix=data_dict.log_suffix,
         ) as tcm:
             # Attempt to set up environment with task instance
             if not tcm.reset_task_env(task_instance):
                 continue
 
             # Attempt to apply prediction
-            patch_type = "pred_try"
+            patch_type = PatchType.PATCH_PRED_TRY.value
             if not tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type) \
                 and task_instance[KEY_PREDICTION] is not None:
                 task_instance[KEY_PREDICTION] = extract_minimal_patch(task_instance[KEY_PREDICTION])
-                patch_type = "pred_minimal_try"
+                patch_type = PatchType.PATCH_PRED_MINIMAL_TRY.value
                 if not tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type):
                     continue
             tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type, revert=True)
-            patch_type = patch_type.replace("_try", "")
+
+            if patch_type == PatchType.PATCH_PRED_MINIMAL_TRY.value:
+                patch_type = PatchType.PATCH_PRED_MINIMAL.value
+            else:
+                patch_type = PatchType.PATCH_PRED.value
 
             # Run installation + testing script
             if (
                 not tcm.run_install_task(task_instance)
-                or not tcm.apply_patch(task_instance["test_patch"], patch_type="test")
                 or not tcm.apply_patch(task_instance[KEY_PREDICTION], patch_type=patch_type)
+                or not tcm.apply_patch(task_instance["test_patch"], patch_type=PatchType.PATCH_TEST.value)
                 or not tcm.run_tests_task(task_instance)
             ):
                 continue
 
 
 def main(args):
     """
```

### Comparing `swebench-1.0.9/swebench/harness/engine_validation.py` & `swebench-1.1.0/swebench/harness/engine_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import argparse, os
 
 from multiprocessing import Pool, cpu_count
+from swebench.harness.constants import PatchType
 from swebench.harness.context_manager import TaskEnvContextManager, TestbedContextManager
 from swebench.harness.utils import get_instances, split_instances, DotDict
 
 
 SKIP_INSTANCES = {"pytest-dev/pytest": ["6387", "7956", "3805"]}
 
 
@@ -59,17 +60,17 @@
                 and task_instance["pull_number"]
                 in SKIP_INSTANCES[task_instance["repo"]]
             ):
                 continue
             if (
                 not tcm.reset_task_env(task_instance)
                 or not tcm.run_install_task(task_instance)
-                or not tcm.apply_patch(task_instance["test_patch"], patch_type="test")
+                or not tcm.apply_patch(task_instance["test_patch"], patch_type=PatchType.PATCH_TEST.value)
                 or not tcm.run_tests_task(task_instance)
-                or not tcm.apply_patch(task_instance["patch"], patch_type="gold")
+                or not tcm.apply_patch(task_instance["patch"], patch_type=PatchType.PATCH_GOLD.value)
                 or not tcm.run_tests_task(task_instance)
             ):
                 continue
 
 
 def setup_testbed(data: dict):
     """
```

### Comparing `swebench-1.0.9/swebench/harness/run_evaluation.py` & `swebench-1.1.0/swebench/harness/run_evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 # Create model/repo/version specific testbed folder
                 testbed_model_name = model
                 if len(testbed_model_name) > 50:
                     # Hash model name for temp_dir path if too long
                     # Issue: https://github.com/conda/conda/issues/12250
                     testbed_model_name = deterministic_hash(testbed_model_name, 10)
                 testbed_model_repo_version_dir = os.path.join(
-                    testbed, testbed_model_name, repo, version)
+                    testbed, testbed_model_name, repo.rsplit('__', 1)[-1], version)
                 os.makedirs(testbed_model_repo_version_dir, exist_ok=True)
 
                 # Create predictions file for model/repo/version
                 file_name = f"{model}_{repo}_{version}_{predictions_path.split('/')[-1]}"
                 file_path = os.path.join(testbed_model_repo_version_dir, file_name)
                 if file_path.endswith(".jsonl"):
                     file_path = file_path[:-1]
```

### Comparing `swebench-1.0.9/swebench/harness/utils.py` & `swebench-1.1.0/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/metrics/conversion.py` & `swebench-1.1.0/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/metrics/getters.py` & `swebench-1.1.0/swebench/metrics/getters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,12 @@
 import re
 import json
 import os
 from datasets import load_from_disk, load_dataset
-
-from swebench.metrics.constants import (
-    APPLY_PATCH_FAIL,
-    APPLY_PATCH_PASS,
-    RESET_FAILED,
-    TESTS_ERROR,
-    TESTS_TIMEOUT,
-)
-from swebench.harness.constants import KEY_INSTANCE_ID
+from swebench.harness.constants import APPLY_PATCH_PASS, KEY_INSTANCE_ID
 from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER, TestStatus
 from typing import Tuple
 
 
 def get_diffs(sm_1: dict, sm_2: dict) -> dict:
     """
     Get differences between two test status maps
@@ -48,15 +40,21 @@
         dict: status map
     """
     repo = get_repo_from_lp(log_fp)
     log_parser = MAP_REPO_TO_PARSER[repo]
 
     with open(log_fp) as f:
         content = f.read()
-        if any([x in content for x in [APPLY_PATCH_FAIL, RESET_FAILED, TESTS_ERROR, TESTS_TIMEOUT, "Failed to reset task environment"]]) or APPLY_PATCH_PASS not in content:
+        if any([
+            x not in content for x in [
+                f"{APPLY_PATCH_PASS} (test)",
+                f"{APPLY_PATCH_PASS} (pred)",
+            ]
+
+        ]):
             # Eval patch was not applied successfully
             return {}, False
 
         # Get status map of evaluation results
         content = content.split(f"{APPLY_PATCH_PASS} (pred)")[-1]
         return log_parser(content), True
```

### Comparing `swebench-1.0.9/swebench/metrics/log_parsers.py` & `swebench-1.1.0/swebench/metrics/log_parsers.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/metrics/metrics.py` & `swebench-1.1.0/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/metrics/monitor.py` & `swebench-1.1.0/swebench/metrics/monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import glob
 import os
 
-from swebench.metrics.constants import (
+from swebench.harness.constants import (
     APPLY_PATCH_FAIL,
     APPLY_PATCH_PASS,
-    TESTS_TIMEOUT
+    TESTS_TIMEOUT,
 )
 from swebench.metrics.getters import (
     log_path_to_sms,
     get_diffs,
     get_repo_from_lp,
 )
 from swebench.metrics.log_parsers import MAP_REPO_TO_PARSER
```

### Comparing `swebench-1.0.9/swebench/metrics/report.py` & `swebench-1.1.0/swebench/metrics/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import glob, json, os
 
 from collections import Counter
 from swebench.harness.constants import (
+    APPLY_PATCH_FAIL,
     INSTALL_FAIL,
     KEY_INSTANCE_ID,
+    RESET_FAILED,
+    TESTS_ERROR,
+    TESTS_TIMEOUT,
+    PatchType,
 )
 from swebench.metrics.constants import (
     FAIL_TO_FAIL,
     FAIL_TO_PASS,
     PASS_TO_FAIL,
     PASS_TO_PASS,
 )
@@ -23,14 +28,15 @@
     compute_fail_to_pass_unweighted,
     compute_fail_to_pass_weighted,
     compute_pass_to_pass_unweighted,
     compute_pass_to_pass_weighted,
     get_resolution_status,
     ResolvedStatus,
 )
+from tqdm.auto import tqdm
 from typing import Tuple
 
 
 ### MARK - Eval Report Generation
 
 
 def get_eval_report(
@@ -259,77 +265,113 @@
             },
         }
 
     return summary
 
 
 def get_model_report(
-    model: str, predictions_path: str, swe_bench_tasks: str, log_dir: str
+    model: str,
+    predictions_path: str,
+    swe_bench_tasks: str,
+    log_dir: str,
+    verbose: bool = False,
 ) -> dict:
     """
     Generate a report of model evaluation results from predictions, task instances,
     and evaluation logs.
 
     Args:
         model (str): model name
         predictions_path (str): path to predictions file
         swe_bench_tasks (str): path to eval references (swe-bench-eval-refs.json)
         log_dir (str): path to directory of evaluation logs
+        verbose (bool): show tqdm to track progress
     Returns:
         report_map (dict): map of repo to report
     """
     eval_refs = get_eval_refs(swe_bench_tasks)
     for k, v in eval_refs.items():
         eval_refs[k] = {key: v[key] for key in [KEY_INSTANCE_ID, FAIL_TO_PASS, PASS_TO_PASS]}
 
     # Get predictions
     predictions = []
     if predictions_path.endswith("jsonl"):
         with open(predictions_path) as f:
             for line in f.readlines():
                 predictions.append(json.loads(line))
-    else:
+    elif predictions_path.endswith("json"):
         predictions = json.load(open(predictions_path))
+    else:
+        raise ValueError("Predictions file must be in json or jsonl format")
     report_map = {}
 
     # Iterate through predictions
-    for p in predictions:
-        repo = p[KEY_INSTANCE_ID].split(".")[0].rsplit("-", 1)[0].replace("__", "/")
-        if repo not in report_map:
-            report_map[repo] = {
-                "none": [],
-                "generated": [],
-                "with_logs": [],
-                "install_fail": [],
-                "applied": [],
-                "resolved": [],
-            }
-
+    report_map = {
+        "no_generation": [],
+        "generated": [],
+        "with_logs": [],
+        "install_fail": [],
+        "reset_failed": [],
+        "no_apply": [],
+        "applied": [],
+        "test_errored": [],
+        "test_timeout": [],
+        "resolved": [],
+    }
+    for p in tqdm(predictions, desc="Processing predictions", disable=not verbose):
         # Check if the model patch exists
-        if p["model_patch"] == None:
-            report_map[repo]["none"].append(p[KEY_INSTANCE_ID])
+        if p["model_patch"] == None or len(p["model_patch"].strip()) == 0:
+            report_map["no_generation"].append(p[KEY_INSTANCE_ID])
             continue
-        report_map[repo]["generated"].append(p[KEY_INSTANCE_ID])
+        report_map["generated"].append(p[KEY_INSTANCE_ID])
 
         # Get log file
         log_path = os.path.join(log_dir, f"{p[KEY_INSTANCE_ID]}.{model}.eval.log")
         if not os.path.exists(log_path):
             continue
-        report_map[repo]["with_logs"].append(p[KEY_INSTANCE_ID])
+        report_map["with_logs"].append(p[KEY_INSTANCE_ID])
+        log_content = open(log_path).read()
+
+        # Check if there is an apply patch failure
+        if any([
+            f"{APPLY_PATCH_FAIL}; ({patch_type})" in log_content
+            for patch_type in [
+                PatchType.PATCH_PRED_TRY.value,
+                PatchType.PATCH_PRED_MINIMAL_TRY.value
+            ]
+        ]):
+            report_map["no_apply"].append(p[KEY_INSTANCE_ID])
+            continue
 
-        # Check if install succeeded
-        if INSTALL_FAIL in open(log_path).read():
-            report_map[repo]["install_fail"].append(p[KEY_INSTANCE_ID])
+        # Check if there is an installation failure
+        if INSTALL_FAIL in log_content:
+            report_map["install_fail"].append(p[KEY_INSTANCE_ID])
+            continue
+
+        # Check if there is a reset failure
+        if RESET_FAILED in log_content:
+            report_map["reset_failed"].append(p[KEY_INSTANCE_ID])
             continue
 
         # Get evaluation logs
         eval_sm, found = get_logs_eval(log_path)
 
+        # Check if any tests errored or timed out
+        for status in [
+            ("test_errored", TESTS_ERROR),
+            ("test_timeout", TESTS_TIMEOUT),
+        ]:
+            if status[1] in log_content:
+                report_map[status[0]].append(p[KEY_INSTANCE_ID])
+                continue
+
+        # Check if patch failed to apply
         if not found:
             continue
-        report_map[repo]["applied"].append(p[KEY_INSTANCE_ID])
+        report_map["applied"].append(p[KEY_INSTANCE_ID])
 
+        # Check if the patch was resolved
         report = get_eval_report(eval_sm, eval_refs[p[KEY_INSTANCE_ID]])
         if get_resolution_status(report) == ResolvedStatus.FULL.value:
-            report_map[repo]["resolved"].append(p[KEY_INSTANCE_ID])
+            report_map["resolved"].append(p[KEY_INSTANCE_ID])
 
     return report_map
```

### Comparing `swebench-1.0.9/swebench/versioning/constants.py` & `swebench-1.1.0/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/versioning/get_versions.py` & `swebench-1.1.0/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench/versioning/utils.py` & `swebench-1.1.0/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.9/swebench.egg-info/PKG-INFO` & `swebench-1.1.0/swebench.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.9
+Version: 1.1.0
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
@@ -22,14 +22,15 @@
 Requires-Dist: chardet
 Requires-Dist: datasets
 Requires-Dist: ghapi
 Requires-Dist: GitPython
 Requires-Dist: python-dotenv
 Requires-Dist: requests
 Requires-Dist: rich
+Requires-Dist: tqdm
 
 <p align="center">
   <a href="https://github.com/princeton-nlp/Llamao">
     <img src="assets/swellama_banner.png" width="50%" alt="Kawi the SWE-Llama" />
   </a>
 </p>
 
@@ -54,14 +55,19 @@
     <a href="https://badge.fury.io/py/swebench">
         <img src="https://badge.fury.io/py/swebench.svg">
     </a>
 </p>
 
 Please refer our [website](http://swe-bench.github.io) for the public leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench benchmark.
 
+## 📰 News
+* **[Apr. 15, 2024]**: SWE-bench has gone through major improvements to resolve issues with the evaluation harness. Read more in our [report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/20240405_eval_bug/README.md).
+* **[Apr. 2, 2024]**: We have released [SWE-agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-the-art on the full SWE-bench test set! ([Tweet 🔗](https://twitter.com/jyangballin/status/1775114444370051582))
+* **[Jan. 16, 2024]**: SWE-bench has been accepted to ICLR 2024 as an oral presentation! ([OpenReview 🔗](https://openreview.net/forum?id=VTF8yNQM66))
+
 ## 👋 Overview
 SWE-bench is a benchmark for evaluating large language models on real world software issues collected from GitHub.
 Given a *codebase* and an *issue*, a language model is tasked with generating a *patch* that resolves the described problem.
 
 <img src="assets/teaser.png">
 
 ## 🚀 Set Up
```

#### html2text {}

```diff
@@ -1,41 +1,49 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.9 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.1.0 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: beautifulsoup4 Requires-Dist: chardet Requires-Dist:
 datasets Requires-Dist: ghapi Requires-Dist: GitPython Requires-Dist: python-
-dotenv Requires-Dist: requests Requires-Dist: rich
+dotenv Requires-Dist: requests Requires-Dist: rich Requires-Dist: tqdm
                              _[_K_a_w_i_ _t_h_e_ _S_W_E_-_L_l_a_m_a_]
 | [æ¥æ¬èª](docs/README_JP.md) | [English](https://github.com/princeton-nlp/
      SWE-bench) | [ä¸­æç®ä½](docs/README_CN.md) | [ä¸­æç¹é«](docs/
                                 README_TW.md) |
 ---
  Code and data for our ICLR 2024 paper _S_W_E_-_b_e_n_c_h_:_ _C_a_n_ _L_a_n_g_u_a_g_e_ _M_o_d_e_l_s_ _R_e_s_o_l_v_e
       _R_e_a_l_-_W_o_r_l_d_ _G_i_t_H_u_b_ _I_s_s_u_e_s_?_[_B_u_i_l_d_]_[_L_i_c_e_n_s_e_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/
                                  _s_w_e_b_e_n_c_h_._s_v_g_]
 Please refer our [website](http://swe-bench.github.io) for the public
 leaderboard and the [change log](https://github.com/princeton-nlp/SWE-bench/
 blob/main/CHANGELOG.md) for information on the latest updates to the SWE-bench
-benchmark. ## ð Overview SWE-bench is a benchmark for evaluating large
-language models on real world software issues collected from GitHub. Given a
-*codebase* and an *issue*, a language model is tasked with generating a *patch*
-that resolves the described problem. [assets/teaser.png]## ð Set Up To build
-SWE-bench from source, follow these steps: 1. Clone this repository locally 2.
-`cd` into the repository. 3. Run `conda env create -f environment.yml` to
-created a conda environment named `swe-bench` 4. Activate the environment with
-`conda activate swe-bench` ## ð½ Usage You can download the SWE-bench dataset
-directly ([dev](https://drive.google.com/
+benchmark. ## ð° News * **[Apr. 15, 2024]**: SWE-bench has gone through major
+improvements to resolve issues with the evaluation harness. Read more in our
+[report](https://github.com/princeton-nlp/SWE-bench/blob/main/docs/
+20240405_eval_bug/README.md). * **[Apr. 2, 2024]**: We have released [SWE-
+agent](https://github.com/princeton-nlp/SWE-agent), which sets the state-of-
+the-art on the full SWE-bench test set! ([Tweet ð](https://twitter.com/
+jyangballin/status/1775114444370051582)) * **[Jan. 16, 2024]**: SWE-bench has
+been accepted to ICLR 2024 as an oral presentation! ([OpenReview ð](https://
+openreview.net/forum?id=VTF8yNQM66)) ## ð Overview SWE-bench is a benchmark
+for evaluating large language models on real world software issues collected
+from GitHub. Given a *codebase* and an *issue*, a language model is tasked with
+generating a *patch* that resolves the described problem. [assets/teaser.png]##
+ð Set Up To build SWE-bench from source, follow these steps: 1. Clone this
+repository locally 2. `cd` into the repository. 3. Run `conda env create -
+f environment.yml` to created a conda environment named `swe-bench` 4. Activate
+the environment with `conda activate swe-bench` ## ð½ Usage You can download
+the SWE-bench dataset directly ([dev](https://drive.google.com/
 uc?export=download&id=1SbOxHiR0eXlq2azPSSOIDZz-Hva0ETpX), [test](https://
 drive.google.com/uc?export=download&id=164g55i3_B78F6EphCZGtgSrd2GneFyRM) sets)
 or from [HuggingFace](https://huggingface.co/datasets/princeton-nlp/SWE-bench).
 To use SWE-Bench, you can: * Train your own models on our pre-processed
 datasets * Run [inference](https://github.com/princeton-nlp/SWE-bench/blob/
 main/inference/) on existing models (either models you have on-disk like LLaMA,
 or models you have access to through an API like GPT-4). The inference step is
```

### Comparing `swebench-1.0.9/swebench.egg-info/SOURCES.txt` & `swebench-1.1.0/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

