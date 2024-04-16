# Comparing `tmp/rx_hqm-0.1.3.tar.gz` & `tmp/rx_hqm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rx_hqm-0.1.3.tar", last modified: Wed Feb  7 13:36:02 2024, max compression
+gzip compressed data, was "rx_hqm-0.1.4.tar", last modified: Tue Apr 16 03:06:25 2024, max compression
```

## Comparing `rx_hqm-0.1.3.tar` & `rx_hqm-0.1.4.tar`

### file list

```diff
@@ -1,355 +1,406 @@
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3639 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/.gitignore
--rw-r--r--   0 acampove  (1000) acampove  (1000)      258 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2310 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/README.md
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.478520 rx_hqm-0.1.3/hqm/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/__init__.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/data_sample/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6548 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm/data_sample/add_selection.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      486 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/add_selection_script.sh
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7322 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm/data_sample/apply_preselection.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1421 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/job_sel
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      924 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/submit_add_selection.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1644 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/submit_all_ee.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3373 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/submit_all_mm.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1416 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/submit_sel
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12000 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/data_sample/truth_match.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/model/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2575 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/model/KDE_shape.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      305 2024-01-22 16:06:03.000000 rx_hqm-0.1.3/hqm/model/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4400 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/model/part_reco.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1283 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/model/plot_rare_part_reco.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1503 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/model/rare_part_reco.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    20187 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/model/signal.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/part_reco/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    13851 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/convolution_shape.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    11612 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/fit_convolution.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/part_reco/mm_comb/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4489 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm/part_reco/mm_comb/comb_shape_mm.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      328 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/part_reco/mm_comb/run_mm.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      385 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/part_reco/run_convolution_shape.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      381 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm/part_reco/run_fit.sh
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.468520 rx_hqm-0.1.3/hqm/part_reco/systematic/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5105 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/convolution_shape_sys1.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8201 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/fit_convolution_sys1.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      395 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/run_convolution_shape_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      668 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/run_fit_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      852 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/submit_fit_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      245 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/run_all.sh
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/signal/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4512 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/fit_Bu2Kee_MC.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3657 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/fit_Bu2Kmm_MC.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      355 2024-01-15 11:41:04.000000 rx_hqm-0.1.3/hqm/signal/run_ee.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      166 2024-01-15 11:41:04.000000 rx_hqm-0.1.3/hqm/signal/run_mm.sh
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.468520 rx_hqm-0.1.3/hqm/signal/systematic/
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.488520 rx_hqm-0.1.3/hqm/signal/systematic/sys1/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3303 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/fit_Bu2Kee_MC_sys1.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1629 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/fit_Bu2Kmm_MC_sys1.py
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      383 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/run_ee_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      280 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/run_mm_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      805 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/submit_ee_sys1.sh
--rwxrwxr-x   0 acampove  (1000) acampove  (1000)      563 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/signal/systematic/sys1/submit_mm_sys1.sh
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.498520 rx_hqm-0.1.3/hqm/tools/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm/tools/Cut.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5286 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm/tools/fit.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2279 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm/tools/selection.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3269 2024-02-07 13:16:05.000000 rx_hqm-0.1.3/hqm/tools/utility.py
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/hqm_data/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    13962 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     5570 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6113 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10271 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3593 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1084 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1776 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6410 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18875 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9465 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10210 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    15942 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7119 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3046 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4304 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    14262 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     8116 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     3797 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     4906 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12017 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2600 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      882 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1587 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10147 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    43243 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10967 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    21769 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    31857 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    11438 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2484 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     6856 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    22379 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    42343 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12558 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    34133 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    27294 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12368 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     2708 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    11218 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    21264 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    31469 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1110 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      438 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    69627 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    34345 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    29536 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    10770 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bdks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      944 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bpk1.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      487 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bpk2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18176 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bpks.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12387 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bsphi.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    24203 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2011_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2011_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2012_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2012_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2015_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2015_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2016_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2016_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       92 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/MC_brem_fraction_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/hqm_data/__init__.py
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2011_B_M_NoBDTprc_jpsi_2011_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1198 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2012_B_M_NoBDTprc_jpsi_2012_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1201 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2015_B_M_NoBDTprc_jpsi_2015_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2016_B_M_NoBDTprc_jpsi_2016_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1201 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2017_B_M_NoBDTprc_jpsi_2017_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2018_B_M_NoBDTprc_jpsi_2018_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1198 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2011_B_M_NoBDTprc_psi2_2011_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1196 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2012_B_M_NoBDTprc_psi2_2012_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1196 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2015_B_M_NoBDTprc_psi2_2015_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1205 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2016_B_M_NoBDTprc_psi2_2016_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1197 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2017_B_M_NoBDTprc_psi2_2017_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2018_B_M_NoBDTprc_psi2_2018_B_M_NoBDTprc_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      790 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      790 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      787 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      788 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      794 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      793 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      788 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1481 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1490 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1496 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1490 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1492 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1507 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1498 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1503 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1500 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1500 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_ETOS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1507 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_GTIS_fit_result.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1037 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      445 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1049 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      444 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      941 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1029 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1045 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1047 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1036 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1038 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      954 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1036 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1044 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1040 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1033 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1029 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      693 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      691 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      703 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1431 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1430 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1437 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1427 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1425 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1421 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1416 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1440 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1432 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1435 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1437 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1439 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1419 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1425 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1444 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1056 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2011_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2012_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1050 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2015_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1055 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2016_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1057 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1056 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      891 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2017_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      889 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2018_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      887 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_all_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      881 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      890 2024-02-03 12:18:52.000000 rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)   596948 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2011_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)  1070576 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2012_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)   308429 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2015_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)  1989533 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2016_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)  1628390 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2017_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)  1711797 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2018_psi2.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    12078 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2011_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    18733 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2012_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    14128 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2015_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    37420 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2016_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    32061 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2017_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    34687 2024-02-03 12:18:53.000000 rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2018_high.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     7032 2024-02-03 12:18:43.000000 rx_hqm-0.1.3/hqm_data/signal_scales.json
--rw-rw-r--   0 acampove  (1000) acampove  (1000)      527 2024-02-07 13:35:46.000000 rx_hqm-0.1.3/pyproject.toml
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       73 2024-01-13 17:14:56.000000 rx_hqm-0.1.3/requirements.txt
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/rx_hqm.egg-info/
--rw-r--r--   0 acampove  (1000) acampove  (1000)      258 2024-02-07 13:36:01.000000 rx_hqm-0.1.3/rx_hqm.egg-info/PKG-INFO
--rw-rw-r--   0 acampove  (1000) acampove  (1000)    20653 2024-02-07 13:36:02.000000 rx_hqm-0.1.3/rx_hqm.egg-info/SOURCES.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-02-07 13:36:01.000000 rx_hqm-0.1.3/rx_hqm.egg-info/dependency_links.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       73 2024-02-07 13:36:01.000000 rx_hqm-0.1.3/rx_hqm.egg-info/requires.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       13 2024-02-07 13:36:01.000000 rx_hqm-0.1.3/rx_hqm.egg-info/top_level.txt
--rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/setup.cfg
-drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-02-07 13:36:02.528520 rx_hqm-0.1.3/tests/
--rw-rw-r--   0 acampove  (1000) acampove  (1000)     9705 2024-02-07 13:30:46.000000 rx_hqm-0.1.3/tests/test_pdf.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3639 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/.gitignore
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      258 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2310 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/README.md
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/check/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/check/part_reco/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3259 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/check/part_reco/Bd2Kspsi2S_MC_highq2_check.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2599 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/check/part_reco/Jpsi_region.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5313 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/check/part_reco/check_psi2S_left_tail.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7985 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/check/part_reco/psi2S_region.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5901 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/check/part_reco/simultaneous_fit.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/data_sample/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6609 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/add_selection.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      486 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/add_selection_script.sh
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7322 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/apply_preselection.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1421 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/job_sel
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      936 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/submit_add_selection.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1806 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/submit_all_ee.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3532 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/submit_all_mm.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1416 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/submit_sel
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12338 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/data_sample/truth_match.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/model/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/model/KDE_shape.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      305 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/model/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5153 2024-04-15 12:37:26.000000 rx_hqm-0.1.4/hqm/model/part_reco.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1960 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/model/plot_rare_part_reco.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1503 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/model/rare_part_reco.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    20187 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/model/signal.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/part_reco/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    13905 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/convolution_shape.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    11612 2024-04-16 02:10:14.000000 rx_hqm-0.1.4/hqm/part_reco/fit_convolution.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/part_reco/mm_comb/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4489 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/mm_comb/comb_shape_mm.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      328 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/mm_comb/run_mm.sh
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/part_reco/ratio/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4003 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/fit_MC.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4956 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/fully_reco_shape.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      352 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/run_fit_MC.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      192 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/run_fully_reco_shape.sh
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    11358 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/simultaneous_fit.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      287 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/simultaneous_fit_script.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      584 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/ratio/submit_simultaneous_fit.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      385 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/run_convolution_shape.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      381 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/run_fit.sh
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/part_reco/systematic/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5105 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/convolution_shape_sys1.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8201 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/fit_convolution_sys1.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      395 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/run_convolution_shape_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      668 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/run_fit_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      852 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/submit_fit_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      245 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/run_all.sh
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/signal/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4512 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/fit_Bu2Kee_MC.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3657 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/fit_Bu2Kmm_MC.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      355 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/run_ee.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      166 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/run_mm.sh
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/signal/systematic/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.189926 rx_hqm-0.1.4/hqm/signal/systematic/sys1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3303 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/fit_Bu2Kee_MC_sys1.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1629 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/fit_Bu2Kmm_MC_sys1.py
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      383 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/run_ee_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      280 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/run_mm_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      805 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/submit_ee_sys1.sh
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      563 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/signal/systematic/sys1/submit_mm_sys1.sh
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.200760 rx_hqm-0.1.4/hqm/tools/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/tools/Cut.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5466 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/tools/fit.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12002 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/tools/plot.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2279 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm/tools/selection.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4004 2024-04-16 02:12:02.000000 rx_hqm-0.1.4/hqm/tools/utility.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/hqm_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    13962 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5570 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6113 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10271 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3593 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1084 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1776 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6410 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18875 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9465 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10210 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    15942 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7119 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3046 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4304 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    14262 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8116 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3797 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4906 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12017 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2600 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      882 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1587 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10147 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    43243 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10967 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    21769 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    31857 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    11438 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2484 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6856 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    22379 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    42343 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1540 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      575 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12558 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    34133 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    27294 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12368 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1016 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2708 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    11218 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    21264 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    31469 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1110 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      438 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    69627 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    34345 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    29536 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10770 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bdks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      944 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bpk1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      487 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bpk2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18176 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bpks.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12387 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bsphi.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    24203 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2011_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2011_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2012_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2012_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2015_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2015_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2016_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2016_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       95 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       92 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       93 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       94 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/MC_brem_fraction_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2011_B_M_NoBDTprc_jpsi_2011_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1198 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2012_B_M_NoBDTprc_jpsi_2012_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1201 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2015_B_M_NoBDTprc_jpsi_2015_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2016_B_M_NoBDTprc_jpsi_2016_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1201 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2017_B_M_NoBDTprc_jpsi_2017_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2018_B_M_NoBDTprc_jpsi_2018_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1198 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2011_B_M_NoBDTprc_psi2_2011_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1196 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2012_B_M_NoBDTprc_psi2_2012_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1196 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2015_B_M_NoBDTprc_psi2_2015_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1205 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2016_B_M_NoBDTprc_psi2_2016_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1197 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2017_B_M_NoBDTprc_psi2_2017_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1202 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2018_B_M_NoBDTprc_psi2_2018_B_M_NoBDTprc_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1153 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1154 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1156 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1155 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1159 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1156 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1155 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1153 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1161 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1153 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1158 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1156 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1158 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      553 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1163 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1156 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      557 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1158 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      790 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      790 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      787 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      788 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      794 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      793 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      789 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      788 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      791 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1172 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1180 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1179 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1173 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1173 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1180 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1481 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1482 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1490 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1496 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1495 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1490 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1489 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1487 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1483 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1484 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1485 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1492 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1493 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1497 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1507 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1498 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1488 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1503 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1500 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1491 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1500 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_ETOS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1507 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_GTIS_fit_result.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1037 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      445 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1049 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      444 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      941 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1029 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1045 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1047 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1036 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1038 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      954 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1036 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1039 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1044 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1040 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1033 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1028 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1029 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1043 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1041 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      696 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      693 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      691 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      702 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      703 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1431 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1430 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1437 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1427 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1425 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1421 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1416 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1440 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1432 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1435 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1437 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1439 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1419 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1425 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1434 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1444 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1056 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2011_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2012_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1050 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2015_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1055 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2016_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1057 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1056 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1042 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1053 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      891 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      889 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      887 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      881 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      890 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)   596948 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2011_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)  1070576 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2012_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)   308429 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2015_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)  1989533 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2016_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)  1628390 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2017_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)  1711797 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2018_psi2.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12078 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2011_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18733 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2012_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    14128 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2015_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    37420 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2016_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    32061 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2017_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    34687 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2018_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5471 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2011_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12474 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2012_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9121 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2015_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    19577 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2016_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18146 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2017_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    20552 2024-04-15 11:22:53.000000 rx_hqm-0.1.4/hqm_data/get_data_psi2_GTIS_2018_high.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       51 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/psi2S_ratio_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       53 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/psi2S_ratio_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       52 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/psi2S_ratio_all.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       52 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/psi2S_ratio_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       52 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/psi2S_ratio_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7032 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/hqm_data/signal_scales.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      527 2024-04-16 03:06:19.000000 rx_hqm-0.1.4/pyproject.toml
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       73 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/requirements.txt
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/rx_hqm.egg-info/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      258 2024-04-16 03:06:25.000000 rx_hqm-0.1.4/rx_hqm.egg-info/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    23585 2024-04-16 03:06:25.000000 rx_hqm-0.1.4/rx_hqm.egg-info/SOURCES.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-16 03:06:25.000000 rx_hqm-0.1.4/rx_hqm.egg-info/dependency_links.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       73 2024-04-16 03:06:25.000000 rx_hqm-0.1.4/rx_hqm.egg-info/requires.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       13 2024-04-16 03:06:25.000000 rx_hqm-0.1.4/rx_hqm.egg-info/top_level.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/setup.cfg
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-16 03:06:25.233260 rx_hqm-0.1.4/tests/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9693 2024-04-15 11:22:54.000000 rx_hqm-0.1.4/tests/test_pdf.py
```

### Comparing `rx_hqm-0.1.3/.gitignore` & `rx_hqm-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/README.md` & `rx_hqm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/data_sample/add_selection.py` & `rx_hqm-0.1.4/hqm/data_sample/add_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import awkward as ak
 from logzero import logger
 from hqm.tools.utility import get_project_root
 import os
 import argparse
 from hqm.tools.Cut import Cut
 from hqm.data_sample.truth_match import truth_match
+import gc
 
 
 class selector:
     def __init__(self, q2, mass, kind, year, version, trigger, target_dir, input_dir):
         self._q2 = q2
         self._mass = mass
         self._kind = kind
@@ -163,14 +164,16 @@
     ]
     for q2 in all_q2:
         for mass in all_mass:
             for trigger in all_trigger:
                 logger.info(f"Processing {kind} {q2} {mass} {year} {version} {trigger}")
                 s = selector(q2, mass, kind, year, version, trigger, target_dir, input_dir)
                 s.save()
+                del s
+                gc.collect()
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--kind", type=str)
     parser.add_argument("--version", type=str)
     parser.add_argument("--year", type=str)
```

### Comparing `rx_hqm-0.1.3/hqm/data_sample/apply_preselection.py` & `rx_hqm-0.1.4/hqm/data_sample/apply_preselection.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/data_sample/job_sel` & `rx_hqm-0.1.4/hqm/data_sample/job_sel`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/data_sample/submit_add_selection.sh` & `rx_hqm-0.1.4/hqm/data_sample/submit_add_selection.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env bash
 
-all_kind=("data" "sign" "ctrl" "psi2" "bpks" "bdks" "bdkpi" "bpk1" "bpk2" "bsphi")
+all_kind=("data" "sign" "ctrl" "psi2" "bpks" "bdks" "bdkpi" "bpk1" "bpk2" "bsphi" "bdpsi2kst")
 all_version=("v10.21p2")
 all_year=("2011" "2012" "2015" "2016" "2017" "2018")
 
 SUMBIT_SCRIPT="/afs/ihep.ac.cn/users/q/qi/work/projects/RK/high_q2_model/hqm/data_sample/add_selection_script.sh"
 
 
 for kind in ${all_kind[@]}; do
```

### Comparing `rx_hqm-0.1.3/hqm/data_sample/submit_all_ee.sh` & `rx_hqm-0.1.4/hqm/data_sample/submit_all_ee.sh`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 OUTPUT_DIR="root_sample"
 WAIT_TIME="mid"
 JOB_SEL_SCRIPT="/afs/ihep.ac.cn/users/q/qi/work/projects/RK/high_q2_model/hqm/data_sample/job_sel"
 
 for year in 2011 2012 2015 2016 2017 2018; do
     for trigger in "ETOS" "GTIS"; do
-        $JOB_SEL_SCRIPT -p data_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt-pid -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p data_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt-pid -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
 
-        $JOB_SEL_SCRIPT -p sign_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p ctrl_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p psi2_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p sign_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p ctrl_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p psi2_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
 
-        $JOB_SEL_SCRIPT -p bpks_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p bdks_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p bdkpi_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bpks_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bdks_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bdkpi_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
 
-        $JOB_SEL_SCRIPT -p bpk1_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 2 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p bpk2_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 2 -w $WAIT_TIME
-        $JOB_SEL_SCRIPT -p bsphi_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 5 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bpk1_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 2 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bpk2_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 2 -w $WAIT_TIME
+        # $JOB_SEL_SCRIPT -p bsphi_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 5 -w $WAIT_TIME
+        $JOB_SEL_SCRIPT -p bdpsi2kst_ee -v v10.21p2 -d $year -t $trigger -q high -r q2-mass-truth-bdt -f $OUTPUT_DIR -b 1 -n 10 -w $WAIT_TIME
     done
 done
```

### Comparing `rx_hqm-0.1.3/hqm/data_sample/submit_all_mm.sh` & `rx_hqm-0.1.4/hqm/data_sample/submit_all_mm.sh`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 OUTPUT_DIR="root_sample"
 WAIT_TIME="mid"
 JOB_SEL_SCRIPT="/afs/ihep.ac.cn/users/q/qi/work/projects/RK/high_q2_model/hqm/data_sample/job_sel"
 
 # 2018
 for year in 2011 2012 2015 2016 2017 2018; do
-    $JOB_SEL_SCRIPT -p data_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME -c 0
+    # $JOB_SEL_SCRIPT -p data_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME -c 0
 
-    $JOB_SEL_SCRIPT -p sign_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
-    $JOB_SEL_SCRIPT -p ctrl_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
-    $JOB_SEL_SCRIPT -p psi2_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME -c 0
+    # $JOB_SEL_SCRIPT -p sign_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
+    # $JOB_SEL_SCRIPT -p ctrl_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
+    # $JOB_SEL_SCRIPT -p psi2_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME -c 0
+
+    $JOB_SEL_SCRIPT -p bdpsi2kst_mm -v v10.21p2 -d $year -t MTOS -q high -r truth-q2-mass-bdt-jpsi_misid -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME -c 0
 done
 
 # $JOB_SEL_SCRIPT -p bp_x -v v10.17 -d 2016 -t MTOS -q high -r q2-mass-bdt -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
 # $JOB_SEL_SCRIPT -p bd_x -v v10.17 -d 2016 -t MTOS -q high -r q2-mass-bdt -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
 # $JOB_SEL_SCRIPT -p bs_x -v v10.17 -d 2016 -t MTOS -q high -r q2-mass-bdt -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
 
 # $JOB_SEL_SCRIPT -p bpks -v v10.18is -d 2018 -t MTOS -q high -r q2-mass -f $OUTPUT_DIR -b 0 -n 10 -w $WAIT_TIME
```

### Comparing `rx_hqm-0.1.3/hqm/data_sample/submit_sel` & `rx_hqm-0.1.4/hqm/data_sample/submit_sel`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/data_sample/truth_match.py` & `rx_hqm-0.1.4/hqm/data_sample/truth_match.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             truth_cut = (
                 cls.Bu
                 & cls.psi2S2ee
                 & cls.Kp
                 & cls.Ksp
                 & Cut(lambda x: (abs(x.H_MC_GD_MOTHER_ID) == cls.Bu_id) & (abs(x.Jpsi_MC_MOTHER_ID) == cls.Bu_id))
             )
-        elif kind in ["11154011", "psi2Kstr"]:
+        elif kind in ["11154011", "psi2Kstr", "bdpsi2kst"]:
             # B0 -> psi2S K*0
             truth_cut = (
                 cls.Bd
                 & cls.psi2S2ee
                 & cls.Kp
                 & cls.Ks0
                 & Cut(lambda x: (abs(x.H_MC_GD_MOTHER_ID) == cls.Bd_id) & (abs(x.Jpsi_MC_MOTHER_ID) == cls.Bd_id))
@@ -306,14 +306,24 @@
                 & cls.Kp
                 & Cut(
                     lambda x: (abs(x.H_MC_GD_MOTHER_ID) == cls.Bu_id)
                     & (abs(x.H_MC_MOTHER_ID) == cls.K1p_id)
                     & (abs(x.Jpsi_MC_MOTHER_ID) == cls.Bu_id)
                 )
             )
+
+        elif kind == "bdpsi2kst":
+            # B0 -> psi2S K*0
+            truth_cut = (
+                cls.Bd
+                & cls.psi2S2mm
+                & cls.Kp
+                & cls.Ks0
+                & Cut(lambda x: (abs(x.H_MC_GD_MOTHER_ID) == cls.Bd_id) & (abs(x.Jpsi_MC_MOTHER_ID) == cls.Bd_id))
+            )
         else:
             raise ValueError(f"Unknown kind: {kind} for mm")
 
         return truth_cut
 
     @classmethod
     def get_truth(cls, kind, is_e):
```

### Comparing `rx_hqm-0.1.3/hqm/model/KDE_shape.py` & `rx_hqm-0.1.4/hqm/model/KDE_shape.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/model/part_reco.py` & `rx_hqm-0.1.4/hqm/model/part_reco.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from hqm.part_reco.convolution_shape import get_convolution_shape
 from hqm.part_reco.systematic.sys1.convolution_shape_sys1 import get_convolution_shape_sys1
+from hqm.tools.utility import load_pickle
+from hqm.tools.utility import cache_json
+from hqm.tools.utility import get_project_root
 from .KDE_shape import get_KDE_shape
 from hqm.tools.utility import get_lumi
 from logzero import logger
 import zfit
 
 
 def get_shape(dataset, trigger, func, *, parameter_name_prefix="", pdf_name="", **kwargs):
@@ -27,60 +30,68 @@
             for year in years
         ]
         lumis = [get_lumi(year) for year in years]
         sum_lumis = sum(lumis)
         frac = [lumi / sum_lumis for lumi in lumis[:-1]]
 
         pdfs = []
-        ratios = []
+        # ratios = []
         for i, value in enumerate(values):
-            pdf, ratio = value
+            pdf = value
             pdfs.append(pdf)
-            ratios.append(ratio * lumis[i])
+            # ratios.append(ratio * lumis[i])
         total_pdf = zfit.pdf.SumPDF(pdfs, fracs=frac, name=f"{pdf_name}_{dataset}_{trigger}")
-        average_ratio = sum(ratios) / sum_lumis
-        return_value = (total_pdf, average_ratio)
+        # average_ratio = sum(ratios) / sum_lumis
+        # return_value = (total_pdf, average_ratio)
+        return_value = total_pdf
 
     return return_value
 
 
 def _get_part_reco(year="2018", trigger="ETOS", parameter_name_prefix="", pdf_name="", systematic="nom"):
     parameter_name_prefix = parameter_name_prefix + "_" if parameter_name_prefix != "" else ""
     suffix = f"{year}_{trigger}"
 
     if systematic == "nom":
-        psi2S_part_reco_shape, psi2S_ratio, _ = get_convolution_shape(
+        psi2S_part_reco_shape, _, _ = get_convolution_shape(
             kind="psi2S_high",
             year=year,
             trigger=trigger,
             parameter_name_prefix=parameter_name_prefix.removesuffix("_"),
         )
     elif systematic == "sys1":
-        psi2S_part_reco_shape, psi2S_ratio, _ = get_convolution_shape_sys1(
+        psi2S_part_reco_shape, _, _ = get_convolution_shape_sys1(
             kind="psi2S_high",
             year=year,
             trigger=trigger,
             parameter_name_prefix=parameter_name_prefix.removesuffix("_"),
         )
     else:
         raise ValueError(f"Invalid systematic: {systematic}")
 
     for param in psi2S_part_reco_shape.get_params():
         param.floating = False
 
-    mass_window = (4500, 6000)
+    return psi2S_part_reco_shape
+
 
-    psi2S_ratio *= psi2S_part_reco_shape.integrate(mass_window)[0]
+def get_ratio(dataset):
+    pickle_path = (
+        get_project_root() + f"data/part_reco/ratio/simultaneous_fit/latest/simultaneous_fit_result_{dataset}.pickle"
+    )
+    obj = load_pickle(pickle_path)
+    ratio = obj.params[f"psi2S_ratio_{dataset}"]["value"]
+    error = obj.params[f"psi2S_ratio_{dataset}"]["hesse"]["error"]
 
-    return psi2S_part_reco_shape, psi2S_ratio
+    return [ratio, error]
 
 
 def get_part_reco(dataset="2018", trigger="ETOS", parameter_name_prefix="", systematic="nom", bts_index=0):
     parameter_name_prefix = parameter_name_prefix + "_" if parameter_name_prefix != "" else ""
-    part_reco_shape, ratio = get_shape(
+    part_reco_shape = get_shape(
         dataset,
         trigger,
         _get_part_reco,
         parameter_name_prefix=parameter_name_prefix,
         pdf_name="part_reco",
         systematic=systematic,
     )
@@ -95,20 +106,27 @@
 
     obs = zfit.Space("B_M", limits=(4500, 6000))
     part_reco_shape_hist_pdf_unbinned = zfit.pdf.SplinePDF(part_reco_shape_hist_pdf, obs=obs)
 
     psi2SK_shape = get_KDE_shape(
         obs, "psi2", "high", bandwidth=None, dataset=dataset, trigger=trigger, pdf_name="psi2SK", bts_index=bts_index
     )
-    ratio /= psi2SK_shape.integrate(mass_window)[0]
+
+    @cache_json(f"psi2S_ratio_{dataset}.json")
+    def _get_ratio():
+        return get_ratio(dataset)
+
+    ratio_and_error = _get_ratio()
+    ratio = ratio_and_error[0]
+    ratio_error = ratio_and_error[1]
+    ratio = ratio * part_reco_shape.integrate(mass_window)[0] / psi2SK_shape.integrate(mass_window)[0]
+    ratio_error = ratio_error * part_reco_shape.integrate(mass_window)[0] / psi2SK_shape.integrate(mass_window)[0]
 
     suffix = f"{dataset}_{trigger}_{systematic}_{bts_index}"
     psi2S_ratio_param = zfit.Parameter(f"{parameter_name_prefix}psi2S_ratio_{suffix}", ratio, 0.1, 10)
-    frac = zfit.param.ComposedParameter(
-        f"{parameter_name_prefix}frac_{suffix}", lambda p: p / (p + 1), psi2S_ratio_param
-    )
+    frac = zfit.param.ComposedParameter(f'{parameter_name_prefix}frac_{suffix}', func=lambda p: p / (p + 1), params=psi2S_ratio_param)
 
     total_pdf = zfit.pdf.SumPDF(
         [part_reco_shape_hist_pdf_unbinned, psi2SK_shape], fracs=[frac], name=f"part_reco_{suffix}"
     )
 
-    return total_pdf, {psi2S_ratio_param.name: [zfit.run(ratio), zfit.run(ratio) * 0.1]}
+    return total_pdf, {psi2S_ratio_param.name: [zfit.run(ratio), zfit.run(ratio_error)]}
```

### Comparing `rx_hqm-0.1.3/hqm/model/rare_part_reco.py` & `rx_hqm-0.1.4/hqm/model/rare_part_reco.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/model/signal.py` & `rx_hqm-0.1.4/hqm/model/signal.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/convolution_shape.py` & `rx_hqm-0.1.4/hqm/part_reco/convolution_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,18 +60,21 @@
 
     correction_right_CB = zfit.pdf.CrystalBall(
         obs=obs, mu=mu, sigma=sigma, alpha=alpha, n=n, name=f"{parameter_name_prefix}correction_right_CB_{suffix}"
     )
     return correction_right_CB
 
 
-def load_pdf(pickle_path: str, pdf, parameter_name_prefix=""):
+def load_pdf(pickle_path: str, pdf, parameter_name_prefix="", cache_json_p=True):
     parameter_name_prefix = parameter_name_prefix + "_" if parameter_name_prefix != "" else ""
 
-    json_path = pickle_path.replace("/", "_").removesuffix("pickle") + "json"
+    if cache_json_p:
+        json_path = pickle_path.replace("/", "_").removesuffix("pickle") + "json"
+    else:
+        json_path = None
 
     @cache_json(json_path)
     def _get_params():
         _pickle_path = get_project_root() + pickle_path
         obj = load_pickle(_pickle_path)
         fit_result = obj["result"]
         params_value = dict(fit_result.params)
@@ -298,17 +301,15 @@
             correction_function=correction_function,
             name=name,
             plot_cmb=plot_cmb,
         )
     elif kind == "Jpsi_Jpsi":
         mm_data = get_data(kind="data", trigger="MTOS", year=year, q2="jpsi")
         obs_kernel = zfit.Space("B_M", limits=(-1000, 1000))
-        correction_function = get_correction_DSCB(
-            obs_kernel, suffix=name, parameter_name_prefix=parameter_name_parameter
-        )
+        correction_function = get_correction_DSCB(obs_kernel, suffix=name, parameter_name_prefix=parameter_name_prefix)
         correction_function = load_pdf(pickle_path, correction_function, parameter_name_prefix)
         cmb_shape = get_cmb_mm_shape(q2="jpsi", obs=obs, year=year)
         return convolution_shape(
             cmb_shape=cmb_shape,
             data_array=mm_data,
             correction_function=correction_function,
             name=name,
```

### Comparing `rx_hqm-0.1.3/hqm/part_reco/fit_convolution.py` & `rx_hqm-0.1.4/hqm/part_reco/fit_convolution.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/mm_comb/comb_shape_mm.py` & `rx_hqm-0.1.4/hqm/part_reco/mm_comb/comb_shape_mm.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/convolution_shape_sys1.py` & `rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/convolution_shape_sys1.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/fit_convolution_sys1.py` & `rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/fit_convolution_sys1.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/run_fit_sys1.sh` & `rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/run_fit_sys1.sh`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/part_reco/systematic/sys1/submit_fit_sys1.sh` & `rx_hqm-0.1.4/hqm/part_reco/systematic/sys1/submit_fit_sys1.sh`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/fit_Bu2Kee_MC.py` & `rx_hqm-0.1.4/hqm/signal/fit_Bu2Kee_MC.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/fit_Bu2Kmm_MC.py` & `rx_hqm-0.1.4/hqm/signal/fit_Bu2Kmm_MC.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/systematic/sys1/fit_Bu2Kee_MC_sys1.py` & `rx_hqm-0.1.4/hqm/signal/systematic/sys1/fit_Bu2Kee_MC_sys1.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/systematic/sys1/fit_Bu2Kmm_MC_sys1.py` & `rx_hqm-0.1.4/hqm/signal/systematic/sys1/fit_Bu2Kmm_MC_sys1.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/systematic/sys1/submit_ee_sys1.sh` & `rx_hqm-0.1.4/hqm/signal/systematic/sys1/submit_ee_sys1.sh`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/signal/systematic/sys1/submit_mm_sys1.sh` & `rx_hqm-0.1.4/hqm/signal/systematic/sys1/submit_mm_sys1.sh`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/tools/Cut.py` & `rx_hqm-0.1.4/hqm/tools/Cut.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/tools/fit.py` & `rx_hqm-0.1.4/hqm/tools/fit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import zfit
 import pickle
 from fitter import zfitter
-from zutils.plot import plot as zfp
+from hqm.tools.plot import plot as zfp
 import matplotlib.pyplot as plt
 import os
 import pandas as pd
 from hqm.tools.utility import get_project_root
 import logzero
 
 
@@ -62,32 +62,36 @@
         self.result = minimizer.minimize(nll)
 
         # if self.result.status != 0:
         #     return
         params_list = list(self.result.params.keys())
         params_name_list = [x.name for x in params_list]
 
-        print(self.result)
         try:
             self.result.hesse()
             covariance_matrix_np = self.result.covariance()
-            self.covariance_matrix_df = pd.DataFrame(
-                covariance_matrix_np, columns=params_name_list, index=params_name_list
-            )
-            self._log.info("covariance matrix:")
-            print(self.covariance_matrix_df)
-
             correlation_matrix_np = self.result.correlation()
-            self.correlation_matrix_df = pd.DataFrame(
-                correlation_matrix_np, columns=params_name_list, index=params_name_list
-            )
-            self._log.info("correlation matrix:")
-            print(self.correlation_matrix_df)
         except:
-            self._log.warning("Hesse failed")
+            self._log.warning("hesse() failed, turn off the autograd")
+            with zfit.run.set_autograd_mode(False):
+                self.result.hesse()
+                covariance_matrix_np = self.result.covariance()
+                correlation_matrix_np = self.result.correlation()
+
+        self.correlation_matrix_df = pd.DataFrame(
+            correlation_matrix_np, columns=params_name_list, index=params_name_list
+        )
+        self._log.info("correlation matrix:")
+        print(self.correlation_matrix_df)
+
+        self.covariance_matrix_df = pd.DataFrame(
+            covariance_matrix_np, columns=params_name_list, index=params_name_list
+        )
+        self._log.info("covariance matrix:")
+        print(self.covariance_matrix_df)
 
         self._log.info("fit result:")
         print(self.result)
 
     def fit_data(self):
         self._fit_setup()
         self._fit_data()
```

### Comparing `rx_hqm-0.1.3/hqm/tools/selection.py` & `rx_hqm-0.1.4/hqm/tools/selection.py`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm/tools/utility.py` & `rx_hqm-0.1.4/hqm/tools/utility.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import json
 import uproot
 import pickle
 import zfit
 from importlib.resources import files
 from logzero import logger as log
+import matplotlib.pyplot as plt
+import mplhep
+import os
+import hist
+import numpy as np
 
 
 def get_lumi(year):
     lumi = {
         "2011": 1.0,
         "2012": 2.0,
         "2015": 0.3,
@@ -97,23 +102,43 @@
     with uproot.open(path) as f:
         events = f[tree_name]
         data_array = events.arrays()
     return data_array
 
 
 def cache_json(json_file_name):
-    json_path = files("hqm_data").joinpath(json_file_name)
+    if json_file_name is not None:
+        json_path = files("hqm_data").joinpath(json_file_name)
+    else:
+        json_path = None
 
     def decorator(func):
         def inner():
-            if os.path.isfile(json_path):
-                log.debug(f'Loading cached: {json_path}')
+            if json_path is None:
+                # turn off caching, do nothing
+                return func()
+            elif os.path.isfile(json_path):
+                log.debug(f'Loading: {json_path}')
                 return load_json(json_path)
             else:
-                log.warning(f'Caching: {json_path}')
+                log.debug(f'Making and caching: {json_path}')
                 obj = func()
                 dump_json(obj, json_path)
                 return obj
 
         return inner
 
     return decorator
+
+
+def plot1d(np_array, nbins, name, plot_path):
+    lower = np.min(np_array)
+    upper = np.max(np_array)
+    h_data = hist.Hist.new.Regular(nbins, lower, upper, name=name, flow=False).Double()
+    h_data.fill(np_array)
+
+    plt.figure()
+    mplhep.histplot(h_data, histtype="errorbar", yerr=True, color="black")
+    os.makedirs(os.path.dirname(plot_path), exist_ok=True)
+    log.info(f"Saving plot to {plot_path}")
+    plt.savefig(plot_path)
+    plt.close()
```

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2011_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2011_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2012_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2012_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2015_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2015_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2016_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2016_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpk2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpk2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2017_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2017_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_ETOS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_ETOS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bdks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bdks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bpk1.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bpk1.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bpks.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bpks.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_bsphi.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_bsphi.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/KDE_2018_GTIS_high_psi2.json` & `rx_hqm-0.1.4/hqm_data/KDE_2018_GTIS_high_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2011_B_M_NoBDTprc_jpsi_2011_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2011_B_M_NoBDTprc_jpsi_2011_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2012_B_M_NoBDTprc_jpsi_2012_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2012_B_M_NoBDTprc_jpsi_2012_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2015_B_M_NoBDTprc_jpsi_2015_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2015_B_M_NoBDTprc_jpsi_2015_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2016_B_M_NoBDTprc_jpsi_2016_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2016_B_M_NoBDTprc_jpsi_2016_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2017_B_M_NoBDTprc_jpsi_2017_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2017_B_M_NoBDTprc_jpsi_2017_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_jpsi_2018_B_M_NoBDTprc_jpsi_2018_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_jpsi_2018_B_M_NoBDTprc_jpsi_2018_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2011_B_M_NoBDTprc_psi2_2011_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2011_B_M_NoBDTprc_psi2_2011_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2012_B_M_NoBDTprc_psi2_2012_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2012_B_M_NoBDTprc_psi2_2012_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2015_B_M_NoBDTprc_psi2_2015_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2015_B_M_NoBDTprc_psi2_2015_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2016_B_M_NoBDTprc_psi2_2016_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2016_B_M_NoBDTprc_psi2_2016_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2017_B_M_NoBDTprc_psi2_2017_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2017_B_M_NoBDTprc_psi2_2017_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_comb_mm_latest_psi2_2018_B_M_NoBDTprc_psi2_2018_B_M_NoBDTprc_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_comb_mm_latest_psi2_2018_B_M_NoBDTprc_psi2_2018_B_M_NoBDTprc_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_psi2S_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_Jpsi_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_high_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2011_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2012_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2015_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2016_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2017_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_ETOS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_ETOS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_GTIS_fit_result.json` & `rx_hqm-0.1.4/hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_psi2S_psi2S_2018_GTIS_fit_result.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2011_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2012_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2015_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2016_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2011_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2012_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2015_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2016_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_2018_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2011_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2012_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2015_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2016_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_2018_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_2018_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_0_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_2018_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_1_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2017_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_2018_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_all_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_ETOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_ee_latest_sys1_latest_fit_Bu2Kee_MC_2_r2p1_GTIS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2011_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2011_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2012_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2012_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2015_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2015_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2016_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2016_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2017_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2017_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2018_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_2018_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_all_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_all_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r1_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r1_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2017_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2017_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2018_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_2018_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_all_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_all_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r1_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r1_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json` & `rx_hqm-0.1.4/hqm_data/data_signal_shape_mm_latest_sys1_latest_fit_Bu2Kmm_MC_r2p1_MTOS.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2011_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2011_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2012_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2012_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2015_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2015_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2016_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2016_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2017_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2017_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_data_MTOS_2018_psi2.json` & `rx_hqm-0.1.4/hqm_data/get_data_data_MTOS_2018_psi2.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2011_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2011_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2012_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2012_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2015_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2015_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2016_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2016_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2017_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2017_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/get_data_psi2_ETOS_2018_high.json` & `rx_hqm-0.1.4/hqm_data/get_data_psi2_ETOS_2018_high.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/hqm_data/signal_scales.json` & `rx_hqm-0.1.4/hqm_data/signal_scales.json`

 * *Files identical despite different names*

### Comparing `rx_hqm-0.1.3/pyproject.toml` & `rx_hqm-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rx_hqm"
-version = "0.1.3"
+version = "0.1.4"
 dynamic = ["dependencies"]
 
 [tool.pyright]
 # reportOptionalMemberAccess = false
 # reportOptionalSubscript = false
 # reportGeneralTypeIssues = false
```

### Comparing `rx_hqm-0.1.3/rx_hqm.egg-info/SOURCES.txt` & `rx_hqm-0.1.4/rx_hqm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 .gitignore
 README.md
 pyproject.toml
 requirements.txt
 hqm/__init__.py
 hqm/run_all.sh
+hqm/check/part_reco/Bd2Kspsi2S_MC_highq2_check.py
+hqm/check/part_reco/Jpsi_region.py
+hqm/check/part_reco/check_psi2S_left_tail.py
+hqm/check/part_reco/psi2S_region.py
+hqm/check/part_reco/simultaneous_fit.py
 hqm/data_sample/add_selection.py
 hqm/data_sample/add_selection_script.sh
 hqm/data_sample/apply_preselection.py
 hqm/data_sample/job_sel
 hqm/data_sample/submit_add_selection.sh
 hqm/data_sample/submit_all_ee.sh
 hqm/data_sample/submit_all_mm.sh
@@ -21,14 +26,21 @@
 hqm/model/signal.py
 hqm/part_reco/convolution_shape.py
 hqm/part_reco/fit_convolution.py
 hqm/part_reco/run_convolution_shape.sh
 hqm/part_reco/run_fit.sh
 hqm/part_reco/mm_comb/comb_shape_mm.py
 hqm/part_reco/mm_comb/run_mm.sh
+hqm/part_reco/ratio/fit_MC.py
+hqm/part_reco/ratio/fully_reco_shape.py
+hqm/part_reco/ratio/run_fit_MC.sh
+hqm/part_reco/ratio/run_fully_reco_shape.sh
+hqm/part_reco/ratio/simultaneous_fit.py
+hqm/part_reco/ratio/simultaneous_fit_script.sh
+hqm/part_reco/ratio/submit_simultaneous_fit.sh
 hqm/part_reco/systematic/sys1/convolution_shape_sys1.py
 hqm/part_reco/systematic/sys1/fit_convolution_sys1.py
 hqm/part_reco/systematic/sys1/run_convolution_shape_sys1.sh
 hqm/part_reco/systematic/sys1/run_fit_sys1.sh
 hqm/part_reco/systematic/sys1/submit_fit_sys1.sh
 hqm/signal/fit_Bu2Kee_MC.py
 hqm/signal/fit_Bu2Kmm_MC.py
@@ -38,14 +50,15 @@
 hqm/signal/systematic/sys1/fit_Bu2Kmm_MC_sys1.py
 hqm/signal/systematic/sys1/run_ee_sys1.sh
 hqm/signal/systematic/sys1/run_mm_sys1.sh
 hqm/signal/systematic/sys1/submit_ee_sys1.sh
 hqm/signal/systematic/sys1/submit_mm_sys1.sh
 hqm/tools/Cut.py
 hqm/tools/fit.py
+hqm/tools/plot.py
 hqm/tools/selection.py
 hqm/tools/utility.py
 hqm_data/KDE_2011_ETOS_high_bdks.json
 hqm_data/KDE_2011_ETOS_high_bpk1.json
 hqm_data/KDE_2011_ETOS_high_bpk2.json
 hqm_data/KDE_2011_ETOS_high_bpks.json
 hqm_data/KDE_2011_ETOS_high_bsphi.json
@@ -143,26 +156,50 @@
 hqm_data/data_part_reco_comb_mm_latest_jpsi_2018_B_M_NoBDTprc_jpsi_2018_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2011_B_M_NoBDTprc_psi2_2011_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2012_B_M_NoBDTprc_psi2_2012_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2015_B_M_NoBDTprc_psi2_2015_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2016_B_M_NoBDTprc_psi2_2016_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2017_B_M_NoBDTprc_psi2_2017_B_M_NoBDTprc_fit_result.json
 hqm_data/data_part_reco_comb_mm_latest_psi2_2018_B_M_NoBDTprc_psi2_2018_B_M_NoBDTprc_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2017_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_Jpsi_2018_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2011_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2012_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2015_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2016_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2017_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_Jpsi_psi2S_2018_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2011_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2012_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2015_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2016_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2017_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_Jpsi_2018_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2011_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2012_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2015_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2016_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2017_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_psi2S_high_2018_GTIS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2011_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2012_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2015_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2016_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2017_ETOS_fit_result.json
+hqm_data/data_part_reco_fit_convolution_latest_psi2S_psi2S_2018_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2011_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2012_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_ETOS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2015_GTIS_fit_result.json
 hqm_data/data_part_reco_fit_convolution_latest_sys1_latest_Jpsi_Jpsi_2016_ETOS_fit_result.json
@@ -325,14 +362,25 @@
 hqm_data/get_data_data_MTOS_2018_psi2.json
 hqm_data/get_data_psi2_ETOS_2011_high.json
 hqm_data/get_data_psi2_ETOS_2012_high.json
 hqm_data/get_data_psi2_ETOS_2015_high.json
 hqm_data/get_data_psi2_ETOS_2016_high.json
 hqm_data/get_data_psi2_ETOS_2017_high.json
 hqm_data/get_data_psi2_ETOS_2018_high.json
+hqm_data/get_data_psi2_GTIS_2011_high.json
+hqm_data/get_data_psi2_GTIS_2012_high.json
+hqm_data/get_data_psi2_GTIS_2015_high.json
+hqm_data/get_data_psi2_GTIS_2016_high.json
+hqm_data/get_data_psi2_GTIS_2017_high.json
+hqm_data/get_data_psi2_GTIS_2018_high.json
+hqm_data/psi2S_ratio_2017.json
+hqm_data/psi2S_ratio_2018.json
+hqm_data/psi2S_ratio_all.json
+hqm_data/psi2S_ratio_r1.json
+hqm_data/psi2S_ratio_r2p1.json
 hqm_data/signal_scales.json
 rx_hqm.egg-info/PKG-INFO
 rx_hqm.egg-info/SOURCES.txt
 rx_hqm.egg-info/dependency_links.txt
 rx_hqm.egg-info/requires.txt
 rx_hqm.egg-info/top_level.txt
 tests/test_pdf.py
```

### Comparing `rx_hqm-0.1.3/tests/test_pdf.py` & `rx_hqm-0.1.4/tests/test_pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,21 +200,19 @@
 
             logger.info(f"saving plot to {plot_path}")
             plt.legend()
             plt.savefig(plot_path)
             plt.close('all')
 #---------------------------------------------
 def main():
-    test_part_reco_nom()
-    test_part_reco_sys()
-    return
-
     test_signal_shape_ee_sys()
     test_signal_shape_ee_nom()
     test_signal_shape_mm_sys()
     test_signal_shape_mm_nom()
+    test_part_reco_nom()
+    test_part_reco_sys()
     test_rare_nom()
     test_rare_sys()
 #---------------------------------------------
 if __name__ == "__main__":
     main()
```

