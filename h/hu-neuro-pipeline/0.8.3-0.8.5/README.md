# Comparing `tmp/hu-neuro-pipeline-0.8.3.tar.gz` & `tmp/hu_neuro_pipeline-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hu-neuro-pipeline-0.8.3.tar", last modified: Sat Dec  9 12:37:10 2023, max compression
+gzip compressed data, was "hu_neuro_pipeline-0.8.5.tar", last modified: Tue Apr 16 11:55:07 2024, max compression
```

## Comparing `hu-neuro-pipeline-0.8.3.tar` & `hu_neuro_pipeline-0.8.5.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.722662 hu-neuro-pipeline-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.710662 hu-neuro-pipeline-0.8.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.710662 hu-neuro-pipeline-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/.github/workflows/build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      750 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2023-12-09 12:37:10.722662 hu-neuro-pipeline-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.710662 hu-neuro-pipeline-0.8.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      420 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.714662 hu-neuro-pipeline-0.8.3/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.714662 hu-neuro-pipeline-0.8.3/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    39318 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    54216 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/_static/flowchart.svg
--rw-r--r--   0 runner    (1001) docker     (127)   193157 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.714662 hu-neuro-pipeline-0.8.3/doc/source/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/examples/n400.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7712 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/examples/ucap.qmd
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/processing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/processing_group.rst
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/processing_overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/processing_participant.rst
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/processing_tfr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      309 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)      808 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.718662 hu-neuro-pipeline-0.8.3/doc/source/tables/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/averaging.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/epoching.csv
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/inputs.csv
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/outputs.csv
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/performance.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/perm.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/preprocessing.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/tables/tfr.csv
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/usage_inputs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/usage_outputs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/doc/source/usage_quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.722662 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5520 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.718662 hu-neuro-pipeline-0.8.3/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-09 12:37:10.000000 hu-neuro-pipeline-0.8.3/pipeline/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/boilerplate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 12:37:10.722662 hu-neuro-pipeline-0.8.3/pipeline/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/erpcore.py
--rw-r--r--   0 runner    (1001) docker     (127)   407296 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/erpcore_manifest.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/ucap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32846 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/ucap_manifest.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/epoching.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     8795 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pipeline/tfr.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-09 12:37:10.722662 hu-neuro-pipeline-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-12-09 12:37:01.000000 hu-neuro-pipeline-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.276379 hu_neuro_pipeline-0.8.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.276379 hu_neuro_pipeline-0.8.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/.github/workflows/build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.280379 hu_neuro_pipeline-0.8.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.280379 hu_neuro_pipeline-0.8.5/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.280379 hu_neuro_pipeline-0.8.5/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    39318 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54216 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/_static/flowchart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   193157 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.284379 hu_neuro_pipeline-0.8.5/doc/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/examples/n400.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/examples/ucap.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/processing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/processing_group.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/processing_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/processing_participant.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/processing_tfr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.284379 hu_neuro_pipeline-0.8.5/doc/source/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/averaging.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/epoching.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/inputs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/outputs.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/performance.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/perm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/preprocessing.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/tables/tfr.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/usage_inputs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/usage_outputs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/doc/source/usage_quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 11:55:07.000000 hu_neuro_pipeline-0.8.5/pipeline/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10176 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/boilerplate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/pipeline/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5327 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/erpcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   407296 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/erpcore_manifest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/ucap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32846 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/ucap_manifest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/epoching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8795 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pipeline/tfr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:55:07.288379 hu_neuro_pipeline-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 11:55:01.000000 hu_neuro_pipeline-0.8.5/setup.py
```

### Comparing `hu-neuro-pipeline-0.8.3/.github/workflows/build_publish.yml` & `hu_neuro_pipeline-0.8.5/.github/workflows/build_publish.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 name: Build & publish package 📦
 
 on:
   release:
     types: [published]
   push:
-    branches:
-      - main
+
+permissions:
+  id-token: write
 
 jobs:
   build:
     name: Build package ⚙️
     runs-on: ubuntu-latest
     steps:
       - name: Checkout source
@@ -43,15 +44,12 @@
           name: package
           path: dist
 
       - name: Publish on TestPyPI
         if: startsWith(github.ref, 'refs/tags') != true
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          repository-url: https://test.pypi.org/legacy/
 
       - name: Publish on PyPI
         if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `hu-neuro-pipeline-0.8.3/.readthedocs.yaml` & `hu_neuro_pipeline-0.8.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/LICENSE` & `hu_neuro_pipeline-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/PKG-INFO` & `hu_neuro_pipeline-0.8.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.8.3
+Version: 0.8.5
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,45 +35,58 @@
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
 ### 1.1 For Python users
 
-Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Install the pipeline via `pip` from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
 
 ```bash
-python3 -m pip install hu-neuro-pipeline
+pip install hu-neuro-pipeline
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
 
 ```bash
-python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
 ```
 
 ### 1.2 For R users
 
-First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
+First install and load [reticulate](https://rstudio.github.io/reticulate/) (an R package for accessing Python functionality from within R):
 
 ```r
 install.packages("reticulate")
-reticulate::install_miniconda()
+library("reticulate")
 ```
 
-Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Check if you already have [conda](https://docs.conda.io/en/latest/) (a scientific Python distribution) installed on your system:
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+conda_exe()
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+If this shows you the path to a conda executable, you can skip the next step.
+If instead it shows you an error, you need to install conda:
 
 ```r
-reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
+install_miniconda()
+```
+
+Then install the pipeline from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
+
+```r
+py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 ### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
```

### Comparing `hu-neuro-pipeline-0.8.3/README.md` & `hu_neuro_pipeline-0.8.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,45 +10,58 @@
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
 ### 1.1 For Python users
 
-Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Install the pipeline via `pip` from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
 
 ```bash
-python3 -m pip install hu-neuro-pipeline
+pip install hu-neuro-pipeline
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
 
 ```bash
-python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
 ```
 
 ### 1.2 For R users
 
-First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
+First install and load [reticulate](https://rstudio.github.io/reticulate/) (an R package for accessing Python functionality from within R):
 
 ```r
 install.packages("reticulate")
-reticulate::install_miniconda()
+library("reticulate")
 ```
 
-Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Check if you already have [conda](https://docs.conda.io/en/latest/) (a scientific Python distribution) installed on your system:
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+conda_exe()
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+If this shows you the path to a conda executable, you can skip the next step.
+If instead it shows you an error, you need to install conda:
 
 ```r
-reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
+install_miniconda()
+```
+
+Then install the pipeline from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
+
+```r
+py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 ### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
```

### Comparing `hu-neuro-pipeline-0.8.3/doc/Makefile` & `hu_neuro_pipeline-0.8.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/make.bat` & `hu_neuro_pipeline-0.8.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/_static/favicon.png` & `hu_neuro_pipeline-0.8.5/doc/source/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/_static/flowchart.svg` & `hu_neuro_pipeline-0.8.5/doc/source/_static/flowchart.svg`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/_static/logo.png` & `hu_neuro_pipeline-0.8.5/doc/source/_static/logo.png`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/conf.py` & `hu_neuro_pipeline-0.8.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/examples/n400.qmd` & `hu_neuro_pipeline-0.8.5/doc/source/examples/n400.qmd`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/examples/ucap.qmd` & `hu_neuro_pipeline-0.8.5/doc/source/examples/ucap.qmd`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,20 @@
 The paths of the downloaded EEG header files (`.vhdr`), behavioral log files (`.txt`), and ocular correction files (`.matrix`) can now be fed into pipeline.
 
 ## Running the pipeline
 
 We run a simple pipeline for single-trial ERP analysis with the following steps:
 
 - Downsampling to 250 Hz
-- Re-referencing to common average (not shown)
+- Re-referencing to common average (per default)
 - Ocular correction with BESA/MSEC matrices
-- Default bandpass filtering between 0.1 and 40 Hz (not_shown)
+- Default bandpass filtering between 0.1 and 40 Hz (per default)
 - Segmentation to epochs around stimulus triggers
-- Baseline correction (not shown)
-- Rejecting bad epochs based on peak-to-peak amplitudes > 200 µV (not shown)
+- Baseline correction (per default)
+- Rejecting bad epochs based on peak-to-peak amplitudes > 200 µV (per default)
 - Computing single trial N2 and P3b amplitudes by averaging across time windows and channels of interest
 - Creating by-participant averages for the blurred and normal conditions
 
 ```{r}
 res <- pipeline$group_pipeline(
 
   # Input/output paths
@@ -93,31 +93,37 @@
   average_by = list(
     blurr = "n_b == 'blurr'",
     normal = "n_b == 'normal'"
   )
 )
 ```
 
+See the [Input arguments](../usage_inputs.rst) page for a list of all available processing options.
+
 ## Checking the results
 
 The resulting object (`res`) is a list with three components: A dataframe of single trial ERP amplitudes, a dataframe of by-participant condition averages, and a dictionary of pipeline metadata.
 
+```{r}
+str(res, max.level = 1)
+```
+
 ### Single-trial ERP amplitudes
 
 These are basically just the log files, concatenated for all participants, with two added columns for the two ERP components of interest.
 Each value in these columns reflects the single trial ERP amplitude, averaged across time points and channels of interest.
 
 Here are the first couple of lines of the dataframe:
 
 ```{r}
 trials <- res[[1]]
 head(trials)
 ```
 
-We can plot the single trial ERP amplitudes (here for the N2 component), separately for the blurred and normal conditions, e.g., as a kernel density plot:
+We can plot the single trial ERP amplitudes (here for the N2 component), separately for the blurred and normal conditions, e.g., as a density plot:
 
 ```{r}
 trials |>
   ggplot(aes(x = N2, fill = n_b)) +
   geom_density(color = NA, alpha = 0.5) +
   labs(x = "N2 amplitude (µV)", y = "Density", fill = "Condition") +
   theme_minimal(base_size = 25.0) +
@@ -132,15 +138,19 @@
 ```{r}
 mod <- lmer(N2 ~ n_b + (1 | participant_id), data = trials)
 summary(mod)
 ```
 
 Here we predict the single trial N2 amplitude based on the fixed effect of blurred vs. normal, and we allow for random variation in the intercept between participants.
 
-Note that for sound inference on the full dataset, we would want to (a) apply proper contrast coding to the `n_b` factor (e.g., [Schad et al., 2020](https://doi.org/10.1016/j.jml.2019.104038)), (b) include random effects not just for participants, but also for items (e.g., [Judd et al., 2012](https://doi.org/10.1037/a0028347)), and (c) include not just random intercepts, but also random slopes (e.g., [Barr et al., 2013](https://doi.org/10.1016/j.jml.2012.11.001)).
+Note that for sound inference on the full dataset, we would want to:
+
+- apply proper contrast coding to the `n_b` factor (e.g., [Schad et al., 2020](https://doi.org/10.1016/j.jml.2019.104038)),
+- include random effects not just for participants, but also for items (e.g., [Judd et al., 2012](https://doi.org/10.1037/a0028347)), and
+- include not just random intercepts, but also random slopes (e.g., [Barr et al., 2013](https://doi.org/10.1016/j.jml.2012.11.001)).
 
 ### By-participant condition averages
 
 This is one big data frame which, unlike `trials`, is averaged across trials (i.e., losing any single trial information) but *not* averaged across time points or channels (i.e., retaining the millisecond-wise ERP waveform at all electrodes).
 
 ```{r}
 evokeds <- res[[2]]
```

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/index.rst` & `hu_neuro_pipeline-0.8.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/installation.rst` & `hu_neuro_pipeline-0.8.5/doc/source/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,37 +12,50 @@
 
 Alternatively, to install the latest development version directly from `GitHub <https://github.com/alexenge/hu-neuro-pipeline>`_:
 
 .. code-block:: bash
 
     pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
 
-The pipeline requires Python Version ≥ 3.8 and a number of `dependency packages <https://github.com/alexenge/hu-neuro-pipeline/blob/doc/add-sphinx/setup.py#L47-L55>`_, which will get installed automatically when running the commands above.
+The pipeline requires Python Version ≥ 3.8 and a number of `dependency packages <https://github.com/alexenge/hu-neuro-pipeline/blob/main/setup.py#L49-L57>`_, which will get installed automatically when running the commands above.
 
 For R users
 -----------
 
-First install `reticulate <https://rstudio.github.io/reticulate>`_ and `Miniconda <https://docs.conda.io/en/latest/miniconda.html>`_ for being able to import Python packages into R:
+First install and load `reticulate <https://rstudio.github.io/reticulate>`_ (an R package for accessing Python functionality from within R):
 
 .. code-block:: r
 
     install.packages("reticulate")
-    reticulate::install_miniconda()
+    library("reticulate")
+
+Check if you already have `conda <https://docs.conda.io/en/latest/>`_ (a scientific Python distribution) installed on your system:
+
+.. code-block:: r
+
+    conda_exe()
+
+If this shows you the path to a conda executable, you can skip the next step.
+If instead it shows you an error, you need to install conda:
+
+.. code-block:: r
+
+    install_miniconda()
 
 Then install the pipeline from the `Python Package Index (PyPI) <https://pypi.org/project/hu-neuro-pipeline>`_:
 
 .. code-block:: r
 
-    reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+    py_install("hu-neuro-pipeline", pip = TRUE)
 
-Alternatively, to install the latest development version directly from `GitHub`_:
+Alternatively, you can install the latest development version from `GitHub`_:
 
 .. code-block:: r
 
-    reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
+    py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 
 What next?
 ----------
 
 To jump right into how to use the pipeline, see :doc:`Usage <usage>`.
 
 To learn about the different steps that the pipeline is carrying out, see :doc:`Processing details <processing>`.
```

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/processing_group.rst` & `hu_neuro_pipeline-0.8.5/doc/source/processing_group.rst`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/processing_participant.rst` & `hu_neuro_pipeline-0.8.5/doc/source/processing_participant.rst`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/references.bib` & `hu_neuro_pipeline-0.8.5/doc/source/references.bib`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/epoching.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/epoching.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/inputs.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/inputs.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/outputs.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/outputs.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/perm.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/perm.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/preprocessing.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/preprocessing.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/tables/tfr.csv` & `hu_neuro_pipeline-0.8.5/doc/source/tables/tfr.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/usage_inputs.rst` & `hu_neuro_pipeline-0.8.5/doc/source/usage_inputs.rst`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/doc/source/usage_quickstart.rst` & `hu_neuro_pipeline-0.8.5/doc/source/usage_quickstart.rst`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/PKG-INFO` & `hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hu-neuro-pipeline
-Version: 0.8.3
+Version: 0.8.5
 Summary: Single trial EEG pipeline at the Abdel Rahman Lab for Neurocognitive Psychology, Humboldt-Universität zu Berlin
 Home-page: https://github.com/alexenge/hu-neuro-pipeline
 Author: Alexander Enge
 Author-email: alexander.enge@hu-berlin.de
 Project-URL: Issue trackers, https://github.com/alexenge/hu-neuro-pipeline/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -35,45 +35,58 @@
 Group-level EEG-processing pipeline for flexible single trial-based analyses including linear mixed models.
 *Frontiers in Neuroscience*, *12*, 48. <https://doi.org/10.3389/fnins.2018.00048>
 
 ## 1. Installation
 
 ### 1.1 For Python users
 
-Install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Install the pipeline via `pip` from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
 
 ```bash
-python3 -m pip install hu-neuro-pipeline
+pip install hu-neuro-pipeline
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
 
 ```bash
-python3 -m pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
+pip install git+https://github.com/alexenge/hu-neuro-pipeline.git
 ```
 
 ### 1.2 For R users
 
-First install [reticulate](https://rstudio.github.io/reticulate/) and [Miniconda](https://docs.conda.io/en/latest/miniconda.html) for being able to import Python packages into R:
+First install and load [reticulate](https://rstudio.github.io/reticulate/) (an R package for accessing Python functionality from within R):
 
 ```r
 install.packages("reticulate")
-reticulate::install_miniconda()
+library("reticulate")
 ```
 
-Then install the pipeline via `pip` from the [Python Package Index](https://pypi.org/project/hu-neuro-pipeline/) (PyPI):
+Check if you already have [conda](https://docs.conda.io/en/latest/) (a scientific Python distribution) installed on your system:
 
 ```r
-reticulate::py_install("hu-neuro-pipeline", pip = TRUE)
+conda_exe()
 ```
 
-To install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+If this shows you the path to a conda executable, you can skip the next step.
+If instead it shows you an error, you need to install conda:
 
 ```r
-reticulate::py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
+install_miniconda()
+```
+
+Then install the pipeline from the [Python Package Index (PyPI)](https://pypi.org/project/hu-neuro-pipeline/):
+
+```r
+py_install("hu-neuro-pipeline", pip = TRUE)
+```
+
+Alternatively, you can install the latest development version from [GitHub](https://github.com/alexenge/hu-neuro-pipeline.git):
+
+```r
+py_install("git+https://github.com/alexenge/hu-neuro-pipeline.git", pip = TRUE)
 ```
 
 ## 2. Usage
 
 ### 2.1 For Python users
 
 Here is a fairly minimal example for a (fictional) N400/P600 experiment with two experimental factors: `semantics` (e.g., related versus unrelated words) and emotional `context` (e.g., emotionally negative versus neutral).
```

### Comparing `hu-neuro-pipeline-0.8.3/hu_neuro_pipeline.egg-info/SOURCES.txt` & `hu_neuro_pipeline-0.8.5/hu_neuro_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/__init__.py` & `hu_neuro_pipeline-0.8.5/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/averaging.py` & `hu_neuro_pipeline-0.8.5/pipeline/averaging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import warnings
+from warnings import warn
 
 import numpy as np
 import pandas as pd
 from mne import Epochs, Evoked, grand_average
 from mne.time_frequency import AverageTFR, EpochsTFR
 
 
@@ -13,19 +13,18 @@
     if average_by is None:
         all_evokeds, all_evokeds_df = compute_evokeds_triggers(
             epochs, bad_ixs, participant_id)
     elif isinstance(average_by, dict):
         all_evokeds, all_evokeds_df = compute_evokeds_queries(
             epochs, average_by, bad_ixs, participant_id)
     else:
-        warnings.warn(
-            'Passing a list of column names to `average_by` will ' +
-            'be deprecated in a future version of the pipeline. ' +
-            'Please use a dict of  labels and log file queries ' +
-            'instead (see https://github.com/alexenge/hu-neuro-pipeline/blob/main/docs/inputs.md#average_by-recommended-default-none)')
+        warn('Passing a list of column names to `average_by` will ' +
+             'be deprecated in a future version of the pipeline. ' +
+             'Please use a dict of  labels and log file queries ' +
+             'instead (see https://github.com/alexenge/hu-neuro-pipeline/blob/main/docs/inputs.md#average_by-recommended-default-none)')
         all_evokeds, all_evokeds_df = compute_evokeds_cols(
             epochs, average_by, bad_ixs, participant_id)
 
     return all_evokeds, all_evokeds_df
 
 
 def compute_evokeds_triggers(epochs, bad_ixs=[], participant_id=None):
@@ -65,31 +64,39 @@
     # Create evokeds for each query
     evokeds = []
     evoked_dfs = []
     for label, query in queries.items():
 
         # Compute evokeds for trials that match the current query
         evoked = compute_evoked_query(epochs[good_ixs], query, label)
-        evokeds.append(evoked)
+        if evoked is not None:
+            evokeds.append(evoked)
 
-        # Convert to data frame
-        extra_cols = \
-            {'participant_id': participant_id, 'label': label, 'query': query}
-        evoked_df = evoked_to_df(evoked, extra_cols)
-        evoked_dfs.append(evoked_df)
+            # Convert to data frame
+            extra_cols = {'participant_id': participant_id,
+                          'label': label,
+                          'query': query}
+            evoked_df = evoked_to_df(evoked, extra_cols)
+            evoked_dfs.append(evoked_df)
 
     # Combine data frames
     evokeds_df = pd.concat(evoked_dfs, ignore_index=True)
 
     return evokeds, evokeds_df
 
 
 def compute_evoked_query(epochs, query, label):
     """Computes one condition average (evoked) based on a log file query."""
 
+    if len(epochs[query]) == 0:
+        warn(f'No trials found for query "{query}" (label: "{label}"). ' +
+             'This condition for this participant won\'t be included in the ' +
+             'evokeds and grand averages.')
+        return None
+
     # Compute evokeds based on ERP or TFR epochs
     if isinstance(epochs, EpochsTFR):
         evoked = epochs[query].average()
     else:  # `EpochsTFR.average()` has no `picks` argument
         evoked = epochs[query].average(picks=['eeg', 'misc'])
     evoked.comment = label
 
@@ -264,13 +271,14 @@
     first_grouping_ix = 1  # Column 0 is participant_id (to average over)
     last_grouping_col = 'freq' if 'freq' in evokeds_df.columns else 'time'
     last_grouping_ix = evokeds_df.columns.get_loc(last_grouping_col)
     grouping_ixs = range(first_grouping_ix, last_grouping_ix + 1)
 
     # Average by grouping columns
     group_cols = list(evokeds_df.columns[grouping_ixs])
-    grands_df = evokeds_df.groupby(group_cols, dropna=False).mean(numeric_only=True)
+    grands_df = evokeds_df.groupby(
+        group_cols, dropna=False).mean(numeric_only=True)
 
     # Convert conditions from index back to columns
     grands_df = grands_df.reset_index()
 
     return grands_df
```

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/boilerplate.py` & `hu_neuro_pipeline-0.8.5/pipeline/boilerplate.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/datasets/erpcore.py` & `hu_neuro_pipeline-0.8.5/pipeline/datasets/erpcore.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/datasets/erpcore_manifest.csv` & `hu_neuro_pipeline-0.8.5/pipeline/datasets/erpcore_manifest.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/datasets/ucap.py` & `hu_neuro_pipeline-0.8.5/pipeline/datasets/ucap.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/datasets/ucap_manifest.csv` & `hu_neuro_pipeline-0.8.5/pipeline/datasets/ucap_manifest.csv`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/datasets/utils.py` & `hu_neuro_pipeline-0.8.5/pipeline/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/epoching.py` & `hu_neuro_pipeline-0.8.5/pipeline/epoching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from warnings import warn
 
 import chardet
 import numpy as np
 import pandas as pd
 from mne import (combine_evoked, events_from_annotations, pick_channels,
                  set_log_level)
 from mne.channels import combine_channels
@@ -22,14 +23,45 @@
         else:
             event_id = {key: value for key, value in event_id.items()
                         if int(key) in triggers}
 
     return events, event_id
 
 
+def update_skip_log_rows(skip_log_rows, epochs):
+    """Updates log file rows to skip, based on dropped epochs."""
+
+    if dropped_ixs := get_dropped_epochs(epochs):
+
+        if skip_log_rows is None:
+            return dropped_ixs
+
+        else:
+            return list(set(skip_log_rows) | set(dropped_ixs))
+
+
+def get_dropped_epochs(epochs):
+    """Gets indices of dropped epochs (e.g., due to 'NO_DATA')."""
+
+    drop_log = [elem for elem in epochs.drop_log if elem != ('IGNORED',)]
+
+    reasons = ['NO_DATA', 'TOO_SHORT']
+    dropped_ixs = set()
+    for reason in reasons:
+        if ixs := [ix for ix, elem in enumerate(drop_log) if reason in elem]:
+            dropped_ixs.update(ixs)
+            message = f'Dropped {len(ixs)} epochs ({ixs}) for reason ' + \
+                f'"{reason}". They will also be dropped from the log file.'
+            if reason == 'TOO_SHORT':
+                message += ' You may want reduce `epochs_tmax` to avoid this.'
+            warn(message)
+
+    return list(dropped_ixs)
+
+
 def read_log(log_file, skip_log_rows=None, skip_log_conditions=None):
     """Reads the behavioral log file with information about each EEG trial."""
 
     # Check if data are already in a DataFrame
     if isinstance(log_file, pd.DataFrame):
         log = log_file
     else:
```

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/group.py` & `hu_neuro_pipeline-0.8.5/pipeline/group.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/io.py` & `hu_neuro_pipeline-0.8.5/pipeline/io.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/participant.py` & `hu_neuro_pipeline-0.8.5/pipeline/participant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 import pandas as pd
-from mne import Epochs, events_from_annotations
+from mne import Epochs
 from mne.time_frequency import tfr_morlet
 
 from .averaging import compute_evokeds
 from .epoching import (compute_single_trials, get_bad_channels, get_bad_epochs,
-                       get_events, match_log_to_epochs, read_log)
+                       get_events, match_log_to_epochs, read_log,
+                       update_skip_log_rows)
 from .io import (read_eeg, save_clean, save_df, save_epochs, save_evokeds,
                  save_montage, save_report)
 from .preprocessing import (add_heog_veog, apply_montage, correct_besa,
                             correct_ica, interpolate_bad_channels)
 from .report import create_report
 from .tfr import compute_single_trials_tfr, subtract_evoked
 
@@ -131,14 +132,15 @@
         config['auto_ica_bad_components'] = [int(x) for x in ica.exclude]
 
     # Drop the last sample to produce a nice even number
     _ = epochs.crop(tmin=None, tmax=epochs_tmax, include_tmax=False)
     print(epochs.__str__().replace(u"\u2013", "-"))
 
     # Read behavioral log file and match to the epochs
+    skip_log_rows = update_skip_log_rows(skip_log_rows, epochs)
     log = read_log(log_file, skip_log_rows, skip_log_conditions)
     if triggers_column is not None:
         log, missing_ixs = match_log_to_epochs(epochs, log, triggers_column)
         config['auto_missing_epochs'] = missing_ixs
     epochs.metadata = log
     epochs.metadata.insert(0, column='participant_id', value=participant_id)
```

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/perm.py` & `hu_neuro_pipeline-0.8.5/pipeline/perm.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/preprocessing.py` & `hu_neuro_pipeline-0.8.5/pipeline/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
     return raw, all_bad_channels
 
 
 def correct_ica(raw, method='fastica', n_components=None, random_seed=1234):
     """Corrects ocular artifacts using ICA and automatic component removal."""
 
     # Convert number of components to integer
-    if n_components is not None and n_components >= 1.0:
+    if n_components is not None and n_components >= 1.0 \
+            and not isinstance(n_components, int):
         warn(f'Converting `ica_n_components` to integer: {n_components} -> ' +
              f'{int(n_components)}')
         n_components = int(n_components)
 
     # Run ICA on a copy of the data
     raw_filt_ica = raw.copy()
     raw_filt_ica.load_data().filter(l_freq=1, h_freq=None, verbose=False)
```

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/report.py` & `hu_neuro_pipeline-0.8.5/pipeline/report.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/pipeline/tfr.py` & `hu_neuro_pipeline-0.8.5/pipeline/tfr.py`

 * *Files identical despite different names*

### Comparing `hu-neuro-pipeline-0.8.3/setup.py` & `hu_neuro_pipeline-0.8.5/setup.py`

 * *Files identical despite different names*

