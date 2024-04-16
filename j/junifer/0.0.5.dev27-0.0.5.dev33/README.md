# Comparing `tmp/junifer-0.0.5.dev27.tar.gz` & `tmp/junifer-0.0.5.dev33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junifer-0.0.5.dev27.tar", last modified: Wed Apr 10 16:34:56 2024, max compression
+gzip compressed data, was "junifer-0.0.5.dev33.tar", last modified: Tue Apr 16 14:30:24 2024, max compression
```

## Comparing `junifer-0.0.5.dev27.tar` & `junifer-0.0.5.dev33.tar`

### file list

```diff
@@ -1,461 +1,462 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.161239 junifer-0.0.5.dev27/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.105239 junifer-0.0.5.dev27/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.105239 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/dataset-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/documention-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/marker-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.105239 junifer-0.0.5.dev27/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/ci-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/docs-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-10 16:34:56.161239 junifer-0.0.5.dev27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.105239 junifer-0.0.5.dev27/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.093239 junifer-0.0.5.dev27/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.105239 junifer-0.0.5.dev27/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.109239 junifer-0.0.5.dev27/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/_static/js/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.109239 junifer-0.0.5.dev27/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.109239 junifer-0.0.5.dev27/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/configs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/datagrabbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/datareaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/markers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/nilearn.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/onthefly.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/storage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/testing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25488 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/builtin.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.109239 junifer-0.0.5.dev27/docs/changes/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/changes/contributors.inc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.109239 junifer-0.0.5.dev27/docs/changes/newsfragments/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/changes/newsfragments/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/changes/newsfragments/161.feature
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/changes/newsfragments/273.feature
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/changes/newsfragments/324.bugfix
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/docs/extending/
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/coordinates.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/parcellations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/extending/preprocessor.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/help.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/images/junifer_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/links.inc
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/maintaining.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/redirect.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/sphinxext/gh_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/starting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/docs/understanding/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/datagrabber.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/datareader.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/marker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/preprocess.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/understanding/storage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/docs/using/
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/using/codeless.rst
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/using/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/using/masks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/using/queueing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/using/running.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26318 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/docs/whats_new.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.113239 junifer-0.0.5.dev27/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/norun_hcpfc_pearson.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/norun_ukbvm_gmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/run_compute_parcel_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/run_datagrabber_bids_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/run_ets_rss_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/run_junifer_julearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/run_run_gmd_mean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.117239 junifer-0.0.5.dev27/examples/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/yamls/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/yamls/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/yamls/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/examples/yamls/ukb_gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/ignore_words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.117239 junifer-0.0.5.dev27/junifer/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 16:34:55.000000 junifer-0.0.5.dev27/junifer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.117239 junifer-0.0.5.dev27/junifer/api/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.117239 junifer-0.0.5.dev27/junifer/api/queue_context/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/htcondor_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/queue_context_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.117239 junifer-0.0.5.dev27/junifer/api/queue_context/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/queue_context/tests/test_htcondor_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/res/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/res/afni/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/afni/3dAFNItoNIFTI
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/afni/3dRSFC
--rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/afni/3dReHo
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/afni/afni
--rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/afni/run_afni_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/res/ants/
--rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/ants/ResampleImage
--rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/ants/antsApplyTransforms
--rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/ants/antsApplyTransformsToPoints
--rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/ants/run_ants_docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/res/fsl/
--rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/fsl/applywarp
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/fsl/flirt
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/fsl/img2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/fsl/run_fsl_docker.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/fsl/std2imgcoord
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/run_conda.bash
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/run_conda.zsh
--rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/run_venv.bash
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/res/run_venv.zsh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/api/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/data/gmd_mean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/data/gmd_mean_htcondor.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/test_api_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    17215 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.121239 junifer-0.0.5.dev27/junifer/configs/juseless/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.125239 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ixi_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.125239 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ucla.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ukb_vbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.125239 junifer-0.0.5.dev27/junifer/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.097239 junifer-0.0.5.dev27/junifer/data/VOIs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.129239 junifer-0.0.5.dev27/junifer/data/VOIs/meta/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/CogAC_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/CogAR_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Empathy_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Motor_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/MultiTask_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Rew_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/ToM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/VigAtt_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/WM_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/eMDN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/eSAD_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/VOIs/meta/extDMN_VOIs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/coordinates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.097239 junifer-0.0.5.dev27/junifer/data/masks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.129239 junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/
--rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
--rw-r--r--   0 runner    (1001) docker     (127)    23473 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    65220 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/template_spaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.129239 junifer-0.0.5.dev27/junifer/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/tests/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/tests/test_parcellations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/tests/test_template_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.129239 junifer-0.0.5.dev27/junifer/datagrabber/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datagrabber/aomic/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/piop2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_id1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_piop1.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_piop2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/dmcc13_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/datalad_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/hcp1200.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/pattern_datalad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datagrabber/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_datagrabber_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_datalad_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_dmcc13_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_multiple.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/tests/test_pattern_datalad.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datagrabber/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datareader/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datareader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datareader/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/datareader/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/datareader/tests/test_default_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.133239 junifer-0.0.5.dev27/junifer/external/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.097239 junifer-0.0.5.dev27/junifer/external/h5io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.137239 junifer-0.0.5.dev27/junifer/external/h5io/h5io/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-10 16:34:52.000000 junifer-0.0.5.dev27/junifer/external/h5io/h5io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-04-10 16:34:52.000000 junifer-0.0.5.dev27/junifer/external/h5io/h5io/_h5io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 16:34:52.000000 junifer-0.0.5.dev27/junifer/external/h5io/h5io/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-10 16:34:52.000000 junifer-0.0.5.dev27/junifer/external/h5io/h5io/chunked_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-10 16:34:52.000000 junifer-0.0.5.dev27/junifer/external/h5io/h5io/chunked_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.137239 junifer-0.0.5.dev27/junifer/external/nilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/external/nilearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/external/nilearn/junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.137239 junifer-0.0.5.dev27/junifer/external/nilearn/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.137239 junifer-0.0.5.dev27/junifer/markers/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.137239 junifer-0.0.5.dev27/junifer/markers/complexity/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/sample_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.141239 junifer-0.0.5.dev27/junifer/markers/complexity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_complexity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_hurst_exponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_range_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_range_entropy_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_sample_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/complexity/weighted_perm_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/ets_rss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.141239 junifer-0.0.5.dev27/junifer/markers/falff/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/_afni_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/_junifer_falff.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/falff_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.141239 junifer-0.0.5.dev27/junifer/markers/falff/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/tests/test_falff_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/falff/tests/test_falff_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.141239 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.141239 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/parcel_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/markers/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/_afni_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/_junifer_reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/reho_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/reho_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/markers/reho/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/tests/test_reho_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/reho/tests/test_reho_spheres.py
--rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/sphere_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/markers/temporal_snr/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/markers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_ets_rss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_marker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_markers_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_parcel_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/tests/test_sphere_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/markers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/onthefly/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/onthefly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/onthefly/read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/onthefly/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/onthefly/tests/test_read_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.145239 junifer-0.0.5.dev27/junifer/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/pipeline/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/tests/test_pipeline_step_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/tests/test_update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/tests/test_workdir_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/update_meta_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/pipeline/workdir_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/ants/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/ants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/ants/ants_apply_transforms_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/ants/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/bold_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/confounds/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/confounds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/confounds/fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/confounds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/fsl/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/fsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/fsl/apply_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/fsl/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/fsl/tests/test_apply_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/_afni_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/_fsl_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/_nilearn_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/smoothing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/smoothing/tests/test_smoothing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.149239 junifer-0.0.5.dev27/junifer/preprocess/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/tests/test_bold_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/tests/test_preprocess_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/preprocess/warping/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/warping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/warping/_ants_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/warping/_fsl_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/warping/space_warper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/preprocess/warping/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/preprocess/warping/tests/test_space_warper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/storage/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/tests/test_pandas_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/tests/test_storage_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/testing/data/
--rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/datagrabbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.153239 junifer-0.0.5.dev27/junifer/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/tests/test_spmauditory_datagrabber.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/tests/test_testing_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.157239 junifer-0.0.5.dev27/junifer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/tests/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.157239 junifer-0.0.5.dev27/junifer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.157239 junifer-0.0.5.dev27/junifer/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/junifer/utils/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.157239 junifer-0.0.5.dev27/junifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14119 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 16:34:56.000000 junifer-0.0.5.dev27/junifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:34:56.161239 junifer-0.0.5.dev27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:34:56.157239 junifer-0.0.5.dev27/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_aomic1000_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_aomicpiop1_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_aomicpiop2_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_bids_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_bids_example_dataset_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_dmcc13_benchmark_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tools/create_hcp1200_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-10 16:34:51.000000 junifer-0.0.5.dev27/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.658128 junifer-0.0.5.dev33/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.590127 junifer-0.0.5.dev33/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.590127 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/dataset-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/documention-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/marker-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.594128 junifer-0.0.5.dev33/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/ci-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/docs-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34354 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-16 14:30:24.658128 junifer-0.0.5.dev33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.594128 junifer-0.0.5.dev33/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.578127 junifer-0.0.5.dev33/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.594128 junifer-0.0.5.dev33/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.594128 junifer-0.0.5.dev33/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/_static/js/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.594128 junifer-0.0.5.dev33/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.598127 junifer-0.0.5.dev33/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/configs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/datagrabbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/datareaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/markers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/nilearn.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/onthefly.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/storage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25488 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/builtin.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.598127 junifer-0.0.5.dev33/docs/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/contributors.inc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.598127 junifer-0.0.5.dev33/docs/changes/newsfragments/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/newsfragments/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/newsfragments/161.feature
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/newsfragments/273.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/newsfragments/323.feature
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/changes/newsfragments/324.bugfix
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.602127 junifer-0.0.5.dev33/docs/extending/
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/coordinates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9693 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/parcellations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/extending/preprocessor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/help.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.602127 junifer-0.0.5.dev33/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    62148 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/images/junifer_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/links.inc
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/maintaining.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/redirect.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.602127 junifer-0.0.5.dev33/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/sphinxext/gh_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/starting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.602127 junifer-0.0.5.dev33/docs/understanding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/datagrabber.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/datareader.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/marker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/preprocess.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/understanding/storage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.602127 junifer-0.0.5.dev33/docs/using/
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/using/codeless.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/using/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/using/masks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/using/queueing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/using/running.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26318 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/docs/whats_new.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.606128 junifer-0.0.5.dev33/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/norun_hcpfc_pearson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/norun_ukbvm_gmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/run_compute_parcel_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/run_datagrabber_bids_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/run_ets_rss_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/run_junifer_julearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/run_run_gmd_mean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.606128 junifer-0.0.5.dev33/examples/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/yamls/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/yamls/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/yamls/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/examples/yamls/ukb_gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/ignore_words.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.606128 junifer-0.0.5.dev33/junifer/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.606128 junifer-0.0.5.dev33/junifer/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12938 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/queue_context/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9561 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/htcondor_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/queue_context_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/queue_context/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/queue_context/tests/test_htcondor_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/res/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/res/afni/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/afni/3dAFNItoNIFTI
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/afni/3dRSFC
+-rwxr-xr-x   0 runner    (1001) docker     (127)       44 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/afni/3dReHo
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/afni/afni
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/afni/run_afni_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/res/ants/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/ants/ResampleImage
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/ants/antsApplyTransforms
+-rwxr-xr-x   0 runner    (1001) docker     (127)       65 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/ants/antsApplyTransformsToPoints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1119 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/ants/run_ants_docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.610128 junifer-0.0.5.dev33/junifer/api/res/fsl/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       46 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/fsl/applywarp
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/fsl/flirt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/fsl/img2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1122 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/fsl/run_fsl_docker.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/fsl/std2imgcoord
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/run_conda.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/run_conda.zsh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      507 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/run_venv.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/res/run_venv.zsh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/api/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/api/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/data/gmd_mean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/data/gmd_mean_htcondor.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/data/partly_cloudy_agg_mean_tian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/test_api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10969 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/configs/juseless/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ixi_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.614127 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ucla.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ukb_vbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.618127 junifer-0.0.5.dev33/junifer/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.582127 junifer-0.0.5.dev33/junifer/data/VOIs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.618127 junifer-0.0.5.dev33/junifer/data/VOIs/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/CogAC_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/CogAR_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/DMNBuckner_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Empathy_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Motor_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/MultiTask_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/PhysioStress_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Rew_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/Somatosensory_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/ToM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/VigAtt_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/WM_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/eMDN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/eSAD_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/VOIs/meta/extDMN_VOIs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/coordinates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.582127 junifer-0.0.5.dev33/junifer/data/masks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.622128 junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/
+-rw-r--r--   0 runner    (1001) docker     (127)    88270 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    12862 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    23473 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65220 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/template_spaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.622128 junifer-0.0.5.dev33/junifer/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/tests/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38222 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/tests/test_parcellations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/tests/test_template_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.622128 junifer-0.0.5.dev33/junifer/datagrabber/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.622128 junifer-0.0.5.dev33/junifer/datagrabber/aomic/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8428 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/piop2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.622128 junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_id1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_piop1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_piop2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12869 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/dmcc13_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/datalad_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/hcp1200.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/tests/test_hcp1200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/pattern_datalad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/datagrabber/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_datagrabber_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_datalad_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_dmcc13_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/tests/test_pattern_datalad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datagrabber/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/datareader/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datareader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datareader/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/datareader/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/datareader/tests/test_default_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.582127 junifer-0.0.5.dev33/junifer/external/h5io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/external/h5io/h5io/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/h5io/h5io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28748 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/h5io/h5io/_h5io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/h5io/h5io/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/h5io/h5io/chunked_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/h5io/h5io/chunked_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/external/nilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/nilearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/nilearn/junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.626128 junifer-0.0.5.dev33/junifer/external/nilearn/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10370 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.630128 junifer-0.0.5.dev33/junifer/markers/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.630128 junifer-0.0.5.dev33/junifer/markers/complexity/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/sample_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.634127 junifer-0.0.5.dev33/junifer/markers/complexity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_complexity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_hurst_exponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_range_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_range_entropy_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_sample_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/complexity/weighted_perm_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/ets_rss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.634127 junifer-0.0.5.dev33/junifer/markers/falff/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/_afni_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/_junifer_falff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/falff_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.634127 junifer-0.0.5.dev33/junifer/markers/falff/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/tests/test_falff_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/falff/tests/test_falff_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.634127 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.634127 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/parcel_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/markers/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/_afni_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/_junifer_reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/reho_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/reho_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/markers/reho/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/tests/test_reho_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/reho/tests/test_reho_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8275 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/sphere_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/markers/temporal_snr/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/test_temporal_snr_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/markers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_ets_rss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_marker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_markers_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_parcel_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/tests/test_sphere_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/markers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.638128 junifer-0.0.5.dev33/junifer/onthefly/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/onthefly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/onthefly/read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/onthefly/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/onthefly/tests/test_read_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/pipeline/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/tests/test_pipeline_step_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/tests/test_update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/tests/test_workdir_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/update_meta_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/pipeline/workdir_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/ants/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/ants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/ants/ants_apply_transforms_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/ants/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/bold_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/confounds/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/confounds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/confounds/fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/confounds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.642128 junifer-0.0.5.dev33/junifer/preprocess/fsl/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/fsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/fsl/apply_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/fsl/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/fsl/tests/test_apply_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/_afni_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/_fsl_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/_nilearn_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/smoothing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/smoothing/tests/test_smoothing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/tests/test_bold_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/tests/test_preprocess_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/warping/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/warping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5690 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/warping/_ants_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/warping/_fsl_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/warping/space_warper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/preprocess/warping/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/preprocess/warping/tests/test_space_warper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.646128 junifer-0.0.5.dev33/junifer/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35631 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/storage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29338 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/tests/test_pandas_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28318 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/tests/test_storage_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   406849 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/datagrabbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/tests/test_partlycloudytesting_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/tests/test_spmauditory_datagrabber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/tests/test_testing_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.650128 junifer-0.0.5.dev33/junifer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.654128 junifer-0.0.5.dev33/junifer/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/junifer/utils/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.654128 junifer-0.0.5.dev33/junifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 14:30:24.000000 junifer-0.0.5.dev33/junifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:30:24.658128 junifer-0.0.5.dev33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:30:24.654128 junifer-0.0.5.dev33/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_aomic1000_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_aomicpiop1_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_aomicpiop2_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_bids_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_bids_example_dataset_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_dmcc13_benchmark_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tools/create_hcp1200_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-16 14:30:20.000000 junifer-0.0.5.dev33/tox.ini
```

### Comparing `junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/bug-report.yml` & `junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/dataset-request.yml` & `junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/dataset-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/documention-request.yml` & `junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/documention-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/feature-request.yml` & `junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/ISSUE_TEMPLATE/marker-request.yml` & `junifer-0.0.5.dev33/.github/ISSUE_TEMPLATE/marker-request.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/ci-docs.yml` & `junifer-0.0.5.dev33/.github/workflows/ci-docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/ci.yml` & `junifer-0.0.5.dev33/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/docs-preview.yml` & `junifer-0.0.5.dev33/.github/workflows/docs-preview.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/docs.yml` & `junifer-0.0.5.dev33/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/lint.yml` & `junifer-0.0.5.dev33/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.github/workflows/pypi.yml` & `junifer-0.0.5.dev33/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.gitignore` & `junifer-0.0.5.dev33/.gitignore`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/.pre-commit-config.yaml` & `junifer-0.0.5.dev33/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/LICENSE.md` & `junifer-0.0.5.dev33/LICENSE.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/PKG-INFO` & `junifer-0.0.5.dev33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev27
+Version: 0.0.5.dev33
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev27/README.md` & `junifer-0.0.5.dev33/README.md`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/codecov.yml` & `junifer-0.0.5.dev33/codecov.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/conda-env.yml` & `junifer-0.0.5.dev33/conda-env.yml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/Makefile` & `junifer-0.0.5.dev33/docs/Makefile`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/_static/css/custom.css` & `junifer-0.0.5.dev33/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/_templates/versions.html` & `junifer-0.0.5.dev33/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/builtin.rst` & `junifer-0.0.5.dev33/docs/builtin.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/changes/contributors.inc` & `junifer-0.0.5.dev33/docs/changes/contributors.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/conf.py` & `junifer-0.0.5.dev33/docs/conf.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/contribution.rst` & `junifer-0.0.5.dev33/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/coordinates.rst` & `junifer-0.0.5.dev33/docs/extending/coordinates.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/datagrabber.rst` & `junifer-0.0.5.dev33/docs/extending/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/dependencies.rst` & `junifer-0.0.5.dev33/docs/extending/dependencies.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/extension.rst` & `junifer-0.0.5.dev33/docs/extending/extension.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/index.rst` & `junifer-0.0.5.dev33/docs/extending/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/marker.rst` & `junifer-0.0.5.dev33/docs/extending/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/masks.rst` & `junifer-0.0.5.dev33/docs/extending/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/parcellations.rst` & `junifer-0.0.5.dev33/docs/extending/parcellations.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/extending/preprocessor.rst` & `junifer-0.0.5.dev33/docs/extending/preprocessor.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/faq.rst` & `junifer-0.0.5.dev33/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/help.rst` & `junifer-0.0.5.dev33/docs/help.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/images/junifer_logo.png` & `junifer-0.0.5.dev33/docs/images/junifer_logo.png`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/index.rst` & `junifer-0.0.5.dev33/docs/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/installation.rst` & `junifer-0.0.5.dev33/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/links.inc` & `junifer-0.0.5.dev33/docs/links.inc`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/maintaining.rst` & `junifer-0.0.5.dev33/docs/maintaining.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/sphinxext/gh_substitutions.py` & `junifer-0.0.5.dev33/docs/sphinxext/gh_substitutions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/starting.rst` & `junifer-0.0.5.dev33/docs/starting.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/data.rst` & `junifer-0.0.5.dev33/docs/understanding/data.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/datagrabber.rst` & `junifer-0.0.5.dev33/docs/understanding/datagrabber.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/datareader.rst` & `junifer-0.0.5.dev33/docs/understanding/datareader.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/index.rst` & `junifer-0.0.5.dev33/docs/understanding/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/marker.rst` & `junifer-0.0.5.dev33/docs/understanding/marker.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/pipeline.rst` & `junifer-0.0.5.dev33/docs/understanding/pipeline.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/preprocess.rst` & `junifer-0.0.5.dev33/docs/understanding/preprocess.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/understanding/storage.rst` & `junifer-0.0.5.dev33/docs/understanding/storage.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/using/codeless.rst` & `junifer-0.0.5.dev33/docs/using/codeless.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/using/index.rst` & `junifer-0.0.5.dev33/docs/using/index.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/using/masks.rst` & `junifer-0.0.5.dev33/docs/using/masks.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/using/queueing.rst` & `junifer-0.0.5.dev33/docs/using/queueing.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/using/running.rst` & `junifer-0.0.5.dev33/docs/using/running.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/docs/whats_new.rst` & `junifer-0.0.5.dev33/docs/whats_new.rst`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/norun_hcpfc_pearson.py` & `junifer-0.0.5.dev33/examples/norun_hcpfc_pearson.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/norun_ukbvm_gmd.py` & `junifer-0.0.5.dev33/examples/norun_ukbvm_gmd.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/run_compute_parcel_mean.py` & `junifer-0.0.5.dev33/examples/run_compute_parcel_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/run_datagrabber_bids_datalad.py` & `junifer-0.0.5.dev33/examples/run_datagrabber_bids_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/run_ets_rss_marker.py` & `junifer-0.0.5.dev33/examples/run_ets_rss_marker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/run_junifer_julearn.py` & `junifer-0.0.5.dev33/examples/run_junifer_julearn.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/run_run_gmd_mean.py` & `junifer-0.0.5.dev33/examples/run_run_gmd_mean.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/yamls/gmd_mean.yaml` & `junifer-0.0.5.dev33/examples/yamls/gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/examples/yamls/ukb_gmd_mean.yaml` & `junifer-0.0.5.dev33/examples/yamls/ukb_gmd_mean.yaml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/cli.py` & `junifer-0.0.5.dev33/junifer/api/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import pathlib
 import subprocess
 import sys
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import click
 import pandas as pd
 
 from ..utils.logging import (
     configure_logging,
     logger,
     raise_error,
     warn_with_log,
 )
 from .functions import collect as api_collect
+from .functions import list_elements as api_list_elements
 from .functions import queue as api_queue
 from .functions import reset as api_reset
 from .functions import run as api_run
 from .parser import parse_yaml
 from .utils import (
     _get_dependency_information,
     _get_environment_information,
@@ -447,14 +448,77 @@
     configure_logging(level=verbose)
     # Parse YAML
     config = parse_yaml(filepath)
     # Perform operation
     api_reset(config)
 
 
+@cli.command()
+@click.argument(
+    "filepath",
+    type=click.Path(
+        exists=True, readable=True, dir_okay=False, path_type=pathlib.Path
+    ),
+)
+@click.option("--element", type=str, multiple=True)
+@click.option(
+    "-o",
+    "--output-file",
+    type=click.Path(dir_okay=False, writable=True, path_type=pathlib.Path),
+)
+@click.option(
+    "-v",
+    "--verbose",
+    type=click.UNPROCESSED,
+    callback=_validate_verbose,
+    default="info",
+)
+def list_elements(
+    filepath: click.Path,
+    element: Tuple[str],
+    output_file: Optional[click.Path],
+    verbose: Union[str, int],
+) -> None:
+    """Element listing command for CLI.
+
+    \f
+
+    Parameters
+    ----------
+    filepath : click.Path
+        The filepath to the configuration file.
+    element : tuple of str
+        The element to operate on.
+    output_file : click.Path or None
+        The path to write the output to. If not None, writing to
+        stdout is not performed.
+    verbose : click.Choice
+        The verbosity level: warning, info or debug (default "info").
+
+    """
+    configure_logging(level=verbose)
+    # Parse YAML
+    config = parse_yaml(filepath)  # type: ignore
+    # Fetch datagrabber
+    datagrabber = config["datagrabber"]
+    # Parse elements
+    elements = _parse_elements(element, config)
+    # Perform operation
+    listed_elements = api_list_elements(
+        datagrabber=datagrabber,
+        elements=elements,
+    )
+    # Check if output file is provided
+    if output_file is not None:
+        output_file.touch()
+        output_file.write_text(listed_elements)
+    else:
+        click.secho(listed_elements, fg="blue")
+
+
 @cli.group()
 def setup() -> None:  # pragma: no cover
     """Configure commands for Junifer."""
     pass
 
 
 @setup.command("afni-docker")
```

### Comparing `junifer-0.0.5.dev27/junifer/api/decorators.py` & `junifer-0.0.5.dev33/junifer/api/decorators.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/functions.py` & `junifer-0.0.5.dev33/junifer/api/functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -357,7 +357,48 @@
         )
         logger.info(f"Deleting job directory at {job_dir.resolve()!s}")
         if job_dir.exists():
             # Remove files and directories
             shutil.rmtree(job_dir)
             # Remove directory
             job_dir.parent.rmdir()
+
+
+def list_elements(
+    datagrabber: Dict,
+    elements: Union[str, List[Union[str, Tuple]], Tuple, None] = None,
+) -> str:
+    """List elements of the datagrabber filtered using `elements`.
+
+    Parameters
+    ----------
+    datagrabber : dict
+        DataGrabber to index. Must have a key ``kind`` with the kind of
+        DataGrabber to use. All other keys are passed to the DataGrabber
+        constructor.
+    elements : str or tuple or list of str or tuple, optional
+        Element(s) to filter using. Will be used to index the DataGrabber
+        (default None).
+
+    """
+    # Get datagrabber to use
+    datagrabber_object = _get_datagrabber(datagrabber)
+
+    # Fetch elements
+    raw_elements_to_list = []
+    with datagrabber_object:
+        if elements is not None:
+            for element in datagrabber_object.filter(elements):
+                raw_elements_to_list.append(element)
+        else:
+            for element in datagrabber_object:
+                raw_elements_to_list.append(element)
+
+    elements_to_list = []
+    for element in raw_elements_to_list:
+        # Stringify elements if tuple for operation
+        str_element = (
+            ",".join(element) if isinstance(element, tuple) else element
+        )
+        elements_to_list.append(str_element)
+
+    return "\n".join(elements_to_list)
```

### Comparing `junifer-0.0.5.dev27/junifer/api/parser.py` & `junifer-0.0.5.dev33/junifer/api/parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/queue_context/gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev33/junifer/api/queue_context/gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/queue_context/htcondor_adapter.py` & `junifer-0.0.5.dev33/junifer/api/queue_context/htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/queue_context/queue_context_adapter.py` & `junifer-0.0.5.dev33/junifer/api/queue_context/queue_context_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py` & `junifer-0.0.5.dev33/junifer/api/queue_context/tests/test_gnu_parallel_local_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/queue_context/tests/test_htcondor_adapter.py` & `junifer-0.0.5.dev33/junifer/api/queue_context/tests/test_htcondor_adapter.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/res/afni/run_afni_docker.sh` & `junifer-0.0.5.dev33/junifer/api/res/afni/run_afni_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/res/ants/run_ants_docker.sh` & `junifer-0.0.5.dev33/junifer/api/res/ants/run_ants_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/res/fsl/run_fsl_docker.sh` & `junifer-0.0.5.dev33/junifer/api/res/fsl/run_fsl_docker.sh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/res/run_conda.bash` & `junifer-0.0.5.dev33/junifer/api/res/run_conda.bash`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/res/run_conda.zsh` & `junifer-0.0.5.dev33/junifer/api/res/run_conda.zsh`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/tests/test_api_utils.py` & `junifer-0.0.5.dev33/junifer/api/tests/test_api_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/tests/test_cli.py` & `junifer-0.0.5.dev33/junifer/api/tests/test_cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import pytest
 from click.testing import CliRunner
 from ruamel.yaml import YAML
 
 from junifer.api.cli import (
     _parse_elements_file,
     collect,
+    list_elements,
     queue,
     reset,
     run,
     selftest,
     wtf,
 )
 
@@ -293,14 +294,96 @@
         ]
         # Run reset
         reset_result = runner.invoke(reset, reset_args)
         # Check
         assert reset_result.exit_code == 0
 
 
+@pytest.mark.parametrize(
+    "elements",
+    [
+        ("sub-01", "sub-02"),
+        ("sub-03", "sub-04"),
+    ],
+)
+def test_list_elements_stdout(
+    elements: Tuple[str, ...],
+) -> None:
+    """Test elements listing to stdout.
+
+    Parameters
+    ----------
+    elements : tuple of str
+        The parametrized elements for filtering.
+
+    """
+    # Get test config
+    infile = Path(__file__).parent / "data" / "partly_cloudy_agg_mean_tian.yml"
+    # List elements command arguments
+    list_elements_args = [
+        str(infile.absolute()),
+        "--verbose",
+        "debug",
+        "--element",
+        elements[0],
+        "--element",
+        elements[1],
+    ]
+    # Invoke list elements command
+    list_elements_result = runner.invoke(list_elements, list_elements_args)
+    # Check
+    assert list_elements_result.exit_code == 0
+    assert f"{elements[0]}\n{elements[1]}" in list_elements_result.stdout
+
+
+@pytest.mark.parametrize(
+    "elements",
+    [
+        ("sub-01", "sub-02"),
+        ("sub-03", "sub-04"),
+    ],
+)
+def test_list_elements_output_file(
+    tmp_path: Path,
+    elements: Tuple[str, ...],
+) -> None:
+    """Test elements listing to output file.
+
+    Parameters
+    ----------
+    tmp_path : pathlib.Path
+        The path to the test directory.
+    elements : tuple of str
+        The parametrized elements for filtering.
+
+    """
+    # Get test config
+    infile = Path(__file__).parent / "data" / "partly_cloudy_agg_mean_tian.yml"
+    # Output file
+    output_file = tmp_path / "elements.txt"
+    # List elements command arguments
+    list_elements_args = [
+        str(infile.absolute()),
+        "--verbose",
+        "debug",
+        "--element",
+        elements[0],
+        "--element",
+        elements[1],
+        "--output-file",
+        str(output_file.resolve()),
+    ]
+    # Invoke list elements command
+    list_elements_result = runner.invoke(list_elements, list_elements_args)
+    # Check
+    assert list_elements_result.exit_code == 0
+    with open(output_file) as f:
+        assert f"{elements[0]}\n{elements[1]}" == f.read()
+
+
 def test_wtf_short() -> None:
     """Test short version of wtf command."""
     # Invoke wtf command
     wtf_result = runner.invoke(wtf)
     # Check
     assert wtf_result.exit_code == 0
```

### Comparing `junifer-0.0.5.dev27/junifer/api/tests/test_functions.py` & `junifer-0.0.5.dev33/junifer/api/tests/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 # Authors: Federico Raimondo <f.raimondo@fz-juelich.de>
 #          Leonard Sasse <l.sasse@fz-juelich.de>
 #          Synchon Mandal <s.mandal@fz-juelich.de>
 # License: AGPL
 
 import logging
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import pytest
 from ruamel.yaml import YAML
 
 import junifer.testing.registry  # noqa: F401
-from junifer.api.functions import collect, queue, reset, run
+from junifer.api.functions import collect, list_elements, queue, reset, run
 from junifer.datagrabber.base import BaseDataGrabber
 from junifer.pipeline.registry import build
 
 
 # Configure YAML class
 yaml = YAML()
 yaml.default_flow_style = False
@@ -633,7 +633,32 @@
                 "storage": storage,
                 "queue": {"kind": "GNUParallelLocal", "jobname": job_name},
             }
         )
 
         assert not Path(storage["uri"]).exists()
         assert not (tmp_path / "junifer_jobs" / job_name).exists()
+
+
+@pytest.mark.parametrize(
+    "elements",
+    [
+        ["sub-01"],
+        None,
+    ],
+)
+def test_list_elements(
+    datagrabber: Dict[str, str],
+    elements: Optional[List[str]],
+) -> None:
+    """Test elements listing.
+
+    Parameters
+    ----------
+    datagrabber : dict
+        Testing datagrabber as dictionary.
+    elements : str of list of str
+        The parametrized elements for filtering.
+
+    """
+    listed_elements = list_elements(datagrabber, elements)
+    assert "sub-01" in listed_elements
```

### Comparing `junifer-0.0.5.dev27/junifer/api/tests/test_parser.py` & `junifer-0.0.5.dev33/junifer/api/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/api/utils.py` & `junifer-0.0.5.dev33/junifer/api/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/camcan_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ixi_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_aomic_id1000_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_camcan_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ixi_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ucla.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/tests/test_ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ucla.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ucla.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/configs/juseless/datagrabbers/ukb_vbm.py` & `junifer-0.0.5.dev33/junifer/configs/juseless/datagrabbers/ukb_vbm.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/AutobiographicalMemory_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/Dosenbach2010_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/Power2011_MNI_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/Power2013_MNI_VOIs.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/Rew_VOIs.txt` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/Rew_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/VOIs/meta/WM_VOIs.txt` & `junifer-0.0.5.dev33/junifer/data/VOIs/meta/WM_VOIs.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/__init__.py` & `junifer-0.0.5.dev33/junifer/data/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/coordinates.py` & `junifer-0.0.5.dev33/junifer/data/coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz` & `junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz` & `junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/CAT12_IXI555_MNI152_TMP_GS_GMprob0.2_clean_3mm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz` & `junifer-0.0.5.dev33/junifer/data/masks/vickery-patil/GMprob0.2_cortex_3mm_NA_rm.nii.gz`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/masks.py` & `junifer-0.0.5.dev33/junifer/data/masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/parcellations.py` & `junifer-0.0.5.dev33/junifer/data/parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/template_spaces.py` & `junifer-0.0.5.dev33/junifer/data/template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/tests/test_coordinates.py` & `junifer-0.0.5.dev33/junifer/data/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/tests/test_data_utils.py` & `junifer-0.0.5.dev33/junifer/data/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/tests/test_masks.py` & `junifer-0.0.5.dev33/junifer/data/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/tests/test_parcellations.py` & `junifer-0.0.5.dev33/junifer/data/tests/test_parcellations.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/tests/test_template_spaces.py` & `junifer-0.0.5.dev33/junifer/data/tests/test_template_spaces.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/data/utils.py` & `junifer-0.0.5.dev33/junifer/data/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/__init__.py` & `junifer-0.0.5.dev33/junifer/datagrabber/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/id1000.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/piop1.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/piop2.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_id1000.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_id1000.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_piop1.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_piop1.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/aomic/tests/test_piop2.py` & `junifer-0.0.5.dev33/junifer/datagrabber/aomic/tests/test_piop2.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/base.py` & `junifer-0.0.5.dev33/junifer/datagrabber/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/datalad_base.py` & `junifer-0.0.5.dev33/junifer/datagrabber/datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/dmcc13_benchmark.py` & `junifer-0.0.5.dev33/junifer/datagrabber/dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/datalad_hcp1200.py` & `junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/datalad_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/hcp1200.py` & `junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/hcp1200/tests/test_hcp1200.py` & `junifer-0.0.5.dev33/junifer/datagrabber/hcp1200/tests/test_hcp1200.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/multiple.py` & `junifer-0.0.5.dev33/junifer/datagrabber/multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/pattern.py` & `junifer-0.0.5.dev33/junifer/datagrabber/pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/pattern_datalad.py` & `junifer-0.0.5.dev33/junifer/datagrabber/pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_base.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_datagrabber_utils.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_datagrabber_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_datalad_base.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_datalad_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_dmcc13_benchmark.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_dmcc13_benchmark.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_multiple.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_multiple.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_pattern.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/tests/test_pattern_datalad.py` & `junifer-0.0.5.dev33/junifer/datagrabber/tests/test_pattern_datalad.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datagrabber/utils.py` & `junifer-0.0.5.dev33/junifer/datagrabber/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datareader/default.py` & `junifer-0.0.5.dev33/junifer/datareader/default.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/datareader/tests/test_default_reader.py` & `junifer-0.0.5.dev33/junifer/datareader/tests/test_default_reader.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/external/h5io/h5io/_h5io.py` & `junifer-0.0.5.dev33/junifer/external/h5io/h5io/_h5io.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/external/h5io/h5io/chunked_array.py` & `junifer-0.0.5.dev33/junifer/external/h5io/h5io/chunked_array.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/external/h5io/h5io/chunked_list.py` & `junifer-0.0.5.dev33/junifer/external/h5io/h5io/chunked_list.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/external/nilearn/junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev33/junifer/external/nilearn/junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py` & `junifer-0.0.5.dev33/junifer/external/nilearn/tests/test_junifer_nifti_spheres_masker.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/__init__.py` & `junifer-0.0.5.dev33/junifer/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/base.py` & `junifer-0.0.5.dev33/junifer/markers/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/collection.py` & `junifer-0.0.5.dev33/junifer/markers/collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/__init__.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/__init__.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/complexity_base.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/complexity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/hurst_exponent.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/multiscale_entropy_auc.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/perm_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/range_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/range_entropy_auc.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/sample_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_hurst_exponent.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_hurst_exponent.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_multiscale_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_perm_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_range_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_range_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_range_entropy_auc.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_range_entropy_auc.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_sample_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_sample_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/tests/test_weighted_perm_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/tests/test_weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/complexity/weighted_perm_entropy.py` & `junifer-0.0.5.dev33/junifer/markers/complexity/weighted_perm_entropy.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/ets_rss.py` & `junifer-0.0.5.dev33/junifer/markers/ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/_afni_falff.py` & `junifer-0.0.5.dev33/junifer/markers/falff/_afni_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/_junifer_falff.py` & `junifer-0.0.5.dev33/junifer/markers/falff/_junifer_falff.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/falff_base.py` & `junifer-0.0.5.dev33/junifer/markers/falff/falff_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/falff_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/falff/falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/falff_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/falff/falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/tests/test_falff_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/falff/tests/test_falff_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/falff/tests/test_falff_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/falff/tests/test_falff_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_base.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/functional_connectivity_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_crossparcellation_functional_connectivity.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_edge_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/functional_connectivity/tests/test_functional_connectivity_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/parcel_aggregation.py` & `junifer-0.0.5.dev33/junifer/markers/parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/_afni_reho.py` & `junifer-0.0.5.dev33/junifer/markers/reho/_afni_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/_junifer_reho.py` & `junifer-0.0.5.dev33/junifer/markers/reho/_junifer_reho.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/reho_base.py` & `junifer-0.0.5.dev33/junifer/markers/reho/reho_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/reho_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/reho/reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/reho_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/reho/reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/tests/test_reho_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/reho/tests/test_reho_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/reho/tests/test_reho_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/reho/tests/test_reho_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/sphere_aggregation.py` & `junifer-0.0.5.dev33/junifer/markers/sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_base.py` & `junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/temporal_snr/temporal_snr_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/temporal_snr/temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py` & `junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/test_temporal_snr_parcels.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py` & `junifer-0.0.5.dev33/junifer/markers/temporal_snr/tests/test_temporal_snr_spheres.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_collection.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_ets_rss.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_ets_rss.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_marker_utils.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_marker_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_markers_base.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_markers_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_parcel_aggregation.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_parcel_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/tests/test_sphere_aggregation.py` & `junifer-0.0.5.dev33/junifer/markers/tests/test_sphere_aggregation.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/markers/utils.py` & `junifer-0.0.5.dev33/junifer/markers/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/onthefly/read_transform.py` & `junifer-0.0.5.dev33/junifer/onthefly/read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/onthefly/tests/test_read_transform.py` & `junifer-0.0.5.dev33/junifer/onthefly/tests/test_read_transform.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/pipeline_step_mixin.py` & `junifer-0.0.5.dev33/junifer/pipeline/pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/registry.py` & `junifer-0.0.5.dev33/junifer/pipeline/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/singleton.py` & `junifer-0.0.5.dev33/junifer/pipeline/singleton.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/tests/test_pipeline_step_mixin.py` & `junifer-0.0.5.dev33/junifer/pipeline/tests/test_pipeline_step_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/tests/test_registry.py` & `junifer-0.0.5.dev33/junifer/pipeline/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/tests/test_update_meta_mixin.py` & `junifer-0.0.5.dev33/junifer/pipeline/tests/test_update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/tests/test_workdir_manager.py` & `junifer-0.0.5.dev33/junifer/pipeline/tests/test_workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/update_meta_mixin.py` & `junifer-0.0.5.dev33/junifer/pipeline/update_meta_mixin.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/utils.py` & `junifer-0.0.5.dev33/junifer/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/pipeline/workdir_manager.py` & `junifer-0.0.5.dev33/junifer/pipeline/workdir_manager.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/ants/ants_apply_transforms_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/ants/ants_apply_transforms_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/ants/tests/test_ants_apply_transforms_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/base.py` & `junifer-0.0.5.dev33/junifer/preprocess/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/bold_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/bold_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/confounds/fmriprep_confound_remover.py` & `junifer-0.0.5.dev33/junifer/preprocess/confounds/fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py` & `junifer-0.0.5.dev33/junifer/preprocess/confounds/tests/test_fmriprep_confound_remover.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/fsl/apply_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/fsl/apply_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/fsl/tests/test_apply_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/fsl/tests/test_apply_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/smoothing/_afni_smoothing.py` & `junifer-0.0.5.dev33/junifer/preprocess/smoothing/_afni_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/smoothing/_fsl_smoothing.py` & `junifer-0.0.5.dev33/junifer/preprocess/smoothing/_fsl_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/smoothing/_nilearn_smoothing.py` & `junifer-0.0.5.dev33/junifer/preprocess/smoothing/_nilearn_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/smoothing/smoothing.py` & `junifer-0.0.5.dev33/junifer/preprocess/smoothing/smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/smoothing/tests/test_smoothing.py` & `junifer-0.0.5.dev33/junifer/preprocess/smoothing/tests/test_smoothing.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/tests/test_bold_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/tests/test_bold_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/tests/test_preprocess_base.py` & `junifer-0.0.5.dev33/junifer/preprocess/tests/test_preprocess_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/warping/_ants_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/warping/_ants_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/warping/_fsl_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/warping/_fsl_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/warping/space_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/warping/space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/preprocess/warping/tests/test_space_warper.py` & `junifer-0.0.5.dev33/junifer/preprocess/warping/tests/test_space_warper.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/stats.py` & `junifer-0.0.5.dev33/junifer/stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/base.py` & `junifer-0.0.5.dev33/junifer/storage/base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/hdf5.py` & `junifer-0.0.5.dev33/junifer/storage/hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/pandas_base.py` & `junifer-0.0.5.dev33/junifer/storage/pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/sqlite.py` & `junifer-0.0.5.dev33/junifer/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/tests/test_hdf5.py` & `junifer-0.0.5.dev33/junifer/storage/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/tests/test_pandas_base.py` & `junifer-0.0.5.dev33/junifer/storage/tests/test_pandas_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/tests/test_sqlite.py` & `junifer-0.0.5.dev33/junifer/storage/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/tests/test_storage_base.py` & `junifer-0.0.5.dev33/junifer/storage/tests/test_storage_base.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/tests/test_utils.py` & `junifer-0.0.5.dev33/junifer/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/storage/utils.py` & `junifer-0.0.5.dev33/junifer/storage/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv` & `junifer-0.0.5.dev33/junifer/testing/data/sub-0001_task-anticipation_acq-seq_desc-confounds_regressors.tsv`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/datagrabbers.py` & `junifer-0.0.5.dev33/junifer/testing/datagrabbers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/registry.py` & `junifer-0.0.5.dev33/junifer/testing/registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py` & `junifer-0.0.5.dev33/junifer/testing/tests/test_oasisvmbtesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/tests/test_partlycloudytesting_datagrabber.py` & `junifer-0.0.5.dev33/junifer/testing/tests/test_partlycloudytesting_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/tests/test_spmauditory_datagrabber.py` & `junifer-0.0.5.dev33/junifer/testing/tests/test_spmauditory_datagrabber.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/tests/test_testing_registry.py` & `junifer-0.0.5.dev33/junifer/testing/tests/test_testing_registry.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/testing/utils.py` & `junifer-0.0.5.dev33/junifer/testing/utils.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/tests/test_stats.py` & `junifer-0.0.5.dev33/junifer/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/utils/helpers.py` & `junifer-0.0.5.dev33/junifer/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/utils/logging.py` & `junifer-0.0.5.dev33/junifer/utils/logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/utils/tests/test_fs.py` & `junifer-0.0.5.dev33/junifer/utils/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/utils/tests/test_helpers.py` & `junifer-0.0.5.dev33/junifer/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer/utils/tests/test_logging.py` & `junifer-0.0.5.dev33/junifer/utils/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/junifer.egg-info/PKG-INFO` & `junifer-0.0.5.dev33/junifer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: junifer
-Version: 0.0.5.dev27
+Version: 0.0.5.dev33
 Summary: JUelich NeuroImaging FEature extractoR
 Author-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 Maintainer-email: Fede Raimondo <f.raimondo@fz-juelich.de>, Synchon Mandal <s.mandal@fz-juelich.de>
 License: AGPL-3.0-only
 Project-URL: Changelog, https://juaml.github.io/junifer/main/whats_new.html
 Project-URL: Documentation, https://juaml.github.io/junifer
 Project-URL: Homepage, https://juaml.github.io/junifer
```

### Comparing `junifer-0.0.5.dev27/junifer.egg-info/SOURCES.txt` & `junifer-0.0.5.dev33/junifer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 docs/api/storage.rst
 docs/api/testing.rst
 docs/api/utils.rst
 docs/changes/contributors.inc
 docs/changes/newsfragments/.gitignore
 docs/changes/newsfragments/161.feature
 docs/changes/newsfragments/273.feature
+docs/changes/newsfragments/323.feature
 docs/changes/newsfragments/324.bugfix
 docs/extending/coordinates.rst
 docs/extending/datagrabber.rst
 docs/extending/dependencies.rst
 docs/extending/extension.rst
 docs/extending/index.rst
 docs/extending/marker.rst
```

### Comparing `junifer-0.0.5.dev27/junifer.egg-info/requires.txt` & `junifer-0.0.5.dev33/junifer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/pyproject.toml` & `junifer-0.0.5.dev33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_aomic1000_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_aomic1000_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_aomicpiop1_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_aomicpiop1_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_aomicpiop2_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_aomicpiop2_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_bids_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_bids_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_bids_example_dataset_sessions.py` & `junifer-0.0.5.dev33/tools/create_bids_example_dataset_sessions.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_dmcc13_benchmark_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_dmcc13_benchmark_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tools/create_hcp1200_example_dataset.py` & `junifer-0.0.5.dev33/tools/create_hcp1200_example_dataset.py`

 * *Files identical despite different names*

### Comparing `junifer-0.0.5.dev27/tox.ini` & `junifer-0.0.5.dev33/tox.ini`

 * *Files identical despite different names*

