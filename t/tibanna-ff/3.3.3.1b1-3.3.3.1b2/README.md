# Comparing `tmp/tibanna_ff-3.3.3.1b1.tar.gz` & `tmp/tibanna_ff-3.3.3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibanna_ff-3.3.3.1b1.tar", max compression
+gzip compressed data, was "tibanna_ff-3.3.3.1b2.tar", max compression
```

## Comparing `tibanna_ff-3.3.3.1b1.tar` & `tibanna_ff-3.3.3.1b2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1083 2021-09-09 16:55:28.100725 tibanna_ff-3.3.3.1b1/LICENSE.txt
--rw-r--r--   0        0        0      188 2024-01-18 20:28:25.185806 tibanna_ff-3.3.3.1b1/README.md
--rw-r--r--   0        0        0     2600 2024-04-15 18:42:10.826053 tibanna_ff-3.3.3.1b1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.176651 tibanna_ff-3.3.3.1b1/tibanna_4dn/__init__.py
--rw-r--r--   0        0        0     9947 2024-01-18 20:28:25.200204 tibanna_ff-3.3.3.1b1/tibanna_4dn/__main__.py
--rw-r--r--   0        0        0     2352 2022-05-12 18:43:14.943285 tibanna_ff-3.3.3.1b1/tibanna_4dn/core.py
--rw-r--r--   0        0        0      317 2021-09-09 16:55:28.177367 tibanna_ff-3.3.3.1b1/tibanna_4dn/iam_utils.py
--rw-r--r--   0        0        0      131 2021-09-23 17:36:29.921830 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/__init__.py
--rw-r--r--   0        0        0      447 2021-09-09 16:55:28.177955 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/check_task.py
--rw-r--r--   0        0        0      106 2023-10-13 15:39:26.771164 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/requirements.txt
--rw-r--r--   0        0        0      435 2021-09-09 16:55:28.178373 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/run_task.py
--rw-r--r--   0        0        0     1066 2023-10-05 20:25:49.983919 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/start_run.py
--rw-r--r--   0        0        0      230 2021-11-02 15:52:14.099351 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/update_cost.py
--rw-r--r--   0        0        0     1252 2023-10-05 20:25:49.984615 tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     6430 2023-05-18 20:05:00.430369 tibanna_ff-3.3.3.1b1/tibanna_4dn/pony_utils.py
--rw-r--r--   0        0        0      934 2022-02-02 21:42:36.484027 tibanna_ff-3.3.3.1b1/tibanna_4dn/start_run.py
--rw-r--r--   0        0        0      318 2021-09-09 16:55:28.180862 tibanna_ff-3.3.3.1b1/tibanna_4dn/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-11-02 15:52:14.100504 tibanna_ff-3.3.3.1b1/tibanna_4dn/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1450 2021-09-09 16:55:28.181306 tibanna_ff-3.3.3.1b1/tibanna_4dn/update_ffmeta.py
--rw-r--r--   0        0        0      863 2024-01-24 20:33:16.205779 tibanna_ff-3.3.3.1b1/tibanna_4dn/vars.py
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.181843 tibanna_ff-3.3.3.1b1/tibanna_cgap/__init__.py
--rw-r--r--   0        0        0     9966 2024-01-18 20:28:25.201217 tibanna_ff-3.3.3.1b1/tibanna_cgap/__main__.py
--rw-r--r--   0        0        0      255 2021-09-09 16:55:28.182378 tibanna_ff-3.3.3.1b1/tibanna_cgap/check_task.py
--rw-r--r--   0        0        0     2769 2022-02-02 21:42:36.486858 tibanna_ff-3.3.3.1b1/tibanna_cgap/core.py
--rw-r--r--   0        0        0      300 2021-09-09 16:55:28.182774 tibanna_ff-3.3.3.1b1/tibanna_cgap/cw_utils.py
--rw-r--r--   0        0        0      318 2021-09-09 16:55:28.182976 tibanna_ff-3.3.3.1b1/tibanna_cgap/iam_utils.py
--rw-r--r--   0        0        0      132 2021-09-16 20:24:20.855907 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/__init__.py
--rw-r--r--   0        0        0      467 2021-09-09 16:55:28.183470 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/check_task.py
--rw-r--r--   0        0        0      125 2024-01-18 20:28:25.202414 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/requirements.txt
--rw-r--r--   0        0        0      436 2021-09-09 16:55:28.183912 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/run_task.py
--rw-r--r--   0        0        0     1069 2023-10-05 20:25:49.986448 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/start_run.py
--rw-r--r--   0        0        0      231 2021-11-02 15:52:14.104064 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/update_cost.py
--rw-r--r--   0        0        0     1286 2023-10-05 20:25:49.987251 tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     1281 2022-02-02 21:42:36.490690 tibanna_ff-3.3.3.1b1/tibanna_cgap/start_run.py
--rw-r--r--   0        0        0      319 2021-09-09 16:55:28.185766 tibanna_ff-3.3.3.1b1/tibanna_cgap/stepfunction.py
--rw-r--r--   0        0        0     1321 2021-11-01 14:42:13.461080 tibanna_ff-3.3.3.1b1/tibanna_cgap/stepfunction_cost_updater.py
--rw-r--r--   0        0        0     1098 2021-09-09 16:55:28.186145 tibanna_ff-3.3.3.1b1/tibanna_cgap/update_ffmeta.py
--rw-r--r--   0        0        0     1106 2024-01-24 20:33:16.206629 tibanna_ff-3.3.3.1b1/tibanna_cgap/vars.py
--rw-r--r--   0        0        0     7783 2024-01-18 20:28:25.203518 tibanna_ff-3.3.3.1b1/tibanna_cgap/zebra_utils.py
--rw-r--r--   0        0        0        0 2021-09-09 16:55:28.186877 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/__init__.py
--rw-r--r--   0        0        0      504 2022-05-12 18:43:14.981898 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/_version.py
--rw-r--r--   0        0        0      677 2021-09-09 16:55:28.187272 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/config.py
--rw-r--r--   0        0        0     4090 2022-12-16 18:49:18.399580 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/core.py
--rw-r--r--   0        0        0     3905 2023-05-04 19:21:43.919773 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/exceptions.py
--rw-r--r--   0        0        0     2314 2023-07-24 20:00:22.501691 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/extra_files.py
--rw-r--r--   0        0        0     2461 2023-12-05 16:52:23.567811 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/file_format.py
--rw-r--r--   0        0        0     9454 2024-01-18 20:28:25.204431 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/generic_qc_utils.py
--rw-r--r--   0        0        0     2197 2024-01-18 20:28:25.205684 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/iam_utils.py
--rw-r--r--   0        0        0    16981 2023-05-01 19:20:54.571865 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/input_files.py
--rw-r--r--   0        0        0     2631 2024-01-18 20:28:25.206190 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/misc_utils.py
--rw-r--r--   0        0        0    80308 2024-03-14 14:07:22.551484 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/portal_utils.py
--rw-r--r--   0        0        0    22815 2023-05-08 18:31:51.928352 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/qc.py
--rw-r--r--   0        0        0     3162 2021-09-09 16:55:28.190327 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/stepfunction.py
--rw-r--r--   0        0        0     3701 2024-04-15 17:36:42.386873 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/vars.py
--rw-r--r--   0        0        0     6579 2023-12-05 16:52:23.574551 tibanna_ff-3.3.3.1b1/tibanna_ffcommon/wfr.py
--rw-r--r--   0        0        0        0 2023-09-06 15:48:58.320465 tibanna_ff-3.3.3.1b1/tibanna_smaht/__init__.py
--rw-r--r--   0        0        0     9926 2024-01-18 20:28:25.209659 tibanna_ff-3.3.3.1b1/tibanna_smaht/__main__.py
--rw-r--r--   0        0        0      231 2023-09-06 15:48:58.322174 tibanna_ff-3.3.3.1b1/tibanna_smaht/check_task.py
--rw-r--r--   0        0        0     2771 2023-09-06 15:48:58.322954 tibanna_ff-3.3.3.1b1/tibanna_smaht/core.py
--rw-r--r--   0        0        0      252 2023-09-06 15:48:58.323332 tibanna_ff-3.3.3.1b1/tibanna_smaht/cw_utils.py
--rw-r--r--   0        0        0      356 2023-09-06 15:48:58.323722 tibanna_ff-3.3.3.1b1/tibanna_smaht/iam_utils.py
--rw-r--r--   0        0        0      133 2023-09-06 15:48:58.324134 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/__init__.py
--rw-r--r--   0        0        0      867 2024-01-18 20:28:25.210376 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/check_task.py
--rw-r--r--   0        0        0      125 2024-01-18 20:28:25.211189 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/requirements.txt
--rw-r--r--   0        0        0      779 2024-01-18 20:28:25.212130 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/run_task.py
--rw-r--r--   0        0        0     1033 2024-01-17 20:43:10.016819 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/start_run.py
--rw-r--r--   0        0        0      594 2024-01-18 20:28:25.212783 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/update_cost.py
--rw-r--r--   0        0        0     1264 2024-01-17 20:43:06.094871 tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/update_ffmeta.py
--rw-r--r--   0        0        0     1243 2023-09-06 15:48:58.326901 tibanna_ff-3.3.3.1b1/tibanna_smaht/start_run.py
--rw-r--r--   0        0        0      319 2023-09-06 15:48:58.327288 tibanna_ff-3.3.3.1b1/tibanna_smaht/stepfunction.py
--rw-r--r--   0        0        0     1321 2023-09-06 15:48:58.327895 tibanna_ff-3.3.3.1b1/tibanna_smaht/stepfunction_cost_updater.py
--rw-r--r--   0        0        0    15557 2024-03-14 14:07:22.552987 tibanna_ff-3.3.3.1b1/tibanna_smaht/tiger_utils.py
--rw-r--r--   0        0        0     1098 2023-09-06 15:48:58.328769 tibanna_ff-3.3.3.1b1/tibanna_smaht/update_ffmeta.py
--rw-r--r--   0        0        0     1135 2024-01-24 20:33:16.211943 tibanna_ff-3.3.3.1b1/tibanna_smaht/vars.py
--rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 tibanna_ff-3.3.3.1b1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2021-09-09 16:55:28.100725 tibanna_ff-3.3.3.1b2/LICENSE.txt
+-rw-r--r--   0        0        0      188 2024-01-18 20:28:25.185806 tibanna_ff-3.3.3.1b2/README.md
+-rw-r--r--   0        0        0     2600 2024-04-16 19:55:18.870961 tibanna_ff-3.3.3.1b2/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.176651 tibanna_ff-3.3.3.1b2/tibanna_4dn/__init__.py
+-rw-r--r--   0        0        0     9947 2024-01-18 20:28:25.200204 tibanna_ff-3.3.3.1b2/tibanna_4dn/__main__.py
+-rw-r--r--   0        0        0     2352 2022-05-12 18:43:14.943285 tibanna_ff-3.3.3.1b2/tibanna_4dn/core.py
+-rw-r--r--   0        0        0      317 2021-09-09 16:55:28.177367 tibanna_ff-3.3.3.1b2/tibanna_4dn/iam_utils.py
+-rw-r--r--   0        0        0      131 2021-09-23 17:36:29.921830 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/__init__.py
+-rw-r--r--   0        0        0      447 2021-09-09 16:55:28.177955 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/check_task.py
+-rw-r--r--   0        0        0      106 2023-10-13 15:39:26.771164 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/requirements.txt
+-rw-r--r--   0        0        0      435 2021-09-09 16:55:28.178373 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/run_task.py
+-rw-r--r--   0        0        0     1066 2023-10-05 20:25:49.983919 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/start_run.py
+-rw-r--r--   0        0        0      230 2021-11-02 15:52:14.099351 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1252 2023-10-05 20:25:49.984615 tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     6430 2023-05-18 20:05:00.430369 tibanna_ff-3.3.3.1b2/tibanna_4dn/pony_utils.py
+-rw-r--r--   0        0        0      934 2022-02-02 21:42:36.484027 tibanna_ff-3.3.3.1b2/tibanna_4dn/start_run.py
+-rw-r--r--   0        0        0      318 2021-09-09 16:55:28.180862 tibanna_ff-3.3.3.1b2/tibanna_4dn/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-11-02 15:52:14.100504 tibanna_ff-3.3.3.1b2/tibanna_4dn/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1450 2021-09-09 16:55:28.181306 tibanna_ff-3.3.3.1b2/tibanna_4dn/update_ffmeta.py
+-rw-r--r--   0        0        0      863 2024-01-24 20:33:16.205779 tibanna_ff-3.3.3.1b2/tibanna_4dn/vars.py
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.181843 tibanna_ff-3.3.3.1b2/tibanna_cgap/__init__.py
+-rw-r--r--   0        0        0     9966 2024-01-18 20:28:25.201217 tibanna_ff-3.3.3.1b2/tibanna_cgap/__main__.py
+-rw-r--r--   0        0        0      255 2021-09-09 16:55:28.182378 tibanna_ff-3.3.3.1b2/tibanna_cgap/check_task.py
+-rw-r--r--   0        0        0     2769 2022-02-02 21:42:36.486858 tibanna_ff-3.3.3.1b2/tibanna_cgap/core.py
+-rw-r--r--   0        0        0      300 2021-09-09 16:55:28.182774 tibanna_ff-3.3.3.1b2/tibanna_cgap/cw_utils.py
+-rw-r--r--   0        0        0      318 2021-09-09 16:55:28.182976 tibanna_ff-3.3.3.1b2/tibanna_cgap/iam_utils.py
+-rw-r--r--   0        0        0      132 2021-09-16 20:24:20.855907 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/__init__.py
+-rw-r--r--   0        0        0      467 2021-09-09 16:55:28.183470 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/check_task.py
+-rw-r--r--   0        0        0      125 2024-01-18 20:28:25.202414 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/requirements.txt
+-rw-r--r--   0        0        0      436 2021-09-09 16:55:28.183912 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/run_task.py
+-rw-r--r--   0        0        0     1069 2023-10-05 20:25:49.986448 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/start_run.py
+-rw-r--r--   0        0        0      231 2021-11-02 15:52:14.104064 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1286 2023-10-05 20:25:49.987251 tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     1281 2022-02-02 21:42:36.490690 tibanna_ff-3.3.3.1b2/tibanna_cgap/start_run.py
+-rw-r--r--   0        0        0      319 2021-09-09 16:55:28.185766 tibanna_ff-3.3.3.1b2/tibanna_cgap/stepfunction.py
+-rw-r--r--   0        0        0     1321 2021-11-01 14:42:13.461080 tibanna_ff-3.3.3.1b2/tibanna_cgap/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0     1098 2021-09-09 16:55:28.186145 tibanna_ff-3.3.3.1b2/tibanna_cgap/update_ffmeta.py
+-rw-r--r--   0        0        0     1106 2024-01-24 20:33:16.206629 tibanna_ff-3.3.3.1b2/tibanna_cgap/vars.py
+-rw-r--r--   0        0        0     7783 2024-01-18 20:28:25.203518 tibanna_ff-3.3.3.1b2/tibanna_cgap/zebra_utils.py
+-rw-r--r--   0        0        0        0 2021-09-09 16:55:28.186877 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/__init__.py
+-rw-r--r--   0        0        0      504 2022-05-12 18:43:14.981898 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/_version.py
+-rw-r--r--   0        0        0      677 2021-09-09 16:55:28.187272 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/config.py
+-rw-r--r--   0        0        0     4090 2022-12-16 18:49:18.399580 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/core.py
+-rw-r--r--   0        0        0     3905 2023-05-04 19:21:43.919773 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/exceptions.py
+-rw-r--r--   0        0        0     2314 2023-07-24 20:00:22.501691 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/extra_files.py
+-rw-r--r--   0        0        0     2461 2023-12-05 16:52:23.567811 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/file_format.py
+-rw-r--r--   0        0        0     9454 2024-01-18 20:28:25.204431 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/generic_qc_utils.py
+-rw-r--r--   0        0        0     2197 2024-01-18 20:28:25.205684 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/iam_utils.py
+-rw-r--r--   0        0        0    16981 2023-05-01 19:20:54.571865 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/input_files.py
+-rw-r--r--   0        0        0     2631 2024-01-18 20:28:25.206190 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/misc_utils.py
+-rw-r--r--   0        0        0    80308 2024-03-14 14:07:22.551484 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/portal_utils.py
+-rw-r--r--   0        0        0    22815 2023-05-08 18:31:51.928352 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/qc.py
+-rw-r--r--   0        0        0     3162 2021-09-09 16:55:28.190327 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/stepfunction.py
+-rw-r--r--   0        0        0     3692 2024-04-16 19:55:02.059573 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/vars.py
+-rw-r--r--   0        0        0     6579 2023-12-05 16:52:23.574551 tibanna_ff-3.3.3.1b2/tibanna_ffcommon/wfr.py
+-rw-r--r--   0        0        0        0 2023-09-06 15:48:58.320465 tibanna_ff-3.3.3.1b2/tibanna_smaht/__init__.py
+-rw-r--r--   0        0        0     9926 2024-01-18 20:28:25.209659 tibanna_ff-3.3.3.1b2/tibanna_smaht/__main__.py
+-rw-r--r--   0        0        0      231 2023-09-06 15:48:58.322174 tibanna_ff-3.3.3.1b2/tibanna_smaht/check_task.py
+-rw-r--r--   0        0        0     2771 2023-09-06 15:48:58.322954 tibanna_ff-3.3.3.1b2/tibanna_smaht/core.py
+-rw-r--r--   0        0        0      252 2023-09-06 15:48:58.323332 tibanna_ff-3.3.3.1b2/tibanna_smaht/cw_utils.py
+-rw-r--r--   0        0        0      356 2023-09-06 15:48:58.323722 tibanna_ff-3.3.3.1b2/tibanna_smaht/iam_utils.py
+-rw-r--r--   0        0        0      133 2023-09-06 15:48:58.324134 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/__init__.py
+-rw-r--r--   0        0        0      867 2024-01-18 20:28:25.210376 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/check_task.py
+-rw-r--r--   0        0        0      125 2024-01-18 20:28:25.211189 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/requirements.txt
+-rw-r--r--   0        0        0      779 2024-01-18 20:28:25.212130 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/run_task.py
+-rw-r--r--   0        0        0     1033 2024-01-17 20:43:10.016819 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/start_run.py
+-rw-r--r--   0        0        0      594 2024-01-18 20:28:25.212783 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/update_cost.py
+-rw-r--r--   0        0        0     1264 2024-01-17 20:43:06.094871 tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/update_ffmeta.py
+-rw-r--r--   0        0        0     1243 2023-09-06 15:48:58.326901 tibanna_ff-3.3.3.1b2/tibanna_smaht/start_run.py
+-rw-r--r--   0        0        0      319 2023-09-06 15:48:58.327288 tibanna_ff-3.3.3.1b2/tibanna_smaht/stepfunction.py
+-rw-r--r--   0        0        0     1321 2023-09-06 15:48:58.327895 tibanna_ff-3.3.3.1b2/tibanna_smaht/stepfunction_cost_updater.py
+-rw-r--r--   0        0        0    15557 2024-03-14 14:07:22.552987 tibanna_ff-3.3.3.1b2/tibanna_smaht/tiger_utils.py
+-rw-r--r--   0        0        0     1098 2023-09-06 15:48:58.328769 tibanna_ff-3.3.3.1b2/tibanna_smaht/update_ffmeta.py
+-rw-r--r--   0        0        0     1135 2024-01-24 20:33:16.211943 tibanna_ff-3.3.3.1b2/tibanna_smaht/vars.py
+-rw-r--r--   0        0        0     1516 1970-01-01 00:00:00.000000 tibanna_ff-3.3.3.1b2/PKG-INFO
```

### Comparing `tibanna_ff-3.3.3.1b1/LICENSE.txt` & `tibanna_ff-3.3.3.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/pyproject.toml` & `tibanna_ff-3.3.3.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tibanna_ff"
-version = "3.3.3.1b1"
+version = "3.3.3.1b2"
 description = "Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tibanna"]
 homepage = "http://github.com/4dn-dcic/tibanna_ff"
 repository = "http://github.com/4dn-dcic/tibanna_ff.git"
```

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/__main__.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/core.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/lambdas/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/pony_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/pony_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/stepfunction_cost_updater.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_4dn/vars.py` & `tibanna_ff-3.3.3.1b2/tibanna_4dn/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/__main__.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/core.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/lambdas/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/stepfunction_cost_updater.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/vars.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_cgap/zebra_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_cgap/zebra_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/config.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/config.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/core.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/exceptions.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/exceptions.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/extra_files.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/extra_files.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/file_format.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/file_format.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/generic_qc_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/generic_qc_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/iam_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/iam_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/input_files.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/input_files.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/misc_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/misc_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/portal_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/portal_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/qc.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/qc.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/stepfunction.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/stepfunction.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/vars.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/vars.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # accounts
 AMI_PER_REGION = {
     'x86': {
         'us-east-1': 'ami-0afc2a6bf9a8c35c6',
         'us-east-2': 'ami-0afbf1ab3268ddf17' # UPDATE
     },
     'Arm': {
-        'us-east-1': 'ami-00936b73c712e5a11', # UPDATE
+        'us-east-1': 'ami-09f3bc14f693e6e25',
         'us-east-2': 'ami-00420b06b90527d69' # UPDATE
     }
 }
 
 if AWS_REGION not in AMI_PER_REGION['x86']:
     logger.warning("Secure Tibanna AMI for region %s is not available." % AWS_REGION)
     raise Exception('')
```

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_ffcommon/wfr.py` & `tibanna_ff-3.3.3.1b2/tibanna_ffcommon/wfr.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/__main__.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/__main__.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/core.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/core.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/check_task.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/check_task.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/run_task.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/run_task.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/update_cost.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/update_cost.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/lambdas/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/lambdas/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/start_run.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/start_run.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/stepfunction_cost_updater.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/stepfunction_cost_updater.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/tiger_utils.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/tiger_utils.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/update_ffmeta.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/update_ffmeta.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/tibanna_smaht/vars.py` & `tibanna_ff-3.3.3.1b2/tibanna_smaht/vars.py`

 * *Files identical despite different names*

### Comparing `tibanna_ff-3.3.3.1b1/PKG-INFO` & `tibanna_ff-3.3.3.1b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tibanna-ff
-Version: 3.3.3.1b1
+Version: 3.3.3.1b2
 Summary: Tibanna runs portable pipelines (in CWL/WDL) on the AWS Cloud.
 Home-page: http://github.com/4dn-dcic/tibanna_ff
 License: MIT
 Keywords: tibanna
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
```

