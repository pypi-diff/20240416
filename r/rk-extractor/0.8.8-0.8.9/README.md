# Comparing `tmp/rk_extractor-0.8.8.tar.gz` & `tmp/rk_extractor-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rk_extractor-0.8.8.tar", last modified: Wed Feb  7 18:19:23 2024, max compression
+gzip compressed data, was "rk_extractor-0.8.9.tar", last modified: Mon Apr 15 14:09:55 2024, max compression
```

## Comparing `rk_extractor-0.8.8.tar` & `rk_extractor-0.8.9.tar`

### file list

```diff
@@ -1,288 +1,273 @@
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:23.000000 rk_extractor-0.8.8/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      526 2024-02-07 18:19:23.000000 rk_extractor-0.8.8/PKG-INFO
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     7162 2023-12-17 15:14:47.000000 rk_extractor-0.8.8/README.md
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:17.000000 rk_extractor-0.8.8/scripts/
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:18.000000 rk_extractor-0.8.8/scripts/jobs/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       35 2024-02-07 17:05:40.000000 rk_extractor-0.8.8/scripts/jobs/README.txt
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4646 2024-01-08 14:38:59.000000 rk_extractor-0.8.8/scripts/jobs/rxe_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)      153 2023-11-09 15:10:51.000000 rk_extractor-0.8.8/scripts/jobs/rxe_clean
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     4573 2023-12-22 15:49:05.000000 rk_extractor-0.8.8/scripts/jobs/rxe_download
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     3584 2024-02-07 14:56:43.000000 rk_extractor-0.8.8/scripts/jobs/rxe_grid_jobs
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1791 2024-01-08 12:36:12.000000 rk_extractor-0.8.8/scripts/jobs/rxe_ihep_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1984 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/scripts/jobs/rxe_ihep_jobs
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     2955 2024-02-07 13:16:22.000000 rk_extractor-0.8.8/scripts/jobs/rxe_local
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    16370 2024-01-17 11:36:45.000000 rk_extractor-0.8.8/scripts/jobs/rxe_plot_pull
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     8803 2023-12-31 20:04:56.000000 rk_extractor-0.8.8/scripts/jobs/rxe_plot_syst
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1353 2024-01-02 11:14:36.000000 rk_extractor-0.8.8/scripts/jobs/rxe_run_check
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)     1439 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/scripts/jobs/rxe_run_toys
--rwxr-xr-x   0 campoverde (12477) lhcb      (1026)    10985 2024-02-07 13:56:08.000000 rk_extractor-0.8.8/scripts/jobs/rxe_toys
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:18.000000 rk_extractor-0.8.8/scripts/offline/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5402 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/scripts/offline/analyze_result
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1297 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/scripts/offline/calculate_sigeff
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4996 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/scripts/offline/check_dist
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4119 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/scripts/offline/cmb_prec_norm
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3690 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/scripts/offline/make_signal_table
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5080 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/scripts/offline/plot_check
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3020 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/scripts/offline/rare_bkg_eff
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4836 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/scripts/offline/sbfit_analyze
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       38 2024-02-07 18:19:23.000000 rk_extractor-0.8.8/setup.cfg
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1539 2024-02-07 18:18:16.000000 rk_extractor-0.8.8/setup.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:18.000000 rk_extractor-0.8.8/src/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.8.8/src/__init__.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     7529 2024-02-07 14:42:07.000000 rk_extractor-0.8.8/src/bdt_scale.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     3662 2023-12-31 20:05:12.000000 rk_extractor-0.8.8/src/cmb_ck.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     9085 2023-11-26 15:18:19.000000 rk_extractor-0.8.8/src/cs_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    22377 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:18.000000 rk_extractor-0.8.8/src/extractor_data/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-16 17:02:20.000000 rk_extractor-0.8.8/src/extractor_data/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:18.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72332 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72172 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72378 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72374 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72334 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72355 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72366 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72360 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72362 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72366 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72360 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72362 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v1/eff_r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72332 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72172 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72378 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72374 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72334 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72355 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72375 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72349 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72372 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72368 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72373 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    72347 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/bdt_eff/v2/eff_r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/config/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/config/__init__.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      154 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/config/v1.toml
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      156 2024-02-07 17:03:26.000000 rk_extractor-0.8.8/src/extractor_data/config/v2.toml
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      750 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1486 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2142 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     2137 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      564 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1126 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v1/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      299 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v1/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v2/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8708 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v2/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v2/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v3/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8685 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v3/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v3/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:19.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v4/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v4/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v4/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v5/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8656 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v5/eff_real.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      398 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/rare_sf/v5/fr_bf.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        0 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/__init__.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      346 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v10/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v10/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v10/all_GTIS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v11/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      381 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v11/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v12/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v12/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v13/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v13/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v14/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v14/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v15/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      377 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v15/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v16/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      379 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v16/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v17/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v17/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v18/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      721 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v18/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v19/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1585 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v19/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      174 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      176 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      172 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      170 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      175 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v20/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v20/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v21/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v21/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v22/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      431 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v22/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v23/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      436 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v23/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v24/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v24/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v25/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1013 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v25/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v26/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      799 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v26/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v27/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1009 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v27/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v28/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1008 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v28/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:20.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v29/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v29/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v30/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v30/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v31/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      433 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v31/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v32/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      435 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v32/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v33/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v33/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v34/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1011 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v34/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v35/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1021 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v35/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v36/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      807 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v36/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v37/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1190 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v37/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v38/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1187 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v38/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v39/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v39/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      263 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      354 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      265 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      342 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v40/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1494 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v40/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v41/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1499 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v41/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v42/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1596 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v42/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v43/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1595 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v43/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v44/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1921 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v44/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v44/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:21.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v45/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      384 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v45/all_ETOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2017_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2017_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2017_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      355 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2018_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      353 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2018_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      267 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/2018_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      350 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      349 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      261 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/all_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      344 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      343 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      260 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r1_MTOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      352 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      351 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      266 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v6/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      264 2023-12-28 12:06:32.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v6/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v7/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      374 2023-12-31 20:05:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v7/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      380 2023-12-31 20:05:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v7/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      281 2023-12-31 20:05:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v7/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v8/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v8/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v8/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-15 21:50:12.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v8/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v9/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      376 2024-01-16 12:05:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v9/all_ETOS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      378 2024-01-16 12:05:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v9/all_GTIS.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      283 2024-01-16 12:05:27.000000 rk_extractor-0.8.8/src/extractor_data/sb_fits/v9/all_MTOS.json
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:17.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      529 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      700 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      530 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      528 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1441 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/src/extset.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     7485 2023-11-27 10:58:34.000000 rk_extractor-0.8.8/src/mc_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     6273 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/model_manager.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    11468 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/normalizer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8193 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/np_reader.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:22.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      526 2024-02-07 18:19:15.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/PKG-INFO
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     8713 2024-02-07 18:19:16.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)        1 2024-02-07 18:19:15.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      194 2024-02-07 18:19:15.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/requires.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)       16 2024-02-07 18:19:15.000000 rk_extractor-0.8.8/src/rk_extractor.egg-info/top_level.txt
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    18440 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/rk_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    17673 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/rkex_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    13795 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/src/scales.py
-drwxr-xr-x   0 campoverde (12477) lhcb      (1026)        0 2024-02-07 18:19:23.000000 rk_extractor-0.8.8/tests/
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      774 2023-12-31 20:05:12.000000 rk_extractor-0.8.8/tests/test_cmb_eff.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      627 2023-11-30 15:15:15.000000 rk_extractor-0.8.8/tests/test_cs_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      675 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/tests/test_effcalc.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    19329 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/tests/test_extractor.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1167 2023-11-27 10:46:34.000000 rk_extractor-0.8.8/tests/test_mc_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4786 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/tests/test_model_analyzer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     4615 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/tests/test_model_manager.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     5005 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/tests/test_normalizer.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      611 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/tests/test_np_reader.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)    10290 2024-02-06 13:59:27.000000 rk_extractor-0.8.8/tests/test_rkmodel.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     6685 2023-12-05 12:26:40.000000 rk_extractor-0.8.8/tests/test_rkrx_model.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1992 2024-01-30 14:14:06.000000 rk_extractor-0.8.8/tests/test_scales.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)      531 2023-12-25 18:44:59.000000 rk_extractor-0.8.8/tests/test_scl_mkr.py
--rw-r--r--   0 campoverde (12477) lhcb      (1026)     1652 2024-02-07 14:42:09.000000 rk_extractor-0.8.8/tests/test_scl_rdr.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.419232 rk_extractor-0.8.9/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      547 2024-04-15 14:09:55.419232 rk_extractor-0.8.9/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8926 2024-04-15 13:55:37.000000 rk_extractor-0.8.9/README.md
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.349233 rk_extractor-0.8.9/scripts/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.359233 rk_extractor-0.8.9/scripts/jobs/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       35 2024-02-15 15:33:22.000000 rk_extractor-0.8.9/scripts/jobs/README.txt
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4646 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/jobs/rxe_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)      153 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/jobs/rxe_clean
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     4573 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/jobs/rxe_download
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     3584 2024-02-15 15:33:22.000000 rk_extractor-0.8.9/scripts/jobs/rxe_grid_jobs
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1791 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/jobs/rxe_ihep_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1984 2024-02-05 13:50:39.000000 rk_extractor-0.8.9/scripts/jobs/rxe_ihep_jobs
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     2750 2024-04-15 11:15:40.000000 rk_extractor-0.8.9/scripts/jobs/rxe_local
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    17088 2024-02-15 15:33:22.000000 rk_extractor-0.8.9/scripts/jobs/rxe_plot_pull
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11926 2024-02-15 15:33:22.000000 rk_extractor-0.8.9/scripts/jobs/rxe_plot_syst
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1353 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/jobs/rxe_run_check
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)     1439 2024-02-05 13:44:47.000000 rk_extractor-0.8.9/scripts/jobs/rxe_run_toys
+-rwxrwxr-x   0 acampove  (1000) acampove  (1000)    11182 2024-04-15 11:15:40.000000 rk_extractor-0.8.9/scripts/jobs/rxe_toys
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.359233 rk_extractor-0.8.9/scripts/offline/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5402 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/offline/analyze_result
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1647 2024-02-15 15:58:01.000000 rk_extractor-0.8.9/scripts/offline/brf_tables
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1297 2024-01-19 15:50:57.000000 rk_extractor-0.8.9/scripts/offline/calculate_sigeff
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8172 2024-03-11 18:23:43.000000 rk_extractor-0.8.9/scripts/offline/check_dist
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4570 2024-02-28 17:05:16.000000 rk_extractor-0.8.9/scripts/offline/check_jpsi_misid
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4119 2024-02-27 17:09:40.000000 rk_extractor-0.8.9/scripts/offline/cmb_prec_norm
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3690 2024-01-21 17:43:02.000000 rk_extractor-0.8.9/scripts/offline/make_signal_table
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4102 2024-02-16 14:35:53.000000 rk_extractor-0.8.9/scripts/offline/make_yields_table
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5080 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/scripts/offline/plot_check
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3020 2024-01-17 18:03:20.000000 rk_extractor-0.8.9/scripts/offline/rare_bkg_eff
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4836 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/scripts/offline/sbfit_analyze
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       38 2024-04-15 14:09:55.419232 rk_extractor-0.8.9/setup.cfg
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1539 2024-04-15 14:09:08.000000 rk_extractor-0.8.9/setup.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7529 2024-02-06 15:53:58.000000 rk_extractor-0.8.9/src/bdt_scale.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     3662 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/cmb_ck.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     9085 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/cs_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    22377 2024-01-24 11:07:35.000000 rk_extractor-0.8.9/src/extractor.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/bdt_eff/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/bdt_eff/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/config/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/config/__init__.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      154 2024-02-05 13:29:13.000000 rk_extractor-0.8.9/src/extractor_data/config/v1.toml
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      156 2024-02-15 15:33:22.000000 rk_extractor-0.8.9/src/extractor_data/config/v2.toml
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      740 2024-04-15 13:53:55.000000 rk_extractor-0.8.9/src/extractor_data/config/v3.toml
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/npr_data/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      750 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1486 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2142 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     2137 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      564 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1126 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/rare_sf/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/rare_sf/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v1/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      299 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v1/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/rare_sf/v2/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8708 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v2/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v2/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/rare_sf/v3/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8685 2024-01-18 13:43:03.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v3/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v3/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.369233 rk_extractor-0.8.9/src/extractor_data/rare_sf/v4/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:08:38.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v4/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v4/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/rare_sf/v5/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8656 2024-01-18 17:20:28.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v5/eff_real.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      398 2024-01-15 11:01:04.000000 rk_extractor-0.8.9/src/extractor_data/rare_sf/v5/fr_bf.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        0 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/__init__.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      346 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v1/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v10/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-01-18 15:25:44.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v10/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-18 15:39:45.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v10/all_GTIS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v11/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      381 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v11/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v12/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v12/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v13/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v13/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v14/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v14/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v15/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      377 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v15/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v16/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      379 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v16/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v17/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v17/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v18/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      721 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v18/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v19/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1585 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v19/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.379233 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      174 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      176 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      172 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      170 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      175 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v2/r2p1_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v20/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v20/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v21/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v21/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v22/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      431 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v22/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v23/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      436 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v23/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v24/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v24/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v25/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1013 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v25/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v26/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      799 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v26/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v27/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1009 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v27/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v28/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1008 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v28/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v29/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v29/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v3/r2p1_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v30/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v30/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v31/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v31/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v32/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      435 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v32/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v33/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v33/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v34/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1011 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v34/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v35/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1021 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v35/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v36/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      807 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v36/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v37/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1190 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v37/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v38/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1187 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v38/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.389232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v39/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v39/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      263 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      354 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      265 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      342 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v4/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v40/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1494 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v40/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v41/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1499 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v41/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v42/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1596 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v42/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v43/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1595 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v43/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v44/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1921 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v44/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v44/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v45/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      384 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v45/all_ETOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v46/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      433 2024-02-26 18:26:46.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v46/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      292 2024-02-27 18:46:21.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v46/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2017_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2017_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2017_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      355 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2018_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      353 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2018_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      267 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/2018_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      350 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      349 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      261 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/all_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      344 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      343 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      260 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r1_MTOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      352 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r2p1_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      351 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r2p1_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      266 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v5/r2p1_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v6/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      264 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v6/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.399232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v7/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      374 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v7/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      380 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v7/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      281 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v7/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.409232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v8/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 12:23:27.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v8/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 12:35:58.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v8/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 12:40:49.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v8/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.409232 rk_extractor-0.8.9/src/extractor_data/sb_fits/v9/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      376 2024-01-15 13:55:12.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v9/all_ETOS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      378 2024-01-15 15:17:46.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v9/all_GTIS.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      283 2024-01-15 15:19:35.000000 rk_extractor-0.8.9/src/extractor_data/sb_fits/v9/all_MTOS.json
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.359233 rk_extractor-0.8.9/src/extractor_data/sig_wgt/
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.409232 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:48.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      529 2024-02-06 15:56:48.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:56:48.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      700 2024-02-06 16:09:04.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      530 2024-02-06 15:56:47.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      181 2024-02-16 14:25:16.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      184 2024-02-16 14:25:16.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      182 2024-02-16 14:25:16.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:53.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:53.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      528 2024-02-06 15:57:56.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-02-06 15:57:52.000000 rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1441 2024-02-06 15:53:52.000000 rk_extractor-0.8.9/src/extset.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7485 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/src/mc_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6270 2024-02-26 17:08:18.000000 rk_extractor-0.8.9/src/model_manager.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    12164 2024-02-27 18:42:34.000000 rk_extractor-0.8.9/src/normalizer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     8193 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/np_reader.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.419232 rk_extractor-0.8.9/src/rk_extractor.egg-info/
+-rw-r--r--   0 acampove  (1000) acampove  (1000)      547 2024-04-15 14:09:55.000000 rk_extractor-0.8.9/src/rk_extractor.egg-info/PKG-INFO
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     7961 2024-04-15 14:09:55.000000 rk_extractor-0.8.9/src/rk_extractor.egg-info/SOURCES.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)        1 2024-04-15 14:09:55.000000 rk_extractor-0.8.9/src/rk_extractor.egg-info/dependency_links.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      200 2024-04-15 14:09:55.000000 rk_extractor-0.8.9/src/rk_extractor.egg-info/requires.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)       16 2024-04-15 14:09:55.000000 rk_extractor-0.8.9/src/rk_extractor.egg-info/top_level.txt
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18432 2024-04-15 13:22:30.000000 rk_extractor-0.8.9/src/rk_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    17951 2024-04-15 12:41:07.000000 rk_extractor-0.8.9/src/rkex_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    13795 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/src/scales.py
+drwxrwxr-x   0 acampove  (1000) acampove  (1000)        0 2024-04-15 14:09:55.419232 rk_extractor-0.8.9/tests/
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      774 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/tests/test_cmb_eff.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      627 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/tests/test_cs_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      675 2024-01-18 12:47:43.000000 rk_extractor-0.8.9/tests/test_effcalc.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    18502 2024-02-16 12:59:44.000000 rk_extractor-0.8.9/tests/test_extractor.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1167 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/tests/test_mc_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4786 2024-01-23 12:48:03.000000 rk_extractor-0.8.9/tests/test_model_analyzer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     4615 2024-02-26 16:45:13.000000 rk_extractor-0.8.9/tests/test_model_manager.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     5005 2024-02-27 18:33:17.000000 rk_extractor-0.8.9/tests/test_normalizer.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      611 2024-02-05 11:35:54.000000 rk_extractor-0.8.9/tests/test_np_reader.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)    10316 2024-04-15 13:34:28.000000 rk_extractor-0.8.9/tests/test_rkmodel.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     6686 2024-04-15 11:31:30.000000 rk_extractor-0.8.9/tests/test_rkrx_model.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1992 2024-01-23 12:09:37.000000 rk_extractor-0.8.9/tests/test_scales.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)      531 2024-01-13 16:48:29.000000 rk_extractor-0.8.9/tests/test_scl_mkr.py
+-rw-rw-r--   0 acampove  (1000) acampove  (1000)     1652 2024-02-06 16:08:51.000000 rk_extractor-0.8.9/tests/test_scl_rdr.py
```

### Comparing `rk_extractor-0.8.8/PKG-INFO` & `rk_extractor-0.8.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rk_extractor
-Version: 0.8.8
+Version: 0.8.9
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
 Requires-Dist: scikit-learn==1.2.2
@@ -13,7 +13,8 @@
 Requires-Dist: rx_tools>=0.1.4
 Requires-Dist: rx_combinatorial>=0.0.1
 Requires-Dist: rx_hqm>=0.0.1
 Requires-Dist: rx_selection
 Requires-Dist: zfit>=0.14.0
 Requires-Dist: scipy
 Requires-Dist: pandas
+Requires-Dist: nlopt
```

### Comparing `rk_extractor-0.8.8/README.md` & `rk_extractor-0.8.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -115,14 +115,45 @@
 This file can be later reused (if `rdr.cache = True` is used) to speed up the processing.
 
 ## Model building
 
 A class is used to build a toy model from the expected rare decays yield and the rare mode efficiencies. 
 This class should be updated to use the correct model when available. 
 
+## Configuration
+
+The configuration is done through `toml` files stored
+[here](https://gitlab.cern.ch/r_k/rk_extractor/-/tree/master/src/extractor_data/config)
+
+and they look like:
+
+```toml
+
+#This will do the fits for the whole R1 + R2 dataset for the TOS category.
+[input]
+datasets=['all_TOS']
+
+[systematics]
+
+fix_var=[]
+# Specify signal models to try in toy fit
+sig_mod=['sig_ETOS:sys1', 'sig_MTOS:sys1']
+# It also can be left empty
+sig_mod=[]
+
+# For backgrounds, we will do bootstrapping. This will turn off the bootstrapping:
+rpr_mod='rpr_ETOS:bts_1_1'
+cpr_mod='cpr_ETOS:bts_1_1'
+
+# This will turn it on for 20 bootstrapped models for each component
+rpr_mod='rpr_ETOS:bts_1_20'
+cpr_mod='cpr_ETOS:bts_1_20'
+```
+
+
 ## Extraction of results
 
 The `extractor` class provides a `zfit` result object, which can be pickled.
 
 # Toy tests
 
 In order to verify that the model is not biased and has the right coverage, a set of scripts are available in
@@ -233,7 +264,49 @@
 
 to 
 
 1. Read all the `JSON` files in the retrieved sandboxes
 1. Make a dataframe with the fit parameters.
 3. Make plots and send them to the `plots` directory.
 
+## Acceprances for partially reconstructed decays
+
+The partially reconstructed decays have acceptances that have to be calculated without requiring that the extra track be in the LHCb acceptance. 
+This is done by:
+
+1. Generate samples with RapidSim
+2. Calculate the acceptances
+
+### Sample generation
+
+One has to:
+
+1. In the IHEP cluster or LXPLUS follow [these](https://github.com/gcowan/RapidSim?tab=readme-ov-file#setup) instructions.
+2. The input decay files are in [this](src/prec_files) directory.
+
+Then run:
+
+```bash
+  $RAPIDSIM_ROOT/bin/RapidSim.exe /publicfs/ucas/user/campoverde/Packages/RapidSim-master/install/user_config/bpk2kpipiee 10000 1
+```
+
+1. Run over a small number of events, alongside the decay files will be the config files, created by this run. 
+2. Modify the lines below:
+
+```
+geometry: LHCb
+paramsStable : P, PT
+```
+
+to
+
+```
+geometry: 4pi
+paramsStable : P, PT, eta
+```
+
+to add the _eta_ branch, which will be used to calculate $`\theta`$.
+
+3. Generate again with the full statistics, 100K.
+
+### Efficiencies calculation
+
```

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_check` & `rk_extractor-0.8.9/scripts/jobs/rxe_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_download` & `rk_extractor-0.8.9/scripts/jobs/rxe_download`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_grid_jobs` & `rk_extractor-0.8.9/scripts/jobs/rxe_grid_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_ihep_check` & `rk_extractor-0.8.9/scripts/jobs/rxe_ihep_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_ihep_jobs` & `rk_extractor-0.8.9/scripts/jobs/rxe_ihep_jobs`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_local` & `rk_extractor-0.8.9/scripts/jobs/rxe_local`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,32 @@
 
 from logzero import logger as log
 
 #----------------------------
 class data:
     jobid   = None
     nfits   = None
-    sandbox = None
+    job_dir = os.environ['JOBDIR']
+    sandbox = f'{job_dir}/extractor'
     vers    = None
     sft_path= '/publicfs/lhcb/user/campoverde/SFT/RK_TOY'
+
 #----------------------------
-def get_args_v1():
+def get_args():
     parser = argparse.ArgumentParser(description='Used to run local tests of toy fits')
-    parser.add_argument('-j', '--job_id' , type=str, help='Index of job'          , required=True)
+    parser.add_argument('-j', '--job_id' , type=int, help='Index of job'          , required=True)
     parser.add_argument('-n', '--nfits'  , type=int, help='Number of fits per job', required=True)
-    parser.add_argument('-s', '--sndbx'  , type=str, help='Directory for output'  , required=True)
+    parser.add_argument('-s', '--sndbx'  , type=str, help='Directory for output'  , default=data.sandbox)
     parser.add_argument('-v', '--vers'   , type=str, help='Version of output'     , required=True)
     args = parser.parse_args()
 
     data.jobid   = args.job_id
     data.nfits   = args.nfits
-    data.sandbox = args.sndbx
+    data.sandbox = f'{args.sndbx}/{str(data.jobid).rjust(3, "0")}_{str(data.nfits).rjust(3, "0")}'
     data.vers    = args.vers
-#----------------------------
-def get_args():
-    jobid        = sys.argv[1]
-    nfits        = sys.argv[2]
-    sandbox      = sys.argv[3]
-    vers         = sys.argv[4]
-
-    data.jobid   = int(jobid)
-    data.nfits   = int(nfits)
-    data.sandbox = f'{sandbox}/{jobid.rjust(3, "0")}_{nfits.rjust(3, "0")}'
-    data.vers    = vers 
 
     try:
         os.makedirs(data.sandbox, exist_ok=True)
     except:
         log.error(f'Cannot make sandbox: {data.sandbox}')
         raise
 #----------------------------
```

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_plot_pull` & `rk_extractor-0.8.9/scripts/jobs/rxe_plot_pull`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,14 @@
     sr_cns = df_pre[f'{var} error']
     sr_pul = (sr_val - sr_pre) / sr_err
 
     plot_pull(sr_pul, var)
 
     plot_vals(sr_val, sr_pre[0], sr_cns[0], var)
     plot_errs(sr_err, sr_pre[0], sr_cns[0], var)
-    plot_qlty(df_pos)
 #-------------------------------------------------------
 def plot_pull(sr_pul, var):
     mu, sd = zut.fit_pull(sr_pul.values, fit_sig=2, plot=True)
 
     store_pull(mu[0], sd[0], var)
 
     os.makedirs(f'{data.out_path}/plots/pulls', exist_ok=True)
@@ -275,41 +274,54 @@
     plot_path = f'{data.out_path}/plots/covariance.png'
     utnr.plot_matrix(plot_path, l_lat, l_lat, cov, upper=False, title='', form=None, fsize=[25, 20])
 
     cor       = utnr.correlation_from_covariance(cov)
     plot_path = f'{data.out_path}/plots/correlation.png'
     utnr.plot_matrix(plot_path, l_lat, l_lat, cor, upper=False, title='', form=None, fsize=[25, 20])
 #-------------------------------------------------------
-def freq_one(df, quantity):
+def freq_one(df, good_val, quantity):
     sr_qnt = df[quantity]
     ntot   = len(sr_qnt)
 
-    sr_one = sr_qnt == 1
-    none   = len(sr_one)
+    sr_good= sr_qnt[sr_qnt == good_val]
+    ngood  = len(sr_good)
+
+    return ngood, ntot - ngood
+#-------------------------------------------------------
+def add_labels(arr_x, arr_y1, arr_y2, xoff, yoff, l_color=['blue', 'orange'], form='{:.0f}'):
+    [color_1, color_2] = l_color
+    for x, y1, y2 in zip(arr_x, arr_y1, arr_y2):
+        label_1 = form.format(y1)
+        label_2 = form.format(y2)
 
-    return none, ntot - none
+        plt.annotate(label_1, (x,y1), fontsize=22, textcoords="offset points", xytext=(xoff, yoff), color=color_1, ha='center')
+        plt.annotate(label_2, (x,y2), fontsize=22, textcoords="offset points", xytext=(xoff, yoff), color=color_2, ha='center')
 #-------------------------------------------------------
 def plot_qlty(df):
     os.makedirs(f'{data.out_path}/plots/quality', exist_ok=True)
     plot_path = f'{data.out_path}/plots/quality/summary.png'
 
-    cnv_y, cnv_n = freq_one(df, 'converged') 
-    sta_y, sta_n = freq_one(df, 'status') 
-    val_y, val_n = freq_one(df, 'valid') 
+    cnv_y, cnv_n = freq_one(df, 1, 'converged') 
+    sta_y, sta_n = freq_one(df, 0, 'status') 
+    val_y, val_n = freq_one(df, 1, 'valid') 
 
     xerr = [0.5, 0.5, 0.5]
     xval = [1.0, 2.0, 3.0]
     plt.errorbar(xval, [cnv_y, sta_y, val_y], xerr=xerr, label='Good' , marker='o', linestyle='None')
     plt.errorbar(xval, [cnv_n, sta_n, val_n], xerr=xerr, label='Bad'  , marker='o', linestyle='None')
 
+    add_labels(xval, [cnv_y, sta_y, val_y], [cnv_n, sta_n, val_n], 40, 20)
+
     plt.title('Fit quality')
     log.debug(f'Saving to: {plot_path}')
     plt.grid()
     plt.legend()
+    plt.ylim(0, 2000)
     plt.xticks(xval, ['Converged', 'Status', 'Valid'])
+    plt.tight_layout()
     plt.savefig(plot_path)
     plt.close('all')
 #-------------------------------------------------------
 def get_var_naming():
     d_name             = {}
     d_name['r0_ee']    = r'$r_0^{ee}$'
     d_name['r1_ee']    = r'$r_1^{ee}$'
@@ -478,18 +490,21 @@
         s_dset.add(dset)
         s_trig.add(trig)
 
     data.l_dset = list(s_dset)
     data.l_trig = list(s_trig)
 #-------------------------------------------------------
 def main():
-    log.setLevel(20)
+    log.setLevel(10)
     plt.style.use(mplhep.style.LHCb2)
 
     df_pos = build_df('pos')
+
+    plot_qlty(df_pos)
+
     df_pre = build_df('pre')
 
     l_pos  = df_pos.columns.tolist()
     l_pre  = df_pre.columns.tolist()
 
     find_dset_trig(l_pos)
```

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_plot_syst` & `rk_extractor-0.8.9/scripts/jobs/rxe_plot_syst`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
 
 import os
 import re
+import tqdm
 import glob
+import math
 import numpy
 import pprint
 import tarfile
 import argparse
 
 import pandas            as pnd
 import utils_noroot      as utnr
@@ -21,15 +23,20 @@
     out_dir   = None
     var       = 'rk'
     d_var_err = {}
     d_var_val = {}
     d_var_name= None
 #-------------------------------------------------------
 def get_var_naming():
-    d_name             = {}
+    d_name                 = {}
+    d_name['rpr_ETOS:bts'] =  'Rare PR BTS'
+    d_name['cpr_ETOS:bts'] = r'$c\bar{c}$ PR BTS'
+    d_name['sig_ETOS:sys'] = r'Signal'
+    d_name['sig_MTOS:sys'] = r'Signal'
+
     d_name['ssg_mm']   = '$r_{\sigma}^{\mu\mu}$'
     d_name['ssg_ee']   = '$r_{\sigma}^{ee}$'
     d_name['ssg']      = '$r_{\sigma}$'
 
     d_name['nsg_mm']   = '$N_{signal}^{\mu\mu}$'
     d_name['nsg_ee']   = '$N_{signal}^{ee}$'
     d_name['nsg'   ]   = '$N_{signal}$'
@@ -111,17 +118,21 @@
 #-----------------------------------
 def add_val(var, qty, d_dat):
     if var in d_dat:
         d_dat[var].append(qty)
     else:
         d_dat[var] = [qty]
 #-----------------------------------
+def get_json_from_wc(json_wc):
+    #Skip original files, pick only processed ones
+    return
+#-----------------------------------
 def update_data(dir_path):
     jsn_wc = f'{dir_path}/*.json'
-    l_jsn  = glob.glob(jsn_wc)
+    l_jsn  = get_json_from_wc(jsn_wc)
     check_size(l_jsn, f'Empty list of JSON files in: {jsn_wc}')
 
     check_job(l_jsn)
 
     d_var = { get_var_name(jsn_path) : jsn_path for jsn_path in l_jsn }
     check_size(d_var, 'Empty variable -> JSON path dictionary')
 
@@ -197,33 +208,107 @@
     if os.path.isdir(f'{dir_path}/result_jsn'):
         return True
 
     with tarfile.open(tar_path) as itar:
         itar.extractall(path=dir_path)
         return True 
 #-----------------------------------
+def split_sys(l_json):
+    d_json = {}
+    for file_path in l_json:
+        file_name       = os.path.basename(file_path)
+        key             = file_name.split(':')[0]
+        if key not in d_json:
+            d_json[key] = [file_path]
+        else:
+            d_json[key].append(file_path)
+
+    return d_json
+#-----------------------------------
+def merge_sys(d_json, d_nom, dir_path):
+    [rk_nom, _] = d_nom['pos']['rk']
+    for sys, l_json_path in d_json.items():
+        l_d_par   = [ utnr.load_json(json_path) for json_path in l_json_path ]
+        l_rk_val  = [ d_par['pos']['rk'][0] for d_par in l_d_par ]
+        rk_sys    = max(l_rk_val, key=lambda rk_val : abs(rk_val - rk_nom))
+        i_var     = l_rk_val.index(rk_sys)
+        d_par_sys = l_d_par[i_var]
+
+        json_path = f'{dir_path}/{sys}:sys.json'
+        utnr.dump_json(d_par_sys, json_path)
+        log.debug(f'Largest variation: {l_json_path[i_var]} -> {json_path}')
+#-----------------------------------
+def merge_bts(d_json, d_nom, dir_path):
+    l_par        = d_nom['pos']['par']
+    for sys, l_json_path in d_json.items():
+        d_mrg        = {}
+        d_mrg['pre'] = d_nom['pre']
+        d_mrg['pos'] = {} 
+
+        l_d_par = [ utnr.load_json(json_path) for json_path in l_json_path ]
+        for par in l_par:
+            par_sys           = merge_bts_par(par, l_d_par, d_nom)
+            d_mrg['pos'][par] = [par_sys, 0]
+
+        json_path = f'{dir_path}/{sys}:bts.json'
+        #utnr.dump_json(d_mrg, json_path)
+        log.debug(f'Mergin bootstrapped parameters into: {json_path}')
+#-----------------------------------
+def merge_bts_par(par_name, l_d_par, d_nom):
+    l_par_val = [ d_par['pos'][par_name][0] for d_par in l_d_par ]
+    par_nom   = d_nom['pos'][par_name][0]
+
+    l_var_val = [ (par_val - par_nom) ** 2 for par_val in l_par_val ]
+    var_avg   = sum(l_var_val) / len(l_d_par) 
+
+    par_sys   = par_nom + math.sqrt(var_avg)
+
+    return par_sys
+#-----------------------------------
+def preprocess(dir_path):
+    json_wc    = f'{dir_path}/*.json'
+    l_json     = glob.glob(json_wc)
+
+    [json_nom] = [json_path for json_path in l_json if ':' not in json_path] 
+    d_nom      = utnr.load_json(json_nom)
+    for sys in ['sys', 'bts']:
+        l_json_sys = [ file_path for file_path in l_json if re.match(f'.*:{sys}\d+\.json', file_path) ]
+        d_json_sys = split_sys(l_json_sys)
+
+        if sys == 'sys':
+            merge_sys(d_json_sys, d_nom, dir_path)
+        else:
+            merge_bts(d_json_sys, d_nom, dir_path)
+
+    exit()
+#-----------------------------------
 def get_df():
     df = pnd.DataFrame(columns=['var', 'val', 'err'])
 
     l_obj = glob.glob(f'{data.res_dir}/*')
+    l_obj = l_obj[:10]
     l_dir = [ obj for obj in l_obj if re.match('\d{8}', os.path.basename(obj)) ]
     l_tar = [ f'{dir_path}/result_jsn.tar.gz' for dir_path in l_dir ]
-    l_dir = [ tar_file.replace('.tar.gz', '') for tar_file in l_tar if is_good_tarfile(tar_file) ]
+    log.info(f'Checking inputs and untarring')
+    l_dir = [ tar_file.replace('.tar.gz', '') for tar_file in tqdm.tqdm(l_tar, ascii=' -') if is_good_tarfile(tar_file) ]
+    [ preprocess(dir_path) for dir_path in l_dir]
 
     njob=len(l_dir)
     if njob == 0:
         log.error(f'Found {njob} jobs in {data.res_dir}')
         raise
     else:
         log.info(f'Found {njob} job outputs')
 
-    log.debug(f'Found {njob} jobs')
-    for dir_path in l_dir:
+    log.debug(f'Found {njob} jobs, building dataframe')
+    for dir_path in tqdm.tqdm(l_dir, ascii=' -'):
         update_data(dir_path) 
 
+    exit()
+
     df_err=plot_error()
     df_val=plot_value()
 
     return df_err, df_val
 #-----------------------------------
 def plot_err_df(df):
     nom_rk = df[df.Variable == 'None'].Value.iloc[0]
@@ -272,14 +357,16 @@
     plt.close('all')
 #-----------------------------------
 def main():
     data.d_var_name = get_var_naming()
 
     df_err, df_val = get_df()
 
+    return
+
     plot_err_df(df_err)
     plot_val_df(df_val)
 #-----------------------------------
 if __name__ == '__main__':
     get_args()
     main()
```

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_run_check` & `rk_extractor-0.8.9/scripts/jobs/rxe_run_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_run_toys` & `rk_extractor-0.8.9/scripts/jobs/rxe_run_toys`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/jobs/rxe_toys` & `rk_extractor-0.8.9/scripts/jobs/rxe_toys`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,19 @@
 
     if   data.for_syst:
         log.info(f'Running systematics job')
     elif data.for_pull:
         log.info(f'Running pulls job')
     else:
         log.error(f'Misconfigured job, seeds/fixed = {nseed}/{nfix}')
+        log.info('-------------')
+        log.info('Valid:')
+        log.info('-------------')
+        log.info('nSeed=1; nFix > 0 or  nMod > 0')
+        log.info('nSeed>1; nFix = 0 and nMod = 0')
         raise
 #--------------------------------
 def cleanup_env():
     d_par = zfit.Parameter._existing_params
     l_key = list(d_par.keys())
 
     for key in l_key:
```

### Comparing `rk_extractor-0.8.8/scripts/offline/analyze_result` & `rk_extractor-0.8.9/scripts/offline/analyze_result`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/calculate_sigeff` & `rk_extractor-0.8.9/scripts/offline/calculate_sigeff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/cmb_prec_norm` & `rk_extractor-0.8.9/scripts/offline/cmb_prec_norm`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/make_signal_table` & `rk_extractor-0.8.9/scripts/offline/make_signal_table`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/plot_check` & `rk_extractor-0.8.9/scripts/offline/plot_check`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/rare_bkg_eff` & `rk_extractor-0.8.9/scripts/offline/rare_bkg_eff`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/scripts/offline/sbfit_analyze` & `rk_extractor-0.8.9/scripts/offline/sbfit_analyze`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/setup.py` & `rk_extractor-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     else:
         raise
 
     return l_pkg
 #----------------------------------------------
 setup(
         name              = 'rk_extractor',
-        version           = '0.8.8',
+        version           = '0.8.9',
         description       = 'Used to extract RK from simultaneous fits',
         scripts           = get_scripts('scripts/jobs') + get_scripts('scripts/offline'),
         long_description  = '',
         packages          = get_packages(),
         package_dir       = {'' : 'src'},
         package_data      = {'extractor_data' : get_data_packages('extractor_data')}, 
         install_requires  = open('requirements.txt').read().splitlines()
```

### Comparing `rk_extractor-0.8.8/src/bdt_scale.py` & `rk_extractor-0.8.9/src/bdt_scale.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/cmb_ck.py` & `rk_extractor-0.8.9/src/cmb_ck.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/cs_reader.py` & `rk_extractor-0.8.9/src/cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor.py` & `rk_extractor-0.8.9/src/extractor.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/eff_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/eff_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sta_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sta_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sys_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/sys_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/yld_ee.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json` & `rk_extractor-0.8.9/src/extractor_data/npr_data/v65_v63_v24/yld_mm.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/rare_sf/v1/eff_real.json` & `rk_extractor-0.8.9/src/extractor_data/rare_sf/v1/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/rare_sf/v2/eff_real.json` & `rk_extractor-0.8.9/src/extractor_data/rare_sf/v2/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/rare_sf/v3/eff_real.json` & `rk_extractor-0.8.9/src/extractor_data/rare_sf/v3/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/rare_sf/v4/eff_real.json` & `rk_extractor-0.8.9/src/extractor_data/rare_sf/v4/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/rare_sf/v5/eff_real.json` & `rk_extractor-0.8.9/src/extractor_data/rare_sf/v5/eff_real.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v18/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v18/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v19/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v19/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v25/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v25/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v26/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v26/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v27/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v27/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v28/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v28/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v34/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v34/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v35/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v35/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v36/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v36/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v37/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v37/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v38/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v38/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v39/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v39/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v40/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v40/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v41/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v41/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v42/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v42/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v43/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v43/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sb_fits/v44/all_ETOS.json` & `rk_extractor-0.8.9/src/extractor_data/sb_fits/v44/all_ETOS.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_all.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json` & `rk_extractor-0.8.9/src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/extset.py` & `rk_extractor-0.8.9/src/extset.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/mc_reader.py` & `rk_extractor-0.8.9/src/mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/model_manager.py` & `rk_extractor-0.8.9/src/model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         return zfit.pdf.SumPDF(l_pdf, name=pdf_name)
     #---------------------------------------------------------------------------
     def _set_instances(self):
         self._d_inst = {}
         for bdt_bin in self._l_bdt_bin:
             mod          = model(preffix=f'{self._preffix}_{bdt_bin}', d_eff=self._d_eff, d_nent=self._d_nent, l_dset=[self._dset])
             mod.bdt_bin  = bdt_bin
+            mod.kind     = 'nom'
             mod.fake     = self._fake_model 
 
             self._d_inst[bdt_bin] = mod
     #---------------------------------------------------------------------------
     def _get_data(self, bdt_bin):
         d_data = self._d_inst[bdt_bin].get_data()
         data   = d_data[self._dset]
@@ -146,17 +147,17 @@
         self._d_mode = d_mode
         self._d_data = d_data
     #---------------------------------------------------------------------------
     def _print_data(self):
         log.debug('-' * 40)
         log.debug(f'{"Name":<20}{"mm entries":<20}{"ee entries":<20}')
         log.debug('-' * 40)
-        for name, (dat_mm, dat_ee) in self._d_data.items():
-            nent_mm = dat_mm.numpy().flatten().size
-            nent_ee = dat_ee.numpy().flatten().size
+        for name, (arr_mm, arr_ee) in self._d_data.items():
+            nent_mm = arr_mm.size
+            nent_ee = arr_ee.size
             log.debug(f'{name:<20}{nent_mm:<20}{nent_ee:<20}')
         log.debug('-' * 40)
     #---------------------------------------------------------------------------
     def _print_model(self):
         for _, (pdf_mm, pdf_ee) in self._d_mode.items():
             zut.print_pdf(pdf_mm, level='debug')
             zut.print_pdf(pdf_ee, level='debug')
```

### Comparing `rk_extractor-0.8.8/src/normalizer.py` & `rk_extractor-0.8.9/src/normalizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy
 import pprint
 import extset
 import utils_noroot      as utnr
 import zutils.utils      as zut
 import matplotlib.pyplot as plt
 
+from misid_check   import misid_check
 from zutils.plot   import plot     as zfp
 from fitter        import zfitter
 from log_store     import log_store
 
 log = log_store.add_logger(name='rk_extractor:normalizer')
 #--------------------------------------
 class normalizer:
@@ -75,15 +76,21 @@
     @property
     def data(self):
         return self._d_data
 
     @data.setter
     def data(self, value):
         self._custom_data = True
-        self._d_data      = value
+        d_data            = {key : self._pick_data(arr_mm, arr_ee) for key, (arr_mm, arr_ee) in value.items()} 
+        self._d_data      = d_data 
+    #--------------------------------------
+    def _pick_data(self, arr_mm, arr_ee):
+        arr_mass = arr_mm if self._trig == 'MTOS' else arr_ee
+
+        return arr_mass.tolist()
     #--------------------------------------
     def _get_bdt_bins(self):
         l_mod_key  = [ key for key in self._d_model ]
         l_bdt_sbin = [ re.match('.*_(\d)$', mod_key).groups()[0] for mod_key in l_mod_key ]
         l_bdt_ibin = [ int(sbin) for sbin in l_bdt_sbin ]
 
         return l_bdt_ibin
@@ -124,19 +131,31 @@
         rdf = rdf.Filter(f'(BDT_prc > {lo_prc}) && (BDT_prc < {hi_prc})', 'PRC')
 
         rep = rdf.Report()
         rep.Print()
 
         return rdf
     #-------------------------------------
-    def _get_mass(self, l_dpath, ibin):
-        rdf = ROOT.RDataFrame(self._trig, l_dpath)
-        rdf = self._filter(rdf, ibin)
+    def _get_jpsi_mass(self, rdf):
+        df  = misid_check.rdf_to_df(rdf, '(L1|L2|H)_(P\w|ID)$')
+        obj = misid_check(df, d_lep={'L1' : 13, 'L2' : 13}, d_had={'H' : 13})
+        df  = obj.get_df()
+
+        arr_mass = df.H_swp.to_numpy()
 
-        arr_mass = rdf.AsNumpy(['B_M'])['B_M']
+        return arr_mass
+    #-------------------------------------
+    def _get_mass(self, rdf, kind):
+        if   kind == 'bp':
+            arr_mass = rdf.AsNumpy(['B_M'])['B_M']
+        elif kind == 'q2':
+            arr_mass = self._get_jpsi_mass(rdf)
+        else:
+            log.error(f'Invalid kind: {kind}')
+            raise
 
         return arr_mass.tolist()
     #--------------------------------------
     @utnr.timeit
     def _get_data(self):
         dat_path = f'{self._out_dir}/data/{self._dset}_{self._trig}.json'
         if   self._d_data is not None:
@@ -147,35 +166,27 @@
             d_dat = utnr.load_json(dat_path)
             return d_dat 
 
         log.info(f'Caching data: {dat_path}')
 
         os.makedirs(f'{self._out_dir}/data', exist_ok=True)
 
-        l_dpath = self._get_data_paths()
-        d_dat   = { f'bdt_{ibin}' : self._get_mass(l_dpath, ibin) for ibin in self._l_bdt_bin}
+        l_dpath  = self._get_data_paths()
+        rdf      = ROOT.RDataFrame(self._trig, l_dpath)
+        d_rdf    = { ibin : self._filter(rdf, ibin) for ibin in self._l_bdt_bin}
+
+        d_dat_bp = { f'bdt_{ibin}'    : self._get_mass(rdf, 'bp') for ibin, rdf in d_rdf.items() }
+        d_dat_q2 = { f'bdt_{ibin}_q2' : self._get_mass(rdf, 'q2') for ibin, rdf in d_rdf.items() }
+        d_dat    = { **d_dat_bp , **d_dat_q2} 
 
         log.info(f'Saving to: {dat_path}')
         utnr.dump_json(d_dat, dat_path) 
 
         return d_dat 
     #--------------------------------------
-    def _plot_data(self, arr_mass):
-        if not self._out_dir:
-            return
-
-        rng_ee = 4800, 6000
-        rng_mm = 5100, 5600
-        rng = rng_mm if self._trig == 'MTOS' else rng_ee
-        plt.hist(arr_mass, range=rng, bins=50, histtype='step')
-        plot_path = f'{self._out_dir}/data/{self._dset}_{self._trig}.png'
-        log.info(f'Saving to: {plot_path}')
-        plt.savefig(plot_path)
-        plt.close('all')
-    #--------------------------------------
     def _prepare_pars(self):
         for par in self._s_par:
             par.floating = False
 
         d_const = {}
         for par in self._s_par:
             for flt_par in self._l_flt_par:
@@ -201,23 +212,24 @@
             os.makedirs(value, exist_ok=True)
         except:
             log.error(f'Cannot create directory: {value}')
             raise
 
         self._out_dir = value
     #--------------------------------------
-    def _get_stats(self, arr_dat):
+    def _get_stats(self, zdata, model):
         if self._trig != 'MTOS':
             return ''
 
+        arr_dat = zdata.numpy()
         arr_flg = (arr_dat > 5180) & (arr_dat < 5400)
         arr_dat = arr_dat[arr_flg]
         ndata   = float(arr_dat.size)
 
-        s_par     = self._model.get_params(floating=False)
+        s_par     = model.get_params(floating=False)
         [pst_val] = [ par.value().numpy() for par      in s_par               if par.name.startswith('nsg_mm_') ]
         [pre_val] = [ val                 for nam, val in self._d_pre.items() if nam.startswith('nsg_mm_')      ]
 
         v1 = f'Data: {ndata:.0f} $m\in [5180, 5400]$'
         v2 = f'Fitted: {pst_val:.0f}'
         v3 = f'Expected: {pre_val:.0f}'
 
@@ -240,20 +252,20 @@
 
         low, hig= self._bln_ee
         l_blnd  = [extset.sig_name, low, hig]
 
         return l_blnd
     #--------------------------------------
     def _plot_fit(self, data=None, model=None, name=None, result=None, stacked=None):
-        stats   = self._get_stats(data)
+        stats   = self._get_stats(data, model)
         rng     = self._rng_mm if self._trig == 'MTOS' else self._rng_ee
         l_blnd  = self._get_blinding()
 
         obj= zfp(data=data, model=model, result=None)
-        obj.plot(skip_pulls=False, blind=l_blnd, nbins=self._nbins, ranges=[rng], d_leg=self._get_pdf_names(), stacked=stacked, ext_text=stats)
+        obj.plot(skip_pulls=False, blind=l_blnd, nbins=self._nbins, plot_range=rng, d_leg=self._get_pdf_names(), stacked=stacked, ext_text=stats)
         obj.axs[0].grid()
 
         if not self._custom_data:
             if   '_all_' in name and 'MTOS' in name:
                 obj.axs[0].set_ylim(0,  250)
             elif '_all_' in name and 'ETOS' in name:
                 obj.axs[0].set_ylim(0,  120)
@@ -271,43 +283,47 @@
     #--------------------------------------
     @utnr.timeit
     def _fit(self, d_mod, d_dat):
         tot_nll = None
         d_fdat  = {}
         d_fmod  = {}
         for bdt_bin in self._l_bdt_bin:
-            _, mod = d_mod[f'bdt_{bdt_bin}']
-            l_dat  = d_dat[f'bdt_{bdt_bin}']
-            arr_mas= numpy.array(l_dat)
-            obs    = mod.space
-            dat    = zfit.Data.from_numpy(obs=obs, array=arr_mas)
+            mod_mm, mod_ee = d_mod[f'bdt_{bdt_bin}']
+
+            mod_mas= mod_mm if self._trig == 'MTOS' else mod_ee
+            l_mas  = d_dat[f'bdt_{bdt_bin}']
+            arr_mas= numpy.array(l_mas)
+            obs    = mod_mas.space
+            dat_mas= zfit.Data.from_numpy(obs=obs, array=arr_mas)
 
-            d_fdat[f'bdt_{bdt_bin}'] = dat
-            d_fmod[f'bdt_{bdt_bin}'] = mod
+            d_fdat[f'bdt_{bdt_bin}'] = dat_mas
+            d_fmod[f'bdt_{bdt_bin}'] = mod_mas
 
             rng    = self._rng_mm if self._trig == 'MTOS' else self._rng_ee
             log.info(f'Adding nll for bin {bdt_bin} in range {rng}')
-            nll    = zfit.loss.ExtendedUnbinnedNLL(model=mod, data=dat, fit_range=rng)
+            nll    = zfit.loss.ExtendedUnbinnedNLL(model=mod_mas, data=dat_mas, fit_range=rng)
 
             tot_nll = nll if tot_nll is None else nll + tot_nll
 
+            if self._trig == 'MTOS':
+                break
+
         minimizer = zfit.minimize.Minuit()
         log.debug('Minimizing')
         result    = minimizer.minimize(tot_nll)
 
         return result, d_fdat, d_fmod
     #--------------------------------------
     def _print_pdfs(self, prefix):
         for key, (mod_mm, mod_ee) in self._d_model.items():
             zut.print_pdf(mod_mm, txt_path=f'{self._out_dir}/pdf/{prefix}_mm_{key}_{self._dset}_{self._trig}.txt', d_const=self._d_const)
             zut.print_pdf(mod_ee, txt_path=f'{self._out_dir}/pdf/{prefix}_ee_{key}_{self._dset}_{self._trig}.txt', d_const=self._d_const)
     #--------------------------------------
     def _plot_fits(self, d_fdat, d_fmod):
-        for ibin in self._l_bdt_bin:
-            key = f'bdt_{ibin}'
+        for key in d_fdat:
             arr_mass = d_fdat[key]
             model    = d_fmod[key]
 
             self._plot_fit(data=arr_mass, model=model, name=f'{self._trig}_{self._dset}_{key}_stk', stacked= True)
     #--------------------------------------
     @utnr.timeit
     def get_fit_result(self):
```

### Comparing `rk_extractor-0.8.8/src/np_reader.py` & `rk_extractor-0.8.9/src/np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/src/rk_extractor.egg-info/PKG-INFO` & `rk_extractor-0.8.9/src/rk_extractor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rk-extractor
-Version: 0.8.8
+Name: rk_extractor
+Version: 0.8.9
 Summary: Used to extract RK from simultaneous fits
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: logzero
 Requires-Dist: attrs
 Requires-Dist: jacobi
 Requires-Dist: scikit-learn==1.2.2
@@ -13,7 +13,8 @@
 Requires-Dist: rx_tools>=0.1.4
 Requires-Dist: rx_combinatorial>=0.0.1
 Requires-Dist: rx_hqm>=0.0.1
 Requires-Dist: rx_selection
 Requires-Dist: zfit>=0.14.0
 Requires-Dist: scipy
 Requires-Dist: pandas
+Requires-Dist: nlopt
```

### Comparing `rk_extractor-0.8.8/src/rk_extractor.egg-info/SOURCES.txt` & `rk_extractor-0.8.9/src/rk_extractor.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,21 @@
 scripts/jobs/rxe_local
 scripts/jobs/rxe_plot_pull
 scripts/jobs/rxe_plot_syst
 scripts/jobs/rxe_run_check
 scripts/jobs/rxe_run_toys
 scripts/jobs/rxe_toys
 scripts/offline/analyze_result
+scripts/offline/brf_tables
 scripts/offline/calculate_sigeff
 scripts/offline/check_dist
+scripts/offline/check_jpsi_misid
 scripts/offline/cmb_prec_norm
 scripts/offline/make_signal_table
+scripts/offline/make_yields_table
 scripts/offline/plot_check
 scripts/offline/rare_bkg_eff
 scripts/offline/sbfit_analyze
 src/__init__.py
 src/bdt_scale.py
 src/cmb_ck.py
 src/cs_reader.py
@@ -32,41 +35,18 @@
 src/normalizer.py
 src/np_reader.py
 src/rk_model.py
 src/rkex_model.py
 src/scales.py
 src/extractor_data/__init__.py
 src/extractor_data/bdt_eff/__init__.py
-src/extractor_data/bdt_eff/v1/eff_2017_ETOS.json
-src/extractor_data/bdt_eff/v1/eff_2017_GTIS.json
-src/extractor_data/bdt_eff/v1/eff_2017_MTOS.json
-src/extractor_data/bdt_eff/v1/eff_2018_ETOS.json
-src/extractor_data/bdt_eff/v1/eff_2018_GTIS.json
-src/extractor_data/bdt_eff/v1/eff_2018_MTOS.json
-src/extractor_data/bdt_eff/v1/eff_r1_ETOS.json
-src/extractor_data/bdt_eff/v1/eff_r1_GTIS.json
-src/extractor_data/bdt_eff/v1/eff_r1_MTOS.json
-src/extractor_data/bdt_eff/v1/eff_r2p1_ETOS.json
-src/extractor_data/bdt_eff/v1/eff_r2p1_GTIS.json
-src/extractor_data/bdt_eff/v1/eff_r2p1_MTOS.json
-src/extractor_data/bdt_eff/v2/eff_2017_ETOS.json
-src/extractor_data/bdt_eff/v2/eff_2017_GTIS.json
-src/extractor_data/bdt_eff/v2/eff_2017_MTOS.json
-src/extractor_data/bdt_eff/v2/eff_2018_ETOS.json
-src/extractor_data/bdt_eff/v2/eff_2018_GTIS.json
-src/extractor_data/bdt_eff/v2/eff_2018_MTOS.json
-src/extractor_data/bdt_eff/v2/eff_r1_ETOS.json
-src/extractor_data/bdt_eff/v2/eff_r1_GTIS.json
-src/extractor_data/bdt_eff/v2/eff_r1_MTOS.json
-src/extractor_data/bdt_eff/v2/eff_r2p1_ETOS.json
-src/extractor_data/bdt_eff/v2/eff_r2p1_GTIS.json
-src/extractor_data/bdt_eff/v2/eff_r2p1_MTOS.json
 src/extractor_data/config/__init__.py
 src/extractor_data/config/v1.toml
 src/extractor_data/config/v2.toml
+src/extractor_data/config/v3.toml
 src/extractor_data/npr_data/__init__.py
 src/extractor_data/npr_data/v65_v63_v24/eff_ee.json
 src/extractor_data/npr_data/v65_v63_v24/eff_mm.json
 src/extractor_data/npr_data/v65_v63_v24/sta_ee.json
 src/extractor_data/npr_data/v65_v63_v24/sta_mm.json
 src/extractor_data/npr_data/v65_v63_v24/sys_ee.json
 src/extractor_data/npr_data/v65_v63_v24/sys_mm.json
@@ -158,14 +138,16 @@
 src/extractor_data/sb_fits/v40/all_ETOS.json
 src/extractor_data/sb_fits/v41/all_ETOS.json
 src/extractor_data/sb_fits/v42/all_ETOS.json
 src/extractor_data/sb_fits/v43/all_ETOS.json
 src/extractor_data/sb_fits/v44/all_ETOS.json
 src/extractor_data/sb_fits/v44/all_MTOS.json
 src/extractor_data/sb_fits/v45/all_ETOS.json
+src/extractor_data/sb_fits/v46/all_ETOS.json
+src/extractor_data/sb_fits/v46/all_MTOS.json
 src/extractor_data/sb_fits/v5/2017_ETOS.json
 src/extractor_data/sb_fits/v5/2017_GTIS.json
 src/extractor_data/sb_fits/v5/2017_MTOS.json
 src/extractor_data/sb_fits/v5/2018_ETOS.json
 src/extractor_data/sb_fits/v5/2018_GTIS.json
 src/extractor_data/sb_fits/v5/2018_MTOS.json
 src/extractor_data/sb_fits/v5/all_ETOS.json
@@ -188,14 +170,18 @@
 src/extractor_data/sb_fits/v9/all_GTIS.json
 src/extractor_data/sb_fits/v9/all_MTOS.json
 src/extractor_data/sig_wgt/v1/yld_ETOS_2017.json
 src/extractor_data/sig_wgt/v1/yld_ETOS_2018.json
 src/extractor_data/sig_wgt/v1/yld_ETOS_all.json
 src/extractor_data/sig_wgt/v1/yld_ETOS_r1.json
 src/extractor_data/sig_wgt/v1/yld_ETOS_r2p1.json
+src/extractor_data/sig_wgt/v1/yld_GTIS_2017.json
+src/extractor_data/sig_wgt/v1/yld_GTIS_2018.json
+src/extractor_data/sig_wgt/v1/yld_GTIS_r1.json
+src/extractor_data/sig_wgt/v1/yld_GTIS_r2p1.json
 src/extractor_data/sig_wgt/v1/yld_MTOS_2017.json
 src/extractor_data/sig_wgt/v1/yld_MTOS_2018.json
 src/extractor_data/sig_wgt/v1/yld_MTOS_all.json
 src/extractor_data/sig_wgt/v1/yld_MTOS_r1.json
 src/extractor_data/sig_wgt/v1/yld_MTOS_r2p1.json
 src/rk_extractor.egg-info/PKG-INFO
 src/rk_extractor.egg-info/SOURCES.txt
```

### Comparing `rk_extractor-0.8.8/src/rk_model.py` & `rk_extractor-0.8.9/src/rk_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,26 +336,26 @@
 
         [sbin] = re.match('.*_(\d)', preffix).groups()
         ibin   = int(sbin)
 
         nsig= 100   * ibin + 100
         nbkg= -1500 * ibin + 1e4
 
-        mu  = zfit.Parameter(f'mu_{preffix}', 5280, 5100, 6000)
-        sg  = zfit.Parameter(f'sg_{preffix}',   30,   10,   50)
-        ns  = zfit.Parameter(f'ns_{preffix}', nsig,    0,  1e5)
+        mu  = zfit.Parameter(f'mu_{preffix}' , 5280, 5100, 6000)
+        sg  = zfit.Parameter(f'sg_{preffix}' ,   30,   10,   50)
+        ns  = zfit.Parameter(f'nsg_{preffix}', nsig,    0,  1e5)
         sig = zfit.pdf.Gauss(obs=self._obs, mu=mu, sigma=sg)
         sig = sig.create_extended(ns, name = 'Signal')
 
         lm  = zfit.Parameter(f'lm_{preffix}', -0.001, -0.1,    0)
         bkg = zfit.pdf.Exponential(obs=self._obs, lam=lm)
         nb  = zfit.Parameter(f'ncb_{preffix}', nbkg,    0,  1e5)
         bkg = bkg.create_extended(nb, name = 'Combinatorial')
 
-        pdf = zfit.pdf.SumPDF([sig, bkg], name=f'fake_{preffix}')
+        pdf = zfit.pdf.SumPDF([bkg, sig], name=f'fake_{preffix}')
 
         return pdf
     #---------------------------------------------------------------
     def _get_pdf(self, preffix='', nent=None):
         preffix   = f'{preffix}_{self._preffix}'
 
         if self._fake_model:
@@ -405,15 +405,15 @@
 
         pdf = zfit.pdf.SumPDF(l_pdf)
 
         return pdf
     #---------------------------------------------------------------
     def _get_pdf_names(self):
         d_leg = {}
-        d_leg['prc' ] = r'$\psi(2S) + c\bar{c}$'
+        d_leg['prc' ] = r'$c\Bar{c}_{prc}+\psi(2S)K^+$'
         d_leg['bpks'] = r'$B^+\to K^{*+}e^+e^-$'
         d_leg['bdks'] = r'$B^0\to K^{*0}e^+e^-$'
         d_leg['bsph'] = r'$B_s\to \phi e^+e^-$'
         d_leg['bpk1'] = r'$B^+\to K_{1}e^+e^-$'
         d_leg['bpk2'] = r'$B^+\to K_{2}e^+e^-$'
 
         return d_leg
@@ -440,15 +440,15 @@
 
         log.info(f'Plotting: {key}')
 
         plt_dir = f'{self._out_dir}/plots/models'
         os.makedirs(plt_dir, exist_ok=True)
 
         with zfit.run.set_graph_mode(False):
-            obj= zfp(data=mod.create_sampler(fixed_params=False), model=mod)
+            obj= zfp(data=mod.create_sampler(), model=mod)
             d_plt_set = self._get_plt_set(ext_txt=key)
             obj.plot(**d_plt_set)
 
             log.info(f'Saving to: {plt_dir}/{key}.png')
             plt.savefig(f'{plt_dir}/{key}.png')
             plt.close('all')
```

### Comparing `rk_extractor-0.8.8/src/rkex_model.py` & `rk_extractor-0.8.9/src/rkex_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,21 @@
         self._comb_vers   = 'v1'
         self._l_all_dset  = ['r1', 'r2p1', '2017', '2018'] 
         self._d_lumi      = {'r1' : 3, 'r2p1' : 1.9, '2017' : 1.7, '2018' : 2.1}
         self._scal_vers   = None #For scaling between signal and rare PRec
         self._l_dset      = None
         self._d_mod       = None
         self._out_dir     = None
-        self._kind        = None
+        self._kind        = 'nom' 
         self._initialized = False
     #----------------------------------------------------
     def _initialize(self):
         if self._initialized:
             return
-        log.info('Starting initializing')
+        log.info('Starting initialization')
 
         if self._bdt_bin is None:
             log.error('No BDT bin was specified')
             raise
 
         if self._d_eff is None:
             log.error(f'No efficiencies found, cannot provide data')
@@ -103,27 +103,33 @@
         '''
         log.info(f'Using {value}th BDT bin')
         self._bdt_bin      = value
 
         d_bdt_wp, vra, vcc = extset.get_bdt_bin_settings(bdt_bin = value)
         self._scal_vers    = vra
         self._d_bdt_wp     = d_bdt_wp 
-        #hqm_set.version    = vcc 
     #---------------------------------------------------------------
     def _check_kind(self):
         log.debug(f'Checking model kinds')
-        if self._kind == 'nom':
+        if   self._kind is None:
+            log.error(f'Kind not specified')
+            raise
+        elif self._kind == 'nom':
             log.debug('Using nominal model')
             return
 
         found = False
         for kind in self._l_all_kind:
-            if re.match(kind, self._kind):
-                found = True
-                break
+            try:
+                if re.match(kind, self._kind):
+                    found = True
+                    break
+            except:
+                log.error(f'Cannot match {self._kind} to {kind}')
+                raise
 
         if not found: 
             log.error(f'Model of kind {self._kind} not supported')
             raise
         else:
             log.debug(f'Using model of kind: {self._kind}')
     #----------------------------------------------------
@@ -158,23 +164,21 @@
     def _get_ds_model(self, ds, nent_mm, nent_ee):
         log.info('Getting model')
         self._pdf_mm = self._get_pdf(preffix=f'mm_{ds}', nent=nent_mm)
         self._pdf_ee = self._get_pdf(preffix=f'ee_{ds}', nent=nent_ee)
     
         return self._pdf_mm, self._pdf_ee
     #----------------------------------------------------
-    def _plot_data(self, key, dat):
+    def _plot_data(self, key, arr_dat):
         if self._out_dir is None:
             return
 
         plt_dir = f'{self._out_dir}/plots/data'
         os.makedirs(plt_dir, exist_ok=True)
 
-        arr_dat = dat.value().numpy()
-
         plt.hist(arr_dat, bins=50)
 
         log.info(f'Saving to: {plt_dir}/{key}.png')
         plt.title(f'{key}; {dat.name}')
         plt.savefig(f'{plt_dir}/{key}.png')
         plt.close('all')
     #---------------------------------------------------------------
@@ -415,18 +419,21 @@
             dst_ee         = pdf_ee.create_sampler(fixed_params=False)
 
             if 'TIS' in ds:
                 dst_mm = dst_mm_tos
             else:
                 dst_mm_tos = dst_mm
 
-            d_data[ds]     = dst_mm, dst_ee
+            arr_mm = dst_mm.value().numpy().flatten()
+            arr_ee = dst_ee.value().numpy().flatten()
+
+            d_data[ds]     = arr_mm, arr_ee
 
-            self._plot_data(f'{ds}_mm', dst_mm)
-            self._plot_data(f'{ds}_ee', dst_ee)
+            self._plot_data(f'{ds}_mm', arr_mm)
+            self._plot_data(f'{ds}_ee', arr_ee)
 
             log.debug(f'Electron data: {dst_ee.numpy().shape[0]}')
             log.debug(f'Muon data: {dst_mm.numpy().shape[0]}')
 
         return d_data
     #----------------------------------------------------
     @staticmethod
```

### Comparing `rk_extractor-0.8.8/src/scales.py` & `rk_extractor-0.8.9/src/scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_cmb_eff.py` & `rk_extractor-0.8.9/tests/test_cmb_eff.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_cs_reader.py` & `rk_extractor-0.8.9/tests/test_cs_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_effcalc.py` & `rk_extractor-0.8.9/tests/test_effcalc.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_extractor.py` & `rk_extractor-0.8.9/tests/test_extractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -427,50 +427,32 @@
     result.hesse()
     result.freeze()
     print(result)
 
     delete_all_pars()
 #----------------------------------------------------
 def test_real_const_dset():
-    skip_test()
     log.info('Running: test_dset')
 
-    rdr          = cs_rdr(version='v4', preffix='dset')
-    rdr.cache_dir= 'tests/extractor/real_const_dset/v4_csrdr'
-    d_val, d_var = rdr.get_constraints()
-
     rdr          = np_rdr(sys='v65', sta='v63', yld='v24')
-    rdr.cache    = True
-    rdr.cache_dir= 'tests/extractor/real_const_dset/v65_v63_v24'
-    cv_sys       = rdr.get_cov(kind='sys')
-    cv_sta       = rdr.get_cov(kind='sta')
     d_eff        = rdr.get_eff()
     d_rjpsi      = rdr.get_rjpsi()
     d_byld       = rdr.get_byields()
     d_nent       = rkut.average_byields(d_byld, l_exclude=['TIS'])
     d_rare_yld   = rkut.reso_to_rare(d_nent, kind='jpsi')
 
-    rdr_mc          = mc_rdr(version='v4', real_data=False)
-    rdr_mc.cache    = False
-    rdr_mc.cache_dir= 'tests/extractor/real_const_dset/v4_mcrdr'
-    d_mcmu          = rdr_mc.get_parameter(name='mu')
-    d_mcsg          = rdr_mc.get_parameter(name='sg')
-
-    rdr_dt          = mc_rdr(version='v4', real_data=True)
-    rdr_dt.cache    = False
-    rdr_dt.cache_dir= 'tests/extractor/real_const_dset/v4_dtrdr'
-    d_dtmu          = rdr_dt.get_parameter(name='mu')
-    d_dtsg          = rdr_dt.get_parameter(name='sg')
-
-    mod          = model(preffix='dset', d_eff=d_eff, d_mcmu=d_mcmu, d_mcsg=d_mcsg)
+    mod          = model(preffix='dset', d_eff=d_eff, d_nent=d_rare_yld, l_dset=['all_TOS'])
+    mod.bdt_bin  = 5
+    mod.kind     = 'nom'
+    d_val, d_var = mod.get_cons()
     d_mod        = mod.get_model()
-    d_dat        = mod.get_data(d_nent=d_rare_yld, d_dtmu=d_dtmu, d_dtsg=d_dtsg)
+    d_dat        = mod.get_data()
 
-    obj          = ext(dset=['2018_TOS'])
-    obj.cov      = cv_sys + cv_sta
+    obj          = ext(dset=['all_TOS'])
+    obj.cov      = numpy.array([[0.23]])
     obj.const    = d_val, d_var
     obj.model    = d_mod 
     obj.eff      = d_eff
     obj.data     = d_dat
     obj.rjpsi    = d_rjpsi
     obj.plt_dir  = 'tests/extractor/dset'
     result       = obj.get_fit_result()
@@ -544,25 +526,25 @@
 
     print(result)
 
     delete_all_pars()
 #----------------------------------------------------
 def main():
     utnr.timer_on=True
-    test_real()
+    test_real_const_dset()
     return
+    test_real()
     test_fix_pars()
     test_dmodel()
     test_simple()
     test_combined()
     test_all_years()
     test_real_const()
     test_json()
     test_constraint()
     test_diagonal()
-    test_real_const_dset()
     test_rjpsi()
     test_efficiency()
 #----------------------------------------------------
 if __name__ == '__main__':
     main()
```

### Comparing `rk_extractor-0.8.8/tests/test_mc_reader.py` & `rk_extractor-0.8.9/tests/test_mc_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_model_analyzer.py` & `rk_extractor-0.8.9/tests/test_model_analyzer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_model_manager.py` & `rk_extractor-0.8.9/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_normalizer.py` & `rk_extractor-0.8.9/tests/test_normalizer.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_np_reader.py` & `rk_extractor-0.8.9/tests/test_np_reader.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_rkmodel.py` & `rk_extractor-0.8.9/tests/test_rkmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,22 +208,23 @@
 
     mod         = rk_model(preffix='allyears', d_eff=d_eff, d_nent=d_nent, l_dset=['all_TOS'])
     mod.out_dir = 'tests/rk_model/all_years'
     d_mod       = mod.get_model()
 
     delete_all_pars()
 #----------------------
-def test_data():
+def test_dataset():
     d_eff = {'d1' :   (0.5, 0.4), 'd2' :   (0.4, 0.3), 'd3' :   (0.3, 0.2), 'd4' :   (0.2, 0.1)}
     d_nent= {'d1' :          1e3, 'd2' :          1e3, 'd3' :          1e3, 'd4' :          1e3}
 
     d_eff =rename_keys(d_eff)
     d_nent=rename_keys(d_nent, use_txs=False)
 
     mod         = rk_model(preffix='data', d_eff=d_eff, d_nent=d_nent, l_dset=['2018_TOS'])
+    mod.bdt_bin = 5
     d_mod       = mod.get_data()
 
     delete_all_pars()
 #----------------------
 def test_rseed():
     d_eff = {'d1' :   (0.5, 0.4), 'd2' :   (0.4, 0.3), 'd3' :   (0.3, 0.2), 'd4' :   (0.2, 0.1)}
     d_nent= {'d1' :          1e3, 'd2' :          1e3, 'd3' :          1e3, 'd4' :          1e3}
@@ -268,23 +269,23 @@
     d_mod       = mod.get_cons()
 
     delete_all_pars()
 #----------------------
 def main():
     utnr.timer_on = True
 
-    test_syst()
     return
-    test_bootstrap()
+    test_dataset()
     test_simple()
+    test_syst()
+    test_bootstrap()
     test_bdt_change()
     test_all_tos()
     test_kind()
     test_wp()
-    test_data()
     test_cons()
     test_rseed()
     test_all_years()
 #----------------------
 if __name__ == '__main__':
     main()
```

### Comparing `rk_extractor-0.8.8/tests/test_rkrx_model.py` & `rk_extractor-0.8.9/tests/test_rkrx_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     d_mcsg= {'d1' :      (2,  4), 'd2' :     (1, 1.8), 'd3' :       (2, 3), 'd4' :       (3, 4)}
 
     d_eff =rename_keys(d_eff)
     d_nent=rename_keys(d_nent, use_txs=False)
     d_mcmu=rename_keys(d_mcmu)
     d_mcsg=rename_keys(d_mcsg)
 
-    mod         = model(preffix='simple', d_eff=d_eff, d_mcmu=d_mcmu, d_mcsg=d_mcsg, d_nent=d_nent)
+    mod         = model(preffix='simple', d_eff=d_eff, d_nent=d_nent, l_dset=['all_TOS'])
     d_mod       = mod.get_model()
     model.show(d_mod)
 
     delete_all_pars()
 #----------------------
 def test_data():
     d_eff = {'d1' :   (0.5, 0.4), 'd2' :   (0.4, 0.3), 'd3' :   (0.3, 0.2), 'd4' :   (0.2, 0.1)}
@@ -175,14 +175,15 @@
 
     pprint.pprint(d_par)
 
     delete_all_pars()
 #----------------------
 def main():
     test_print()
+    return
     test_simple()
     test_const()
     test_data()
     test_real()
     test_pars()
 #----------------------
 if __name__ == '__main__':
```

### Comparing `rk_extractor-0.8.8/tests/test_scales.py` & `rk_extractor-0.8.9/tests/test_scales.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_scl_mkr.py` & `rk_extractor-0.8.9/tests/test_scl_mkr.py`

 * *Files identical despite different names*

### Comparing `rk_extractor-0.8.8/tests/test_scl_rdr.py` & `rk_extractor-0.8.9/tests/test_scl_rdr.py`

 * *Files identical despite different names*

