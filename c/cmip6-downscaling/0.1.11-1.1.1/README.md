# Comparing `tmp/cmip6-downscaling-0.1.11.tar.gz` & `tmp/cmip6_downscaling-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmip6-downscaling-0.1.11.tar", last modified: Fri Sep 30 21:19:20 2022, max compression
+gzip compressed data, was "cmip6_downscaling-1.1.1.tar", last modified: Tue Apr 16 17:05:27 2024, max compression
```

## Comparing `cmip6-downscaling-0.1.11.tar` & `cmip6_downscaling-1.1.1.tar`

### file list

```diff
@@ -1,408 +1,392 @@
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.089787 cmip6-downscaling-0.1.11/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.985705 cmip6-downscaling-0.1.11/.github/
--rw-r--r--   0 nrhagen    (501) staff       (20)      199 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/.github/dependabot.yml
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.985873 cmip6-downscaling-0.1.11/.github/workflows/
--rw-r--r--   0 nrhagen    (501) staff       (20)      670 2022-09-30 20:16:27.000000 cmip6-downscaling-0.1.11/.github/workflows/main.yaml
--rw-r--r--   0 nrhagen    (501) staff       (20)     1838 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/.gitignore
--rw-r--r--   0 nrhagen    (501) staff       (20)     1211 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/.pre-commit-config.yaml
--rw-r--r--   0 nrhagen    (501) staff       (20)       45 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/.prettierrc.toml
--rw-r--r--   0 nrhagen    (501) staff       (20)     1067 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/LICENSE
--rw-r--r--   0 nrhagen    (501) staff       (20)     3797 2022-09-30 21:19:20.089891 cmip6-downscaling-0.1.11/PKG-INFO
--rw-r--r--   0 nrhagen    (501) staff       (20)     3321 2022-09-19 21:14:58.000000 cmip6-downscaling-0.1.11/README.md
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.987712 cmip6-downscaling-0.1.11/cmip6_downscaling/
--rw-r--r--   0 nrhagen    (501) staff       (20)      357 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      202 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/_version.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.990581 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    39440 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/analyses_template.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     6492 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/analysis.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     7199 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/metrics.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    11957 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/plot.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     1698 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/qaqc.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     3693 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/config.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      399 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/constants.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.991721 cmip6-downscaling-0.1.11/cmip6_downscaling/data/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/data/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     5842 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/data/cmip.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     3723 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/data/observations.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     2153 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/data/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.993382 cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4075 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/derived_variables.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    15410 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/terraclimate.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4509 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/wrapper.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.993567 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/__init__.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.994075 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     9493 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      775 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.995404 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     3406 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/bias_correction.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     2912 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/containers.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    24078 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     9511 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.996174 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      614 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/deepsd_config.ini
--rw-r--r--   0 nrhagen    (501) staff       (20)    17612 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     5015 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.996628 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    10544 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     2948 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.997455 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/__init__.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    12965 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/core.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    11679 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     8371 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/utils.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4941 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/runtimes.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      900 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/cmip6_downscaling/utils.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.988622 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/
--rw-r--r--   0 nrhagen    (501) staff       (20)     3797 2022-09-30 21:19:19.000000 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/PKG-INFO
--rw-r--r--   0 nrhagen    (501) staff       (20)    32465 2022-09-30 21:19:19.000000 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/SOURCES.txt
--rw-r--r--   0 nrhagen    (501) staff       (20)        1 2022-09-30 21:19:19.000000 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/dependency_links.txt
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-09-30 21:19:19.000000 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/requires.txt
--rw-r--r--   0 nrhagen    (501) staff       (20)       18 2022-09-30 21:19:19.000000 cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/top_level.txt
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.981263 cmip6-downscaling-0.1.11/configs/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.997984 cmip6-downscaling-0.1.11/configs/generate_valid_configs/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.010064 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)      490 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      484 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      484 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      480 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      476 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      485 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      481 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      481 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      481 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      475 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      492 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      486 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      488 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      488 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      488 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      482 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      489 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      483 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      483 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      485 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      485 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      485 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      479 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.014798 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)      488 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      495 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      495 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      484 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      484 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      484 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      491 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      498 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      498 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      487 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      487 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.032923 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/
--rw-r--r--   0 nrhagen    (501) staff       (20)      700 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      696 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      696 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      696 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      696 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      692 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      692 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      692 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      687 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      691 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      686 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      702 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      697 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      697 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      698 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      698 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      698 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      693 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      699 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      694 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      694 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      695 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      690 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.035321 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/
--rw-r--r--   0 nrhagen    (501) staff       (20)      720 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      721 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      727 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      731 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      722 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      715 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      724 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      719 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      720 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_ua_va_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      715 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)     7740 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/generate_valid_json_parameters.ipynb
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.044117 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      386 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      378 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      378 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      378 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      382 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      377 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      377 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      377 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      384 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      384 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      384 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      388 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      381 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      385 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)   152313 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/generate_valid_configs/valid_catalog.csv
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.051338 cmip6-downscaling-0.1.11/configs/make_configs/
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      336 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      336 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      328 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      328 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      328 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      332 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      335 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      335 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      327 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      327 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      327 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      331 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      330 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      330 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      322 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      322 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      322 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      326 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
--rw-r--r--   0 nrhagen    (501) staff       (20)    24868 2022-09-27 19:09:40.000000 cmip6-downscaling-0.1.11/datasets.md
--rw-r--r--   0 nrhagen    (501) staff       (20)       51 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/dev-requirements.txt
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.053965 cmip6-downscaling-0.1.11/docs/
--rw-r--r--   0 nrhagen    (501) staff       (20)     6806 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/Makefile
--rw-r--r--   0 nrhagen    (501) staff       (20)     1760 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/docs/api.md
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.054893 cmip6-downscaling-0.1.11/docs/components/
--rw-r--r--   0 nrhagen    (501) staff       (20)      184 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/docs/components/contents.js
--rw-r--r--   0 nrhagen    (501) staff       (20)      716 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/components/section.js
--rw-r--r--   0 nrhagen    (501) staff       (20)     3862 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/components/sidenav.js
--rw-r--r--   0 nrhagen    (501) staff       (20)     6268 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/components/themify.js
--rw-r--r--   0 nrhagen    (501) staff       (20)     2715 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/docs/conf.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      340 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/create-mamba-env.sh
--rw-r--r--   0 nrhagen    (501) staff       (20)      239 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/docs-deploy.sh
--rw-r--r--   0 nrhagen    (501) staff       (20)      618 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/environment.yml
--rwxr-xr-x   0 nrhagen    (501) staff       (20)      132 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/make-sphinx-json.sh
--rw-r--r--   0 nrhagen    (501) staff       (20)      559 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/next.config.js
--rw-r--r--   0 nrhagen    (501) staff       (20)   206558 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/package-lock.json
--rw-r--r--   0 nrhagen    (501) staff       (20)      945 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/package.json
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.055757 cmip6-downscaling-0.1.11/docs/pages/
--rw-r--r--   0 nrhagen    (501) staff       (20)      424 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/_app.js
--rw-r--r--   0 nrhagen    (501) staff       (20)      531 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/_document.js
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.059060 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/
--rw-r--r--   0 nrhagen    (501) staff       (20)      708 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/api-reference.js
--rw-r--r--   0 nrhagen    (501) staff       (20)     3929 2022-07-26 23:58:52.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/downscaling-methods.md
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.059798 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/generated/
--rw-r--r--   0 nrhagen    (501) staff       (20)      922 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/generated/[id].js
--rw-r--r--   0 nrhagen    (501) staff       (20)     1688 2022-07-26 23:58:46.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/index.md
--rw-r--r--   0 nrhagen    (501) staff       (20)     2389 2022-07-26 23:58:46.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/input-datasets.md
--rw-r--r--   0 nrhagen    (501) staff       (20)      164 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/overview.md
--rw-r--r--   0 nrhagen    (501) staff       (20)      841 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/quick-start.md
--rw-r--r--   0 nrhagen    (501) staff       (20)     8594 2022-08-04 21:24:14.000000 cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/running-flows.md
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.060087 cmip6-downscaling-0.1.11/docs/public/
--rw-r--r--   0 nrhagen    (501) staff       (20)        0 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/docs/public/dummy.txt
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.062178 cmip6-downscaling-0.1.11/flows/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.063391 cmip6-downscaling-0.1.11/flows/ERA5/
--rw-r--r--   0 nrhagen    (501) staff       (20)     3964 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/ERA5/ERA5_resample.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     5996 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/ERA5/ERA5_transfer.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.064234 cmip6-downscaling-0.1.11/flows/catalogs/
--rw-r--r--   0 nrhagen    (501) staff       (20)     1894 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/catalogs/era5-full-space.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4225 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/catalogs/era5.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4723 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/catalogs/final_catalog.py
--rw-r--r--   0 nrhagen    (501) staff       (20)    19514 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/catalogs/web_catalog.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     1031 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/cloud_flow_test.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     7537 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/cmip6_raw_pyramids.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4712 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/cmip6_transfer.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     1851 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/downscaled_pyramid_weights.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     3003 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/era5-resample-rechunk.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     4586 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/gcm_obs_weights.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     3250 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/gcm_pyramid_weights.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.982397 cmip6-downscaling-0.1.11/flows/methods/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.064654 cmip6-downscaling-0.1.11/flows/methods/bcsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)     6458 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/methods/bcsd/flow.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.064793 cmip6-downscaling-0.1.11/flows/methods/deepsd/
--rw-r--r--   0 nrhagen    (501) staff       (20)     7720 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/methods/deepsd/flow.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.065129 cmip6-downscaling-0.1.11/flows/methods/gard/
--rw-r--r--   0 nrhagen    (501) staff       (20)     6218 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/methods/gard/flow.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      700 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/flows/methods/gard/multivariate_test.json
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.065369 cmip6-downscaling-0.1.11/flows/methods/maca/
--rw-r--r--   0 nrhagen    (501) staff       (20)     7881 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/methods/maca/flow.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     1469 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/flows/run_subsets_cloud.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.083486 cmip6-downscaling-0.1.11/notebooks/
--rw-r--r--   0 nrhagen    (501) staff       (20)  1066371 2022-09-27 03:14:17.000000 cmip6-downscaling-0.1.11/notebooks/accessing_data_example.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    23913 2022-09-27 03:14:17.000000 cmip6-downscaling-0.1.11/notebooks/catalog_audit.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    21618 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/check_model_completeness.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     5634 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/compare_bcsd.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    44179 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/deepsd_data_prep.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    17741 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/deepsd_inference.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    29111 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/deepsd_model_train.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    15963 2022-09-27 03:14:17.000000 cmip6-downscaling-0.1.11/notebooks/figures.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     5143 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/gard_flow_runs.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)  1495559 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/gard_model_options.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    14380 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/prefect_cloud_runner.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     4125 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/run_analyses.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)    27514 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/scrf.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     5702 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/terraclimate_evaluation.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     6366 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/terraclimate_model.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)     5704 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/workflow.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)  4395376 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/worldcities.csv
--rw-r--r--   0 nrhagen    (501) staff       (20)     3088 2022-06-30 21:01:55.000000 cmip6-downscaling-0.1.11/notebooks/xpersist_overwrite_example.ipynb
--rw-r--r--   0 nrhagen    (501) staff       (20)      252 2022-09-30 20:40:10.000000 cmip6-downscaling-0.1.11/pyproject.toml
--rw-r--r--   0 nrhagen    (501) staff       (20)      416 2022-09-30 20:16:27.000000 cmip6-downscaling-0.1.11/requirements.txt
--rw-r--r--   0 nrhagen    (501) staff       (20)      621 2022-09-30 21:19:20.090401 cmip6-downscaling-0.1.11/setup.cfg
--rw-r--r--   0 nrhagen    (501) staff       (20)     1399 2022-09-30 21:19:17.000000 cmip6-downscaling-0.1.11/setup.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.089166 cmip6-downscaling-0.1.11/tests/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.089364 cmip6-downscaling-0.1.11/tests/analysis/
--rw-r--r--   0 nrhagen    (501) staff       (20)      770 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/analysis/test_metrics.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     1106 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/conftest.py
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:19.982730 cmip6-downscaling-0.1.11/tests/methods/
-drwxr-xr-x   0 nrhagen    (501) staff       (20)        0 2022-09-30 21:19:20.089527 cmip6-downscaling-0.1.11/tests/methods/common/
--rw-r--r--   0 nrhagen    (501) staff       (20)     5495 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/methods/common/test_tasks.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      653 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/test_config.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      494 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/test_data.py
--rw-r--r--   0 nrhagen    (501) staff       (20)      421 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/test_runtimes.py
--rw-r--r--   0 nrhagen    (501) staff       (20)     2041 2022-09-30 21:07:55.000000 cmip6-downscaling-0.1.11/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:26.998131 cmip6_downscaling-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.002131 cmip6_downscaling-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.prettierrc.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.002131 cmip6_downscaling-1.1.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/ci/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.006131 cmip6_downscaling-1.1.1/cmip6_downscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.006131 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39440 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/analyses_template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7199 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/qaqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.006131 cmip6_downscaling-1.1.1/cmip6_downscaling/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/data/cmip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/data/observations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/derived_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15409 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/terraclimate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/bias_correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/deepsd_config.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    17627 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8371 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/runtimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/cmip6_downscaling/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-16 17:05:26.000000 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32033 2024-04-16 17:05:26.000000 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:05:26.000000 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 17:05:26.000000 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 17:05:26.000000 cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:26.998131 cmip6_downscaling-1.1.1/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.010131 cmip6_downscaling-1.1.1/configs/generate_valid_configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.022130 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/bcsd/bcsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.026130 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/deepsd/deepsd_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.038130 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.038130 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_ua_va_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/generate_valid_json_parameters.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.046130 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_pr_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_tasmax_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/maca/maca_ERA5_NorESM2-LM_r1i1p1f1_ssp245_tasmin_-90_90_-180_180_1981_2010_1950_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)   152313 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/generate_valid_configs/valid_catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.054130 cmip6_downscaling-1.1.1/configs/make_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_AWI-CM-1-1-M_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_BCC-CSM2-MR_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_historical_pr_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_historical_tasmax_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_historical_tasmin_-90_90_-180_180_1981_2010_1950_2014.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp245_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
+-rw-r--r--   0 runner    (1001) docker     (127)   127431 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/datasets.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.054130 cmip6_downscaling-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.054130 cmip6_downscaling-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    26339 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/_static/monogram-dark-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23620 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/_static/monogram-light-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/downscaling-methods.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/input-datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/quick-start.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/docs/running-flows.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.054130 cmip6_downscaling-1.1.1/flows/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.054130 cmip6_downscaling-1.1.1/flows/ERA5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/ERA5/ERA5_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/ERA5/ERA5_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.058130 cmip6_downscaling-1.1.1/flows/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/catalogs/era5-full-space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/catalogs/era5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/catalogs/final_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/catalogs/web_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/cloud_flow_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/cmip6_raw_pyramids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/cmip6_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/downscaled_pyramid_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/era5-resample-rechunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/gcm_obs_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/gcm_pyramid_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.002131 cmip6_downscaling-1.1.1/flows/methods/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.058130 cmip6_downscaling-1.1.1/flows/methods/bcsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/methods/bcsd/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.058130 cmip6_downscaling-1.1.1/flows/methods/deepsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     7718 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/methods/deepsd/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.058130 cmip6_downscaling-1.1.1/flows/methods/gard/
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/methods/gard/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/methods/gard/multivariate_test.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.058130 cmip6_downscaling-1.1.1/flows/methods/maca/
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/methods/maca/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/resample_to_yearly_monthly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/flows/run_subsets_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)  1066371 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/accessing_data_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23913 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/catalog_audit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21614 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/check_model_completeness.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/compare_bcsd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44169 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/deepsd_data_prep.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/deepsd_inference.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/deepsd_model_train.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/figures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/gard_flow_runs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1495559 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/gard_model_options.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/prefect_cloud_runner.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/run_analyses.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/scrf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/terraclimate_evaluation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/terraclimate_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5704 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/workflow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  4395376 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/worldcities.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/notebooks/xpersist_overwrite_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/analysis/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.002131 cmip6_downscaling-1.1.1/tests/methods/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:05:27.070130 cmip6_downscaling-1.1.1/tests/methods/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/methods/common/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/test_runtimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-16 17:05:18.000000 cmip6_downscaling-1.1.1/tests/test_utils.py
```

### Comparing `cmip6-downscaling-0.1.11/.gitignore` & `cmip6_downscaling-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/.pre-commit-config.yaml` & `cmip6_downscaling-1.1.1/.pre-commit-config.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,44 @@
 ci:
   autoupdate_schedule: quarterly
   autofix_prs: false
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-docstring-first
       - id: check-json
       - id: check-yaml
       - id: debug-statements
       - id: mixed-line-ending
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.14.0
     hooks:
       - id: pyupgrade
         args:
           - '--py38-plus'
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.9.1
     hooks:
       - id: black
       - id: black-jupyter
 
   - repo: https://github.com/keewis/blackdoc
-    rev: v0.3.4
+    rev: v0.3.8
     hooks:
       - id: blackdoc
 
-  - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: 'v0.0.276'
     hooks:
-      - id: flake8
-
-  - repo: https://github.com/asottile/seed-isort-config
-    rev: v2.2.0
-    hooks:
-      - id: seed-isort-config
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+      - id: ruff
+        args: ['--fix']
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.7.1
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
-        language_version: system
-        additional_dependencies:
-          - prettier
-          - '@carbonplan/prettier'
```

### Comparing `cmip6-downscaling-0.1.11/LICENSE` & `cmip6_downscaling-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/PKG-INFO` & `cmip6_downscaling-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,238 +1,214 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 636d 6970  : 2.1.Name: cmip
-00000020: 362d 646f 776e 7363 616c 696e 670a 5665  6-downscaling.Ve
-00000030: 7273 696f 6e3a 2030 2e31 2e31 310a 5375  rsion: 0.1.11.Su
-00000040: 6d6d 6172 793a 2063 6c69 6d61 7465 2064  mmary: climate d
-00000050: 6f77 6e73 6361 6c69 6e67 2075 7369 6e67  ownscaling using
-00000060: 2063 6d69 7036 2064 6174 610a 486f 6d65   cmip6 data.Home
-00000070: 2d70 6167 653a 2068 7474 7073 3a2f 2f67  -page: https://g
-00000080: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
-00000090: 706c 616e 2f63 6d69 7036 2d64 6f77 6e73  plan/cmip6-downs
-000000a0: 6361 6c69 6e67 0a4d 6169 6e74 6169 6e65  caling.Maintaine
-000000b0: 723a 205b 274f 7269 616e 6120 4368 6567  r: ['Oriana Cheg
-000000c0: 7769 6464 656e 272c 2027 5261 7068 6165  widden', 'Raphae
-000000d0: 6c20 4861 6765 6e27 2c20 274a 6f65 2048  l Hagen', 'Joe H
-000000e0: 616d 6d61 6e27 2c20 2741 6e64 6572 736f  amman', 'Anderso
-000000f0: 6e20 4261 6e69 6869 7277 6527 2c20 274d  n Banihirwe', 'M
-00000100: 6178 204a 6f6e 6573 275d 0a4c 6963 656e  ax Jones'].Licen
-00000110: 7365 3a20 4d49 540a 4b65 7977 6f72 6473  se: MIT.Keywords
-00000120: 3a20 6361 7262 6f6e 2c64 6174 612c 636c  : carbon,data,cl
-00000130: 696d 6174 652c 646f 776e 7363 616c 696e  imate,downscalin
-00000140: 670a 506c 6174 666f 726d 3a20 554e 4b4e  g.Platform: UNKN
-00000150: 4f57 4e0a 5265 7175 6972 6573 2d50 7974  OWN.Requires-Pyt
-00000160: 686f 6e3a 203e 3d33 2e38 0a44 6573 6372  hon: >=3.8.Descr
-00000170: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
-00000180: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
-00000190: 776e 0a50 726f 7669 6465 732d 4578 7472  wn.Provides-Extr
-000001a0: 613a 2064 6565 7073 640a 5072 6f76 6964  a: deepsd.Provid
-000001b0: 6573 2d45 7874 7261 3a20 616e 616c 7973  es-Extra: analys
-000001c0: 6973 0a4c 6963 656e 7365 2d46 696c 653a  is.License-File:
-000001d0: 204c 4943 454e 5345 0a0a 3c69 6d67 0a20   LICENSE..<img. 
-000001e0: 2073 7263 3d27 6874 7470 733a 2f2f 6361   src='https://ca
-000001f0: 7262 6f6e 706c 616e 2d61 7373 6574 732e  rbonplan-assets.
-00000200: 7333 2e61 6d61 7a6f 6e61 7773 2e63 6f6d  s3.amazonaws.com
-00000210: 2f6d 6f6e 6f67 7261 6d2f 6461 726b 2d73  /monogram/dark-s
-00000220: 6d61 6c6c 2e70 6e67 270a 2020 6865 6967  mall.png'.  heig
-00000230: 6874 3d27 3438 270a 2f3e 0a0a 2a2a 636c  ht='48'./>..**cl
-00000240: 696d 6174 6520 646f 776e 6e73 6361 6c69  imate downnscali
-00000250: 6e67 2075 7369 6e67 2063 6d69 7036 2064  ng using cmip6 d
-00000260: 6174 612a 2a0a 0a23 2063 6172 626f 6e70  ata**..# carbonp
-00000270: 6c61 6e20 2f20 636d 6970 362d 646f 776e  lan / cmip6-down
-00000280: 7363 616c 696e 670a 0a5f 4e6f 7465 3a20  scaling.._Note: 
-00000290: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
-000002a0: 756e 6465 7220 6163 7469 7665 2064 6576  under active dev
-000002b0: 656c 6f70 6d65 6e74 2e20 5765 2065 7870  elopment. We exp
-000002c0: 6563 7420 746f 206d 616b 6520 6272 6561  ect to make brea
-000002d0: 6b69 6e67 2063 6861 6e67 6573 2075 6e74  king changes unt
-000002e0: 696c 2072 6561 6368 696e 6720 7665 7273  il reaching vers
-000002f0: 696f 6e20 312e 302e 302e 5f0a 0a5b 215b  ion 1.0.0._..[![
-00000300: 4769 7448 7562 5d5b 6769 7468 7562 2d62  GitHub][github-b
-00000310: 6164 6765 5d5d 5b67 6974 6875 625d 0a5b  adge]][github].[
-00000320: 215b 4275 696c 6420 5374 6174 7573 5d5d  ![Build Status]]
-00000330: 5b61 6374 696f 6e73 5d0a 215b 4d49 5420  [actions].![MIT 
-00000340: 4c69 6365 6e73 655d 5b5d 0a0a 5b67 6974  License][]..[git
-00000350: 6875 625d 3a20 6874 7470 733a 2f2f 6769  hub]: https://gi
-00000360: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
-00000370: 6c61 6e2f 636d 6970 362d 646f 776e 7363  lan/cmip6-downsc
-00000380: 616c 696e 670a 5b67 6974 6875 622d 6261  aling.[github-ba
-00000390: 6467 655d 3a20 6874 7470 733a 2f2f 6261  dge]: https://ba
-000003a0: 6467 656e 2e6e 6574 2f62 6164 6765 2f2d  dgen.net/badge/-
-000003b0: 2f67 6974 6875 623f 6963 6f6e 3d67 6974  /github?icon=git
-000003c0: 6875 6226 6c61 6265 6c0a 5b62 7569 6c64  hub&label.[build
-000003d0: 2073 7461 7475 735d 3a20 6874 7470 733a   status]: https:
-000003e0: 2f2f 6769 7468 7562 2e63 6f6d 2f63 6172  //github.com/car
-000003f0: 626f 6e70 6c61 6e2f 636d 6970 362d 646f  bonplan/cmip6-do
-00000400: 776e 7363 616c 696e 672f 6163 7469 6f6e  wnscaling/action
-00000410: 732f 776f 726b 666c 6f77 732f 6d61 696e  s/workflows/main
-00000420: 2e79 616d 6c2f 6261 6467 652e 7376 670a  .yaml/badge.svg.
-00000430: 5b61 6374 696f 6e73 5d3a 2068 7474 7073  [actions]: https
-00000440: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
-00000450: 7262 6f6e 706c 616e 2f63 6d69 7036 2d64  rbonplan/cmip6-d
-00000460: 6f77 6e73 6361 6c69 6e67 2f61 6374 696f  ownscaling/actio
-00000470: 6e73 2f77 6f72 6b66 6c6f 7773 2f6d 6169  ns/workflows/mai
-00000480: 6e2e 7961 6d6c 0a5b 6d69 7420 6c69 6365  n.yaml.[mit lice
-00000490: 6e73 655d 3a20 6874 7470 733a 2f2f 6261  nse]: https://ba
-000004a0: 6467 656e 2e6e 6574 2f62 6164 6765 2f6c  dgen.net/badge/l
-000004b0: 6963 656e 7365 2f4d 4954 2f62 6c75 650a  icense/MIT/blue.
-000004c0: 0a3c 696d 670a 7372 633d 2768 7474 7073  .<img.src='https
-000004d0: 3a2f 2f69 6d61 6765 732e 6361 7262 6f6e  ://images.carbon
-000004e0: 706c 616e 2e6f 7267 2f68 6967 686c 6967  plan.org/highlig
-000004f0: 6874 732f 636d 6970 362d 646f 776e 7363  hts/cmip6-downsc
-00000500: 616c 696e 672d 6461 726b 2e70 6e67 270a  aling-dark.png'.
-00000510: 2f3e 0a0a 5468 6973 2072 6570 6f73 6974  />..This reposit
-00000520: 6f72 7920 696e 636c 7564 6573 206f 7572  ory includes our
-00000530: 2074 6f6f 6c73 2f73 6372 6970 7473 2f6d   tools/scripts/m
-00000540: 6f64 656c 732f 6574 6320 666f 7220 636c  odels/etc for cl
-00000550: 696d 6174 6520 646f 776e 7363 616c 696e  imate downscalin
-00000560: 672e 2054 6869 7320 776f 726b 2069 7320  g. This work is 
-00000570: 6465 7363 7269 6265 6420 696e 206d 6f72  described in mor
-00000580: 6520 6465 7461 696c 2069 6e20 6120 5b77  e detail in a [w
-00000590: 6562 2061 7274 6963 6c65 5d28 6874 7470  eb article](http
-000005a0: 733a 2f2f 6361 7262 6f6e 706c 616e 2e6f  s://carbonplan.o
-000005b0: 7267 2f72 6573 6561 7263 682f 636d 6970  rg/research/cmip
-000005c0: 362d 646f 776e 7363 616c 696e 672d 6578  6-downscaling-ex
-000005d0: 706c 6169 6e65 7229 2077 6974 680a 6120  plainer) with.a 
-000005e0: 636f 6d70 616e 696f 6e20 5b6d 6170 2074  companion [map t
-000005f0: 6f6f 6c5d 2868 7474 7073 3a2f 2f63 6172  ool](https://car
-00000600: 626f 6e70 6c61 6e2e 6f72 672f 7265 7365  bonplan.org/rese
-00000610: 6172 6368 2f63 6d69 7036 2d64 6f77 6e73  arch/cmip6-downs
-00000620: 6361 6c69 6e67 2920 746f 2065 7870 6c6f  caling) to explo
-00000630: 7265 2074 6865 2064 6174 612e 2057 6520  re the data. We 
-00000640: 656e 636f 7572 6167 6520 796f 7520 746f  encourage you to
-00000650: 2072 6561 6368 206f 7574 2069 6620 796f   reach out if yo
-00000660: 7520 6172 6520 696e 7465 7265 7374 6564  u are interested
-00000670: 2069 6e20 7573 696e 6720 7468 6520 636f   in using the co
-00000680: 6465 206f 7220 6461 7461 7365 7473 2062  de or datasets b
-00000690: 7920 5b6f 7065 6e69 6e67 2061 6e20 6973  y [opening an is
-000006a0: 7375 655d 2868 7474 7073 3a2f 2f67 6974  sue](https://git
-000006b0: 6875 622e 636f 6d2f 6361 7262 6f6e 706c  hub.com/carbonpl
-000006c0: 616e 2f63 6d69 7036 2d64 6f77 6e73 6361  an/cmip6-downsca
-000006d0: 6c69 6e67 2f69 7373 7565 732f 6e65 7729  ling/issues/new)
-000006e0: 206f 7220 5b73 656e 6469 6e67 2075 7320   or [sending us 
-000006f0: 616e 2065 6d61 696c 5d28 6d61 696c 746f  an email](mailto
-00000700: 3a68 656c 6c6f 4063 6172 626f 6e70 6c61  :hello@carbonpla
-00000710: 6e2e 6f72 6729 2e0a 0a23 2320 696e 7374  n.org)...## inst
-00000720: 616c 6c0a 0a60 6060 7368 656c 6c0a 7069  all..```shell.pi
-00000730: 7020 696e 7374 616c 6c20 2d65 202e 0a60  p install -e ..`
-00000740: 6060 0a0a 2323 2075 7361 6765 0a0a 6060  ``..## usage..``
-00000750: 6070 7974 686f 6e0a 6672 6f6d 2063 6d69  `python.from cmi
-00000760: 7036 5f64 6f77 6e73 6361 6c69 6e67 2e6d  p6_downscaling.m
-00000770: 6574 686f 6473 2069 6d70 6f72 7420 2e2e  ethods import ..
-00000780: 2e0a 6060 600a 0a23 2320 6461 7461 2061  ..```..## data a
-00000790: 6363 6573 730a 0a54 6865 7265 2061 7265  ccess..There are
-000007a0: 2074 776f 2077 6179 7320 746f 2061 6363   two ways to acc
-000007b0: 6573 7320 7468 6520 6461 7461 2075 7369  ess the data usi
-000007c0: 6e67 2050 7974 686f 6e2e 0a0a 4669 7273  ng Python...Firs
-000007d0: 742c 2074 6865 2065 6e74 6972 6520 636f  t, the entire co
-000007e0: 6c6c 6563 7469 6f6e 206f 6620 6461 7461  llection of data
-000007f0: 7365 7473 2061 7420 6461 696c 7920 7469  sets at daily ti
-00000800: 6d65 7363 616c 6573 2069 7320 6176 6169  mescales is avai
-00000810: 6c61 626c 6520 7468 726f 7567 6820 616e  lable through an
-00000820: 2060 696e 7461 6b65 6020 6361 7461 6c6f   `intake` catalo
-00000830: 6720 7573 696e 6720 7468 6520 666f 6c6c  g using the foll
-00000840: 6f77 696e 6720 636f 6465 2073 6e69 7070  owing code snipp
-00000850: 6574 2e0a 0a60 6060 0a69 6d70 6f72 7420  et...```.import 
-00000860: 696e 7461 6b65 0a63 6174 203d 2069 6e74  intake.cat = int
-00000870: 616b 652e 6f70 656e 5f65 736d 5f64 6174  ake.open_esm_dat
-00000880: 6173 746f 7265 280a 2020 2768 7474 7073  astore(.  'https
-00000890: 3a2f 2f63 7064 6174 6165 7577 6573 742e  ://cpdataeuwest.
-000008a0: 626c 6f62 2e63 6f72 652e 7769 6e64 6f77  blob.core.window
-000008b0: 732e 6e65 742f 6370 2d63 6d69 702f 7665  s.net/cp-cmip/ve
-000008c0: 7273 696f 6e31 2f63 6174 616c 6f67 732f  rsion1/catalogs/
-000008d0: 676c 6f62 616c 2d64 6f77 6e73 6361 6c65  global-downscale
-000008e0: 642d 636d 6970 362e 6a73 6f6e 270a 290a  d-cmip6.json'.).
-000008f0: 6060 600a 0a59 6f75 2063 616e 2063 6865  ```..You can che
-00000900: 636b 206f 7574 2074 6869 7320 6578 616d  ck out this exam
-00000910: 706c 6520 5b4a 7570 7974 6572 206e 6f74  ple [Jupyter not
-00000920: 6562 6f6f 6b5d 2868 7474 7073 3a2f 2f67  ebook](https://g
-00000930: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
-00000940: 706c 616e 2f63 6d69 7036 2d64 6f77 6e73  plan/cmip6-downs
-00000950: 6361 6c69 6e67 2f62 6c6f 622f 6d61 696e  caling/blob/main
-00000960: 2f6e 6f74 6562 6f6f 6b73 2f61 6363 6573  /notebooks/acces
-00000970: 7369 6e67 5f64 6174 615f 6578 616d 706c  sing_data_exampl
-00000980: 652e 6970 796e 6229 2074 6f20 7365 6520  e.ipynb) to see 
-00000990: 686f 7720 746f 2061 6363 6573 7320 7468  how to access th
-000009a0: 6520 6461 7461 2c20 7065 7266 6f72 6d20  e data, perform 
-000009b0: 736f 6d65 2073 696d 706c 6520 616e 616c  some simple anal
-000009c0: 7973 6973 2c20 616e 6420 646f 776e 6c6f  ysis, and downlo
-000009d0: 6164 2073 7562 7365 7473 2e0a 0a59 6f75  ad subsets...You
-000009e0: 2063 616e 2061 6c73 6f20 6163 6365 7373   can also access
-000009f0: 2074 6865 2064 6174 6120 6279 2075 7369   the data by usi
-00000a00: 6e67 2074 6865 2055 524c 206f 6620 616e  ng the URL of an
-00000a10: 2069 6e64 6976 6964 7561 6c20 6461 7461   individual data
-00000a20: 7365 742e 2053 6565 205b 7468 6520 6461  set. See [the da
-00000a30: 7461 7365 7473 2070 6167 655d 2864 6174  tasets page](dat
-00000a40: 6173 6574 732e 6d64 2920 666f 7220 6120  asets.md) for a 
-00000a50: 7461 626c 6520 6f66 2061 6c6c 2061 7661  table of all ava
-00000a60: 696c 6162 6c65 2064 6174 6173 6574 7320  ilable datasets 
-00000a70: 696e 2074 6869 7320 636f 6c6c 6563 7469  in this collecti
-00000a80: 6f6e 2077 6974 6820 7374 6f72 6167 6520  on with storage 
-00000a90: 6c6f 6361 7469 6f6e 7320 616e 6420 6f74  locations and ot
-00000aa0: 6865 7220 6d65 7461 6461 7461 2e20 4120  her metadata. A 
-00000ab0: 636f 6465 2073 6e69 7070 6574 2073 686f  code snippet sho
-00000ac0: 7769 6e67 2068 6f77 2074 6f20 7573 6520  wing how to use 
-00000ad0: 7468 6520 5552 4c20 6973 2073 686f 776e  the URL is shown
-00000ae0: 2062 656c 6f77 3a0a 0a60 6060 0a69 6d70   below:..```.imp
-00000af0: 6f72 7420 7861 7272 6179 2061 7320 7872  ort xarray as xr
-00000b00: 0a78 722e 6f70 656e 5f7a 6172 7228 2768  .xr.open_zarr('h
-00000b10: 7474 7073 3a2f 2f63 7064 6174 6165 7577  ttps://cpdataeuw
-00000b20: 6573 742e 626c 6f62 2e63 6f72 652e 7769  est.blob.core.wi
-00000b30: 6e64 6f77 732e 6e65 742f 6370 2d63 6d69  ndows.net/cp-cmi
-00000b40: 702f 7665 7273 696f 6e31 2f64 6174 612f  p/version1/data/
-00000b50: 4465 6570 5344 2f53 6365 6e61 7269 6f4d  DeepSD/ScenarioM
-00000b60: 4950 2e43 4343 6d61 2e43 616e 4553 4d35  IP.CCCma.CanESM5
-00000b70: 2e73 7370 3234 352e 7231 6931 7031 6631  .ssp245.r1i1p1f1
-00000b80: 2e64 6179 2e44 6565 7053 442e 7072 2e7a  .day.DeepSD.pr.z
-00000b90: 6172 7227 290a 6060 600a 0a23 2320 6c69  arr').```..## li
-00000ba0: 6365 6e73 650a 0a41 6c6c 2074 6865 2063  cense..All the c
-00000bb0: 6f64 6520 696e 2074 6869 7320 7265 706f  ode in this repo
-00000bc0: 7369 746f 7279 2069 7320 5b4d 4954 5d28  sitory is [MIT](
-00000bd0: 6874 7470 733a 2f2f 6368 6f6f 7365 616c  https://chooseal
-00000be0: 6963 656e 7365 2e63 6f6d 2f6c 6963 656e  icense.com/licen
-00000bf0: 7365 732f 6d69 742f 2920 6c69 6365 6e73  ses/mit/) licens
-00000c00: 6564 2e20 536f 6d65 206f 6620 7468 6520  ed. Some of the 
-00000c10: 6461 7461 2070 726f 7669 6465 6420 6279  data provided by
-00000c20: 2074 6869 7320 4150 4920 6973 2073 6f75   this API is sou
-00000c30: 7263 6564 2066 726f 6d20 636f 6e74 656e  rced from conten
-00000c40: 7420 6d61 6465 2061 7661 696c 6162 6c65  t made available
-00000c50: 2075 6e64 6572 2061 205b 4343 2d42 592d   under a [CC-BY-
-00000c60: 342e 305d 2868 7474 7073 3a2f 2f63 686f  4.0](https://cho
-00000c70: 6f73 6561 6c69 6365 6e73 652e 636f 6d2f  osealicense.com/
-00000c80: 6c69 6365 6e73 6573 2f63 632d 6279 2d34  licenses/cc-by-4
-00000c90: 2e30 2f29 206c 6963 656e 7365 2e20 5765  .0/) license. We
-00000ca0: 2069 6e63 6c75 6465 2061 7474 7269 6275   include attribu
-00000cb0: 7469 6f6e 2066 6f72 2074 6869 7320 636f  tion for this co
-00000cc0: 6e74 656e 742c 2061 6e64 2077 6520 706c  ntent, and we pl
-00000cd0: 6561 7365 2072 6571 7565 7374 2074 6861  ease request tha
-00000ce0: 7420 796f 7520 616c 736f 206d 6169 6e74  t you also maint
-00000cf0: 6169 6e20 7468 6174 2061 7474 7269 6275  ain that attribu
-00000d00: 7469 6f6e 2069 6620 7573 696e 6720 7468  tion if using th
-00000d10: 6973 2064 6174 612e 0a0a 2323 2061 626f  is data...## abo
-00000d20: 7574 2075 730a 0a43 6172 626f 6e50 6c61  ut us..CarbonPla
-00000d30: 6e20 6973 2061 206e 6f6e 2d70 726f 6669  n is a non-profi
-00000d40: 7420 6f72 6761 6e69 7a61 7469 6f6e 2074  t organization t
-00000d50: 6861 7420 7573 6573 2064 6174 6120 616e  hat uses data an
-00000d60: 6420 7363 6965 6e63 6520 666f 7220 636c  d science for cl
-00000d70: 696d 6174 6520 6163 7469 6f6e 2e20 5765  imate action. We
-00000d80: 2061 696d 2074 6f20 696d 7072 6f76 6520   aim to improve 
-00000d90: 7468 6520 7472 616e 7370 6172 656e 6379  the transparency
-00000da0: 2061 6e64 2073 6369 656e 7469 6669 6320   and scientific 
-00000db0: 696e 7465 6772 6974 7920 6f66 2063 6172  integrity of car
-00000dc0: 626f 6e20 7265 6d6f 7661 6c20 616e 6420  bon removal and 
-00000dd0: 636c 696d 6174 6520 736f 6c75 7469 6f6e  climate solution
-00000de0: 7320 7468 726f 7567 6820 6f70 656e 2064  s through open d
-00000df0: 6174 6120 616e 6420 746f 6f6c 732e 2046  ata and tools. F
-00000e00: 696e 6420 6f75 7420 6d6f 7265 2061 7420  ind out more at 
-00000e10: 5b63 6172 626f 6e70 6c61 6e2e 6f72 675d  [carbonplan.org]
-00000e20: 2868 7474 7073 3a2f 2f63 6172 626f 6e70  (https://carbonp
-00000e30: 6c61 6e2e 6f72 672f 2920 6f72 2067 6574  lan.org/) or get
-00000e40: 2069 6e20 746f 7563 6820 6279 205b 6f70   in touch by [op
-00000e50: 656e 696e 6720 616e 2069 7373 7565 5d28  ening an issue](
-00000e60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000e70: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 636d  om/carbonplan/cm
-00000e80: 6970 362d 646f 776e 7363 616c 696e 672f  ip6-downscaling/
-00000e90: 6973 7375 6573 2f6e 6577 2920 6f72 205b  issues/new) or [
-00000ea0: 7365 6e64 696e 6720 7573 2061 6e20 656d  sending us an em
-00000eb0: 6169 6c5d 286d 6169 6c74 6f3a 6865 6c6c  ail](mailto:hell
-00000ec0: 6f40 6361 7262 6f6e 706c 616e 2e6f 7267  o@carbonplan.org
-00000ed0: 292e 0a0a 0a                             )....
+00000000: 3c70 2061 6c69 676e 3d22 6c65 6674 2220  <p align="left" 
+00000010: 3e0a 3c61 2068 7265 663d 2768 7474 7073  >.<a href='https
+00000020: 3a2f 2f63 6172 626f 6e70 6c61 6e2e 6f72  ://carbonplan.or
+00000030: 6727 3e0a 3c70 6963 7475 7265 3e0a 2020  g'>.<picture>.  
+00000040: 3c73 6f75 7263 6520 6d65 6469 613d 2228  <source media="(
+00000050: 7072 6566 6572 732d 636f 6c6f 722d 7363  prefers-color-sc
+00000060: 6865 6d65 3a20 6461 726b 2922 2073 7263  heme: dark)" src
+00000070: 7365 743d 2268 7474 7073 3a2f 2f63 6172  set="https://car
+00000080: 626f 6e70 6c61 6e2d 6173 7365 7473 2e73  bonplan-assets.s
+00000090: 332e 616d 617a 6f6e 6177 732e 636f 6d2f  3.amazonaws.com/
+000000a0: 6d6f 6e6f 6772 616d 2f6c 6967 6874 2d73  monogram/light-s
+000000b0: 6d61 6c6c 2e70 6e67 223e 0a20 203c 696d  mall.png">.  <im
+000000c0: 6720 616c 743d 2243 6172 626f 6e50 6c61  g alt="CarbonPla
+000000d0: 6e20 6d6f 6e6f 6772 616d 2e22 2068 6569  n monogram." hei
+000000e0: 6768 743d 2234 3822 2073 7263 3d22 6874  ght="48" src="ht
+000000f0: 7470 733a 2f2f 6361 7262 6f6e 706c 616e  tps://carbonplan
+00000100: 2d61 7373 6574 732e 7333 2e61 6d61 7a6f  -assets.s3.amazo
+00000110: 6e61 7773 2e63 6f6d 2f6d 6f6e 6f67 7261  naws.com/monogra
+00000120: 6d2f 6461 726b 2d73 6d61 6c6c 2e70 6e67  m/dark-small.png
+00000130: 223e 0a3c 2f70 6963 7475 7265 3e0a 3c2f  ">.</picture>.</
+00000140: 613e 0a3c 2f70 3e0a 0a23 2063 6172 626f  a>.</p>..# carbo
+00000150: 6e70 6c61 6e20 2f20 636d 6970 362d 646f  nplan / cmip6-do
+00000160: 776e 7363 616c 696e 670a 0a2a 2a63 6c69  wnscaling..**cli
+00000170: 6d61 7465 2064 6f77 6e73 6361 6c69 6e67  mate downscaling
+00000180: 2075 7369 6e67 2063 6d69 7036 2064 6174   using cmip6 dat
+00000190: 612a 2a0a 0a5b 215b 4349 5d28 6874 7470  a**..[![CI](http
+000001a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+000001b0: 6172 626f 6e70 6c61 6e2f 636d 6970 362d  arbonplan/cmip6-
+000001c0: 646f 776e 7363 616c 696e 672f 6163 7469  downscaling/acti
+000001d0: 6f6e 732f 776f 726b 666c 6f77 732f 6d61  ons/workflows/ma
+000001e0: 696e 2e79 616d 6c2f 6261 6467 652e 7376  in.yaml/badge.sv
+000001f0: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000200: 7562 2e63 6f6d 2f63 6172 626f 6e70 6c61  ub.com/carbonpla
+00000210: 6e2f 636d 6970 362d 646f 776e 7363 616c  n/cmip6-downscal
+00000220: 696e 672f 6163 7469 6f6e 732f 776f 726b  ing/actions/work
+00000230: 666c 6f77 732f 6d61 696e 2e79 616d 6c29  flows/main.yaml)
+00000240: 0a5b 215b 5079 5049 5d28 6874 7470 733a  .[![PyPI](https:
+00000250: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000260: 2f70 7970 692f 762f 636d 6970 362d 646f  /pypi/v/cmip6-do
+00000270: 776e 7363 616c 696e 6729 5d28 6874 7470  wnscaling)](http
+00000280: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000290: 6a65 6374 2f63 6d69 7036 2d64 6f77 6e73  ject/cmip6-downs
+000002a0: 6361 6c69 6e67 290a 5b21 5b4c 6963 656e  caling).[![Licen
+000002b0: 7365 3a20 4d49 545d 2868 7474 7073 3a2f  se: MIT](https:/
+000002c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+000002d0: 6261 6467 652f 4c69 6365 6e73 652d 4d49  badge/License-MI
+000002e0: 542d 626c 7565 2e73 7667 295d 2868 7474  T-blue.svg)](htt
+000002f0: 7073 3a2f 2f6f 7065 6e73 6f75 7263 652e  ps://opensource.
+00000300: 6f72 672f 6c69 6365 6e73 6573 2f4d 4954  org/licenses/MIT
+00000310: 290a 0a3c 696d 670a 7372 633d 2768 7474  )..<img.src='htt
+00000320: 7073 3a2f 2f69 6d61 6765 732e 6361 7262  ps://images.carb
+00000330: 6f6e 706c 616e 2e6f 7267 2f68 6967 686c  onplan.org/highl
+00000340: 6967 6874 732f 636d 6970 362d 646f 776e  ights/cmip6-down
+00000350: 7363 616c 696e 672d 6461 726b 2e70 6e67  scaling-dark.png
+00000360: 270a 2f3e 0a0a 5468 6973 2072 6570 6f73  './>..This repos
+00000370: 6974 6f72 7920 696e 636c 7564 6573 206f  itory includes o
+00000380: 7572 2074 6f6f 6c73 2f73 6372 6970 7473  ur tools/scripts
+00000390: 2f6d 6f64 656c 732f 6574 6320 666f 7220  /models/etc for 
+000003a0: 636c 696d 6174 6520 646f 776e 7363 616c  climate downscal
+000003b0: 696e 672e 2054 6869 7320 776f 726b 2069  ing. This work i
+000003c0: 7320 6465 7363 7269 6265 6420 696e 206d  s described in m
+000003d0: 6f72 6520 6465 7461 696c 2069 6e20 6120  ore detail in a 
+000003e0: 5b77 6562 2061 7274 6963 6c65 5d28 6874  [web article](ht
+000003f0: 7470 733a 2f2f 6361 7262 6f6e 706c 616e  tps://carbonplan
+00000400: 2e6f 7267 2f72 6573 6561 7263 682f 636d  .org/research/cm
+00000410: 6970 362d 646f 776e 7363 616c 696e 672d  ip6-downscaling-
+00000420: 6578 706c 6169 6e65 7229 2077 6974 680a  explainer) with.
+00000430: 6120 636f 6d70 616e 696f 6e20 5b6d 6170  a companion [map
+00000440: 2074 6f6f 6c5d 2868 7474 7073 3a2f 2f63   tool](https://c
+00000450: 6172 626f 6e70 6c61 6e2e 6f72 672f 7265  arbonplan.org/re
+00000460: 7365 6172 6368 2f63 6d69 7036 2d64 6f77  search/cmip6-dow
+00000470: 6e73 6361 6c69 6e67 2920 746f 2065 7870  nscaling) to exp
+00000480: 6c6f 7265 2074 6865 2064 6174 612e 2057  lore the data. W
+00000490: 6520 656e 636f 7572 6167 6520 796f 7520  e encourage you 
+000004a0: 746f 2072 6561 6368 206f 7574 2069 6620  to reach out if 
+000004b0: 796f 7520 6172 6520 696e 7465 7265 7374  you are interest
+000004c0: 6564 2069 6e20 7573 696e 6720 7468 6520  ed in using the 
+000004d0: 636f 6465 206f 7220 6461 7461 7365 7473  code or datasets
+000004e0: 2062 7920 5b6f 7065 6e69 6e67 2061 6e20   by [opening an 
+000004f0: 6973 7375 655d 2868 7474 7073 3a2f 2f67  issue](https://g
+00000500: 6974 6875 622e 636f 6d2f 6361 7262 6f6e  ithub.com/carbon
+00000510: 706c 616e 2f63 6d69 7036 2d64 6f77 6e73  plan/cmip6-downs
+00000520: 6361 6c69 6e67 2f69 7373 7565 732f 6e65  caling/issues/ne
+00000530: 7729 206f 7220 5b73 656e 6469 6e67 2075  w) or [sending u
+00000540: 7320 616e 2065 6d61 696c 5d28 6d61 696c  s an email](mail
+00000550: 746f 3a68 656c 6c6f 4063 6172 626f 6e70  to:hello@carbonp
+00000560: 6c61 6e2e 6f72 6729 2e0a 0a23 2320 696e  lan.org)...## in
+00000570: 7374 616c 6c0a 0a60 6060 7368 656c 6c0a  stall..```shell.
+00000580: 7079 7468 6f6e 202d 6d20 7069 7020 696e  python -m pip in
+00000590: 7374 616c 6c20 636d 6970 365f 646f 776e  stall cmip6_down
+000005a0: 7363 616c 696e 670a 6060 600a 0a23 2320  scaling.```..## 
+000005b0: 7573 6167 650a 0a60 6060 7079 7468 6f6e  usage..```python
+000005c0: 0a66 726f 6d20 636d 6970 365f 646f 776e  .from cmip6_down
+000005d0: 7363 616c 696e 672e 6d65 7468 6f64 7320  scaling.methods 
+000005e0: 696d 706f 7274 202e 2e2e 0a60 6060 0a0a  import ....```..
+000005f0: 2323 2064 6174 6120 6163 6365 7373 0a0a  ## data access..
+00000600: 5468 6572 6520 6172 6520 7477 6f20 7761  There are two wa
+00000610: 7973 2074 6f20 6163 6365 7373 2074 6865  ys to access the
+00000620: 2064 6174 6120 7573 696e 6720 5079 7468   data using Pyth
+00000630: 6f6e 2e0a 0a46 6972 7374 2c20 7468 6520  on...First, the 
+00000640: 656e 7469 7265 2063 6f6c 6c65 6374 696f  entire collectio
+00000650: 6e20 6f66 2064 6174 6173 6574 7320 6174  n of datasets at
+00000660: 2064 6169 6c79 2074 696d 6573 6361 6c65   daily timescale
+00000670: 7320 6973 2061 7661 696c 6162 6c65 2074  s is available t
+00000680: 6872 6f75 6768 2061 6e20 6069 6e74 616b  hrough an `intak
+00000690: 6560 2063 6174 616c 6f67 2075 7369 6e67  e` catalog using
+000006a0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+000006b0: 6f64 6520 736e 6970 7065 742e 0a0a 6060  ode snippet...``
+000006c0: 600a 696d 706f 7274 2069 6e74 616b 650a  `.import intake.
+000006d0: 6361 7420 3d20 696e 7461 6b65 2e6f 7065  cat = intake.ope
+000006e0: 6e5f 6573 6d5f 6461 7461 7374 6f72 6528  n_esm_datastore(
+000006f0: 0a20 2027 6874 7470 733a 2f2f 6370 6461  .  'https://cpda
+00000700: 7461 6575 7765 7374 2e62 6c6f 622e 636f  taeuwest.blob.co
+00000710: 7265 2e77 696e 646f 7773 2e6e 6574 2f63  re.windows.net/c
+00000720: 702d 636d 6970 2f76 6572 7369 6f6e 312f  p-cmip/version1/
+00000730: 6361 7461 6c6f 6773 2f67 6c6f 6261 6c2d  catalogs/global-
+00000740: 646f 776e 7363 616c 6564 2d63 6d69 7036  downscaled-cmip6
+00000750: 2e6a 736f 6e27 0a29 0a60 6060 0a0a 596f  .json'.).```..Yo
+00000760: 7520 6361 6e20 6368 6563 6b20 6f75 7420  u can check out 
+00000770: 7468 6973 2065 7861 6d70 6c65 205b 4a75  this example [Ju
+00000780: 7079 7465 7220 6e6f 7465 626f 6f6b 5d28  pyter notebook](
+00000790: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000007a0: 6f6d 2f63 6172 626f 6e70 6c61 6e2f 636d  om/carbonplan/cm
+000007b0: 6970 362d 646f 776e 7363 616c 696e 672f  ip6-downscaling/
+000007c0: 626c 6f62 2f6d 6169 6e2f 6e6f 7465 626f  blob/main/notebo
+000007d0: 6f6b 732f 6163 6365 7373 696e 675f 6461  oks/accessing_da
+000007e0: 7461 5f65 7861 6d70 6c65 2e69 7079 6e62  ta_example.ipynb
+000007f0: 2920 746f 2073 6565 2068 6f77 2074 6f20  ) to see how to 
+00000800: 6163 6365 7373 2074 6865 2064 6174 612c  access the data,
+00000810: 2070 6572 666f 726d 2073 6f6d 6520 7369   perform some si
+00000820: 6d70 6c65 2061 6e61 6c79 7369 732c 2061  mple analysis, a
+00000830: 6e64 2064 6f77 6e6c 6f61 6420 7375 6273  nd download subs
+00000840: 6574 732e 0a0a 596f 7520 6361 6e20 616c  ets...You can al
+00000850: 736f 2061 6363 6573 7320 7468 6520 6461  so access the da
+00000860: 7461 2062 7920 7573 696e 6720 7468 6520  ta by using the 
+00000870: 5552 4c20 6f66 2061 6e20 696e 6469 7669  URL of an indivi
+00000880: 6475 616c 2064 6174 6173 6574 2e20 5365  dual dataset. Se
+00000890: 6520 5b74 6865 2064 6174 6173 6574 7320  e [the datasets 
+000008a0: 7061 6765 5d28 6874 7470 733a 2f2f 6769  page](https://gi
+000008b0: 7468 7562 2e63 6f6d 2f63 6172 626f 6e70  thub.com/carbonp
+000008c0: 6c61 6e2f 636d 6970 362d 646f 776e 7363  lan/cmip6-downsc
+000008d0: 616c 696e 672f 626c 6f62 2f6d 6169 6e2f  aling/blob/main/
+000008e0: 6461 7461 7365 7473 2e6d 6429 2066 6f72  datasets.md) for
+000008f0: 2061 2074 6162 6c65 206f 6620 616c 6c20   a table of all 
+00000900: 6176 6169 6c61 626c 6520 6461 7461 7365  available datase
+00000910: 7473 2069 6e20 7468 6973 2063 6f6c 6c65  ts in this colle
+00000920: 6374 696f 6e20 7769 7468 2073 746f 7261  ction with stora
+00000930: 6765 206c 6f63 6174 696f 6e73 2061 6e64  ge locations and
+00000940: 206f 7468 6572 206d 6574 6164 6174 612e   other metadata.
+00000950: 2041 2063 6f64 6520 736e 6970 7065 7420   A code snippet 
+00000960: 7368 6f77 696e 6720 686f 7720 746f 2075  showing how to u
+00000970: 7365 2074 6865 2055 524c 2069 7320 7368  se the URL is sh
+00000980: 6f77 6e20 6265 6c6f 773a 0a0a 6060 600a  own below:..```.
+00000990: 696d 706f 7274 2078 6172 7261 7920 6173  import xarray as
+000009a0: 2078 720a 7872 2e6f 7065 6e5f 7a61 7272   xr.xr.open_zarr
+000009b0: 2827 6874 7470 733a 2f2f 6370 6461 7461  ('https://cpdata
+000009c0: 6575 7765 7374 2e62 6c6f 622e 636f 7265  euwest.blob.core
+000009d0: 2e77 696e 646f 7773 2e6e 6574 2f63 702d  .windows.net/cp-
+000009e0: 636d 6970 2f76 6572 7369 6f6e 312f 6461  cmip/version1/da
+000009f0: 7461 2f44 6565 7053 442f 5363 656e 6172  ta/DeepSD/Scenar
+00000a00: 696f 4d49 502e 4343 436d 612e 4361 6e45  ioMIP.CCCma.CanE
+00000a10: 534d 352e 7373 7032 3435 2e72 3169 3170  SM5.ssp245.r1i1p
+00000a20: 3166 312e 6461 792e 4465 6570 5344 2e70  1f1.day.DeepSD.p
+00000a30: 722e 7a61 7272 2729 0a60 6060 0a0a 2323  r.zarr').```..##
+00000a40: 206c 6963 656e 7365 0a0a 416c 6c20 7468   license..All th
+00000a50: 6520 636f 6465 2069 6e20 7468 6973 2072  e code in this r
+00000a60: 6570 6f73 6974 6f72 7920 6973 205b 4d49  epository is [MI
+00000a70: 545d 2868 7474 7073 3a2f 2f63 686f 6f73  T](https://choos
+00000a80: 6561 6c69 6365 6e73 652e 636f 6d2f 6c69  ealicense.com/li
+00000a90: 6365 6e73 6573 2f6d 6974 2f29 2d6c 6963  censes/mit/)-lic
+00000aa0: 656e 7365 642e 2053 6f6d 6520 6f66 2074  ensed. Some of t
+00000ab0: 6865 2064 6174 6120 7072 6f76 6964 6564  he data provided
+00000ac0: 2062 7920 7468 6973 2041 5049 2069 7320   by this API is 
+00000ad0: 736f 7572 6365 6420 6672 6f6d 2063 6f6e  sourced from con
+00000ae0: 7465 6e74 206d 6164 6520 6176 6169 6c61  tent made availa
+00000af0: 626c 6520 756e 6465 7220 6120 5b43 432d  ble under a [CC-
+00000b00: 4259 2d34 2e30 5d28 6874 7470 733a 2f2f  BY-4.0](https://
+00000b10: 6368 6f6f 7365 616c 6963 656e 7365 2e63  choosealicense.c
+00000b20: 6f6d 2f6c 6963 656e 7365 732f 6363 2d62  om/licenses/cc-b
+00000b30: 792d 342e 302f 2920 6c69 6365 6e73 652e  y-4.0/) license.
+00000b40: 2057 6520 696e 636c 7564 6520 6174 7472   We include attr
+00000b50: 6962 7574 696f 6e20 666f 7220 7468 6973  ibution for this
+00000b60: 2063 6f6e 7465 6e74 2c20 616e 6420 7765   content, and we
+00000b70: 2070 6c65 6173 6520 7265 7175 6573 7420   please request 
+00000b80: 7468 6174 2079 6f75 2061 6c73 6f20 6d61  that you also ma
+00000b90: 696e 7461 696e 2074 6861 7420 6174 7472  intain that attr
+00000ba0: 6962 7574 696f 6e20 6966 2075 7369 6e67  ibution if using
+00000bb0: 2074 6869 7320 6461 7461 2e0a 0a23 2320   this data...## 
+00000bc0: 6162 6f75 7420 7573 0a0a 4361 7262 6f6e  about us..Carbon
+00000bd0: 506c 616e 2069 7320 6120 6e6f 6e70 726f  Plan is a nonpro
+00000be0: 6669 7420 6f72 6761 6e69 7a61 7469 6f6e  fit organization
+00000bf0: 2074 6861 7420 7573 6573 2064 6174 6120   that uses data 
+00000c00: 616e 6420 7363 6965 6e63 6520 666f 7220  and science for 
+00000c10: 636c 696d 6174 6520 6163 7469 6f6e 2e20  climate action. 
+00000c20: 5765 2061 696d 2074 6f20 696d 7072 6f76  We aim to improv
+00000c30: 6520 7468 6520 7472 616e 7370 6172 656e  e the transparen
+00000c40: 6379 2061 6e64 2073 6369 656e 7469 6669  cy and scientifi
+00000c50: 6320 696e 7465 6772 6974 7920 6f66 2063  c integrity of c
+00000c60: 6c69 6d61 7465 2073 6f6c 7574 696f 6e73  limate solutions
+00000c70: 2077 6974 6820 6f70 656e 2064 6174 6120   with open data 
+00000c80: 616e 6420 746f 6f6c 732e 2046 696e 6420  and tools. Find 
+00000c90: 6f75 7420 6d6f 7265 2061 7420 5b63 6172  out more at [car
+00000ca0: 626f 6e70 6c61 6e2e 6f72 675d 2868 7474  bonplan.org](htt
+00000cb0: 7073 3a2f 2f63 6172 626f 6e70 6c61 6e2e  ps://carbonplan.
+00000cc0: 6f72 672f 2920 6f72 2067 6574 2069 6e20  org/) or get in 
+00000cd0: 746f 7563 6820 6279 205b 6f70 656e 696e  touch by [openin
+00000ce0: 6720 616e 2069 7373 7565 5d28 6874 7470  g an issue](http
+00000cf0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000d00: 6172 626f 6e70 6c61 6e2f 636d 6970 362d  arbonplan/cmip6-
+00000d10: 646f 776e 7363 616c 696e 672f 6973 7375  downscaling/issu
+00000d20: 6573 2f6e 6577 2920 6f72 205b 7365 6e64  es/new) or [send
+00000d30: 696e 6720 7573 2061 6e20 656d 6169 6c5d  ing us an email]
+00000d40: 286d 6169 6c74 6f3a 6865 6c6c 6f40 6361  (mailto:hello@ca
+00000d50: 7262 6f6e 706c 616e 2e6f 7267 292e 0a    rbonplan.org)..
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/analyses_template.ipynb` & `cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/analyses_template.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/analysis.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             big_cities = pd.concat(
                 [big_cities, cities[cities['city'] == additional_city][['city', 'lat', 'lng']]]
             )
 
     if plot:
         ax = plt.axes(projection=ccrs.PlateCarree())
         ax.stock_img()
-        for (lat, lon) in big_cities[['lat', 'lng']].values:
+        for lat, lon in big_cities[['lat', 'lng']].values:
             plt.plot(
                 lon,
                 lat,
                 color='blue',
                 marker='o',
             )
     return big_cities
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/metrics.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/metrics.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/plot.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/analysis/qaqc.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/analysis/qaqc.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/config.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/config.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/data/cmip.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/data/cmip.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import dask
 import intake
 import pandas as pd
 import xarray as xr
 
 from .. import config
-from .utils import lon_to_180, to_standard_calendar as convert_to_standard_calendar
+from .utils import lon_to_180
+from .utils import to_standard_calendar as convert_to_standard_calendar
 
 xr.set_options(keep_attrs=True)
 
 
 def postprocess(ds: xr.Dataset, to_standard_calendar: bool = True) -> xr.Dataset:
     """Post process input experiment
 
@@ -53,15 +54,14 @@
         ds = lon_to_180(ds)
 
         # Reorders latitudes to [-90, 90]
         if ds.lat[0] > ds.lat[-1]:
             ds = ds.reindex({"lat": ds.lat[::-1]})
 
         if to_standard_calendar:
-
             # checks calendar
             ds = convert_to_standard_calendar(ds)
 
             # Shifts time from Noon (12:00) start to Midnight (00:00) start to match with Obs
             # ds.coords['time'] = ds['time'].resample(time='1D').first()
 
             ds['time'] = pd.date_range(
@@ -106,15 +106,14 @@
 
     Returns
     -------
     ds : xr.Dataset
         Dataset or zarr group with CMIP data
     """
     with dask.config.set(**{'array.slicing.split_large_chunks': False}):
-
         col = intake.open_esm_datastore(config.get("data_catalog.cmip.json"))
 
         col_subset = col.search(
             activity_id=activity_ids,
             experiment_id=experiment_ids,
             member_id=member_ids,
             source_id=source_ids,
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/data/observations.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/data/observations.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/data/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/data/utils.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/derived_variables.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/derived_variables.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/terraclimate.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/terraclimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,14 @@
         snowpack_prev = 0.0
     if tmean_prev is None:
         tmean_prev = df['tmean'][0]
     if soil_prev is None:
         soil_prev = awc
 
     for i, row in df.iterrows():
-
         radiation = row['srad'] * MGM2D_PER_WM2
 
         # run snow routine
         mfsnow = mf(row['tmean'])
 
         # run pet routine
         pet = monthly_pet(
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/disagg/wrapper.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/disagg/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import os
-from typing import Iterable
+from collections.abc import Iterable
 
 import dask
 import numba
 import numpy as np
 import pandas as pd
 import xarray as xr
 
@@ -87,15 +87,14 @@
     ds_out = create_template(ds_in['ppt'], model_vars)
 
     df_point = pd.DataFrame(
         index=ds_in.indexes['time'], columns=force_vars + model_vars, dtype=np.float32
     )
 
     with dask.config.set(scheduler='single-threaded'):
-
         for index, mask_val in np.ndenumerate(ds_in['mask'].values):
             if not mask_val:
                 # skip values outside the mask
                 continue
             y, x = index
 
             # extract aux vars
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/tasks.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import xarray as xr
 from carbonplan_data.metadata import get_cf_global_attrs
 from prefect import task
 from skdownscale.pointwise_models import PointWiseDownscaler
 from skdownscale.pointwise_models.bcsd import BcsdPrecipitation, BcsdTemperature
 from upath import UPath
 
-from ... import __version__ as version, config
+from ... import __version__ as version
+from ... import config
 from ...constants import ABSOLUTE_VARS, RELATIVE_VARS
 from ...utils import str_to_hash
 from ..common.containers import RunParameters
 from ..common.utils import apply_land_mask, zmetadata_exists
 from .utils import reconstruct_finescale
 
 xr.set_options(keep_attrs=True)
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/bcsd/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/bcsd/utils.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/bias_correction.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/bias_correction.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/containers.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
     def __str__(self) -> str:
         return f"TimePeriod([{self.start}, {self.stop}])"
 
 
 @dataclass
 class CMIP6Experiment:
-
     model: str
     scenario: str
     member: str
 
 
 @dataclass
 class RunParameters:
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/tasks.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 from ndpyramid import pyramid_regrid
 from prefect import task
 from prefect.triggers import any_failed
 from upath import UPath
 from xarray_schema import DataArraySchema, DatasetSchema
 from xarray_schema.base import SchemaError
 
-from ... import __version__ as version, config
+from ... import __version__ as version
+from ... import config
 from ...data.cmip import get_gcm
 from ...data.observations import open_era5
 from ...utils import str_to_hash
 from .containers import RunParameters, TimePeriod
 from .utils import (
     blocking_to_zarr,
     calc_auspicious_chunks_dict,
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/common/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,22 @@
     -------
     valid : bool
     """
     errors = []
 
     try:
         store = zarr.open_consolidated(target)
-    except:
+    except Exception:
         errors.append('error opening zarr store')
 
     if not errors:
         groups = list(store.groups())
         # if groups is empty (not a datatree)
         if not groups:
-            groups = [("root", store["/"])]
+            groups = [('root', store['/'])]
 
         for key, group in groups:
             data_group = group
 
             variables = list(data_group.keys())
             for variable in variables:
                 variable_array = data_group[variable]
@@ -88,15 +88,15 @@
 
     The function blocks until the write is complete then writes Zarr's consolidated metadata
     '''
 
     if write_empty_chunks:
         if packaging.version.Version(
             packaging.version.Version(xr.__version__).base_version
-        ) < packaging.version.Version("2022.03"):
+        ) < packaging.version.Version('2022.03'):
             raise NotImplementedError(
                 f'`write_empty_chunks` not supported in xarray < 2022.06. Your xarray version is: {xr.__version__}'
             )
 
         for variable in ds.data_vars:
             ds[variable].encoding['write_empty_chunks'] = True
     ds = dask.optimize(ds)[0]
@@ -184,15 +184,15 @@
         gdf = gpd.read_file(file)
     mask = regionmask.from_geopandas(gdf).mask(ds, wrap_lon=False)
     return ds.where(mask == 0)
 
 
 def calc_auspicious_chunks_dict(
     da: xr.DataArray,
-    chunk_dims: tuple = ("lat", "lon"),
+    chunk_dims: tuple = ('lat', 'lon'),
 ) -> dict:
     """Figure out a chunk size that, given the size of the dataset, the dimension(s) you want to chunk on
     and the data type, will fit under the target_size. Currently only works for 100mb which
     is the recommended chunk size for dask processing.
 
     Parameters
     ----------
@@ -206,15 +206,15 @@
     chunks_dict : dict
         Dictionary of chunk sizes with the dimensions not listed in `chunk_dims` being the
         length of that dimension (avoiding the shorthand -1 in order to play nice
         with rechunker)
     """
     if not isinstance(chunk_dims, tuple):
         raise TypeError(
-            "Your chunk_dims likely includes one string but needs a comma after it! to be a tuple!"
+            'Your chunk_dims likely includes one string but needs a comma after it! to be a tuple!'
         )
     # setting target_size_bytes to the 100mb chunksize recommended by dask. could modify in future.
     target_size_bytes = 100e6
     dim_sizes = dict(zip(da.dims, da.shape))
 
     # initialize chunks_dict
     chunks_dict = {}
@@ -224,15 +224,15 @@
     for dim in dim_sizes.keys():
         if dim not in chunk_dims:
             # we'll only add the unchunked dimensions to chunks_dict right now
             # rechunker doesn't like the the shorthand of -1 meaning the full length
             # so we'll always just give it the full length of the dimension
             chunks_dict[dim] = dim_sizes[dim]
     # calculate the bytesize given the dtype bitsize and divide by 8
-    data_bytesize = int(re.findall(r"\d+", str(da.dtype))[0]) / 8
+    data_bytesize = int(re.findall(r'\d+', str(da.dtype))[0]) / 8
     # calculate the size of the smallest minimum chunk based upon dtype and the
     # length of the unchunked dim(s). chunks_dict currently only has unchunked dims right now
     smallest_size_one_chunk = data_bytesize * np.prod([dim_sizes[dim] for dim in chunks_dict])
 
     # the dims in chunk_dims should be of an array size (as in number of elements in the array)
     # that creates ~100 mb. `perfect_chunk` is the how many of the smallest_size_chunks you can
     # handle at once while still staying below the `target_size_bytes`
@@ -284,12 +284,11 @@
     # Use _resample_func() to make template dataset
     template = _resample_func(ds, freq=freq).chunk({'time': -1})
     # Apply map_blocks input dataset
     return xr.map_blocks(_resample_func, ds, kwargs={'freq': freq}, template=template)
 
 
 def set_zarr_encoding(ds: xr.Dataset):
-
     for da in ds.data_vars.values():
         da.encoding = {'compressor': zarr.Blosc(clevel=1)}
 
     return ds
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/deepsd_config.ini` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/deepsd_config.ini`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/tasks.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import tensorflow as tf
 import xarray as xr
 import zarr
 from carbonplan_data.metadata import get_cf_global_attrs
 from prefect import task
 from upath import UPath
 
-from ... import __version__ as version, config
+from ... import __version__ as version
+from ... import config
 from ...data.observations import open_era5
 from ...data.utils import lon_to_180
 from ..common.bias_correction import bias_correct_gcm_by_method
 from ..common.containers import RunParameters, str_to_hash
 from ..common.utils import (
     apply_land_mask,
     blocking_to_zarr,
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/deepsd/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/deepsd/utils.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/tasks.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from carbonplan_data.metadata import get_cf_global_attrs
 from prefect import task
 from scipy.special import cbrt
 from skdownscale.pointwise_models import PointWiseDownscaler
 from skdownscale.pointwise_models.utils import default_none_kwargs
 from upath import UPath
 
-from ... import __version__ as version, config
+from ... import __version__ as version
+from ... import config
 from ..common.bias_correction import bias_correct_gcm_by_method
 from ..common.containers import RunParameters, str_to_hash
 from ..common.utils import apply_land_mask, blocking_to_zarr, set_zarr_encoding, zmetadata_exists
 from .utils import add_random_effects, get_gard_model
 
 xr.set_options(keep_attrs=True)
 scratch_dir = UPath(config.get("storage.scratch.uri"))
@@ -66,15 +67,14 @@
     interpolated_ds = set_zarr_encoding(interpolated_ds)
     blocking_to_zarr(ds=interpolated_ds, target=target, validate=True, write_empty_chunks=True)
 
     return target
 
 
 def _fit_and_predict_wrapper(xtrain, ytrain, xpred, scrf, run_parameters, dim='time'):
-
     xpred = xpred.rename({'t2': 'time'})
     scrf = scrf.rename({'t2': 'time'})
     kws = default_none_kwargs(run_parameters.bias_correction_kwargs, copy=True)
 
     # transformed gcm is the interpolated GCM for the prediction period transformed
     # w.r.t. the interpolated obs used in the training (because that transformation
     # is essentially part of the model)
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/gard/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/gard/utils.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/core.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,14 @@
     # pre-load to speed up for loop (lots of indexing into x & y)
     X = X.load()
     y = y.load()
 
     # train a linear regression model for each day in coarsen GCM dataset, where the features are each coarsened observation
     # analogs, and examples are each pixels within the coarsened domain
     for i in range(len(y)):
-
         # get data from the GCM day being downscaled
         yi = y.isel(ndays_in_gcm=i)
         # get data from the coarsened obs analogs
         ind = inds.isel(ndays_in_gcm=i).values
 
         # save obs_analogs for later
         obs_analogs.append(da_obs_fine.isel(time=ind).rename({'time': 'analog'}).drop('analog'))
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/tasks.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import regionmask
 import xarray as xr
 import zarr
 from carbonplan_data.metadata import get_cf_global_attrs
 from prefect import task
 from upath import UPath
 
-from cmip6_downscaling import __version__ as version, config
+from cmip6_downscaling import __version__ as version
+from cmip6_downscaling import config
 from cmip6_downscaling.methods.common.containers import RunParameters
 from cmip6_downscaling.methods.common.utils import blocking_to_zarr, is_cached
 from cmip6_downscaling.methods.maca import core as maca_core
 from cmip6_downscaling.methods.maca.utils import (
     initialize_out_store,
     make_regions_mask,
     merge_block_to_zarr,
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/methods/maca/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/methods/maca/utils.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/runtimes.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/runtimes.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
             image=config.get("runtime.cloud.image"),
             labels=[config.get("runtime.cloud.agent")],
             env=self._generate_env(),
         )
 
     @cached_property
     def executor(self) -> Executor:
-
         executor = DaskExecutor(
             cluster_kwargs={
                 'resources': {'taskslots': 1},
                 'n_workers': config.get("runtime.cloud.n_workers"),
                 'threads_per_worker': config.get("runtime.cloud.threads_per_worker"),
             }
         )
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling/utils.py` & `cmip6_downscaling-1.1.1/cmip6_downscaling/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 def str_to_hash(s: str) -> str:
     return blake2b(s.encode(), digest_size=8).hexdigest()
 
 
 def write(ds: xr.Dataset | datatree.DataTree, target, use_cache: bool = True) -> str:
-
     from .methods.common.utils import zmetadata_exists
 
     if use_cache and zmetadata_exists(target):
         print(f'found existing target: {target}')
         return target
 
     else:
```

### Comparing `cmip6-downscaling-0.1.11/cmip6_downscaling.egg-info/SOURCES.txt` & `cmip6_downscaling-1.1.1/cmip6_downscaling.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 .prettierrc.toml
+.readthedocs.yaml
+.zenodo.json
 LICENSE
 README.md
 datasets.md
-dev-requirements.txt
 pyproject.toml
-requirements.txt
-setup.cfg
-setup.py
-.github/dependabot.yml
 .github/workflows/main.yaml
+.github/workflows/pypi-release.yaml
+ci/environment.yaml
 cmip6_downscaling/__init__.py
 cmip6_downscaling/_version.py
 cmip6_downscaling/config.py
 cmip6_downscaling/constants.py
 cmip6_downscaling/runtimes.py
 cmip6_downscaling/utils.py
 cmip6_downscaling.egg-info/PKG-INFO
@@ -292,45 +291,32 @@
 configs/make_configs/bcsd_ERA5_MIROC6_ssp370_pr_-90_90_-180_180_1981_2010_2015_2099.json
 configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
 configs/make_configs/bcsd_ERA5_MIROC6_ssp370_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
 configs/make_configs/bcsd_ERA5_MIROC6_ssp585_pr_-90_90_-180_180_1981_2010_2015_2099.json
 configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmax_-90_90_-180_180_1981_2010_2015_2099.json
 configs/make_configs/bcsd_ERA5_MIROC6_ssp585_tasmin_-90_90_-180_180_1981_2010_2015_2099.json
 docs/Makefile
-docs/api.md
+docs/api.rst
 docs/conf.py
-docs/create-mamba-env.sh
-docs/docs-deploy.sh
+docs/downscaling-methods.md
 docs/environment.yml
-docs/make-sphinx-json.sh
-docs/next.config.js
-docs/package-lock.json
-docs/package.json
-docs/components/contents.js
-docs/components/section.js
-docs/components/sidenav.js
-docs/components/themify.js
-docs/pages/_app.js
-docs/pages/_document.js
-docs/pages/cmip6-downscaling/api-reference.js
-docs/pages/cmip6-downscaling/downscaling-methods.md
-docs/pages/cmip6-downscaling/index.md
-docs/pages/cmip6-downscaling/input-datasets.md
-docs/pages/cmip6-downscaling/overview.md
-docs/pages/cmip6-downscaling/quick-start.md
-docs/pages/cmip6-downscaling/running-flows.md
-docs/pages/cmip6-downscaling/generated/[id].js
-docs/public/dummy.txt
+docs/index.rst
+docs/input-datasets.md
+docs/quick-start.md
+docs/running-flows.md
+docs/_static/monogram-dark-cropped.png
+docs/_static/monogram-light-cropped.png
 flows/cloud_flow_test.py
 flows/cmip6_raw_pyramids.py
 flows/cmip6_transfer.py
 flows/downscaled_pyramid_weights.py
 flows/era5-resample-rechunk.py
 flows/gcm_obs_weights.py
 flows/gcm_pyramid_weights.py
+flows/resample_to_yearly_monthly.ipynb
 flows/run_subsets_cloud.py
 flows/ERA5/ERA5_resample.py
 flows/ERA5/ERA5_transfer.py
 flows/catalogs/era5-full-space.py
 flows/catalogs/era5.py
 flows/catalogs/final_catalog.py
 flows/catalogs/web_catalog.py
```

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_BCC-CSM2-MR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_CanESM5_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MIROC6_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MPI-ESM1-2-HR_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmin_tasmin_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp245_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp370_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard/gard_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmin_tasmin_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_pr_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_psl_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MIROC6_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_pr_ua_va_pr_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_historical_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_1950_2014.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_ua_va_pr_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_pr_ua_va_pr_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_2015_2099.json` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/gard_multivariate/gard_multivariate_ERA5_MRI-ESM2-0_r1i1p1f1_ssp585_tasmax_ua_va_tasmax_-90_90_-180_180_1981_2010_2015_2099.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/generate_valid_json_parameters.ipynb` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/generate_valid_json_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/configs/generate_valid_configs/valid_catalog.csv` & `cmip6_downscaling-1.1.1/configs/generate_valid_configs/valid_catalog.csv`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/docs/Makefile` & `cmip6_downscaling-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/docs/api.md` & `cmip6_downscaling-1.1.1/docs/api.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,98 @@
-# API
+.. _api:
+
+API
+===
+
+.. automodule:: cmip6_downscaling
 
-```{eval-rst}
 .. currentmodule:: cmip6_downscaling
-```
 
-## Data
+Data
+----
 
-```{eval-rst}
 .. autosummary::
    :toctree: generated/
 
    data.cmip.postprocess
    data.cmip.load_cmip
    data.cmip.get_gcm
 
    data.observations.open_era5
 
    data.utils.to_standard_calendar
    data.utils.lon_to_180
-```
 
-## Downscaling Methods
+Downscaling Methods
+-------------------
 
-```{eval-rst}
 .. currentmodule:: cmip6_downscaling.methods
-```
 
-### BCSD
 
-```{eval-rst}
+BCSD
+----
+
 .. autosummary::
    :toctree: generated/
 
    bcsd.tasks.spatial_anomalies
    bcsd.tasks.fit_and_predict
    bcsd.tasks.postprocess_bcsd
    bcsd.utils.reconstruct_finescale
-```
 
-### GARD
+GARD
+----
 
-```{eval-rst}
 .. autosummary::
    :toctree: generated/
 
    gard.tasks.coarsen_and_interpolate
    gard.tasks.fit_and_predict
    gard.tasks.read_scrf
    gard.utils.get_gard_model
    gard.utils.add_random_effects
 
-```
-
-### DEEPSD
+DEEPSD
+------
 
-```{eval-rst}
 .. autosummary::
    :toctree: generated/
 
    deepsd.tasks.shift
    deepsd.tasks.normalize_gcm
    deepsd.tasks.inference
    deepsd.tasks.rescale
    deepsd.tasks.bias_correction
    deepsd.utils.bilinear_interpolate
    deepsd.utils.conservative_interpolate
    deepsd.utils.normalize
-```
 
-### MACA
+MACA
+----
 
-```{eval-rst}
 .. autosummary::
    :toctree: generated/
 
    maca.tasks.bias_correction
    maca.tasks.epoch_trend
    maca.tasks.construct_analogs
    maca.tasks.split_by_region
    maca.tasks.combine_regions
    maca.tasks.replace_epoch_trend
-```
 
-### Common Tasks
+Common Tasks
+------------
 
-```{eval-rst}
 .. autosummary::
    :toctree: generated/
 
    common.tasks.make_run_parameters
    common.tasks.get_obs
    common.tasks.get_experiment
    common.tasks.rechunk
    common.tasks.time_summary
    common.tasks.get_weights
    common.tasks.get_pyramid_weights
    common.tasks.regrid
    common.tasks.pyramid
    common.tasks.run_analyses
    common.tasks.finalize
-```
```

### Comparing `cmip6-downscaling-0.1.11/docs/conf.py` & `cmip6_downscaling-1.1.1/docs/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,19 +39,23 @@
     "myst_parser",
 ]
 
 autosummary_generate = True
 numpydoc_class_members_toctree = False
 numpydoc_show_class_members = False
 
-# The suffix of source filenames.
-source_suffix = ".rst"
+autodoc_mock_imports = ["xesmf", "tensorflow"]
+
 
-# The master toctree document.
-master_doc = "api"
+# Sphinx project configuration
+source_suffix = ".rst"
+needs_sphinx = "1.8"
+# The encoding of source files.
+source_encoding = "utf-8-sig"
+root_doc = "index"
 
 # General information about the project.
 project = "cmip6_downscaling"
 copyright = "2022, CarbonPlan"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
@@ -64,19 +68,35 @@
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 language = "Python"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ["_build", "node_modules"]
+exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "numpy": ("https://numpy.org/doc/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "python": ("https://docs.python.org/3/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy", None),
 }
+
+# -- Options for HTML output ----------------------------------------------
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+
+html_title = "CMIP6-Downscaling"
+html_theme_options = {
+    "logo": {
+        "image_light": "_static/monogram-dark-cropped.png",
+        "image_dark": "_static/monogram-light-cropped.png",
+    }
+}
+html_theme = "sphinx_book_theme"
+html_title = ""
+repository = "carbonplan/cmip6-downscaling"
+repository_url = "https://github.com/carbonplan/cmip6-downscaling"
```

### Comparing `cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/downscaling-methods.md` & `cmip6_downscaling-1.1.1/docs/downscaling-methods.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-import Section from '../../components/section'
-
 # Downscaling methods
 
 We implemented four downscaling methods globally. Descriptions of these implementations are below, along with references to further information. Our [explainer article](https://carbonplan.org/research/cmip6-downscaling-explainer) discusses the importance of downscaling, and describes some of the key methodological differences, in more detail.
 
-### MACA
+## MACA
 
 The Multivariate Adaptive Constructed Analogs method [(Abatzoglou and Brown, 2012)](https://rmets.onlinelibrary.wiley.com/doi/abs/10.1002/joc.2312) finds common spatial patterns among GCM and reference datasets to construct downscaled future projections from actual weather patterns from the past. The method involves a combination of coarse and fine-scale bias-correction, detrending of GCM data, and analog selection, steps which are detailed thoroughly in the [MACA Datasets documentation](https://climate.northwestknowledge.net/MACA/MACAmethod.php). MACA is designed to operate at the regional scale. As a result, we split the global domain into smaller regions using the AR6 delineations from the `regionmask` [package](https://regionmask.readthedocs.io/en/stable/) and downscaled each region independently. We then stitched the regions back together to create a seamless global product. Of the methods we have implemented, MACA is the most established.
 
-### GARD-SV
+## GARD-SV
 
 The Generalized Analog Regression Downscaling (GARD) (Guttmann et al., in review) approach is a downscaling sandbox that allows scientists to create custom downscaling implementations, supporting single or multiple predictor variables, pure regression and pure analog approaches, and different bias-correction routines. At its core, GARD builds a linear model for every pixel relating the reference dataset at the fine-scale to the same data coarsened to the scale of the GCM. The downscaled projections are then further perturbed by spatially-correlated random fields to reflect the error in the regression models. Our GARD-SV (single-variate) implementation uses the same variable for training and prediction (e.g. precipitation is the only predictor for downscaling precipitation). For regression, we used the PureRegression method, building a single model for each pixel from the entire timeseries of training data. The precipitation model included a logistic regression component, with a threshold of 0 mm/day for constituting a precipitation event.
 
-### GARD-MV
+## GARD-MV
 
 The GARD-MV (multi-variate) implementation follows the same process as the GARD-SV method but uses multiple predictor variables for model training and inference. Specifically, we used three predictors for each downscaling model, adding the two directions of 500mb winds to each model. Thus, the predictors for precipitation in this model are precipitation, longitudinal wind, and latitudinal wind.
 
-### DeepSD
+## DeepSD
 
 DeepSD uses a computer vision approach to learn spatial patterns at multiple resolutions [Vandal et al., 2017](https://dl.acm.org/doi/10.1145/3097983.3098004). Specifically, DeepSD is a stacked super-resolution convolutional neural network. We adapted the [open-source DeepSD implementation](https://github.com/tjvandal/deepsd) for downscaling global ensembles by updating the source code for Python 3 and TensorFlow2, removing the batch normalization layer, normalizing based on historical observations, training models for temperature and precipitation, and training on a global reanalysis product (ERA5). In addition, we trained the model for fewer iterations than in Vandal et al., 2017 and clipped aphysical precipitation values at 0. Our dataset includes an additional bias-corrected product (DeepSD-BC). Given its origin in deep learning, this method is the most different from those included here, and is an experimental contribution to our dataset.
-
-export default ({ children }) => <Section name='Downscaling Methods'>{children}</Section>
```

### Comparing `cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/index.md` & `cmip6_downscaling-1.1.1/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,60 @@
-import Section from '../../components/section'
+.. _Intro:
 
-# CMIP6-Downscaling
+CMIP6-Downscaling
+-----------------
 
 This project implements a collection of statistical climate downscaling methods and provides workflows to generate downscaled climate data.
 
-Statistical climate downscaling refers to a collection of algorithms that, when applied to raw climate model output, correct for systemic biases and generate data at higher spatial resolutions. These methods are an important part of many analytical workflows in climate impacts and climate mitigation.
+Statistical climate downscaling refers to a collection of algorithms that, when applied to raw climate model output, correct for systemic biases
+and generate data at higher spatial resolutions. These methods are an important part of many analytical workflows in climate impacts and climate mitigation.
 
 The project was designed with two primary goals in mind:
 
 1. to provide a sandbox for developing and comparing across a wide range of downscaling methods
 2. to develop production-ready pipelines for downscaling CMIP6 model output.
 
-The package currently provides [Prefect flows](https://docs.prefect.io/core/) for the following methods:
+The package currently provides `Prefect flows <https://docs.prefect.io/core/>`_ for the following methods:
 
-- [Bias-correction and Statistical Downscaling (BCSD)](https://link.springer.com/article/10.1023/B:CLIM.0000013685.99609.9e)
-- [Ensemble Generalized Statistical Downscaling (En-GARD)](https://gard.readthedocs.io/en/develop/)
-- [Multivariate Adapted Constructed Analogs (MACA)](https://doi.org/10.1002/joc.2312)
-- [DeepSD](https://dl.acm.org/doi/10.1145/3097983.3098004)
+- `Bias-correction and Statistical Downscaling (BCSD) <https://link.springer.com/article/10.1023/B:CLIM.0000013685.99609.9e>`_
+- `Ensemble Generalized Statistical Downscaling (En-GARD) <https://gard.readthedocs.io/en/develop/>`_
+- `Multivariate Adapted Constructed Analogs (MACA) <https://doi.org/10.1002/joc.2312>`_
+- `DeepSD <https://dl.acm.org/doi/10.1145/3097983.3098004>`_
 
-Many of these workflows build on or extend functionality in [Scikit-downscale](https://scikit-downscale.readthedocs.io/en/latest/), providing complete end-to-end pipelines for generating downscaled climate data. The workflows are designed to be run on the cloud (Azure West Europe for best performance) but smaller applications should be possible using Prefect's local deployment methods.
+Many of these workflows build on or extend functionality in `Scikit-downscale <https://scikit-downscale.readthedocs.io/en/latest/>`_,
+providing complete end-to-end pipelines for generating downscaled climate data. The workflows are designed to be run on the cloud
+(Azure West Europe for best performance) but smaller applications should be possible using Prefect's local deployment methods.
 
-export default ({ children }) => <Section name='intro'>{children}</Section>
+.. toctree::
+   :hidden:
+
+   self
+
+.. toctree::
+    :maxdepth: 1
+    :hidden:
+    :caption: Getting Started
+
+    Quickstart <quick-start>
+
+.. toctree::
+    :maxdepth: 1
+    :hidden:
+    :caption: How-To Guides
+
+    Running Flows <running-flows>
+
+
+.. toctree::
+    :maxdepth: 1
+    :hidden:
+    :caption: Explanation
+
+    Input Datasets <input-datasets>
+    Downscaling Methods <downscaling-methods>
+
+.. toctree::
+    :maxdepth: 2
+    :hidden:
+    :caption: Reference
+
+    API <api>
```

### Comparing `cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/input-datasets.md` & `cmip6_downscaling-1.1.1/docs/input-datasets.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import Section from '../../components/section'
-
 # Input Datasets
 
 ## CMIP6 raw datasets
 
 The downscaled datasets shown here are derived from results from the [Coupled Model Intercomparison Project Phase 6](https://doi.org/10.5194/gmd-9-1937-2016). Raw datasets are also available in the web catalog (labeled “Raw”). GCMs are run at different spatial resolutions, and the data presented here are displayed in their original spatial resolution. The raw CMIP6 datasets were accessed via the Pangeo data catalog.
 
 ### ERA5 Reanalysis
@@ -26,9 +24,7 @@
 https://apps.ecmwf.int/datasets/licences/general/
 
 ## CMIP6 raw datasets
 
 The downscaled datasets shown here are derived from results from the [Coupled Model Intercomparison Project Phase 6](https://doi.org/10.5194/gmd-9-1937-2016). Raw datasets are also available in the web catalog (labeled “Raw”). GCMs are run at different spatial resolutions, and the data presented here are displayed in their original spatial resolution. The raw CMIP6 datasets were accessed via the Pangeo data catalog.
 
 The transfer script can be found [here](https://github.com/carbonplan/cmip6-downscaling/blob/main/flows/cmip6_transfer.py)
-
-export default ({ children }) => <Section name='Input Datasets'>{children}</Section>
```

### Comparing `cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/quick-start.md` & `cmip6_downscaling-1.1.1/docs/quick-start.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import Section from '../../components/section'
-
 # Quick start
 
 ## Dependencies
 
 - Python 3.8 or later
 - numpy
 - scipy
@@ -21,14 +19,12 @@
 
 ```
 python -m pip install git+https://github.com/carbonplan/cmip6-dowscaling
 ```
 
 ## Usage
 
-The `cmip6-downscaling` package provides a number of downscaling implementations. See the [API docs](/api) for a complete listing of functions and utilities or the [How-to Guides](/how-to-guide) for detailed example on how to use the `cmip6-downscaling` package for specific tasks.
+The `cmip6-downscaling` package provides a number of downscaling implementations. See the [API docs](/api) for a complete listing of functions and utilities or the [Running Flows Guide](/running-flows) for detailed example on how to use the `cmip6-downscaling` package for specific tasks.
 
 ```python
 import cmip6_downscaling
 ```
-
-export default ({ children }) => <Section name='Quick Start'>{children}</Section>
```

### Comparing `cmip6-downscaling-0.1.11/docs/pages/cmip6-downscaling/running-flows.md` & `cmip6_downscaling-1.1.1/docs/running-flows.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,57 @@
-import Section from '../../components/section'
-
 # Running Flows
 
 In this project each downscaling method [BCSD, GARD, MACA, DEEPSD] has it's own workflow for generating results. These data production workflows are handled by the python library, prefect, which encapsulates the data processing steps into individual tasks, which are organized into a 'Flow'.
 
 Prefect allows us to run these downscaling flows with many different parameter combinations (gcms, observations, training period, prediction period) without modifying the specific downscaling method script.
 
 ## Choosing a Runtime
 
 Prefect has the ability to run flows with different `runtimes`. Choosing the correct runtime can be crucial to help with scaling multiple flows or debugging a single issue.
 
 Pre-configured runtimes are stored in [`cmip6_downscaling.runtimes.py`](https://github.com/carbonplan/cmip6-downscaling/blob/main/cmip6_downscaling/runtimes.py)
 
 The current runtime options are:
 
-[`cloud`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L57) `executor: dask-distrubted` - Runtime for queuing multiple flows on prefect cloud.
-
-[`local`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L113) `executor: local` - Runtime for developing on local machine
-
-[`CI`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L130) `executor: local` - Runtime used for Continuous Integration
-
-[`pangeo`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L140) `executor: dask-distrubted` - Runtime for processing on jupyter-hub
+- [`cloud`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L57) `executor: dask-distrubted` - Runtime for queuing multiple flows on prefect cloud.
+- [`local`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L113) `executor: local` - Runtime for developing on local machine
+- [`CI`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L130) `executor: local` - Runtime used for Continuous Integration
+- [`pangeo`](https://github.com/carbonplan/cmip6-downscaling/blob/a0379110c33b557f959a1d6fa53e9f93891a45b3/cmip6_downscaling/runtimes.py#L140) `executor: dask-distrubted` - Runtime for processing on jupyter-hub
 
 ## Infrastructure
 
 These flows were ran on a machine ~32 CPU and ~256GB RAM. The `pangeo` runtime and the `cloud` runtime both used similar spec machines. Using Dask's `LocalCluster` for parallel processing, the 256GB RAM was distributed over the number of workers (max 32). The ideal number of workers for most flows seemed to be 8, giving each worker over 32GB of RAM each. If you are getting `KilledWorker` errors from Dask, try reducing the number of workers. The tradeoff of this is the increase in flow processing time. The number of workers can be set in `config.py`, modifying the line: `'n_workers': 8`.
 
 ## Modifying Flow Config
 
 Project level configuration settings are in [`cmip6_downscaling.config.py`](https://github.com/carbonplan/cmip6-downscaling/blob/main/cmip6_downscaling/config.py) and configured using the python package [`donfig`](https://donfig.readthedocs.io/en/latest/). Default configuration options can be overwritten in multiple ways with donfig. Below are two options for specifying use of the cloud runtime. Note: any `connection_strings` or other sensitive information is best stored in a local .yaml or as an environment variable.
 
-#### Python Context
+### Python Context
 
 [donfig python context configuration options](https://donfig.readthedocs.io/en/latest/configuration.html#directly-within-python)
 
 In a python context with `config.set()`. ex:
 
 ```python
 
 config.set({'runtime': 'cloud'})
 
 ```
 
-#### yaml
+### yaml
 
 [donfig yaml configuration options](https://donfig.readthedocs.io/en/latest/configuration.html#specify-configuration). Default config options can be overwritten with a top-level yaml file. Details on setup are provided in the donfig docs above.
 
 ```yaml
 run_options:
 
 runtime: 'cloud'
 ```
 
-#### Environment Variables
+### Environment Variables
 
 Config options can also be set with specifically formatted environment variables. Details can be found below.
 
 [environment variables](https://donfig.readthedocs.io/en/latest/configuration.html#environment-variables)
 
 ## Parameter Files
 
@@ -192,9 +187,7 @@
 Note: This url is specific to username, jupyter-hub name and port.
 
 `https://prod.azure.carbonplan.2i2c.cloud/user/<username>/<jupyter-hub name>/proxy/<port>/status`
 
 ex:
 
 `https://prod.azure.carbonplan.2i2c.cloud/user/norlandrhagen/bcsd/proxy/8787/status`
-
-export default ({ children }) => <Section name='Running Prefect Flows'>{children}</Section>
```

### Comparing `cmip6-downscaling-0.1.11/flows/ERA5/ERA5_resample.py` & `cmip6_downscaling-1.1.1/flows/ERA5/ERA5_resample.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/ERA5/ERA5_transfer.py` & `cmip6_downscaling-1.1.1/flows/ERA5/ERA5_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Imports -----------------------------------------------------------
 import json
 import os
-from typing import Dict, List
 
 import fsspec  # type: ignore
 import pandas as pd  # type: ignore
 import xarray as xr
 from prefect import Flow, task
 from prefect.run_configs import KubernetesRun
 from prefect.storage import Azure
@@ -102,15 +101,15 @@
         output xarray dataset
     """
     mapped_key = fsspec.get_mapper(file_loc_str, anon=True)
     ds = xr.open_zarr(mapped_key, consolidated=True)
     return ds
 
 
-def create_formatted_links() -> List:
+def create_formatted_links() -> list:
     """Create list of tuples representing all year/month/variable combinations
 
     Returns
     -------
     List
         list of potential file patterns
     """
@@ -137,15 +136,15 @@
         for month in month_list:
             for var in vars_list:
                 file_pattern = f"s3://era5-pds/zarr/{year}/{month}/data/{var}.zarr/"
                 file_pattern_list.append(file_pattern)
     return file_pattern_list
 
 
-def open_json_catalog() -> Dict:
+def open_json_catalog() -> dict:
     """Loads local CMIP6 JSON intake catalog
 
     Returns
     -------
     Dict
         dictionary as json
     """
```

### Comparing `cmip6-downscaling-0.1.11/flows/catalogs/era5-full-space.py` & `cmip6_downscaling-1.1.1/flows/catalogs/era5-full-space.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/catalogs/era5.py` & `cmip6_downscaling-1.1.1/flows/catalogs/era5.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     attrs['timescale'] = 'hourly'
     attrs['time'] = f'{attrs["year"]}-{attrs["month"]}'
     return attrs
 
 
 @task(log_stdout=True)
 def build_catalog(*, name: str, bucket: str) -> None:
-
     import ecgtools
 
     print(ecgtools.__version__)
 
     storage_options = {'account_name': 'cmip6downscaling'}
     builder = ecgtools.Builder(
         paths=['az://training/ERA5'],
```

### Comparing `cmip6-downscaling-0.1.11/flows/catalogs/final_catalog.py` & `cmip6_downscaling-1.1.1/flows/catalogs/final_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     {
         'runtime.cloud.extra_pip_packages': 'git+https://github.com/carbonplan/cmip6-downscaling.git git+https://github.com/intake/intake-esm.git git+https://github.com/ncar-xdev/ecgtools.git'
     }
 )
 
 
 def parse_store(store: str):
-
     from ecgtools.builder import INVALID_ASSET, TRACEBACK
 
     try:
         path = UPath(store)
         path_parts = path.parts
 
         (
@@ -50,21 +49,19 @@
             'variable_id': variable_id,
             'method': method,
             'downscaled_daily_data_uri': f"{store.replace('abfs://', 'https://cmip6downscaling.blob.core.windows.net/')}",
             'version': 'v1',
         }
 
     except Exception:
-
         return {INVALID_ASSET: path, TRACEBACK: traceback.format_exc()}
 
 
 @task(log_stdout=True)
 def generate_intake_esm_catalog(*, intake_esm_catalog_bucket: str):
-
     import ecgtools
 
     builder = ecgtools.Builder(
         paths=['az://version1/data'],
         depth=1,
         joblib_parallel_kwargs={'n_jobs': -1, 'verbose': 1},
         exclude_patterns=["*.json"],
@@ -98,15 +95,14 @@
     )
 
 
 @task(log_stdout=True)
 def generate_minified_web_catalog(
     *, parent_catalog: str, web_catalog: str, cdn: str = None
 ) -> None:
-
     with fsspec.open(parent_catalog) as f:
         data = json.load(f)
 
     df = pd.DataFrame.from_records(data['datasets'])
     df = (
         df.drop(
             columns=[
@@ -142,15 +138,14 @@
 
 with Flow(
     'final-catalog',
     executor=runtime.executor,
     storage=runtime.storage,
     run_config=runtime.run_config,
 ) as flow:
-
     parent_catalog = Parameter(
         'parent-catalog',
         default="az://scratch/results/pyramids/combined-cmip6-era5-pyramids-catalog-web.json",
     )
 
     web_catalog = Parameter(
         'web-catalog',
```

### Comparing `cmip6-downscaling-0.1.11/flows/catalogs/web_catalog.py` & `cmip6_downscaling-1.1.1/flows/catalogs/web_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,30 +39,30 @@
         The license."""
 
     LICENSE_MAPPING = {
         'ACCESS-CM2': '',
         'ACCESS-ESM1-5': 'CC-BY-4.0',
         'AWI-CM-1-1-MR': 'CC-BY-4.0',
         'AWI-ESM-1-1-LR': 'CC-BY-4.0',
-        'BCC-CSM2-MR': 'CC-BY-SA-4.0',
+        'BCC-CSM2-MR': 'CC-BY-4.0',
         'BCC-ESM1': 'CC-BY-SA-4.0',
         'CAMS-CSM1-0': 'CC-BY-SA-4.0',
         'CAS-ESM2-0': '',
         'CESM2': 'CC-BY-4.0',
         'CESM2-FV2': 'CC-BY-4.0',
         'CESM2-WACCM': 'CC-BY-4.0',
         'CESM2-WACCM-FV2': 'CC-BY-4.0',
         'CMCC-CM2-HR4': 'CC-BY-4.0',
         'CMCC-CM2-SR5': 'CC-BY-4.0',
         'CMCC-ESM2': 'CC-BY-4.0',
         'CNRM-CM6-1': 'CC-BY-4.0',
         'CNRM-CM6-1-HR': 'CC-BY-4.0',
         'CNRM-ESM2-1': 'CC-BY-4.0',
-        'CanESM5': 'CC-BY-SA-4.0',
-        'CanESM5-CanOE': 'CC-BY-SA-4.0',
+        'CanESM5': 'CC-BY-4.0',
+        'CanESM5-CanOE': 'CC-BY-4.0',
         'EC-Earth3': 'CC-BY-4.0',
         'EC-Earth3-AerChem': 'CC-BY-4.0',
         'EC-Earth3-CC': 'CC-BY-4.0',
         'EC-Earth3-Veg': 'CC-BY-4.0',
         'EC-Earth3-Veg-LR': 'CC-BY-4.0',
         'FGOALS-g3': 'CC-BY-SA-4.0',
         'FIO-ESM-2-0': 'CC-BY-SA-4.0',
@@ -121,21 +121,19 @@
 
         return licences[license]
     else:
         return {}
 
 
 def parse_cmip6(store: str, root_path: str) -> dict[str, str]:
-
     from ecgtools.builder import INVALID_ASSET, TRACEBACK
 
     from cmip6_downscaling.methods.common.utils import zmetadata_exists
 
     try:
-
         path = UPath(store)
         if not zmetadata_exists(path):
             raise ValueError(f'{path} not a valid zarr store')
 
         aggregation = None
         name = path.name
         (
@@ -256,15 +254,14 @@
     """
     return f"{root}/{uri.split('//')[-1]}" if uri else None
 
 
 def parse_cmip6_downscaled_pyramid(
     data, cdn: str, root_path: str, derived_product: bool = True
 ) -> list[dict]:
-
     """
     Parse metadata for given CMIP6 downscaled pyramid.
 
     Parameters
     ----------
     data : str
         Prefect run metadata.
@@ -431,15 +428,14 @@
     print(f'{len(latest_results)} of {len(results)} results are kept')
     return latest_results
 
 
 def filter_version_results(
     *, minimum_version: str, maximum_version: str, exclude_local_version: bool, results: list[str]
 ) -> list[str]:
-
     """
     Filter the results by version.
 
     Parameters
     ----------
     minimum_version : str
         The minimum version to keep.
@@ -492,15 +488,14 @@
     path,
     cdn: str,
     root_path: str,
     minimum_version: str,
     maximum_version: str = None,
     exclude_local_version: bool = True,
 ):
-
     """
     Get CMIP6 downscaled pyramids.
 
     Parameters
     ----------
     path : str
         Path to the CMIP6 downscaled pyramids.
@@ -550,15 +545,14 @@
 def create_catalog(
     *,
     catalog_path: str,
     cmip6_raw_pyramids: list[dict] = None,
     cmip6_downscaled_pyramids: list[dict] = None,
     era5_pyramids: list[dict] = None,
 ):
-
     """
     Create catalog.
 
     Parameters
     ----------
     catalog_path : str
         Path to the catalog.
@@ -599,15 +593,14 @@
     print(f'{len(datasets)} datasets are included')
     print(f'Sample datasets: {random.sample(datasets, 2)}')
 
 
 with Flow(
     'web-catalog', executor=runtime.executor, run_config=runtime.run_config, storage=runtime.storage
 ) as flow:
-
     paths = Parameter('paths', default=['az://flow-outputs/results/cmip6-pyramids-raw'])
     web_catalog_path = Parameter(
         'web-catalog-path',
         default='az://scratch/results/pyramids/combined-cmip6-era5-pyramids-catalog-web.json',
     )
     downscaled_pyramids_path = Parameter(
         'downscaled-pyramids-path',
```

### Comparing `cmip6-downscaling-0.1.11/flows/cloud_flow_test.py` & `cmip6_downscaling-1.1.1/flows/cloud_flow_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,12 +32,11 @@
 
 with Flow(
     name="test_task_multi",
     storage=runtime.storage,
     run_config=runtime.run_config,
     executor=runtime.executor,
 ) as flow:
-
     nums = range(4)
     my_task.map(nums)
 
     tasks = [make_grid((59, 87)), make_grid((60, 88)), make_grid((61, 89)), make_grid((62, 90))]
```

### Comparing `cmip6-downscaling-0.1.11/flows/cmip6_raw_pyramids.py` & `cmip6_downscaling-1.1.1/flows/cmip6_raw_pyramids.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import dask
 import xarray as xr
 from prefect import Flow, Parameter, task
 from prefect.backend.flow_run import FlowRunView
 from prefect.client import Client
 from upath import UPath
 
-from cmip6_downscaling import __version__ as version, config, runtimes
+from cmip6_downscaling import __version__ as version
+from cmip6_downscaling import config, runtimes
 from cmip6_downscaling.data.cmip import postprocess
 from cmip6_downscaling.methods.common.tasks import _pyramid_postprocess
 from cmip6_downscaling.utils import write
 
 config.set(
     {
         'runtime.cloud.extra_pip_packages': 'git+https://github.com/carbonplan/cmip6-downscaling.git@main git+https://github.com/intake/intake-esm.git'
@@ -37,15 +38,14 @@
     source_id: list[str] | str,
     variable_id: list[str] | str,
     experiment_id: list[str] | str,
     table_id: list[str] | str = 'day',
     grid_label: list[str] | str = 'gn',
     member_id: list[str] | str = 'r1i1p1f1',
 ) -> list[tuple(str, str)]:
-
     import intake
 
     cat = intake.open_esm_datastore(cat_url).search(
         member_id=member_id,
         table_id=table_id,
         grid_label=grid_label,
         variable_id=variable_id,
```

### Comparing `cmip6-downscaling-0.1.11/flows/cmip6_transfer.py` & `cmip6_downscaling-1.1.1/flows/cmip6_transfer.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/downscaled_pyramid_weights.py` & `cmip6_downscaling-1.1.1/flows/downscaled_pyramid_weights.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/era5-resample-rechunk.py` & `cmip6_downscaling-1.1.1/flows/era5-resample-rechunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     keys = sorted(cat.keys())[start:stop]
     print(keys)
     return keys
 
 
 @task(log_stdout=True)
 def resample_to_daily(*, catalog_path: str, key: str):
-
     import dask
     import intake
     import xarray as xr
 
     cat = intake.open_esm_datastore(catalog_path)
     ds = cat[key](xarray_open_kwargs={'chunks': {}}).to_dask()
```

### Comparing `cmip6-downscaling-0.1.11/flows/gcm_obs_weights.py` & `cmip6_downscaling-1.1.1/flows/gcm_obs_weights.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 
     with dask.config.set(**{'array.slicing.split_large_chunks': False}):
         # use tasmax to retrieve ERA5 grid
         ds_out = open_era5('tasmax', time_period=slice('2000', '2000')).isel(time=0)
         print(ds_out)
 
         for store in stores:
-
             target_prefix = (
                 static_dir / store['source_id'] / store['table_id'] / store['grid_label'] / method
             )
 
             target_forwards = target_prefix / f"{store['source_id']}_to_era5.zarr"
             target_reverse = target_prefix / f"era5_to_{store['source_id']}.zarr"
 
@@ -124,15 +123,14 @@
 
 with Flow(
     name='xesmf-weights',
     storage=runtime.storage,
     run_config=runtime.run_config,
     executor=runtime.executor,
 ) as flow:
-
     cat_url = Parameter(
         'cat_url', default='https://cmip6downscaling.blob.core.windows.net/cmip6/pangeo-cmip6.json'
     )
     method = Parameter('method', default='bilinear')
     stores = get_stores(cat_url)
     vals = generate_weights(stores, method=method)
     catalog(vals)
```

### Comparing `cmip6-downscaling-0.1.11/flows/gcm_pyramid_weights.py` & `cmip6_downscaling-1.1.1/flows/gcm_pyramid_weights.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/methods/bcsd/flow.py` & `cmip6_downscaling-1.1.1/flows/methods/bcsd/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 runtime = runtimes.get_runtime()
 print(runtime)
 
 
 with Flow(
     name="bcsd", storage=runtime.storage, run_config=runtime.run_config, executor=runtime.executor
 ) as flow:
-
     run_parameters = make_run_parameters(
         method=Parameter("method"),
         obs=Parameter("obs"),
         model=Parameter("model"),
         member=Parameter("member"),
         grid_label=Parameter("grid_label"),
         table_id=Parameter("table_id"),
```

### Comparing `cmip6-downscaling-0.1.11/flows/methods/deepsd/flow.py` & `cmip6_downscaling-1.1.1/flows/methods/deepsd/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 runtime = runtimes.get_runtime()
 print(runtime)
 
 with Flow(
     name="deepsd", storage=runtime.storage, run_config=runtime.run_config, executor=runtime.executor
 ) as flow:
-
     run_parameters = make_run_parameters(
         method=Parameter("method"),
         obs=Parameter("obs"),
         model=Parameter("model"),
         member=Parameter("member"),
         grid_label=Parameter("grid_label"),
         table_id=Parameter("table_id"),
@@ -132,15 +131,14 @@
     p['bias_corrected_annual_summary_path'] = update_var_attrs(
         target_path=p['bias_corrected_annual_summary_path'],
         source_path=p['raw_annual_summary_path'],
         run_parameters=run_parameters,
     )
 
     if config.get('run_options.generate_pyramids'):
-
         # since pyramids require full space we now rechunk everything into full
         # space before passing into pyramid step. we probably want to add a cleanup
         # to this step in particular since otherwise we will have an exact
         # duplicate of the daily, monthly, and annual datasets
         # p['full_space_model_output_path'] = rechunk(
         #     p['shifted_model_output_path'], pattern='full_space'
         # )
```

### Comparing `cmip6-downscaling-0.1.11/flows/methods/gard/flow.py` & `cmip6_downscaling-1.1.1/flows/methods/gard/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 runtime = runtimes.get_runtime()
 print(runtime)
 
 
 with Flow(
     name="gard", storage=runtime.storage, run_config=runtime.run_config, executor=runtime.executor
 ) as flow:
-
     run_parameters = make_run_parameters(
         method=Parameter("method"),
         obs=Parameter("obs"),
         model=Parameter("model"),
         member=Parameter("member"),
         grid_label=Parameter("grid_label"),
         table_id=Parameter("table_id"),
@@ -122,15 +121,14 @@
     p['monthly_summary_path'] = time_summary(p['model_output_path'], freq='1MS')
     p['annual_summary_path'] = time_summary(p['model_output_path'], freq='1AS')
 
     # analysis notebook (shared with BCSD)
     # analysis_location = run_analyses(model_output_path, run_parameters)
 
     if config.get('run_options.generate_pyramids'):
-
         # since pyramids require full space we now rechunk everything into full
         # space before passing into pyramid step. we probably want to add a cleanup
         # to this step in particular since otherwise we will have an exact
         # duplicate of the daily, monthly, and annual datasets
         p['full_space_model_output_path'] = rechunk(p['model_output_path'], pattern='full_space')
 
         # make temporal summaries
```

### Comparing `cmip6-downscaling-0.1.11/flows/methods/gard/multivariate_test.json` & `cmip6_downscaling-1.1.1/flows/methods/gard/multivariate_test.json`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/flows/methods/maca/flow.py` & `cmip6_downscaling-1.1.1/flows/methods/maca/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
             gcm_path=p['bias_corrected_gcm_region_paths'],
             coarse_obs_path=p['coarse_obs_region_paths'],
             fine_obs_path=p['obs_region_paths'],
             run_parameters=unmapped(run_parameters),
         )
 
         if config.get('run_options.combine_regions'):
-
             p['combined_analogs_full_time_path'] = combine_regions(
                 regions=p['region_numbers'],
                 region_paths=p['constructed_analogs_region_paths'],
                 template_path=p['fine_epoch_trend_full_space_path'],
             )
 
             p['fine_epoch_trend_full_time_path'] = rechunk(
@@ -180,15 +179,14 @@
                 p['final_bias_corrected_full_time_path'], freq='1AS'
             )
 
             # analysis notebook
             # analysis_location = run_analyses(p['final_bias_corrected_full_time_path'], run_parameters)
 
             if config.get('run_options.generate_pyramids'):
-
                 # make temporal summaries
                 p['monthly_summary_full_space_path'] = rechunk(
                     p['monthly_summary_path'], pattern='full_space'
                 )
                 p['annual_summary_full_space_path'] = rechunk(
                     p['annual_summary_path'], pattern='full_space'
                 )
```

### Comparing `cmip6-downscaling-0.1.11/flows/run_subsets_cloud.py` & `cmip6_downscaling-1.1.1/flows/run_subsets_cloud.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/accessing_data_example.ipynb` & `cmip6_downscaling-1.1.1/notebooks/accessing_data_example.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/catalog_audit.ipynb` & `cmip6_downscaling-1.1.1/notebooks/catalog_audit.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/check_model_completeness.ipynb` & `cmip6_downscaling-1.1.1/notebooks/check_model_completeness.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999502732807528%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(2, '    for gcm, ensemble_member in gcms:\\n')], delete: "*

 * *            "[2]}}, 5: {'source': {insert: [(1, '    for gcm, ensemble_member in gcms:\\n')], "*

 * *            'delete: [1]}}}'}*

```diff
@@ -66,15 +66,15 @@
             "execution_count": null,
             "id": "noble-friday",
             "metadata": {},
             "outputs": [],
             "source": [
                 "models = []\n",
                 "for scenario in [\"historical\", \"ssp245\", \"ssp370\", \"ssp585\"]:\n",
-                "    for (gcm, ensemble_member) in gcms:\n",
+                "    for gcm, ensemble_member in gcms:\n",
                 "        models.append(\"{}-{}\".format(gcm, scenario))\n",
                 "path = get_store(\n",
                 "    \"carbonplan-downscaling\",\n",
                 "    zarr_template.format(gcms[0][0], \"historical\", gcms[0][1]),\n",
                 "    account_key=account_key,\n",
                 ")\n",
                 "ds = xr.open_zarr(path)\n",
@@ -85,15 +85,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "floral-devil",
             "metadata": {},
             "outputs": [],
             "source": [
                 "for scenario in [\"historical\", \"ssp245\", \"ssp370\", \"ssp585\"]:\n",
-                "    for (gcm, ensemble_member) in gcms:\n",
+                "    for gcm, ensemble_member in gcms:\n",
                 "        path = get_store(\n",
                 "            \"carbonplan-downscaling\",\n",
                 "            zarr_template.format(gcm, scenario, ensemble_member),\n",
                 "            account_key=account_key,\n",
                 "        )\n",
                 "        ds = xr.open_zarr(path)\n",
                 "        for var in ds.data_vars:\n",
```

### Comparing `cmip6-downscaling-0.1.11/notebooks/compare_bcsd.ipynb` & `cmip6_downscaling-1.1.1/notebooks/compare_bcsd.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/deepsd_data_prep.ipynb` & `cmip6_downscaling-1.1.1/notebooks/deepsd_data_prep.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999905901836796%*

 * *Differences: {"'cells'": "{25: {'source': {delete: [5]}}}"}*

```diff
@@ -845,15 +845,14 @@
             "outputs": [],
             "source": [
                 "import random\n",
                 "\n",
                 "# for plotting with lat/lon potentially use the following\n",
                 "# batch.isel(input_batch=1).tf..plot.pcolormesh(strings)\n",
                 "for _ in range(10):\n",
-                "\n",
                 "    i = random.randint(0, len(batch.input_batch))\n",
                 "    patch = batch.isel(input_batch=i)\n",
                 "    print(patch.lat.min().values, patch.lat.max().values)\n",
                 "    print(patch.lon.min().values, patch.lon.max().values)\n",
                 "    test_vals = patch.tf.values\n",
                 "\n",
                 "    plt.figure(figsize=(17, 4))\n",
```

### Comparing `cmip6-downscaling-0.1.11/notebooks/deepsd_inference.ipynb` & `cmip6_downscaling-1.1.1/notebooks/deepsd_inference.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/deepsd_model_train.ipynb` & `cmip6_downscaling-1.1.1/notebooks/deepsd_model_train.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999879436728395%*

 * *Differences: {"'cells'": "{8: {'source': {delete: [17]}}}"}*

```diff
@@ -207,15 +207,14 @@
                 "    \"lon\": tf.io.FixedLenFeature([], tf.string),\n",
                 "    # TODO: this needs to be string\n",
                 "    \"time\": tf.io.FixedLenFeature([], tf.string),\n",
                 "}\n",
                 "\n",
                 "\n",
                 "def read_and_decode(filename_queue, input_size, input_depth, output_depth):\n",
-                "\n",
                 "    reader = tf.compat.v1.TFRecordReader()\n",
                 "    _, serialized_example = reader.read(filename_queue)\n",
                 "    features = tf.compat.v1.parse_single_example(serialized_example, features=feature)\n",
                 "\n",
                 "    label = tf.io.parse_tensor(features[\"label\"], out_type=tf.float32)\n",
                 "    img_in = tf.io.parse_tensor(features[\"img_in\"], out_type=tf.float32)\n",
                 "    lat = tf.io.parse_tensor(features[\"lat\"], out_type=tf.float32)\n",
```

### Comparing `cmip6-downscaling-0.1.11/notebooks/figures.ipynb` & `cmip6_downscaling-1.1.1/notebooks/figures.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/gard_flow_runs.ipynb` & `cmip6_downscaling-1.1.1/notebooks/gard_flow_runs.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/gard_model_options.ipynb` & `cmip6_downscaling-1.1.1/notebooks/gard_model_options.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/prefect_cloud_runner.ipynb` & `cmip6_downscaling-1.1.1/notebooks/prefect_cloud_runner.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999841088227815%*

 * *Differences: {"'cells'": "{2: {'source': {delete: [29, 6]}}}"}*

```diff
@@ -69,15 +69,14 @@
             "source": [
                 "def retrieve_test_parms():\n",
                 "    \"\"\"retrieve list of all .json param files in method subdir\"\"\"\n",
                 "    return glob.glob(f'{config_file_dir}*.json')\n",
                 "\n",
                 "\n",
                 "def create_run_params_from_json(parameter_fpath: str) -> RunParameters:\n",
-                "\n",
                 "    df = pd.read_json(parameter_fpath)\n",
                 "    run_parameters = RunParameters(\n",
                 "        method=df.method.iloc[0],\n",
                 "        obs=df.obs.iloc[0],\n",
                 "        model=df.model.iloc[0],\n",
                 "        member=df.member.iloc[0],\n",
                 "        grid_label=df.grid_label.iloc[0],\n",
@@ -92,15 +91,14 @@
                 "        predict_dates=[df.predict_period.iloc[0], df.predict_period.iloc[1]],\n",
                 "    )\n",
                 "\n",
                 "    return run_parameters\n",
                 "\n",
                 "\n",
                 "def run_flow(flow_id: str, param_file_path: str) -> list[str]:\n",
-                "\n",
                 "    json_path = pathlib.Path(param_file_path).read_text()\n",
                 "    flow_hash = str_to_hash(json_path)\n",
                 "    param_dict = json.loads(json_path)\n",
                 "    param_dict[\"predict_period\"] = param_dict.pop(\"predict_dates\")\n",
                 "    param_dict[\"train_period\"] = param_dict.pop(\"train_dates\")\n",
                 "\n",
                 "    client = Client()\n",
```

### Comparing `cmip6-downscaling-0.1.11/notebooks/run_analyses.ipynb` & `cmip6_downscaling-1.1.1/notebooks/run_analyses.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/scrf.ipynb` & `cmip6_downscaling-1.1.1/notebooks/scrf.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/terraclimate_evaluation.ipynb` & `cmip6_downscaling-1.1.1/notebooks/terraclimate_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/terraclimate_model.ipynb` & `cmip6_downscaling-1.1.1/notebooks/terraclimate_model.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998809523809524%*

 * *Differences: {"'cells'": "{4: {'source': {delete: [3]}}, 6: {'source': {delete: [1]}}}"}*

```diff
@@ -113,15 +113,14 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# run our version of the terraclimate hydrology model for all points\n",
                 "v2 = {}\n",
                 "for k, df_point in data.items():\n",
-                "\n",
                 "    df = df_point.copy(deep=True)\n",
                 "\n",
                 "    awc = df[\"awc\"][0]\n",
                 "    print(k, awc)\n",
                 "    if awc < 50:\n",
                 "        print(k, \"< 50mm\")\n",
                 "        awc = 50\n",
@@ -143,15 +142,14 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def plot_points(v1, v2, var=\"pdsi\", tslice=slice(200, 300)):\n",
-                "\n",
                 "    fig, axes = plt.subplots(nrows=2, ncols=len(v2), figsize=(24, 4), squeeze=False)\n",
                 "\n",
                 "    for i, k in enumerate(v2):\n",
                 "        v1[k][var][tslice].plot(label=\"v1\", ax=axes[0, i])\n",
                 "        v2[k][var][tslice].plot(label=\"v2\", ax=axes[0, i])\n",
                 "        (v2[k][var][tslice] - v1[k][var][tslice]).plot(label=\"v2 - v1\", c=\"k\", ax=axes[1, i])\n",
                 "        axes[0, i].set_title(k.title())\n",
```

### Comparing `cmip6-downscaling-0.1.11/notebooks/workflow.ipynb` & `cmip6_downscaling-1.1.1/notebooks/workflow.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/worldcities.csv` & `cmip6_downscaling-1.1.1/notebooks/worldcities.csv`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/notebooks/xpersist_overwrite_example.ipynb` & `cmip6_downscaling-1.1.1/notebooks/xpersist_overwrite_example.ipynb`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/tests/analysis/test_metrics.py` & `cmip6_downscaling-1.1.1/tests/analysis/test_metrics.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/tests/conftest.py` & `cmip6_downscaling-1.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/tests/methods/common/test_tasks.py` & `cmip6_downscaling-1.1.1/tests/methods/common/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 
 
 def check_global_attrs(ds):
     for key in ['history', 'hostname', 'institution', 'source', 'title', 'username', 'version']:
         assert key in ds.attrs
 
 
+@pytest.mark.xfail
 def test_get_obs(run_parameters):
     obs_path = get_obs.run(run_parameters)
     print(obs_path)
     ds = xr.open_zarr(obs_path)
     print(ds)
     check_global_attrs(ds)
     schema = DatasetSchema(
@@ -131,15 +132,14 @@
             )
         }
     )
     schema.validate(ds)
 
 
 def test_regrid(tmp_path):
-
     pytest.importorskip('xesmf')
 
     ds = xr.tutorial.open_dataset('air_temperature').chunk({'time': 10, 'lat': -1, 'lon': -1})
     source_path = UPath(tmp_path) / UPath('regrid_source.zarr')
     ds.to_zarr(source_path)
 
     target_ds = ds.isel(time=0).coarsen(lat=4, lon=4, boundary='trim').mean()
```

### Comparing `cmip6-downscaling-0.1.11/tests/test_config.py` & `cmip6_downscaling-1.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cmip6-downscaling-0.1.11/tests/test_utils.py` & `cmip6_downscaling-1.1.1/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ds_lon_corrected = lon_to_180(ds)
     assert ds_lon_corrected.lon.min() < -1
     assert ds_lon_corrected.lon.max() <= 180
     assert (ds_lon_corrected.lon.diff(dim='lon') > 0).all()
 
 
 def test_to_standard_calendar(da_noleap):
-
     da_std = to_standard_calendar(da_noleap)
     assert da_noleap.sizes['time'] == 365
     assert da_std.sizes['time'] == 366
     assert not da_std.isnull().any().compute().item()
 
 
 def test_str_to_hash():
```

