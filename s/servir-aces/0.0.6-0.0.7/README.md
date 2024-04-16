# Comparing `tmp/servir-aces-0.0.6.tar.gz` & `tmp/servir_aces-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servir-aces-0.0.6.tar", last modified: Mon Apr  1 22:21:51 2024, max compression
+gzip compressed data, was "servir_aces-0.0.7.tar", last modified: Tue Apr 16 15:28:27 2024, max compression
```

## Comparing `servir-aces-0.0.6.tar` & `servir_aces-0.0.7.tar`

### file list

```diff
@@ -1,74 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.585326 servir-aces-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.589326 servir-aces-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.589326 servir-aces-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-01 22:21:41.000000 servir-aces-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-01 22:21:41.000000 servir-aces-0.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-01 22:21:41.000000 servir-aces-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-01 22:21:41.000000 servir-aces-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-01 22:21:51.597325 servir-aces-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-01 22:21:41.000000 servir-aces-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.593325 servir-aces-0.0.6/aces/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/ee_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    20236 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/model_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/remote_sensing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-01 22:21:41.000000 servir-aces-0.0.6/aces/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.593325 servir-aces-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/data_processor.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/ee_utils.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/model_builder.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/model_trainer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.593325 servir-aces-0.0.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/remote_sensing.md
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-01 22:21:41.000000 servir-aces-0.0.6/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:41.000000 servir-aces-0.0.6/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-01 22:21:41.000000 servir-aces-0.0.6/examples/count_sample_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-01 22:21:41.000000 servir-aces-0.0.6/examples/run_model_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-01 22:21:41.000000 servir-aces-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 22:21:41.000000 servir-aces-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:21:41.000000 servir-aces-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-01 22:21:41.000000 servir-aces-0.0.6/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/servir_aces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-01 22:21:51.000000 servir-aces-0.0.6/servir_aces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-01 22:21:51.000000 servir-aces-0.0.6/servir_aces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:21:51.000000 servir-aces-0.0.6/servir_aces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 22:21:51.000000 servir-aces-0.0.6/servir_aces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-01 22:21:51.000000 servir-aces-0.0.6/servir_aces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:21:51.597325 servir-aces-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 22:21:41.000000 servir-aces-0.0.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.589326 servir-aces-0.0.6/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/workflow/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v1/1.s1_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:21:51.597325 servir-aces-0.0.6/workflow/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/1.planet_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/2.generate_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/4.export_image_for_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/5.prediction_dnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/5.prediction_unet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/generate_training_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-01 22:21:41.000000 servir-aces-0.0.6/workflow/v2/host_vertex_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.974435 servir_aces-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.978435 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.978435 servir_aces-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-16 15:28:17.000000 servir_aces-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-16 15:28:17.000000 servir_aces-0.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-16 15:28:17.000000 servir_aces-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 15:28:17.000000 servir_aces-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:28:27.990435 servir_aces-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:28:17.000000 servir_aces-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/aces/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25100 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/ee_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19558 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20238 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/model_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/remote_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-16 15:28:17.000000 servir_aces-0.0.7/aces/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/data_processor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/ee_utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/model_builder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/model_trainer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/remote_sensing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 15:28:17.000000 servir_aces-0.0.7/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.982435 servir_aces-0.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/count_sample_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-16 15:28:17.000000 servir_aces-0.0.7/examples/run_model_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-16 15:28:17.000000 servir_aces-0.0.7/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)  2316819 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/aces_rice_classification_paro_2021.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    57598 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/count_sample_size.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    61100 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/prediction_dnn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    81476 2024-04-16 15:28:17.000000 servir_aces-0.0.7/notebook/prediction_unet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-16 15:28:17.000000 servir_aces-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:17.000000 servir_aces-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 15:28:17.000000 servir_aces-0.0.7/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/servir_aces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-16 15:28:27.000000 servir_aces-0.0.7/servir_aces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:28:27.990435 servir_aces-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-16 15:28:17.000000 servir_aces-0.0.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.974435 servir_aces-0.0.7/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.986435 servir_aces-0.0.7/workflow/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v1/1.s1_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:27.990435 servir_aces-0.0.7/workflow/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/1.planet_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/2.generate_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/4.export_image_for_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/5.prediction_dnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/5.prediction_unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18247 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/generate_training_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-04-16 15:28:17.000000 servir_aces-0.0.7/workflow/v2/host_vertex_ai.py
```

### Comparing `servir-aces-0.0.6/.env.example` & `servir_aces-0.0.7/.env.example`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/.github/workflows/macos.yml` & `servir_aces-0.0.7/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/.github/workflows/pypi.yml` & `servir_aces-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/.github/workflows/ubuntu.yml` & `servir_aces-0.0.7/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/.github/workflows/windows.yml` & `servir_aces-0.0.7/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/.gitignore` & `servir_aces-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/CODE_OF_CONDUCT.md` & `servir_aces-0.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/LICENSE` & `servir_aces-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/PKG-INFO` & `servir_aces-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.6
+Version: 0.0.7
 Summary: Agricultural Classification and Estimation Service (ACES)
 Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -44,15 +44,16 @@
 Here's an example of how to use the ACES module:
 
 ```python
 from aces.config import Config
 from aces.model_trainer import ModelTrainer
 
 if __name__ == "__main__":
-    config = Config()
+    config_file = "config.env"
+    config = Config(config_file)
     trainer = ModelTrainer(config)
     trainer.train_model()
 ```
 
 ## Contributing
 Contributions to ACES are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
```

### Comparing `servir-aces-0.0.6/README.md` & `servir_aces-0.0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 Here's an example of how to use the ACES module:
 
 ```python
 from aces.config import Config
 from aces.model_trainer import ModelTrainer
 
 if __name__ == "__main__":
-    config = Config()
+    config_file = "config.env"
+    config = Config(config_file)
     trainer = ModelTrainer(config)
     trainer.train_model()
 ```
 
 ## Contributing
 Contributions to ACES are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
```

### Comparing `servir-aces-0.0.6/aces/config.py` & `servir_aces-0.0.7/aces/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,17 +91,23 @@
         # AI platform expects a need a serialized model, this parameter does this.
         # See its uses in `data_processor.py` and `model_training.py`
         USE_AI_PLATFORM (bool): Flag to use Google Cloud AI Platform.
         # Get machine type here: https://cloud.google.com/vertex-ai/docs/predictions/configure-compute
         GCP_MACHINE_TYPE (str): The Google Cloud Platform machine type.
     """
 
-    def __init__(self, config_file) -> None:
+    def __init__(self, config_file, override=False) -> None:
+        """
+        ACES Configuration Class Constructor
 
-        load_dotenv(config_file)
+        Args:
+            config_file (str): The path to the configuration file.
+            override (bool): Flag to override the configuration settings.
+        """
+        load_dotenv(config_file, override=override)
 
         self.BASEDIR = Path(os.getenv("BASEDIR"))
         _DATADIR = os.getenv("DATADIR")
         if _DATADIR.startswith("gs://"):
             self.DATADIR = _DATADIR
             self.TRAINING_DIR = f"{self.DATADIR}/training"
             self.TESTING_DIR = f"{self.DATADIR}/testing"
```

### Comparing `servir-aces-0.0.6/aces/data_processor.py` & `servir_aces-0.0.7/aces/data_processor.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/aces/ee_utils.py` & `servir_aces-0.0.7/aces/ee_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,31 +32,43 @@
         """
         import json
         service_account = json.load(open(key))
         credentials = ee.ServiceAccountCredentials(service_account["client_email"], key)
         return credentials
 
     @staticmethod
-    def initialize_session(use_highvolume : bool = False, key : Union[str, None] = None):
+    def initialize_session(use_highvolume : bool = False, key : Union[str, None] = None, project: str = None):
         """
         Initialize the Earth Engine session.
+        If use_highvolume is True, the high-volume Earth Engine API will be used.
+        If a project is provided, the session will be initialized with the project ID. Recommended to use project.
+        If a key is provided, the service account key will be used.
 
         Parameters:
         use_highvolume (bool): Whether to use the high-volume Earth Engine API.
         key (str or None): The path to the service account key JSON file. If None, the default credentials will be used.
+        project (str): The Google Cloud project ID to use for the session.
         """
         if key is None:
-            if use_highvolume:
+            if use_highvolume and project:
+                ee.Initialize(opt_url="https://earthengine-highvolume.googleapis.com", project=project)
+            elif use_highvolume:
                 ee.Initialize(opt_url="https://earthengine-highvolume.googleapis.com")
+            elif project:
+                ee.Initialize(project=project)
             else:
                 ee.Initialize()
         else:
             credentials = EEUtils.get_credentials_by_service_account_key(key)
-            if use_highvolume:
+            if use_highvolume and project:
+                ee.Initialize(credentials, opt_url="https://earthengine-highvolume.googleapis.com", project=project)
+            elif use_highvolume:
                 ee.Initialize(credentials, opt_url="https://earthengine-highvolume.googleapis.com")
+            elif project:
+                ee.Initialize(credentials, project=project)
             else:
                 ee.Initialize(credentials)
 
     @staticmethod
     def calculate_avg_min_max_statistics(image: ee.Image, geometry: ee.FeatureCollection, scale: int = 30) -> ee.Dictionary:
         """
         Calculate min and max of an image over a specific region.
```

### Comparing `servir-aces-0.0.6/aces/metrics.py` & `servir_aces-0.0.7/aces/metrics.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/aces/model_builder.py` & `servir_aces-0.0.7/aces/model_builder.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/aces/model_trainer.py` & `servir_aces-0.0.7/aces/model_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,21 +361,23 @@
     def save_plots(self) -> None:
         """
         Save plots and model visualization.
 
         Saves the model architecture plot, training history plot, and model object.
         """
         print(f"Saving plots and model visualization at {self.config.MODEL_SAVE_DIR}...")
+
+        Utils.plot_metrics([key.replace("val_", "") for key in self.history.history.keys() if key.startswith("val_")],
+                           self.history.history, len(self.history.epoch), self.config.MODEL_SAVE_DIR)
+
         if self.config.USE_AI_PLATFORM:
             keras.utils.plot_model(self._model, f"{self.config.MODEL_SAVE_DIR}/model.png", show_shapes=True, rankdir="TB")
             keras.utils.plot_model(self.model, f"{self.config.MODEL_SAVE_DIR}/wrapped_model.png", show_shapes=True, rankdir="LR") # rankdir='TB'
         else:
             keras.utils.plot_model(self.model, f"{self.config.MODEL_SAVE_DIR}/model.png", show_shapes=True, rankdir="TB") # rankdir='TB'
-        Utils.plot_metrics([key.replace("val_", "") for key in self.history.history.keys() if key.startswith("val_")],
-                           self.history.history, len(self.history.epoch), self.config.MODEL_SAVE_DIR)
 
     def save_history_object(self) -> None:
         """
         Save the history object.
         """
         with open(f"{self.config.MODEL_SAVE_DIR}/model.pkl", "wb") as f:
             pickle.dump(self.history.history, f)
```

### Comparing `servir-aces-0.0.6/aces/refs.bib` & `servir_aces-0.0.7/aces/refs.bib`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/aces/remote_sensing.py` & `servir_aces-0.0.7/aces/remote_sensing.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/aces/utils.py` & `servir_aces-0.0.7/aces/utils.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/docs/contributing.md` & `servir_aces-0.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/docs/index.md` & `servir_aces-0.0.7/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # ACES (Agricultural Classification and Estimation Service)
 
+[![image](https://img.shields.io/pypi/v/servir-aces.svg)](https://pypi.python.org/pypi/servir-aces)
+
 ACES (Agricultural Classification and Estimation Service) is a Python module for generating training data and training machine learning models for remote sensing applications. It provides functionalities for data processing, data loading from Earth Engine, feature extraction, and model training.
 
 ## Features
 
 - Data loading and processing from Earth Engine.
 - Generation of training data for machine learning models.
 - Training and evaluation of machine learning models (DNN, CNN, UNET).
 - Support for remote sensing feature extraction.
 - Integration with Apache Beam for data processing.
 
 
 ## Usage
-Define all your configuration in `.env` file. An example of the file is provided as `.env.example`.
+Define all your configuration in `.env` file. An example of the file is provided as [`.env.example`](https://github.com/SERVIR/servir-aces/blob/main/.env.example) file.
 
 Here's an example of how to use the ACES module:
 
 ```python
 from aces.config import Config
 from aces.model_trainer import ModelTrainer
 
 if __name__ == "__main__":
-    config = Config()
+    config_file = "config.env"
+    config = Config(config_file)
     trainer = ModelTrainer(config)
     trainer.train_model()
 ```
 
 ## Contributing
 Contributions to ACES are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
-This project is licensed under the GPL-3 License - see the LICENSE file for details.
+This project is licensed under the [GNU General Public License v3.0](https://github.com/SERVIR/servir-aces/blob/main/LICENSE).
```

### Comparing `servir-aces-0.0.6/examples/count_sample_size.py` & `servir_aces-0.0.7/examples/count_sample_size.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/examples/run_model_example.py` & `servir_aces-0.0.7/examples/run_model_example.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/mkdocs.yml` & `servir_aces-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/pyproject.toml` & `servir_aces-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "servir-aces"
-version = "0.0.6"
+version = "0.0.7"
 dynamic = [
     "dependencies",
 ]
 description = "Agricultural Classification and Estimation Service (ACES)"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
@@ -37,15 +37,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.6"
+current_version = "0.0.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `servir-aces-0.0.6/servir_aces.egg-info/PKG-INFO` & `servir_aces-0.0.7/servir_aces.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servir-aces
-Version: 0.0.6
+Version: 0.0.7
 Summary: Agricultural Classification and Estimation Service (ACES)
 Author-email: Biplov Bhandari <bionicbiplov45@gmail.com>
 License: GNU General Public License v3.0
 Project-URL: Homepage, https://github.com/SERVIR/servir-aces
 Keywords: remote sensing,agriculture,machine learning,deep learning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -44,15 +44,16 @@
 Here's an example of how to use the ACES module:
 
 ```python
 from aces.config import Config
 from aces.model_trainer import ModelTrainer
 
 if __name__ == "__main__":
-    config = Config()
+    config_file = "config.env"
+    config = Config(config_file)
     trainer = ModelTrainer(config)
     trainer.train_model()
 ```
 
 ## Contributing
 Contributions to ACES are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.
```

### Comparing `servir-aces-0.0.6/servir_aces.egg-info/SOURCES.txt` & `servir_aces-0.0.7/servir_aces.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mkdocs.yml
 pyproject.toml
 requirements.txt
 requirements_dev.txt
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/docs.yml
 .github/workflows/macos.yml
 .github/workflows/pypi.yml
 .github/workflows/ubuntu.yml
 .github/workflows/windows.yml
 aces/__init__.py
 aces/config.py
 aces/data_processor.py
@@ -22,29 +23,35 @@
 aces/metrics.py
 aces/model_builder.py
 aces/model_trainer.py
 aces/refs.bib
 aces/remote_sensing.py
 aces/utils.py
 docs/changelog.md
+docs/config.md
 docs/contributing.md
 docs/data_processor.md
 docs/ee_utils.md
 docs/faq.md
 docs/index.md
 docs/installation.md
 docs/metrics.md
 docs/model_builder.md
 docs/model_trainer.md
 docs/remote_sensing.md
 docs/usage.md
+docs/utils.md
 docs/overrides/main.html
 examples/__init__.py
 examples/count_sample_size.py
 examples/run_model_example.py
+notebook/aces_rice_classification_paro_2021.ipynb
+notebook/count_sample_size.ipynb
+notebook/prediction_dnn.ipynb
+notebook/prediction_unet.ipynb
 servir_aces.egg-info/PKG-INFO
 servir_aces.egg-info/SOURCES.txt
 servir_aces.egg-info/dependency_links.txt
 servir_aces.egg-info/requires.txt
 servir_aces.egg-info/top_level.txt
 tests/__init__.py
 workflow/v1/1.s1_preprocess.py
```

### Comparing `servir-aces-0.0.6/workflow/v1/1.s1_preprocess.py` & `servir_aces-0.0.7/workflow/v1/1.s1_preprocess.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/1.planet_composites.py` & `servir_aces-0.0.7/workflow/v2/1.planet_composites.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/2.generate_samples.py` & `servir_aces-0.0.7/workflow/v2/2.generate_samples.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/4.export_image_for_prediction.py` & `servir_aces-0.0.7/workflow/v2/4.export_image_for_prediction.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,55 +74,58 @@
 composite_before = composite_before.select(bands)
 composite_during = composite_during.select(bands)
 
 composite_before = composite_before.regexpRename("$(.*)", "_before")
 composite_during = composite_during.regexpRename("$(.*)", "_during")
 image = composite_before.addBands(composite_during).toFloat()
 
-if Config.USE_ELEVATION:
+config_file = "config.env"
+config = Config(config_file)
+
+if config.USE_ELEVATION:
     elevation = ee.Image("projects/servir-sco-assets/assets/Bhutan/ACES_2/elevationParo")
     slope = ee.Image("projects/servir-sco-assets/assets/Bhutan/ACES_2/slopeParo")
     image = image.addBands(elevation).addBands(slope).toFloat()
-    Config.FEATURES.extend(["elevation", "slope"])
+    config.FEATURES.extend(["elevation", "slope"])
 
 
-if Config.USE_S1:
+if config.USE_S1:
     sentinel1_asc_before_composite = ee.Image("projects/servir-sco-assets/assets/Bhutan/Sentinel1Ascending2021/s1AscBefore")
     sentinel1_asc_during_composite = ee.Image("projects/servir-sco-assets/assets/Bhutan/Sentinel1Ascending2021/s1AscDuring")
     sentinel1_desc_before_composite = ee.Image("projects/servir-sco-assets/assets/Bhutan/Sentinel1Descending2021/s1DescBefore")
     sentinel1_desc_during_composite = ee.Image("projects/servir-sco-assets/assets/Bhutan/Sentinel1Descending2021/s1DescDuring")
 
     image = image.addBands(sentinel1_asc_before_composite).addBands(sentinel1_asc_during_composite).addBands(sentinel1_desc_before_composite).addBands(sentinel1_desc_during_composite).toFloat()
-    Config.FEATURES.extend(["vv_asc_before", "vh_asc_before", "vv_asc_during", "vh_asc_during",
+    config.FEATURES.extend(["vv_asc_before", "vh_asc_before", "vv_asc_during", "vh_asc_during",
                             "vv_desc_before", "vh_desc_before", "vv_desc_during", "vh_desc_during"])
 
 # dem = ee.Image("MERIT/DEM/v1_0_3") # ee.Image('USGS/SRTMGL1_003');
 # dem = dem.clip(fc_country)
 # riceZone = dem.gt(rice_zone[region]["min"]).And(dem.lte(rice_zone[region]["max"]))
 # image = image.clip(region_fc).updateMask(riceZone)
 
-image = image.select(Config.FEATURES)
+image = image.select(config.FEATURES)
 print("image", image.bandNames().getInfo())
 
 # Specify patch and file dimensions.
 formatOptions = {
-  "patchDimensions": [Config.PATCH_SHAPE_SINGLE, Config.PATCH_SHAPE_SINGLE],
+  "patchDimensions": [config.PATCH_SHAPE_SINGLE, config.PATCH_SHAPE_SINGLE],
   "maxFileSize": 104857600,
   "compressed": True
 }
 
-if Config.KERNEL_BUFFER:
-    formatOptions["kernelSize"] = Config.KERNEL_BUFFER
+if config.KERNEL_BUFFER:
+    formatOptions["kernelSize"] = config.KERNEL_BUFFER
 
 # Setup the task
 image_export_options = {
-    "description": Config.GCS_IMAGE_DIR.split("/")[-1],
-    "file_name_prefix": f"{Config.GCS_IMAGE_DIR}/{Config.GCS_IMAGE_PREFIX}",
-    "bucket": Config.GCS_BUCKET,
-    "scale": Config.SCALE,
+    "description": "export_task_for_prediction",
+    "file_name_prefix": f"{config.GCS_IMAGE_DIR}/{config.GCS_IMAGE_PREFIX}",
+    "bucket": config.GCS_BUCKET,
+    "scale": config.SCALE,
     "file_format": "TFRecord",
     "region": region_fc, # image.geometry(),
     "format_options": formatOptions,
     "max_pixels": 1e13,
 }
 
 print("image_export_options", image_export_options)
```

### Comparing `servir-aces-0.0.6/workflow/v2/5.prediction_dnn.py` & `servir_aces-0.0.7/workflow/v2/5.prediction_dnn.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/5.prediction_unet.py` & `servir_aces-0.0.7/workflow/v2/5.prediction_unet.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,29 +12,32 @@
 import json
 import os
 import tensorflow as tf
 import numpy as np
 import subprocess
 
 
-OUTPUT_IMAGE_FILE = str(Config.MODEL_DIR / "prediction" / f"{Config.OUTPUT_NAME}.TFRecord")
-if not os.path.exists(str(Config.MODEL_DIR / "prediction")): os.mkdir(str(Config.MODEL_DIR / "prediction"))
+config_file = "config.env"
+config = Config(config_file)
+
+OUTPUT_IMAGE_FILE = str(config.MODEL_DIR / "prediction" / f"{config.OUTPUT_NAME}.TFRecord")
+if not os.path.exists(str(config.MODEL_DIR / "prediction")): os.mkdir(str(config.MODEL_DIR / "prediction"))
 print(f"OUTPUT_IMAGE_FILE: {OUTPUT_IMAGE_FILE}")
 
-OUTPUT_GCS_PATH = f"gs://{Config.GCS_BUCKET}/prediction/{Config.OUTPUT_NAME}.TFRecord"
+OUTPUT_GCS_PATH = f"gs://{config.GCS_BUCKET}/prediction/{config.OUTPUT_NAME}.TFRecord"
 print(f"OUTPUT_GCS_PATH: {OUTPUT_GCS_PATH}")
 
-ls = f"sudo gsutil ls gs://{Config.GCS_BUCKET}/{Config.GCS_IMAGE_DIR}/"
+ls = f"sudo gsutil ls gs://{config.GCS_BUCKET}/{config.GCS_IMAGE_DIR}/"
 print(f"ls >> : {ls}")
 files_list = subprocess.check_output(ls, shell=True)
 files_list = files_list.decode("utf-8")
 files_list = files_list.split("\n")
 
 # Get only the files generated by the image export.
-exported_files_list = [s for s in files_list if Config.GCS_IMAGE_PREFIX in s]
+exported_files_list = [s for s in files_list if config.GCS_IMAGE_PREFIX in s]
 
 print(f"exported_files_list: {exported_files_list}")
 
 # Get the list of image files and the JSON mixer file.
 image_files_list = []
 json_file = None
 for f in exported_files_list:
@@ -47,19 +50,19 @@
 image_files_list.sort()
 
 print(f"image_files_list: {image_files_list}")
 
 print(f"json_file: {json_file}")
 
 if Config.USE_BEST_MODEL_FOR_INFERENCE:
-    print(f"Using best model for inference.\nLoading model from {str(Config.MODEL_DIR)}/{Config.MODEL_CHECKPOINT_NAME}.tf")
-    this_model = tf.keras.models.load_model(f"{str(Config.MODEL_DIR)}/{Config.MODEL_CHECKPOINT_NAME}.tf")
+    print(f"Using best model for inference.\nLoading model from {str(config.MODEL_DIR)}/{config.MODEL_CHECKPOINT_NAME}.tf")
+    this_model = tf.keras.models.load_model(f"{str(config.MODEL_DIR)}/{config.MODEL_CHECKPOINT_NAME}.tf")
 else:
-    print(f"Using last model for inference.\nLoading model from {str(Config.MODEL_DIR)}/trained-model")
-    this_model = tf.keras.models.load_model(f"{str(Config.MODEL_DIR)}/trained-model")
+    print(f"Using last model for inference.\nLoading model from {str(config.MODEL_DIR)}/trained-model")
+    this_model = tf.keras.models.load_model(f"{str(config.MODEL_DIR)}/trained-model")
 
 print(this_model.summary())
 
 
 cat = f"gsutil cat {json_file}"
 read_t = subprocess.check_output(cat, shell=True)
 read_t = read_t.decode("utf-8")
@@ -70,48 +73,48 @@
 # Get relevant info from the JSON mixer file.
 patch_width = mixer["patchDimensions"][0]
 patch_height = mixer["patchDimensions"][1]
 patches = mixer["totalPatches"]
 patch_dimensions_flat = [patch_width * patch_height, 1]
 
 # Get set up for prediction.
-if Config.KERNEL_BUFFER:
-    x_buffer = Config.KERNEL_BUFFER[0] // 2
-    y_buffer = Config.KERNEL_BUFFER[1] // 2
+if config.KERNEL_BUFFER:
+    x_buffer = config.KERNEL_BUFFER[0] // 2
+    y_buffer = config.KERNEL_BUFFER[1] // 2
 
     buffered_shape = [
-        Config.PATCH_SHAPE[0] + Config.KERNEL_BUFFER[0],
-        Config.PATCH_SHAPE[1] + Config.KERNEL_BUFFER[1],
+        config.PATCH_SHAPE[0] + config.KERNEL_BUFFER[0],
+        config.PATCH_SHAPE[1] + config.KERNEL_BUFFER[1],
     ]
 else:
     x_buffer = 0
     y_buffer = 0
-    buffered_shape = Config.PATCH_SHAPE
+    buffered_shape = config.PATCH_SHAPE
 
-if Config.USE_ELEVATION:
-    Config.FEATURES.extend(["elevation", "slope"])
+if config.USE_ELEVATION:
+    config.FEATURES.extend(["elevation", "slope"])
 
 
-if Config.USE_S1:
-    Config.FEATURES.extend(["vv_asc_before", "vh_asc_before", "vv_asc_during", "vh_asc_during",
+if config.USE_S1:
+    config.FEATURES.extend(["vv_asc_before", "vh_asc_before", "vv_asc_during", "vh_asc_during",
                             "vv_desc_before", "vh_desc_before", "vv_desc_during", "vh_desc_during"])
 
-print(f"Config.FEATURES: {Config.FEATURES}")
+print(f"Config.FEATURES: {config.FEATURES}")
 
 image_columns = [
-    tf.io.FixedLenFeature(shape=buffered_shape, dtype=tf.float32) for k in Config.FEATURES
+    tf.io.FixedLenFeature(shape=buffered_shape, dtype=tf.float32) for k in config.FEATURES
 ]
 
-image_features_dict = dict(zip(Config.FEATURES, image_columns))
+image_features_dict = dict(zip(config.FEATURES, image_columns))
 
 def parse_image(example_proto):
     return tf.io.parse_single_example(example_proto, image_features_dict)
 
 def toTupleImage(inputs):
-    inputsList = [inputs.get(key) for key in Config.FEATURES]
+    inputsList = [inputs.get(key) for key in config.FEATURES]
     stacked = tf.stack(inputsList, axis=0)
     stacked = tf.transpose(stacked, [1, 2, 0])
     return stacked
 
 # Create a dataset from the TFRecord file(s) in Cloud Storage.
 image_dataset = tf.data.TFRecordDataset(image_files_list, compression_type="GZIP")
 image_dataset = image_dataset.map(parse_image, num_parallel_calls=5)
@@ -135,16 +138,16 @@
         print(f"Starting with patch {i}...")
         print(f"predictionPatch: {prediction_patch.shape}")
 
     if i % 50 == 0:
         print(f"Writing patch {i}...")
 
     prediction_patch = prediction_patch[
-        x_buffer: x_buffer+Config.PATCH_SHAPE[0],
-        y_buffer: y_buffer+Config.PATCH_SHAPE[1]
+        x_buffer: x_buffer+config.PATCH_SHAPE[0],
+        y_buffer: y_buffer+config.PATCH_SHAPE[1]
     ]
 
     example = tf.train.Example(
         features=tf.train.Features(
             feature={
             "prediction": tf.train.Feature(
                 int64_list=tf.train.Int64List(
@@ -177,10 +180,10 @@
 
 # upload to gcp
 upload_to_gcp = f"sudo gsutil cp {OUTPUT_IMAGE_FILE} {OUTPUT_GCS_PATH}"
 result = subprocess.check_output(upload_to_gcp, shell=True)
 print(f"uploading classified image to earth engine: {result}")
 
 # upload to earth engine asset
-upload_image = f"earthengine upload image --asset_id={Config.EE_OUTPUT_ASSET}/{Config.OUTPUT_NAME} --pyramiding_policy=mode {OUTPUT_GCS_PATH} {json_file}"
+upload_image = f"earthengine upload image --asset_id={config.EE_OUTPUT_ASSET}/{config.OUTPUT_NAME} --pyramiding_policy=mode {OUTPUT_GCS_PATH} {json_file}"
 result = subprocess.check_output(upload_image, shell=True)
 print(f"uploading classified image to earth engine: {result}")
```

### Comparing `servir-aces-0.0.6/workflow/v2/README.md` & `servir_aces-0.0.7/workflow/v2/README.md`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/generate_training_patches.py` & `servir_aces-0.0.7/workflow/v2/generate_training_patches.py`

 * *Files identical despite different names*

### Comparing `servir-aces-0.0.6/workflow/v2/host_vertex_ai.py` & `servir_aces-0.0.7/workflow/v2/host_vertex_ai.py`

 * *Files identical despite different names*

