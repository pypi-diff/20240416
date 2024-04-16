# Comparing `tmp/regional_mom6-0.2.1.tar.gz` & `tmp/regional_mom6-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regional_mom6-0.2.1.tar", last modified: Fri Nov 17 03:50:30 2023, max compression
+gzip compressed data, was "regional_mom6-0.5.0.tar", last modified: Tue Apr 16 09:17:49 2024, max compression
```

## Comparing `regional_mom6-0.2.1.tar` & `regional_mom6-0.5.0.tar`

### file list

```diff
@@ -1,64 +1,58 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.692483 regional_mom6-0.2.1/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.680483 regional_mom6-0.2.1/.github/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.684483 regional_mom6-0.2.1/.github/workflows/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1507 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/.github/workflows/testing.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      116 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/.gitignore
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/.readthedocs.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1063 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      473 2023-11-17 03:50:30.692483 regional_mom6-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5011 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/codecov.yml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.684483 regional_mom6-0.2.1/demos/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   269104 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/demos/model-forced.ipynb
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   147791 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/demos/reanalysis-forced.ipynb
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.684483 regional_mom6-0.2.1/docs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      634 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/Makefile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      124 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/api.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      896 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/conf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1810 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/contributing.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/demos.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      372 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/index.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/installation.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       47 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/docs/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/environment-ci.yml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      642 2023-11-17 03:14:01.000000 regional_mom6-0.2.1/pyproject.toml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.688483 regional_mom6-0.2.1/regional_mom6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      129 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      411 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6/_version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.680483 regional_mom6-0.2.1/regional_mom6/default_rundir/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.688483 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8407 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/MOM_input
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      436 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/MOM_override
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      249 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/SIS_input
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      537 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/config.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1289 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/data_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/diag_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     6512 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/env.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       64 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/field_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1371 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/input.nml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      364 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/job.yaml
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.692483 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     8407 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/MOM_input
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      436 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/MOM_override
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      249 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/README.md
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1395 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/SIS_input
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      537 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/config.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1340 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/data_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/diag_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     6512 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/env.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)       64 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/field_table
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1371 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/input.nml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      364 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/job.yaml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    60401 2023-11-17 02:50:05.000000 regional_mom6-0.2.1/regional_mom6/regional_mom6.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       77 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/regional_mom6/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.688483 regional_mom6-0.2.1/regional_mom6.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      473 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1823 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       94 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-11-17 03:50:30.000000 regional_mom6-0.2.1/regional_mom6.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-11-17 03:50:30.692483 regional_mom6-0.2.1/setup.cfg
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-11-17 03:50:30.692483 regional_mom6-0.2.1/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7860 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/tests/test_expt_class.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2965 2023-11-15 03:42:59.000000 regional_mom6-0.2.1/tests/test_grid_generation.py
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/.github/
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/.github/workflows/
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     2024 2024-04-16 09:17:39.000000 regional_mom6-0.5.0/.github/workflows/testing.yml
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      142 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/.gitignore
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      567 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/.readthedocs.yaml
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1063 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/LICENSE
+-rw-r--r--   0 angusgibson  (1001) angusgibson  (1002)      504 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/PKG-INFO
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     7170 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/README.md
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      306 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/codecov.yml
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/demos/
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)   152481 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/access_om2-forced.ipynb
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.952148 regional_mom6-0.5.0/demos/premade_run_directories/
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/common_files/
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)    44918 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_input
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     2039 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_layout
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       67 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/MOM_override
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1321 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/SIS_input
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      426 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/config.yaml
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      912 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/data_table
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     3255 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/diag_table
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)       64 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/field_table
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1398 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/common_files/input.nml
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1264 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/data_table
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1436 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/input.nml
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)      455 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/config.yaml
+-rwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)     1340 2024-02-19 22:45:18.000000 regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/data_table
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      427 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/demos/premade_run_directories/readme_premade_rundirs.md
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    14957 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/demos/reanalysis-forced.ipynb
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/docs/
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      634 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/docs/Makefile
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      312 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/api.rst
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      896 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/docs/conf.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1997 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/contributing.md
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      164 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/docs/demos.rst
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      441 2024-02-21 06:00:04.000000 regional_mom6-0.5.0/docs/index.rst
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1899 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/docs/installation.md
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       47 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/docs/requirements.txt
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       74 2024-02-23 03:07:30.000000 regional_mom6-0.5.0/environment-ci.yml
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      870 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/pyproject.toml
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/regional_mom6/
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      129 2023-09-06 00:16:41.000000 regional_mom6-0.5.0/regional_mom6/__init__.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      411 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6/_version.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    81967 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/regional_mom6/regional_mom6.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     6373 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/regional_mom6/utils.py
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/regional_mom6.egg-info/
+-rw-r--r--   0 angusgibson  (1001) angusgibson  (1002)      504 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/PKG-INFO
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1458 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/SOURCES.txt
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)        1 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/dependency_links.txt
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)      110 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/requires.txt
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       14 2024-04-16 09:17:49.000000 regional_mom6-0.5.0/regional_mom6.egg-info/top_level.txt
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)       38 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/setup.cfg
+drwxrwxr-x   0 angusgibson  (1001) angusgibson  (1002)        0 2024-04-16 09:17:49.956148 regional_mom6-0.5.0/tests/
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)    12071 2024-04-16 09:16:37.000000 regional_mom6-0.5.0/tests/test_expt_class.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     4674 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/tests/test_grid_generation.py
+-rw-rw-r--   0 angusgibson  (1001) angusgibson  (1002)     1212 2024-04-08 22:54:20.000000 regional_mom6-0.5.0/tests/test_utils.py
```

### Comparing `regional_mom6-0.2.1/.github/workflows/testing.yml` & `regional_mom6-0.5.0/.github/workflows/testing.yml`

 * *Files 9% similar despite different names*

```diff
@@ -13,43 +13,52 @@
       - uses: psf/black@stable
         with:
           src: "./regional_mom6 ./tests"
 
   testing:
     needs: formatting
     runs-on: ubuntu-latest
+    container: ghcr.io/cosima/regional-test-env:updated
     defaults:
       run:
         shell: bash -el {0}
     strategy:
       matrix:
         python-version: ["3.9", "3.10"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: conda-incubator/setup-miniconda@v2
         with:
+          miniconda-version: "latest"
           auto-update-conda: true
           auto-activate-base: false
           environment-file: environment-ci.yml
           python-version: ${{ matrix.python-version }}
       - name: Install from source
         run: |
           python -m pip install .
       - name: Install pytest
         run: |
-          python -m pip install pytest pytest-cov
+          python -m pip install pytest pytest-cov nbval
       - name: Test with pytest
         run: |
           if [[ "${{ matrix.python-version }}" == "3.10" ]]; then
-            python -m pytest --cov=regional_mom6 --cov-report=xml tests/
+            python -m pytest -v --doctest-modules --cov=regional_mom6 --cov-report=xml tests/ regional_mom6/
           else
-            python -m pytest tests/
+            python -m pytest -v --doctest-modules tests/ regional_mom6/
           fi
+      - name: Test the example notebook
+        run: |
+          ln -s /data demos/PATH_TO_GLORYS_DATA
+          ln -s /data demos/PATH_TO_GEBCO_FILE
+          ln -s /build/FRE-NCtools/tools demos/PATH_TO_FRE_TOOLS
+          python -m pytest --nbval demos/reanalysis-forced.ipynb --nbval-current-env --cov=regional_mom6 --cov-report=xml tests/
+
       - name: Upload coverage to Codecov
         uses: codecov/codecov-action@v3
         if: ${{ matrix.python-version == '3.10' }}
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           directory: ./coverage/reports/
           env_vars: OS,PYTHON
```

### Comparing `regional_mom6-0.2.1/.readthedocs.yaml` & `regional_mom6-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.2.1/LICENSE` & `regional_mom6-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.2.1/README.md` & `regional_mom6-0.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,112 @@
 # regional_mom6
 
 *Python package for automatic generation of regional configurations for the [Modular Ocean Model 6](https://github.com/mom-ocean/MOM6).*
 
-[![Repo status](https://www.repostatus.org/badges/latest/active.svg?style=flat-square)](https://www.repostatus.org/#active) [![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://mit-license.org) [![codecov](https://codecov.io/gh/COSIMA/regional-mom6/branch/main/graph/badge.svg?token=7OEZ1UZRY4)](https://codecov.io/gh/COSIMA/regional-mom6) [![Documentation Status](https://readthedocs.org/projects/regional-mom6/badge/?version=latest)](https://regional-mom6.readthedocs.io/en/latest/?badge=latest) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Repo status](https://www.repostatus.org/badges/latest/active.svg?style=flat-square)](https://www.repostatus.org/#active)
+[![conda forge](https://img.shields.io/conda/vn/conda-forge/regional-mom6.svg)](https://anaconda.org/conda-forge/regional-mom6)
+[![pypi](https://badge.fury.io/py/regional-mom6.svg)](https://badge.fury.io/py/regional-mom6)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](https://mit-license.org)
+[![codecov](https://codecov.io/gh/COSIMA/regional-mom6/branch/main/graph/badge.svg?token=7OEZ1UZRY4)](https://codecov.io/gh/COSIMA/regional-mom6)
+[![Documentation Status](https://readthedocs.org/projects/regional-mom6/badge/?version=latest)](https://regional-mom6.readthedocs.io/en/latest/?badge=latest)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Users just need to provide some information about where, when, and how big their domain is and also where raw input forcing files are. The package sorts out all the boring details and creates a set of MOM6-friendly input files along with setup directories ready to go! 
 
-The idea behind this package is that it should the user sidestep some of the tricky issues with getting the model to run in the first place. This removes some of the steep learning curve for people new to working with the model. Note that the resultant model configuration might still need some tweaking (e.g., fiddling with timestep to avoid CFL-related numerical stability issues or fiddling with bathymetry to deal with very narrow fjords or channels that may exist).
+The idea behind this package is that it should let the user sidestep some of the tricky issues with getting the model to run in the first place. This removes some of the steep learning curve for people new to working with MOM6. Note that the resultant model configuration might still need some tweaking (e.g., fiddling with timestep to avoid CFL-related numerical stability issues or fiddling with bathymetry to deal with very narrow fjords or channels that may exist).
 
 Limitations: Currently the package supports only one horizontal grid type (that is equally spaced in longitude); there are plans to add more grid options. We have designed the package in a way that it is modular so, for example, one needs to implement just another method for a different type of grid and the rest should be good to go.
 
 If you find this package useful and have any suggestions please feel free to open an [issue](https://github.com/COSIMA/regional-mom6/issues) or a [discussion](https://github.com/COSIMA/regional-mom6/discussions). We'd love to have [new contributors](https://regional-mom6.readthedocs.io/en/latest/contributing.html) and we are very keen to help you out along the way!
 
-## What you need to get started
-1. A cool idea for a new regional MOM6 domain
-2. A working MOM6 executable on a machine of your choice. 
-3. A bathymetry file that at least covers your domain
-4. 3D ocean forcing files *of any resolution* on your choice of A, B or C Arakawa grid
-5. Surface forcing files (eg ERA or JRA reanalysis)
-6. [GFDL's FRE tools](https://github.com/NOAA-GFDL/FRE-NCtools) must be downloaded and compiled on the machine you are using.
+## What you need to get started:
+1. a cool idea for a new regional MOM6 domain,
+2. a working MOM6 executable on a machine of your choice, 
+3. a bathymetry file that at least covers your domain,
+4. 3D ocean forcing files *of any resolution* on your choice of A, B, or C Arakawa grid,
+5. surface forcing files (e.g., from ERA or JRA reanalysis), and
+6. [GFDL's FRE tools](https://github.com/NOAA-GFDL/FRE-NCtools) be downloaded and compiled on the machine you are using.
 
-Check out the the [documentation](https://regional-mom6.readthedocs.io/en/latest/) and browse through the [demos](https://regional-mom6.readthedocs.io/en/latest/demos.html).
+Check out the [documentation](https://regional-mom6.readthedocs.io/en/latest/) and browse through the [demos](https://regional-mom6.readthedocs.io/en/latest/demos.html).
 
 ## Installation
 
-At the moment you can install the package via `pip` from
-GitHub. Before this, the binary `esmpy` dependency is required. This
-is easiest to install using Conda. To do so, first create a custom
-Conda environment, or activate an existing environment into which you
-want to install `esmpy` and `regional_mom6`. Then install `emspy`:
+#### Easy, clean, one liner
+
+The easiest way is to install `regional-mom6` via [`conda`](https://anaconda.org/conda-forge/regional-mom6).
+We encourage creating a new or using an existing conda environment and then simply
+
+```bash
+conda install conda-forge::regional-mom6
+```
+
+That's it -- now enjoy!
+
+#### "*But I want `pip`, can't I install with `pip`*?"
+
+We can install via `pip` but it's a bit more cumbersome.
+Again, we encourage creating a new or using an existing conda environment.
+
+A prerequisite is the binary `esmpy` dependency, which provides regridding capabilities.
+The easiest way to install `esmpy` is via conda:
 
 ```bash
 conda install -c conda-forge esmpy
 ```
 
-Alternatively, it's possible to follow the [Installing ESMPy from
-Source](https://earthsystemmodeling.org/esmpy_doc/release/latest/html/install.html#installing-esmpy-from-source)
-instructions to do this in a Conda-free way. With `esmpy` available, you can then install
-`regional_mom6` via pip. If your environment doesn't yet have pip, then `conda install pip` should do the job.
+Alternatively, to install `esmpy` in a Conda-free way, follow the instructions for [installing ESMPy from
+source](https://earthsystemmodeling.org/esmpy_doc/release/latest/html/install.html#installing-esmpy-from-source).
+With `esmpy` available, we can then install `regional_mom6` via pip. (If we don't have have pip, then
+`conda install pip` should do the job.)
+
+With `esmpy` installed we can now install `regional-mom6` via [`pip`](https://pypi.org/project/regional-mom6/):
 
 ```bash
-pip install git+https://github.com/COSIMA/regional-mom6.git
+pip install regional-mom6
 ```
 
-This installs the latest version of `regional_mom6` plus any required dependencies.
-`esmpy` won't be installed as a dependency and that's why need to install it separately.
+The above installs the version of `regional-mom6` (plus any required dependencies) that corresponds to the latest tagged release of the package.
 
-Alternatively, you can also install a particular tag or git commit using, e.g.,
+#### "*I'd like to be on the cutting edge of the development*?"
+
+Alternatively, we can install directly `regional-mom6` directly via GitHub using `pip`.
+First install `esmpy` as described above and then:
 
 ```bash
-pip install git+https://github.com/COSIMA/regional-mom6.git@v0.X.X
+pip install git+https://github.com/COSIMA/regional-mom6.git
 ```
 
-or
+to get the version that corresponds to the latest commit in GitHub.
+Or, install the version that corresponds to a particular git commit using
 
 ```bash
 pip install git+https://github.com/COSIMA/regional-mom6.git@061b0ef80c7cbc04de0566df329c4ea472002f7e
 ```
 
+## MOM6 Configuration and Version Requirements
+
+The package and demos assume a coupled SIS2-MOM6 configuration.
+The examples could work for an ocean-only MOM6 run but this has not been tested. 
+
+The current release of this package assumes the latest source code of all components needed to run MOM6 as of
+January 2024. A forked version of the [`setup-mom6-nci`](https://github.com/ashjbarnes/setup-mom6-nci) repository
+contains scripts for compiling MOM6 and, furthermore, its [`src`](https://github.com/ashjbarnes/setup-mom6-nci/tree/setup-mom6/src)
+directory lists the particular commits that were used to compile MOM6 and its submodules for this package.
+
+Note that the commits used for MOM6 submodules (e.g., Flexible Modelling System (FMS), coupler, SIS2) are _not_
+necessarily those used by the GFDL's [`MOM6_examples`](https://github.com/NOAA-GFDL/MOM6-examples) repository.
 
 ## Getting started
 
-The [example notebooks](https://regional-mom6.readthedocs.io/en/latest/demos.html) walk you through how to use the package using two different sets of input datasets.
-Make sure that you can get at least one of these working on your setup with your MOM6 executable, and then try to modify them to apply to your domain with your bathymethry, forcing, and boundary conditions.
 
-The `xesmf` the package attempts to regrid in parallel, and if it's not able to do so, it throws a warning and run in serial.
-You also get a print out of the relevant `mpirun` command which you could use as a backup.
-Depending on your setup of your machine, you may need to write scripts that implement the package to access more computational resources than might be available, e.g., on the HPC machine of you are working on.
+The [example notebooks](https://regional-mom6.readthedocs.io/en/latest/demos.html) walk you through how to use
+the package using two different sets of input datasets.
+Please ensure that you can get at least one of these working on your setup with your MOM6 executable before trying modify the example to suit your domain with your bathymethry, forcing, and boundary conditions.
+
+You can download the notebooks [from Github](https://github.com/COSIMA/regional-mom6/tree/ncc/installation/demos) or by clicking on the download <img width="22" alt="download" src="https://github.com/COSIMA/regional-mom6/assets/7112768/2c1ae149-c6a8-4395-ab09-2f77588008d9"> button, e.g., at the top-right of the [regional tasmania forced by ERA5 example](https://regional-mom6.readthedocs.io/en/latest/demo_notebooks/reanalysis-forced.html).
+
+**Note**
+
+The `xesmf` the package attempts to regrid in parallel, and if it's not able to do so, it throws a warning and
+runs in serial. You also get a print out of the relevant `mpirun` command which you could use as a backup.
+Depending on your setup of your machine, you may need to write scripts that implement the package to access more
+computational resources than might be available, e.g., on the HPC machine of you are working on.
```

### Comparing `regional_mom6-0.2.1/demos/reanalysis-forced.ipynb` & `regional_mom6-0.5.0/demos/access_om2-forced.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9522073328571845%*

 * *Differences: {"'cells'": "{3: {'source': ['Start a dask client.']}, 4: {'metadata': {replace: "*

 * *            "OrderedDict([('tags', [])])}, 'outputs': {0: {'data': {'text/html': {insert: [(4, "*

 * *            '\'        <p style="color: #9D9D9D; margin-bottom: '*

 * *            '0px;">Client-c70f819d-e4f5-11ee-8dfd-0000080efe80</p>\\n\'), (17, '*

 * *            '\'                    <strong>Dashboard: </strong> <a href="/proxy/8787/status" '*

 * *            'target="_blank">/proxy/8787/status</a>\\n\'), (26, \'            <button '*

 * *   […]*

```diff
@@ -1,79 +1,128 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# Forcing with a reanalysis dataset"
+                "# Regional Tasmania forced by JRA-55 reanalysis and ACCESS-OM2 model output\n",
+                "\n",
+                "### Note: This example requires access to [NCI's Gadi HPC system](https://nci.org.au/our-systems/hpc-systems)\n",
+                "\n",
+                "**Ensure you have access to the relevant NCI projects to access the data listed below**\n",
+                "\n",
+                "## What does this notebook do?\n",
+                "This notebook is designed to set you up with a working MOM6 regional configuration. First, try and get it running with our default Tasmania case, then you can clone the notebook and modify for your region of interest. \n",
+                "\n",
+                "Input Type | Source | Location on NCI\n",
+                "---|---|---\n",
+                "Surface | [JRA55 surface forcing](https://climatedataguide.ucar.edu/climate-data/jra-55) | `/g/data/ik11`\n",
+                "Ocean | [ACCESS-OM2-01](https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/description) |  `/g/data/ik11`  \n",
+                "Bathymetry | [GEBCO](https://www.gebco.net/data_and_products/gridded_bathymetry_data/) | `/g/data/ik11`\n",
+                "\n",
+                "Additionally, you'll need access to `/g/data/x77/` if you want to use the same executable using the latest FMS build (a good idea for troubleshooting)."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "To use your own version of regional_mom6 package, clone the entire github repository\n",
+                "on your machine and set the regional-mom6 path using the `os` library, like shown below:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [],
+            "source": [
+                "import os\n",
+                "os.chdir(\"/g/data/v45/nc3020/dhruvs-regional-mom6/\")\n",
+                "\n",
+                "import regional_mom6 as rmom6\n",
+                "import xarray as xr\n",
+                "from pathlib import Path\n",
+                "from dask.distributed import Client"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "Start a dask client."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "    <div style=\"width: 24px; height: 24px; background-color: #e1e1e1; border: 3px solid #9D9D9D; border-radius: 5px; position: absolute;\"> </div>\n",
                             "    <div style=\"margin-left: 48px;\">\n",
                             "        <h3 style=\"margin-bottom: 0px;\">Client</h3>\n",
-                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Client-42ab73fe-5753-11ee-8b2f-0000076bfe80</p>\n",
+                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Client-c70f819d-e4f5-11ee-8dfd-0000080efe80</p>\n",
                             "        <table style=\"width: 100%; text-align: left;\">\n",
                             "\n",
                             "        <tr>\n",
                             "        \n",
                             "            <td style=\"text-align: left;\"><strong>Connection method:</strong> Cluster object</td>\n",
                             "            <td style=\"text-align: left;\"><strong>Cluster type:</strong> distributed.LocalCluster</td>\n",
                             "        \n",
                             "        </tr>\n",
                             "\n",
                             "        \n",
                             "            <tr>\n",
                             "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Dashboard: </strong> <a href=\"/proxy/44739/status\" target=\"_blank\">/proxy/44739/status</a>\n",
+                            "                    <strong>Dashboard: </strong> <a href=\"/proxy/8787/status\" target=\"_blank\">/proxy/8787/status</a>\n",
                             "                </td>\n",
                             "                <td style=\"text-align: left;\"></td>\n",
                             "            </tr>\n",
                             "        \n",
                             "\n",
                             "        </table>\n",
                             "\n",
                             "        \n",
-                            "            <button style=\"margin-bottom: 12px;\" data-commandlinker-command=\"dask:populate-and-launch-layout\" data-commandlinker-args='{\"url\": \"/proxy/44739/status\" }'>\n",
+                            "            <button style=\"margin-bottom: 12px;\" data-commandlinker-command=\"dask:populate-and-launch-layout\" data-commandlinker-args='{\"url\": \"/proxy/8787/status\" }'>\n",
                             "                Launch dashboard in JupyterLab\n",
                             "            </button>\n",
                             "        \n",
                             "\n",
                             "        \n",
                             "            <details>\n",
                             "            <summary style=\"margin-bottom: 20px;\"><h3 style=\"display: inline;\">Cluster Info</h3></summary>\n",
                             "            <div class=\"jp-RenderedHTMLCommon jp-RenderedHTML jp-mod-trusted jp-OutputArea-output\">\n",
                             "    <div style=\"width: 24px; height: 24px; background-color: #e1e1e1; border: 3px solid #9D9D9D; border-radius: 5px; position: absolute;\">\n",
                             "    </div>\n",
                             "    <div style=\"margin-left: 48px;\">\n",
                             "        <h3 style=\"margin-bottom: 0px; margin-top: 0px;\">LocalCluster</h3>\n",
-                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">a6df0577</p>\n",
+                            "        <p style=\"color: #9D9D9D; margin-bottom: 0px;\">605907d0</p>\n",
                             "        <table style=\"width: 100%; text-align: left;\">\n",
                             "            <tr>\n",
                             "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Dashboard:</strong> <a href=\"/proxy/44739/status\" target=\"_blank\">/proxy/44739/status</a>\n",
+                            "                    <strong>Dashboard:</strong> <a href=\"/proxy/8787/status\" target=\"_blank\">/proxy/8787/status</a>\n",
                             "                </td>\n",
                             "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Workers:</strong> 4\n",
+                            "                    <strong>Workers:</strong> 7\n",
                             "                </td>\n",
                             "            </tr>\n",
                             "            <tr>\n",
                             "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Total threads:</strong> 16\n",
+                            "                    <strong>Total threads:</strong> 28\n",
                             "                </td>\n",
                             "                <td style=\"text-align: left;\">\n",
-                            "                    <strong>Total memory:</strong> 64.00 GiB\n",
+                            "                    <strong>Total memory:</strong> 112.00 GiB\n",
                             "                </td>\n",
                             "            </tr>\n",
                             "            \n",
                             "            <tr>\n",
                             "    <td style=\"text-align: left;\"><strong>Status:</strong> running</td>\n",
                             "    <td style=\"text-align: left;\"><strong>Using processes:</strong> True</td>\n",
                             "</tr>\n",
@@ -87,38 +136,38 @@
                             "            </summary>\n",
                             "\n",
                             "            <div style=\"\">\n",
                             "    <div>\n",
                             "        <div style=\"width: 24px; height: 24px; background-color: #FFF7E5; border: 3px solid #FF6132; border-radius: 5px; position: absolute;\"> </div>\n",
                             "        <div style=\"margin-left: 48px;\">\n",
                             "            <h3 style=\"margin-bottom: 0px;\">Scheduler</h3>\n",
-                            "            <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Scheduler-03233fab-1e0e-4db4-8d02-5f4b7bd9c35a</p>\n",
+                            "            <p style=\"color: #9D9D9D; margin-bottom: 0px;\">Scheduler-d0a3d984-11d5-42df-8e6c-396c4a92f8ee</p>\n",
                             "            <table style=\"width: 100%; text-align: left;\">\n",
                             "                <tr>\n",
                             "                    <td style=\"text-align: left;\">\n",
-                            "                        <strong>Comm:</strong> tcp://127.0.0.1:45817\n",
+                            "                        <strong>Comm:</strong> tcp://127.0.0.1:42135\n",
                             "                    </td>\n",
                             "                    <td style=\"text-align: left;\">\n",
-                            "                        <strong>Workers:</strong> 4\n",
+                            "                        <strong>Workers:</strong> 7\n",
                             "                    </td>\n",
                             "                </tr>\n",
                             "                <tr>\n",
                             "                    <td style=\"text-align: left;\">\n",
-                            "                        <strong>Dashboard:</strong> <a href=\"/proxy/44739/status\" target=\"_blank\">/proxy/44739/status</a>\n",
+                            "                        <strong>Dashboard:</strong> <a href=\"/proxy/8787/status\" target=\"_blank\">/proxy/8787/status</a>\n",
                             "                    </td>\n",
                             "                    <td style=\"text-align: left;\">\n",
-                            "                        <strong>Total threads:</strong> 16\n",
+                            "                        <strong>Total threads:</strong> 28\n",
                             "                    </td>\n",
                             "                </tr>\n",
                             "                <tr>\n",
                             "                    <td style=\"text-align: left;\">\n",
                             "                        <strong>Started:</strong> Just now\n",
                             "                    </td>\n",
                             "                    <td style=\"text-align: left;\">\n",
-                            "                        <strong>Total memory:</strong> 64.00 GiB\n",
+                            "                        <strong>Total memory:</strong> 112.00 GiB\n",
                             "                    </td>\n",
                             "                </tr>\n",
                             "            </table>\n",
                             "        </div>\n",
                             "    </div>\n",
                             "\n",
                             "    <details style=\"margin-left: 48px;\">\n",
@@ -133,37 +182,37 @@
                             "            <details>\n",
                             "                <summary>\n",
                             "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 0</h4>\n",
                             "                </summary>\n",
                             "                <table style=\"width: 100%; text-align: left;\">\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Comm: </strong> tcp://127.0.0.1:38687\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:46769\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Total threads: </strong> 4\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/41735/status\" target=\"_blank\">/proxy/41735/status</a>\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/40325/status\" target=\"_blank\">/proxy/40325/status</a>\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Memory: </strong> 16.00 GiB\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:41549\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:46493\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\"></td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
-                            "                            <strong>Local directory: </strong> /jobfs/95589519.gadi-pbs/dask-scratch-space/worker-hn9y5hob\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-58jauj48\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "\n",
                             "                    \n",
                             "\n",
                             "                    \n",
                             "\n",
@@ -178,37 +227,37 @@
                             "            <details>\n",
                             "                <summary>\n",
                             "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 1</h4>\n",
                             "                </summary>\n",
                             "                <table style=\"width: 100%; text-align: left;\">\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Comm: </strong> tcp://127.0.0.1:35617\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:34353\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Total threads: </strong> 4\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/36911/status\" target=\"_blank\">/proxy/36911/status</a>\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/39537/status\" target=\"_blank\">/proxy/39537/status</a>\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Memory: </strong> 16.00 GiB\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:36389\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:33661\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\"></td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
-                            "                            <strong>Local directory: </strong> /jobfs/95589519.gadi-pbs/dask-scratch-space/worker-_lj8t8bo\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-977asp09\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "\n",
                             "                    \n",
                             "\n",
                             "                    \n",
                             "\n",
@@ -223,37 +272,37 @@
                             "            <details>\n",
                             "                <summary>\n",
                             "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 2</h4>\n",
                             "                </summary>\n",
                             "                <table style=\"width: 100%; text-align: left;\">\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Comm: </strong> tcp://127.0.0.1:43353\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:39573\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Total threads: </strong> 4\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/38847/status\" target=\"_blank\">/proxy/38847/status</a>\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/46155/status\" target=\"_blank\">/proxy/46155/status</a>\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Memory: </strong> 16.00 GiB\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:33113\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:41125\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\"></td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
-                            "                            <strong>Local directory: </strong> /jobfs/95589519.gadi-pbs/dask-scratch-space/worker-hanya5z3\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-uezlbzoy\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "\n",
                             "                    \n",
                             "\n",
                             "                    \n",
                             "\n",
@@ -268,37 +317,172 @@
                             "            <details>\n",
                             "                <summary>\n",
                             "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 3</h4>\n",
                             "                </summary>\n",
                             "                <table style=\"width: 100%; text-align: left;\">\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Comm: </strong> tcp://127.0.0.1:33149\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:35251\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Total threads: </strong> 4\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/40965/status\" target=\"_blank\">/proxy/40965/status</a>\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/34627/status\" target=\"_blank\">/proxy/34627/status</a>\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\">\n",
                             "                            <strong>Memory: </strong> 16.00 GiB\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td style=\"text-align: left;\">\n",
-                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:42157\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:44007\n",
                             "                        </td>\n",
                             "                        <td style=\"text-align: left;\"></td>\n",
                             "                    </tr>\n",
                             "                    <tr>\n",
                             "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
-                            "                            <strong>Local directory: </strong> /jobfs/95589519.gadi-pbs/dask-scratch-space/worker-ubamd8wz\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-uvo757bf\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                </table>\n",
+                            "            </details>\n",
+                            "            </div>\n",
+                            "        </div>\n",
+                            "        \n",
+                            "        <div style=\"margin-bottom: 20px;\">\n",
+                            "            <div style=\"width: 24px; height: 24px; background-color: #DBF5FF; border: 3px solid #4CC9FF; border-radius: 5px; position: absolute;\"> </div>\n",
+                            "            <div style=\"margin-left: 48px;\">\n",
+                            "            <details>\n",
+                            "                <summary>\n",
+                            "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 4</h4>\n",
+                            "                </summary>\n",
+                            "                <table style=\"width: 100%; text-align: left;\">\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:41141\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Total threads: </strong> 4\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/39723/status\" target=\"_blank\">/proxy/39723/status</a>\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Memory: </strong> 16.00 GiB\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:38367\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\"></td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-elwg_v_a\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                </table>\n",
+                            "            </details>\n",
+                            "            </div>\n",
+                            "        </div>\n",
+                            "        \n",
+                            "        <div style=\"margin-bottom: 20px;\">\n",
+                            "            <div style=\"width: 24px; height: 24px; background-color: #DBF5FF; border: 3px solid #4CC9FF; border-radius: 5px; position: absolute;\"> </div>\n",
+                            "            <div style=\"margin-left: 48px;\">\n",
+                            "            <details>\n",
+                            "                <summary>\n",
+                            "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 5</h4>\n",
+                            "                </summary>\n",
+                            "                <table style=\"width: 100%; text-align: left;\">\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:45185\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Total threads: </strong> 4\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/37657/status\" target=\"_blank\">/proxy/37657/status</a>\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Memory: </strong> 16.00 GiB\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:40011\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\"></td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-6vv2nwx5\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                    \n",
+                            "\n",
+                            "                </table>\n",
+                            "            </details>\n",
+                            "            </div>\n",
+                            "        </div>\n",
+                            "        \n",
+                            "        <div style=\"margin-bottom: 20px;\">\n",
+                            "            <div style=\"width: 24px; height: 24px; background-color: #DBF5FF; border: 3px solid #4CC9FF; border-radius: 5px; position: absolute;\"> </div>\n",
+                            "            <div style=\"margin-left: 48px;\">\n",
+                            "            <details>\n",
+                            "                <summary>\n",
+                            "                    <h4 style=\"margin-bottom: 0px; display: inline;\">Worker: 6</h4>\n",
+                            "                </summary>\n",
+                            "                <table style=\"width: 100%; text-align: left;\">\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Comm: </strong> tcp://127.0.0.1:38707\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Total threads: </strong> 4\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Dashboard: </strong> <a href=\"/proxy/36375/status\" target=\"_blank\">/proxy/36375/status</a>\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Memory: </strong> 16.00 GiB\n",
+                            "                        </td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td style=\"text-align: left;\">\n",
+                            "                            <strong>Nanny: </strong> tcp://127.0.0.1:41659\n",
+                            "                        </td>\n",
+                            "                        <td style=\"text-align: left;\"></td>\n",
+                            "                    </tr>\n",
+                            "                    <tr>\n",
+                            "                        <td colspan=\"2\" style=\"text-align: left;\">\n",
+                            "                            <strong>Local directory: </strong> /jobfs/111160700.gadi-pbs/dask-scratch-space/worker-mkyjxysh\n",
                             "                        </td>\n",
                             "                    </tr>\n",
                             "\n",
                             "                    \n",
                             "\n",
                             "                    \n",
                             "\n",
@@ -317,94 +501,76 @@
                             "            </details>\n",
                             "        \n",
                             "\n",
                             "    </div>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "<Client: 'tcp://127.0.0.1:45817' processes=4 threads=16, memory=64.00 GiB>"
+                            "<Client: 'tcp://127.0.0.1:42135' processes=7 threads=28, memory=112.00 GiB>"
                         ]
                     },
                     "execution_count": 2,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "import numpy as np\n",
-                "from itertools import cycle\n",
-                "import os\n",
-                "import dask.array as da\n",
-                "import dask.bag as db\n",
-                "import matplotlib.pyplot as plt\n",
-                "import numpy as np\n",
-                "import xarray as xr\n",
-                "import xesmf as xe\n",
-                "import subprocess\n",
-                "from scipy.ndimage import binary_fill_holes\n",
-                "from importlib import reload\n",
-                "\n",
-                "## For NCI users, uncomment the following line if you just want to import from my copy of the code and sidestep the installation process\n",
-                "## In this case just use the latest version of the analysis env. HOWEVER! Note that without the latest version of xesmf which is not yet\n",
-                "## available on analysis3, the regridding will only work in serial and won't be suitable for large domains\n",
-                "\n",
-                "# os.chdir(\"/home/149/ab8992/cosima_regional/regional-mom6/regional_mom6/\")\n",
-                "\n",
-                "\n",
-                "import regional_mom6 as rm\n",
-                "from dask.distributed import Client\n",
                 "client = Client()\n",
                 "client"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## What does this package do?\n",
                 "\n",
-                "Setting up a regional model in MOM6 is a pain. The goal of this package is that users should spend their debugging time fixing a model that's running and doing weird things, rather than puzzling over a model that won't even start.\n",
+                "Setting up a regional model in MOM6 can be a pain. The goal of this package is that users should spend their debugging time fixing a model that's running and doing weird things, rather than puzzling over a model that won't even start.\n",
                 "\n",
-                "In running this notebook, you'll hopefully have a running MOM6 regional model. There will still be a lot of fiddling to do with the MOM_input file to make sure that the parameters are set up right for your domain, and you might want to manually edit some of the input files. BUT, this package should help you bypass most of the woes of regridding, encoding and understanding the arcane arts of the MOM6 boundary segment files. \n"
+                "In running this notebook, you'll hopefully have a running MOM6 regional model. There will still be a lot of fiddling to do with the MOM_input file to make sure that the parameters are set up right for your domain, and you might want to manually edit some of the input files. *But*, this package should help you bypass most of the woes of regridding, encoding and understanding the arcane arts of the MOM6 boundary segment files. "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## What does this notebook do?\n",
-                "This notebook is designed to showcase where we're up to so far. By the end you should have a running MOM6 experiment on the domain of your choice. To make a stable test case:\n",
+                "\n",
+                "This notebook demonstrates how to set up a regional domain using the package. By the end you should have a running MOM6 experiment on the domain of your choice. To make a stable test case:\n",
                 "\n",
                 "* Avoid any regions with ice\n",
                 "* Avoid regions near the north pole\n",
                 "* Although the default configuration is meant to be RYF, I've not fixed up the calendar and encoding to run longer than a year just yet\n",
                 "\n",
+                "\n",
                 "Input Type | Source\n",
                 "---|---\n",
-                "Surface | ERA5\n",
-                "Ocean | GLORYS reanalysis product\n",
+                "Surface | JRA \n",
+                "Ocean | ACCESS OM2-01\n",
                 "Bathymetry | Gebco"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 0: Your personal environment variables"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "scratch = \"/scratch/v45/ab8992\"\n",
-                "home = \"/home/149/ab8992\"\n",
-                "## If using GLORYs, you'll need an email and password to access their database. make an account here: https://www.copernicus.eu/en/user/login?\n"
+                "scratch = \"/scratch/v45/nc3020\"\n",
+                "gdata = \"/g/data/v45/nc3020\"\n",
+                "home = \"/home/552/nc3020\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 1: Choose our domain, define workspace paths\n",
@@ -413,219 +579,348 @@
                 "\n",
                 "To find the lat/lon of the domain you want to test you can use <a href=\"https://data.marine.copernicus.eu/product/GLOBAL_MULTIYEAR_PHY_001_030/download\" > this GUI </a> and copy paste below"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "expt_name = \"tasmania-example-reanalysis\"\n",
+                "expt_name = \"tassie-glorys\"\n",
                 "\n",
-                "## Choose your coordinates and the name of your experiment\n",
-                "yextent = [-48,-38.95] ## latitude\n",
-                "xextent = [143,150] ## longitude\n",
+                "latitude_extent = [-48, -38.95]\n",
+                "longitude_extent = [143, 150]\n",
                 "\n",
-                "daterange = [\"2003-01-01 00:00:00\", \"2003-01-05 00:00:00\"] ## 2003 is a good compimise for GLORYs and JRA forcing as they overlap. JRA ends in 2012, GLORYS starts in 1993\n",
+                "date_range = [\"2003-01-01 00:00:00\", \"2003-01-05 00:00:00\"]\n",
                 "\n",
                 "## Place where all your input files go\n",
-                "inputdir = f\"{scratch}/regional_mom6_configs/{expt_name}/\"\n",
+                "input_dir = f\"{scratch}/regional_mom6_configs/{expt_name}/\"\n",
                 "\n",
                 "## Directory where you'll run the experiment from\n",
-                "rundir = f\"{home}/mom6_rundirs/{expt_name}/\"\n",
+                "run_dir = f\"{home}/mom6_rundirs/{expt_name}/\"\n",
                 "\n",
                 "## Directory where fre tools are stored\n",
-                "toolpath = \"/home/157/ahg157/repos/mom5/src/tools/\" ## Compiled tools needed for construction of mask tables\n",
+                "toolpath_dir = \"/home/157/ahg157/repos/mom5/src/tools/\" ## Compiled tools needed for construction of mask tables\n",
                 "\n",
-                "## Directory where raw downloads go before processing\n",
-                "tmpdir = f\"{scratch}/regional_tmp/{expt_name}\"\n",
+                "## Directory where ocean model cut-outs go before processing\n",
+                "tmp_dir = f\"{gdata}/{expt_name}\"\n",
                 "\n",
-                "for i in [rundir,tmpdir,inputdir]:\n",
+                "for i in [run_dir, tmp_dir, input_dir]:\n",
                 "    if not os.path.exists(i):\n",
-                "        subprocess.run(f\"mkdir {i} -p\",shell=True)\n",
-                "\n",
-                "\n"
+                "        os.makedirs(str(i))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 2: Prepare ocean forcing data\n",
                 "\n",
-                "We need to cut out our ocean forcing. The pipeline expects an initial condition and one time-dependent segment per non-land boundary. Naming convention is \"east_unprocessed\" and \"ic_unprocessed\" for initial condition. If you're an NCI user you can execute the following cell to use my already downloaded boundaries for the test domain, OR make an account with copernicus to download forcing files of your choosing using the second cell"
+                "We need to cut out our ocean forcing. The pipeline expects an initial condition and one time-dependent segment per non-land boundary. Naming convention is `\"east_unprocessed\"` and `\"ic_unprocessed\"` for initial condition. The following provides an example for cutting out the necessary forcing files from an ocean model. It's hardcoded to pull data from a Repeat-Year Forced ACCESS-OM2-01 database, but you should be able to recycle parts of the code to cut out data from a dataset of your choice"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### For default 'Tassie' domain:\n",
-                "You can just read in the boundaries I've already downloaded. Overwrite your tmpdir and continue with the notebook without generating ocean forcing files"
+                "**NOTE: this is hardcoded for the year of 1990, which corresponds to output files `1077`-`1082`. If you want to modify, you'll need to choose the right path to the year of your choice, or use the COSIMA cookbook to locate your data files**"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "tmpdir = \"/g/data/v45/ab8992/tassie-glorys\""
+                "## Cut out 3 months of forcing from 2003\n",
+                "om2_input = xr.open_mfdataset(\n",
+                "    f\"/g/data/ik11/outputs/access-om2-01/01deg_jra55v13_ryf9091/output1077/ocean/ocean_daily*\",\n",
+                "    parallel=True, chunks='auto')[[\"u\", \"v\", \"salt\", \"temp\", \"eta_t\"]].sel(\n",
+                "        yu_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[1] + 0.2),\n",
+                "        yt_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[1] + 0.2)).isel(time = slice(0, 5))\n",
+                "\n",
+                "## Cut out initial condition and save\n",
+                "ic = om2_input.isel(time = 0)\n",
+                "\n",
+                "## `longitude_slicer` handles seams in longitude and different grid and ensures that the output matches our 'longitude_extent'\n",
+                "ic = rmom6.longitude_slicer(ic, [longitude_extent[0], longitude_extent[1]], [\"xu_ocean\", \"xt_ocean\"])\n",
+                "ic.to_netcdf(tmp_dir + \"/ic_unprocessed.nc\")\n",
+                "\n",
+                "## Cut out East and West segments. Does lat slice first then uses `longitude_slicer` for lon slice\n",
+                "eastwest = om2_input.sel(    \n",
+                "    yu_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[1] + 0.2),\n",
+                "    yt_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[1] + 0.2)\n",
+                ")\n",
+                "rmom6.longitude_slicer(eastwest, [longitude_extent[1], longitude_extent[1]], [\"xu_ocean\", \"xt_ocean\"]).to_netcdf(tmp_dir + \"/east_unprocessed.nc\")\n",
+                "rmom6.longitude_slicer(eastwest, [longitude_extent[0], longitude_extent[0]], [\"xu_ocean\", \"xt_ocean\"]).to_netcdf(tmp_dir + \"/west_unprocessed.nc\")\n",
+                "\n",
+                "## Cut out North and South segments\n",
+                "northsouth = rmom6.longitude_slicer(om2_input, [longitude_extent[0], longitude_extent[1]], [\"xu_ocean\", \"xt_ocean\"])\n",
+                "northsouth.sel(\n",
+                "    yu_ocean = slice(latitude_extent[1] - 0.2, latitude_extent[1] + 0.2),\n",
+                "    yt_ocean = slice(latitude_extent[1] - 0.2, latitude_extent[1] + 0.2)\n",
+                ").to_netcdf(tmp_dir + \"/north_unprocessed.nc\")\n",
+                "northsouth.sel(\n",
+                "    yu_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[0] + 0.2),\n",
+                "    yt_ocean = slice(latitude_extent[0] - 0.2, latitude_extent[0] + 0.2)\n",
+                ").to_netcdf(tmp_dir + \"/south_unprocessed.nc\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### OR download your own ocean forcing\n",
-                "The following cell generates a bash script in your designated 'temporary directory'. This should be on scratch somewhere and just a container for your raw downloads.\n",
-                "\n",
-                "To do this you'll need to register with the Copernicus data centre to get a username and password. Fill these in below.\n",
+                "## Step 3: Make experiment object\n",
+                "This object keeps track of your domain basics, as well as generating the hgrid, vgrid and setting up the folder structures. \n",
                 "\n",
-                "After executing, navigate to this directory in your terminal and double check that all the files are there! Sometimes the data centre hangs and only retrieves a couple of files. In thise case, comment out the completed segments in `get_oceanfiles.sh` and run it again from terminal."
+                "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
+            "execution_count": 6,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "pwd = \"YOUR COPERNICUS PASSWORD\"    \n",
-                "usr = \"YOUR COPERNICUS USERNAME\"  \n",
-                "file = open(f\"{tmpdir}/get_oceanfiles.sh\",\"w\")\n",
-                "file.write(\n",
-                "        rm.motu_requests(xextent, yextent, daterange, tmpdir, usr, pwd,[\"north\",\"south\",\"east\",\"west\"])\n",
-                ")\n",
-                "file.close()\n",
-                "\n",
-                "### NOTE!! This will only work as a subprocess if your kernel has internet access. If not, you'll need to navigate to your tmpdir in a login node terminal and run bash get_oceanfiles.sh\n",
-                "subprocess.run(\n",
-                "    f\"bash {tmpdir}/get_oceanfiles.sh\",shell=True\n",
-                ")\n"
+                "expt = rmom6.experiment(\n",
+                "    longitude_extent = longitude_extent,\n",
+                "    latitude_extent = latitude_extent,\n",
+                "    date_range = date_range,\n",
+                "    resolution = 0.05,\n",
+                "    number_vertical_layers = 75,\n",
+                "    layer_thickness_ratio = 10,\n",
+                "    depth = 4500,\n",
+                "    mom_run_dir = run_dir,\n",
+                "    mom_input_dir = input_dir,\n",
+                "    toolpath_dir = toolpath_dir\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Step 3: Make experiment object\n",
-                "This object keeps track of your domain basics, as well as generating the hgrid, vgrid and setting up the folder structures. \n",
-                "\n",
                 "After running you can have a look at your grids by calling `expt.hgrid` and `expt.vgrid`\n",
                 "\n",
-                "Plotting vgrid with marker = '.' option lets you see the spacing, or plotting \n",
+                "Plotting the vertical grid with `marker = '.'` option lets you see the spacing. For example, you can use `numpy.diff` to compute the vertical spacings, e.g.,\n",
                 "```python\n",
-                "np.diff(expt.hgrid.zl).plot(marker = '.')\n",
+                "import numpy as np\n",
+                "np.diff(expt.vgrid.zl)\n",
                 "```\n",
-                " shows you the vertical spacing profile.\n",
+                "and then visualise this with the package of your liking.\n",
                 "\n",
                 "### Modular workflow!\n",
                 "\n",
-                "After constructing your expt object, if you don't like my lazy default hgrid and vgrid you can simply modify and overwrite them. However, you'll also need to save them to disk again as I've not automated this just yet. For example:\n",
+                "After constructing your expt object, if you don't like the default hgrid and vgrids you can simply modify and overwrite them. However, you'll then also need to save them to disk again. For example:\n",
+                "\n",
+                "```python\n",
+                "new_hgrid = xr.open_dataset(input_dir / \"hgrid.nc\")\n",
+                "```\n",
+                "Modify `new_hgrid`, ensuring that metadata is retained to keep MOM6 happy. Then, save your changes\n",
                 "\n",
                 "```python\n",
-                "expt.hgrid = custom_hgrid\n",
-                "expt.hgrid.to_netcdf(f\"{inputdir}/hgrid.nc\")\n",
+                "expt.hgrid = new_hgrid\n",
+                "\n",
+                "expt.hgrid.to_netcdf(input_dir / \"hgrid.nc\")\n",
                 "```"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 6,
+            "cell_type": "markdown",
             "metadata": {},
+            "source": [
+                "## Step 4: Set up bathymetry\n",
+                "\n",
+                "Similarly to ocean forcing, we point our 'bathymetry' method at the location of the file of choice, and pass it a dictionary mapping variable names. This time we don't need to preprocess the topography since it's just a 2D field and easier to deal with. Afterwards you can run `expt.topog` and have a look at your domain. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 7,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "NOTE from make_solo_mosaic: there are 0 contacts (align-contact)\n",
-                        "congradulation: You have successfully run make_solo_mosaic\n",
-                        "FRE TOOLS: Make solo mosaic\n",
+                        "Begin regridding bathymetry...\n",
+                        "\n",
+                        "If this process hangs it means that the chosen domain might be too big to handle this way. After ensuring access to appropriate computational resources, try calling ESMF directly from a terminal in the input directory via\n",
                         "\n",
+                        "mpirun ESMF_Regrid -s bathy_original.nc -d topog_raw.nc -m bilinear --src_var elevation --dst_var elevation --netcdf4 --src_regional --dst_regional\n",
                         "\n",
-                        "CompletedProcess(args=['/home/157/ahg157/repos/mom5/src/tools/make_solo_mosaic/make_solo_mosaic', '--num_tiles', '1', '--dir', '.', '--mosaic_name', 'ocean_mosaic', '--tile_file', 'hgrid.nc'], returncode=0)\n"
+                        "For details see https://xesmf.readthedocs.io/en/latest/large_problems_on_HPC.html\n",
+                        "\n",
+                        "Aftewards, run the bathymetry method again but set 'make_topography = False' so the computationally expensive step is skiped and instead the method ensures that only the metadata are fixed.\n",
+                        "Regridding in parallel: True\n",
+                        "Regridding finished. Now excavating inland lakes and fixing up metadata...\n",
+                        "Reading in regridded bathymetry to fix up metadata...done.\n"
                     ]
                 }
             ],
             "source": [
-                "expt = rm.experiment(\n",
-                "    xextent,\n",
-                "    yextent,\n",
-                "    daterange,\n",
-                "    0.05,  # Resolution\n",
-                "    75,    # Number of vertical layers\n",
-                "    10,    # Ratio of largest to smallest vertical layer. Select 1 for linear, negative number for higher resolution at bottom\n",
-                "    4500,  # Depth of simulation\n",
-                "    rundir,\n",
-                "    inputdir,\n",
-                "    toolpath\n",
-                ")"
+                "expt.setup_bathymetry(\n",
+                "    bathymetry_path='/g/data/ik11/inputs/GEBCO_2022/GEBCO_2022.nc',\n",
+                "    longitude_coordinate_name='lon',\n",
+                "    latitude_coordinate_name='lat',\n",
+                "    vertical_coordinate_name='elevation',\n",
+                "    minimum_layers=1\n",
+                "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Step 4: Set up bathymetry\n",
-                "\n",
-                "Similarly to ocean forcing, we point our 'bathymetry' method at the location of the file of choice, and pass it a dictionary mapping variable names. This time we don't need to preprocess the topography since it's just a 2D field and easier to deal with. Afterwards you can run `expt.topog` and have a look at your domain. After running this cell, your input directory will contain other topography - adjacent things like the ocean mosaic and mask table too. This defaults to a 10x10 layout which can be updated later."
+                "### Check out your domain:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
-            "metadata": {},
+            "execution_count": 8,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        " Starting weight generation with these inputs: \n",
-                        "   Source File: bathy_original.nc\n",
-                        "   Destination File: topog_raw.nc\n",
-                        "   Source variable names: elevation\n",
-                        "   Destination variable names: elevation\n",
-                        "   Souce Grid has a mask, using missingvalue    1.0000000000000000E+020\n",
-                        "   Source File is in GRIDSPEC format with coordinate names lon lat\n",
-                        "   Source Grid is a regional grid\n",
-                        "   Destination File is in GRIDSPEC format with coordinate names lon lat\n",
-                        "   Destination Grid is a regional grid\n",
-                        "   Regrid Method: bilinear\n",
-                        "   Pole option: NONE\n",
-                        "\n",
-                        " Completed file regrid successfully.\n",
-                        "\n",
-                        "NOTE from make_solo_mosaic: there are 0 contacts (align-contact)\n",
-                        "congradulation: You have successfully run make_solo_mosaic\n",
-                        "MAKE SOLO MOSAIC\n",
-                        "\n",
-                        "CompletedProcess(args='/home/157/ahg157/repos/mom5/src/tools/make_solo_mosaic/make_solo_mosaic --num_tiles 1 --dir . --mosaic_name ocean_mosaic --tile_file hgrid.nc', returncode=0)\n"
-                    ]
+                    "data": {
+                        "text/plain": [
+                            "<matplotlib.collections.QuadMesh at 0x14ae191683a0>"
+                        ]
+                    },
+                    "execution_count": 8,
+                    "metadata": {},
+                    "output_type": "execute_result"
                 },
                 {
-                    "name": "stderr",
+                    "data": {
+                        "image/png": "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G5Lf5/I5VqtV+fjHPy7r1q2Tzs5OOf744+VTn/qU1FHMaq6d3w9/+EN561vfKqtWrZJUKiX//u//rn5v53xKpZJ88IMflKVLl0p3d7dcdtll8tJLL83iWewb+zrHSqUiH/3oR+X000+X7u5uWbVqlVxxxRXy8ssvq30c7ecYsIARBUR33313lMvlojvvvDN68skno2uuuSbq7u6OXnzxxSPdtf3Gm970pugrX/lK9Pjjj0cbN26M3vzmN0dr1qyJJiYmkja33npr1NPTE33rW9+KHnvsseid73xntHLlymhsbOwI9vzA8PDDD0fHHXdc9KpXvSq65pprkvVz/Rz37NkTrV27NvqDP/iD6KGHHoo2b94c3XvvvdGzzz6btJnL53jTTTdFS5Ysif7zP/8z2rx5c/Rv//Zv0aJFi6LbbrstaTPXzu973/tedMMNN0Tf+ta3IhGJvvOd76jf2zmfq666KjrmmGOi9evXR4888kj0ute9LjrjjDOiarU6y2fjxr7OcWRkJLr44oujb37zm9Evf/nL6Mc//nF07rnnRmeddZbax9F+jgELF8EgiqLonHPOia666iq17qSTToquv/76I9SjQ4fh4eFIRKL7778/iqIoqtfr0eDgYHTrrbcmbYrFYtTX1xf9wz/8w5Hq5gFhfHw8OuGEE6L169dHF154YWIQzYdz/OhHPxpdcMEF3t/n+jm++c1vjv7oj/5IrXv7298evfe9742iaO6f30xjoZ3zGRkZiXK5XHT33XcnbbZt2xal0+nonnvumbW+twuX0TcTDz/8cCQiyeRyrp1jwMLCgneZlctl2bBhg1xyySVq/SWXXCIPPvjgEerVocPo6KiIiAwMDIiIyObNm2VoaEidb6FQkAsvvHDOne9f/MVfyJvf/Ga5+OKL1fr5cI7f/e535eyzz5bf+73fk+XLl8uZZ54pd955Z/L7XD/HCy64QP7nf/5HnnnmGRER+fnPfy4PPPCA/NZv/ZaIzP3zm4l2zmfDhg1SqVRUm1WrVslpp502J89ZpDH+pFIp6e/vF5H5eY4B8wfzRqn6QLFr1y6p1WqyYsUKtX7FihUyNDR0hHp1aBBFkVx33XVywQUXyGmnnSYikpyT63xffPHFWe/jgeLuu++WRx55RH760582/TYfzvH555+XL33pS3LdddfJX//1X8vDDz8sV199tRQKBbniiivm/Dl+9KMfldHRUTnppJMkk8lIrVaTT3/60/Lud79bRObHPSTaOZ+hoSHJ5/OyePHipjZzcSwqFoty/fXXy3ve856kwOt8O8eA+YUFbxAZpFIp9XcURU3r5ho+8IEPyC9+8Qt54IEHmn6by+e7detWueaaa+T73//+PitBz+VzrNfrcvbZZ8vNN98sIiJnnnmmPPHEE/KlL31JrrjiiqTdXD3Hb37zm3LXXXfJN77xDTn11FNl48aNcu2118qqVavkyiuvTNrN1fPz4UDOZy6ec6VSkXe9611Sr9fl9ttvb9l+Lp5jwPzDgneZLV26VDKZTNPsZHh4uGk2N5fwwQ9+UL773e/KfffdJ8cee2yyfnBwUERkTp/vhg0bZHh4WM466yzJZrOSzWbl/vvvl7/7u7+TbDabnMdcPseVK1fKKaecotadfPLJsmXLFhGZ+/fxr/7qr+T666+Xd73rXXL66afL5ZdfLh/60IfklltuEZG5f34z0c75DA4OSrlclr1793rbzAVUKhV5xzveIZs3b5b169cn7JDI/DnHgPmJBW8Q5fN5Oeuss2T9+vVq/fr16+U1r3nNEerVgSOKIvnABz4g3/72t+V///d/Zd26der3devWyeDgoDrfcrks999//5w53ze84Q3y2GOPycaNG5N/Z599tvz+7/++bNy4UY4//vg5f46//uu/3iSX8Mwzz8jatWtFZO7fx6mpKUmn9fCTyWSStPu5fn4z0c75nHXWWZLL5VSb7du3y+OPPz5nztkYQ5s2bZJ7771XlixZon6fD+cYMI9xpKK5jyaYtPsvf/nL0ZNPPhlde+21UXd3d/TCCy8c6a7tN/78z/886uvri37wgx9E27dvT/5NTU0lbW699daor68v+va3vx099thj0bvf/e6jOp25HTDLLIrm/jk+/PDDUTabjT796U9HmzZtir7+9a9HXV1d0V133ZW0mcvneOWVV0bHHHNMknb/7W9/O1q6dGn0kY98JGkz185vfHw8evTRR6NHH300EpHo85//fPToo48mGVbtnM9VV10VHXvssdG9994bPfLII9HrX//6oyolfV/nWKlUossuuyw69thjo40bN6rxp1QqJfs42s8xYOEiGEQxvvjFL0Zr166N8vl89Gu/9mtJmvpcg4g4/33lK19J2tTr9egTn/hENDg4GBUKheg3fuM3oscee+zIdfoQYKZBNB/O8T/+4z+i0047LSoUCtFJJ50U3XHHHer3uXyOY2Nj0TXXXBOtWbMm6ujoiI4//vjohhtuUB/OuXZ+9913n/Pdu/LKK6Moau98pqenow984APRwMBA1NnZGb3lLW+JtmzZcgTOxo19nePmzZu94899992X7ONoP8eAhYtUFEXR7PFRAQEBAQEBAQFHHxZ8DFFAQEBAQEBAQDCIAgICAgICAhY8gkEUEBAQEBAQsOARDKKAgICAgICABY9gEAUEBAQEBAQseASDKCAgICAgIGDBIxhEAQEBAQEBAQsewSAKCAgICAgIWPAIBlFAQEBAQEDAgkcwiAICAgICAgIWPIJBFBCwwHHRRRfJ1VdfLR/5yEdkYGBABgcH5cYbbxQRkR/84AeSz+flRz/6UdL+c5/7nCxdulS2b99+hHocEBAQcOgRDKKAgAD52te+Jt3d3fLQQw/JZz7zGfnUpz4l69evl4suukiuvfZaufzyy2V0dFR+/vOfyw033CB33nmnrFy58kh3OyAgIOCQIRR3DQhY4LjoooukVqspFuicc86R17/+9XLrrbdKuVyW8847T0444QR54okn5Pzzz5c777zzCPY4ICAg4NAje6Q7EBAQcOTxqle9Sv29cuVKGR4eFhGRfD4vd911l7zqVa+StWvXym233XYEehgQEBBweBFcZgEBAZLL5dTfqVRK6vV68veDDz4oIiJ79uyRPXv2zGrfAgICAmYDwSAKCAjYJ5577jn50Ic+JHfeeaecd955csUVVyhjKSAgIGA+IBhEAQEBXtRqNbn88svlkksukT/8wz+Ur3zlK/L444/L5z73uSPdtYCAgIBDimAQBQQEePHpT39aXnjhBbnjjjtERGRwcFD+6Z/+ST7+8Y/Lxo0bj2znAgICAg4hQpZZQEBAQEBAwIJHYIgCAgICAgICFjyCQRQQEBAQEBCw4BEMooCAgICAgIAFj2AQBQQEBAQEBCx4BIMoICAgICAgYMEjGEQBAQEBAQEBCx7BIAoICAgICAhY8AgGUUBAQEBAQMCCRzCIAgICAgICAhY8gkEUEBAQEBAQsOARDKKAgICAgICABY9gEAUEBAQEBAQsePz/LOUhC/oBD7oAAAAASUVORK5CYII=",
+                        "text/plain": [
+                            "<Figure size 640x480 with 2 Axes>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                }
+            ],
+            "source": [
+                "expt.topog.depth.plot()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "##  Step 5: Handle the ocean forcing - where the magic happens\n",
+                "\n",
+                "This cuts out and interpolates the initial condition as well as all boundaries (unless you don't pass it boundaries).\n",
+                "\n",
+                "The dictionary maps the MOM6 variable names to what they're called in your ocean input file. Notice how the horizontal dimensions are `x` and `y` in the GLORYS reanalysis example, vs `xh`, `yh`, `xq`, `yq`. This is because ACCESS-OM2-01 is on a `B` grid, so we need to differentiate between `q` and `t` points. \n",
+                "\n",
+                "If one of your segments is land, you can delete its string from the 'boundaries' list. You'll need to update `MOM_input` to reflect this though so it knows how many segments to look for, and their orientations. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 9,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
+                {
+                    "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "cp: './ocean_mosaic.nc' and 'ocean_mosaic.nc' are the same file\n",
-                        "cp: './hgrid.nc' and 'hgrid.nc' are the same file\n"
+                        "INITIAL CONDITIONS\n",
+                        "Regridding Velocities...Done.\n",
+                        "Regridding Tracers...\n",
+                        "Done.\n",
+                        "Regridding Free surface...\n",
+                        "Saving outputs... done setting up initial condition.\n",
+                        "Processing south boundary...Done.\n",
+                        "Processing north boundary...Done.\n",
+                        "Processing west boundary...Done.\n",
+                        "Processing east boundary...Done.\n"
                     ]
-                },
+                }
+            ],
+            "source": [
+                "# Define a mapping from the MOM5 B grid variables and dimensions to the MOM6 C grid ones\n",
+                "ocean_varnames = {\"time\": \"time\",\n",
+                "                  \"yh\": \"yt_ocean\",\n",
+                "                  \"xh\": \"xt_ocean\",\n",
+                "                  \"xq\": \"xu_ocean\",\n",
+                "                  \"yq\": \"yu_ocean\",\n",
+                "                  \"zl\": \"st_ocean\",\n",
+                "                  \"eta\": \"eta_t\",\n",
+                "                  \"u\": \"u\",\n",
+                "                  \"v\": \"v\",\n",
+                "                  \"tracers\": {\"salt\": \"salt\", \"temp\": \"temp\"}\n",
+                "                  }\n",
+                "\n",
+                "# Set up the initial condition\n",
+                "expt.initial_condition(\n",
+                "    tmp_dir + '/ic_unprocessed.nc', # directory where the unprocessed initial condition is stored, as defined earlier\n",
+                "    ocean_varnames,\n",
+                "    gridtype=\"B\"\n",
+                "    )\n",
+                "\n",
+                "# Now iterate through our four boundaries \n",
+                "for i, orientation in enumerate([\"south\", \"north\", \"west\", \"east\"]):\n",
+                "    expt.rectangular_boundary(\n",
+                "        tmp_dir + '/' + orientation + \"_unprocessed.nc\",\n",
+                "        ocean_varnames,\n",
+                "        orientation,    # Needs to know the cardinal direction of the boundary\n",
+                "        i + 1,          # Just a number to identify the boundary. Indexes from 1 \n",
+                "        arakawa_grid=\"B\"\n",
+                "        )"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Step 6 Run the FRE tools\n",
+                "\n",
+                "This is just a wrapper for the FRE tools needed to make the mosaics and masks for the experiment. The only thing you need to tell it is the processor layout. In this case we're saying that we want a 10 by 10 grid of 100 processors. "
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 10,
+            "metadata": {
+                "tags": []
+            },
+            "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
+                        "Running GFDL's FRE Tools. The following information is all printed by the FRE tools themselves\n",
+                        "NOTE from make_solo_mosaic: there are 0 contacts (align-contact)\n",
+                        "congradulation: You have successfully run make_solo_mosaic\n",
+                        "OUTPUT FROM MAKE SOLO MOSAIC:\n",
+                        "\n",
+                        "CompletedProcess(args='/home/157/ahg157/repos/mom5/src/tools/make_solo_mosaic/make_solo_mosaic --num_tiles 1 --dir . --mosaic_name ocean_mosaic --tile_file hgrid.nc', returncode=0)\n",
                         "cp ./hgrid.nc hgrid.nc \n",
                         "\n",
                         "NOTE from make_coupler_mosaic: the ocean land/sea mask will be determined by field depth from file topog.nc\n",
                         "mosaic_file is grid_spec.nc\n",
                         "\n",
                         "***** Congratulation! You have successfully run make_quick_mosaic\n",
-                        "QUICK MOSAIC\n",
+                        "OUTPUT FROM QUICK MOSAIC:\n",
                         "\n",
                         "CompletedProcess(args='/home/157/ahg157/repos/mom5/src/tools/make_quick_mosaic/make_quick_mosaic --input_mosaic ocean_mosaic.nc --mosaic_name grid_spec --ocean_topog topog.nc', returncode=0)\n",
                         "\n",
                         " ===>NOTE from check_mask: when layout is specified, min_pe and max_pe is set to layout(1)*layout(2)=100\n",
                         "\n",
                         " ===>NOTE from check_mask: Below is the list of command line arguments.\n",
                         "\n",
@@ -683,331 +978,106 @@
                         "\n",
                         "NOTE from check_mask: The following is for using model source code with version siena_201207 or newer,\n",
                         "                      specify ocean_model_nml/ice_model_nml/atmos_model_nml/land_model/nml \n",
                         "                      variable mask_table with the mask_table created here.\n",
                         "                      Also specify the layout variable in each namelist using corresponding layout\n",
                         "\n",
                         "***** Congratulation! You have successfully run check_mask\n",
-                        "CHECK MASK CompletedProcess(args='/home/157/ahg157/repos/mom5/src/tools/check_mask/check_mask --grid_file ocean_mosaic.nc --ocean_topog topog.nc --layout 10,10 --halo 4', returncode=0)\n"
+                        "OUTPUT FROM CHECK MASK:\n",
+                        "\n",
+                        " CompletedProcess(args='/home/157/ahg157/repos/mom5/src/tools/check_mask/check_mask --grid_file ocean_mosaic.nc --ocean_topog topog.nc --layout 10,10 --halo 4', returncode=0)\n"
+                    ]
+                },
+                {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "cp: './ocean_mosaic.nc' and 'ocean_mosaic.nc' are the same file\n",
+                        "cp: './hgrid.nc' and 'hgrid.nc' are the same file\n"
                     ]
                 }
             ],
             "source": [
-                "expt.bathymetry(\n",
-                "    '/g/data/ik11/inputs/GEBCO_2022/GEBCO_2022.nc',\n",
-                "    {\"xh\":\"lon\",\n",
-                "     \"yh\":\"lat\",\n",
-                "     \"elevation\":\"elevation\"}, ## Again this dictionary just maps mom6 variable names to what they are in your topog.\n",
-                "     minimum_layers = 1\n",
-                "    )"
+                "expt.FRE_tools(layout = (10, 10))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Check out your domain:"
+                "## Step 7: Modify the default input directory to make a (hopefully) runnable configuration out of the box\n",
+                "\n",
+                "This step copies the default directory, and modifies the `MOM_input` and `SIS_input` files to match your experiment. If you use Payu to run mom6, set the `using_payu` flag to `True` and an example `config.yaml` file will be copied to your run directory. This still needs to be modified manually to work with your projects, executable etc.\n",
+                "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
+            "execution_count": 11,
+            "metadata": {
+                "tags": []
+            },
             "outputs": [
                 {
-                    "data": {
-                        "text/plain": [
-                            "<matplotlib.collections.QuadMesh at 0x1460e66a9100>"
-                        ]
-                    },
-                    "execution_count": 8,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                },
-                {
-                    "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAkQAAAHFCAYAAAAT5Oa6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjcuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8pXeV/AAAACXBIWXMAAA9hAAAPYQGoP6dpAAEAAElEQVR4nOz9eZxdVZU2jq8z3amGW6kklUoghBkZlRcFgtogCIGXwanFV+zIJPJpEeQDqO3UBpuGFrsVf+D82oQGaWzfr0Njd9OAA7YdUInSgiAqBiSQkJDUXHc6w++Pc/bZz667d917q27dqqTWw+d+sjl1zj77nnvOPmuvZ61nWVEURcRgMBgMBoOxiGHP9wAYDAaDwWAw5htsEDEYDAaDwVj0YIOIwWAwGAzGogcbRAwGg8FgMBY92CBiMBgMBoOx6MEGEYPBYDAYjEUPNogYDAaDwWAserBBxGAwGAwGY9GDDSIGg8FgMBiLHmwQMRY9NmzYQJZldfScP/zhD+mSSy6hV7ziFdTV1UX77LMPvelNb6LNmzcr+wVBQJ/97GfpzDPPpH333ZcKhQIdfvjh9Fd/9Vc0PDzc1Lm+//3v07vf/W46+uijyfO8ht/1iSeeoLe//e20fPlyymaztP/++9P73ve+hue56KKLyLIssiyLjjrqqKbG1m5s2rSJNmzY0PS1mQu86lWvSq/DOeecM2/jYDAYrYENIsaix3ve8x56+OGHO3rOL33pS/Tss8/SBz7wAfr3f/93+vznP087duygE088kX74wx+m+5VKJdqwYQOtWbOGbrnlFvr3f/93uuyyy+irX/0qvfa1r6VSqdTwXN/5znfokUceoSOOOIJe+cpXTrvvj370Izr++ONpdHSUvvzlL9P9999Pf/M3f0O5XK6p7zU4OEgPP/ww3X333U3t325s2rSJrr/++nk1iO688056+OGHaXBwcN7GwGAwWoc73wNgMOYb++67L+27774dPecXvvAFGhgYULadeeaZdPDBB9ONN95Ip556KhER5fN52rJlCy1dujTd75RTTqH99tuP3v72t9P/9//9f/QXf/EX057ra1/7Gtl2vPZ5//vfX+eFEpicnKR3vetddOqpp9K9996reJLWr1/f1PfKZrN04oknNrXvnoTJyUkqFApN7Xv00UcTUXwtGAzGngP2EDH2agjqQvd59tlniWh+KLOpxhARUXd3Nx1xxBH0/PPPp9scx1GMIYHjjz+eiEjZ1wRhDDXCt771Ldq2bRt98IMfbPv1sCyL3v/+99Ptt99Ohx12GOXzeXr1q19NjzzyCEVRRJ/5zGfogAMOoO7ubjr11FPpD3/4Q10fDz74IJ122mnU29tLhUKBXvva19IPfvCD9O8bNmygD37wg0REdMABB6S/849//ON0n29+85u0du1a6urqou7ublq3bh396le/Us5z0UUXUXd3Nz3++ON0xhlnUE9PD5122mlERPSrX/2KzjnnHBoYGKBsNkurVq2is88+m7Zu3drW68VgMDoPNogYezUefvhh5fPDH/6Q9tlnHxocHKT+/v6W+oqiiHzfb+ozE4yMjNAvf/lLOvLIIxvuK2i1ZvZtFj/5yU+IKI5bet3rXkeZTIaWLFlC73znO+nFF1+cdf/f//736f/+3/9Lf/d3f0f//M//TGNjY3T22WfTtddeS//93/9Nt912G331q1+lJ598kt72trdRFEXpsXfddRedccYZ1NvbS3fccQf9y7/8C/X399O6detSo+g973kPXXnllURE9O1vfzv9zf/X//pfRER044030jvf+U464ogj6F/+5V/ozjvvpLGxMXr9619PTz75pDLWarVK5513Hp166qn0ve99j66//nqamJig008/nV566SX6whe+QA888ADdcssttN9++9HY2Nisrw+DwZhnRAzGIoHv+9Gb3vSmqLu7O9q8eXO6/ZOf/GTUzKNw++23R0TU1GcmeNe73hW5rhs9+uij0+63devWaMWKFdGrX/3qKAiCls5xxRVXGMe3bt26iIiivr6+6EMf+lD0wx/+MPryl78cLV26NDr44IOjiYmJafu+8MILozVr1mj/RkTR4OBgND4+nm777ne/GxFR9KpXvSoKwzDdfsstt0REFP3617+OoiiKJiYmov7+/ujcc89V+gyCIHrlK18ZHX/88em2z3zmMxERRVu2bFH2/dOf/hS5rhtdeeWVyvaxsbFocHAwOv/885XvQUTRP/7jPyr7PvrooxERRd/97nenvQ4Ca9asic4+++ym9mUwGPMPjiFiLBq8//3vp3/7t3+je++9N/UatIJzzz2XfvGLX8zByIg+8YlP0De+8Q269dZb6bjjjjPut3v3bvrf//t/UxRF9M1vfrNpOqwZhGFIRETveMc76NOf/jQREb3hDW+gwcFBevOb30x33303vec975lx/294wxuoq6sr/f/DDz+ciIjOOusshaIT25977jk6+uijadOmTbR792668MIL67xvZ555Jt188800MTGh9D0V//mf/0m+79O73/1upY9cLkcnn3wy/ehHP6o75m1ve5vy/wcffDAtWbKEPvzhD9O2bdvoz/7sz+iII45o4QowGIyFDDaIGIsCN9xwA335y1+mr3/963TmmWfOqI/+/n4qFottHhnR9ddfTzfccAP97d/+Lb3//e837jc0NESnn346vfDCC/TDH/6QDjzwwLaOQ8QqrVu3Ttm+bt06siyLfvnLX86q/6kUZSaTmXZ7uVwmIqKXXnqJiIj+/M//3Nj37t27pzWIRB+vec1rtH+falgWCgXq7e1VthWLRXrooYfob//2b+mjH/0oDQ0N0cqVK+myyy6jj3/84+R5nvH8DAZj4YMNIsZej40bN9InPvEJ2rBhA11yySUz7ueOO+6giy++uKl9I4h/mQ7XX389bdiwgTZs2EAf/ehHjfsNDQ3RG9/4RtqyZQv94Ac/oGOOOaap/lvBMcccQ/fcc4/x7+30RrWCZcuWERHRrbfeasxgW7FiRVN9/L//9/9ozZo1Dc9pCio/+uij6Z577qEoiujXv/41bdy4kT71qU9RPp+nv/qrv2rYL4PBWLhgg4ixV+O+++6jyy67jC655BL65Cc/Oau+2k2Z/c3f/A1t2LCBPv7xj087NmEM/fGPf6QHHniAjj322LaNAfGWt7yFPvaxj9F//Md/0Fve8pZ0+3/8x39QFEXzlk7/2te+lvr6+ujJJ5+c1oNGJFPdp+ozrVu3jlzXpWeeeaaOCpsJLMuiV77ylfS5z32ONm7cOGvvGYPBmH+wQcTYa7FlyxZ6+9vfTgceeCBdfPHF9Mgjjyh/P/bYY1vSilm6dKk2BX4m+Id/+Af667/+azrzzDPp7LPPrhubMD5KpVKaGn7LLbeQ7/vKvsuXL6eDDjoo/X/Xdenkk09W0tGfe+651JB75plniCj2lBAR7b///vTqV7+aiIhe8YpX0BVXXEFf/OIXqaenh8466yz63e9+Rx//+Mfp2GOPpfPPP78t371VdHd306233koXXngh7d69m/78z/+cBgYGaOfOnfQ///M/tHPnTvrSl75ERFID6POf/zxdeOGF5Hke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ZUt0xx13RI8//njSZj6f4/XXXx8tWbIk+o//+I9oy5Yt0b/9279Fvb290c0335y0mW/n9/3vfz+69tpro29961uRiET//u//rj7v5HyuuOKK6Nhjj402bNgQ3XfffdGrX/3q6Mwzz4xqtdocn40b+zvH8fHx6KKLLoq++c1vRr/+9a+jn/3sZ9E555wTrVu3TvVxtJ9jwOJFMIiiKHrFK14RXXHFFWrfySefHF1zzTVHaESHDzt27IhEJLrrrruiKIqiRqMRDQ8PRzfddFPSplQqRQMDA9E//uM/HqlhHhQmJyejE088MdqwYUN0wQUXJAbRQjjHj370o9GrXvUq7+fz/Rxf//rXR3/8x3+s9r35zW+O3vWud0VRNP/Pb7ax0Mn5jI+PR7lcLrr99tuTNs8991yUTqejH/zgB3M29k7hMvpm4957741EJFlczrdzDFhcWPSSWaVSkY0bN8rFF1+s9l988cVy9913H6FRHT7s3btXRESGhoZERGTLli0yOjqqzrdQKMgFF1ww7873L//yL+X1r3+9XHTRRWr/QjjH7373u3L22WfLH/zBH8jy5cvlrLPOkltvvTX5fL6f46te9Sr57//+b3nsscdEROSXv/yl/PSnP5Xf/d3fFZH5f36z0cn5bNy4UarVqmozMjIip59++rw8Z5Hm/JNKpWRwcFBEFuY5BiwcLJhM1QeLXbt2Sb1elxUrVqj9K1askNHR0SM0qsODKIrk6quvlle96lVy+umni4gk5+Q636effnrOx3iwuP322+W+++6T//3f/235bCGc45NPPilf+tKX5Oqrr5a//uu/lnvvvVc+8IEPSKFQkMsuu2zen+NHP/pR2bt3r5x88smSyWSkXq/Lpz/9aXnHO94hIgvjHhKdnM/o6Kjk83k55phjWtrMx7moVCrJNddcI+985zuTAq8L7RwDFhYWvUFkkEql1N9RFLXsm2943/veJw888ID89Kc/bflsPp/v1q1b5corr5Qf/vCH+60EPZ/PsdFoyNlnny033HCDiIicddZZ8vDDD8uXvvQlueyyy5J28/Ucv/nNb8ptt90m3/jGN+S0006TTZs2yVVXXSUjIyNy+eWXJ+3m6/n5cDDnMx/PuVqtytvf/nZpNBryxS9+sW37+XiOAQsPi14yW7p0qWQymZbVyY4dO1pWc/MJ73//++W73/2u3HnnnXLccccl+4eHh0VE5vX5bty4UXbs2CHr1q2TbDYr2WxW7rrrLvn7v/97yWazyXnM53NcuXKlnHrqqWrfKaecIs8884yIzP/7+Fd/9VdyzTXXyNvf/nY544wzZP369fLBD35QbrzxRhGZ/+c3G52cz/DwsFQqFdmzZ4+3zXxAtVqVt771rbJlyxbZsGFDwg6JLJxzDFiYWPQGUT6fl3Xr1smGDRvU/g0bNsgrX/nKIzSqg0cURfK+971Pvv3tb8v//M//yNq1a9Xna9euleHhYXW+lUpF7rrrrnlzvq997WvlwQcflE2bNiX/zj77bPnDP/xD2bRpk5xwwgnz/hx/8zd/syVdwmOPPSZr1qwRkfl/H6enpyWd1tNPJpNJwu7n+/nNRifns27dOsnlcqrNtm3b5KGHHpo352yMoc2bN8sdd9whS5YsUZ8vhHMMWMA4Ut7cRxNM2P2Xv/zl6JFHHomuuuqqqKenJ3rqqaeO9NAOGH/xF38RDQwMRD/60Y+ibdu2Jf+mp6eTNjfddFM0MDAQffvb344efPDB6B3veMdRHc7cCRhlFkXz/xzvvffeKJvNRp/+9KejzZs3R1//+tej7u7u6LbbbkvazOdzvPzyy6Njjz02Cbv/9re/HS1dujT6yEc+krSZb+c3OTkZ3X///dH9998fiUj0uc99Lrr//vuTCKtOzueKK66IjjvuuOiOO+6I7rvvvug1r3nNURWSvr9zrFar0aWXXhodd9xx0aZNm9T8Uy6Xkz6O9nMMWLwIBlGML3zhC9GaNWuifD4fvexlL0vC1OcbRMT57ytf+UrSptFoRJ/4xCei4eHhqFAoRL/1W78VPfjgg0du0IcBsw2ihXCO3/ve96LTTz89KhQK0cknnxzdcsst6vP5fI4TExPRlVdeGa1evToqFovRCSecEF177bXqxTnfzu/OO+90/vYuv/zyKIo6O5+ZmZnofe97XzQ0NBR1dXVFb3jDG6JnnnnmCJyNG/s7xy1btnjnnzvvvDPp42g/x4DFi1QURdHc8VEBAQEBAQEBAUcfFr0PUUBAQEBAQEBAMIgCAgICAgICFj2CQRQQEBAQEBCw6BEMooCAgICAgIBFj2AQBQQEBAQEBCx6BIMoICAgICAgYNEjGEQBAQEBAQEBix7BIAoICAgICAhY9AgGUUBAQEBAQMCiRzCIAgICAgICAhY9gkEUELDIceGFF8oHPvAB+chHPiJDQ0MyPDws1113nYiI/OhHP5J8Pi8/+clPkvaf/exnZenSpbJt27YjNOKAgICAw49gEAUEBMjXvvY16enpkXvuuUc+85nPyKc+9SnZsGGDXHjhhXLVVVfJ+vXrZe/evfLLX/5Srr32Wrn11ltl5cqVR3rYAQEBAYcNobhrQMAix4UXXij1el2xQK94xSvkNa95jdx0001SqVTk3HPPlRNPPFEefvhhOe+88+TWW289giMOCAgIOPzIHukBBAQEHHm85CUvUX+vXLlSduzYISIi+XxebrvtNnnJS14ia9askZtvvvkIjDAgICDghUWQzAICAiSXy6m/U6mUNBqN5O+7775bRETGxsZkbGxsTscWEBAQMBcIBlFAQMB+8cQTT8gHP/hBufXWW+Xcc8+Vyy67TBlLAQEBAQsBwSAKCAjwol6vy/r16+Xiiy+Wd7/73fKVr3xFHnroIfnsZz97pIcWEBAQcFgRDKKAgAAvPv3pT8tTTz0lt9xyi4iIDA8Pyz//8z/Lxz/+cdm0adORHVxAQEDAYUSIMgsICAgICAhY9AgMUUBAQEBAQMCiRzCIAgICAgICAhY9gkEUEBAQEBAQsOgRDKKAgICAgICARY9gEAUEBAQEBAQsegSDKCAgICAgIGDRIxhEAQEBAQEBAYsewSAKCAgICAgIWPQIBlFAQEBAQEDAokcwiAICAgICAgIWPYJBFBAQEBAQELDoEQyigICAgICAgEWP/w/Gk89SmIu4WgAAAABJRU5ErkJggg==",
-                        "text/plain": [
-                            "<Figure size 640x480 with 2 Axes>"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "demos/premade_run_directories/jra_surface\n",
+                        "Number of CPUs required:  98\n"
+                    ]
                 }
             ],
             "source": [
-                "expt.topog.depth.plot()"
+                "expt.setup_run_directory(surface_forcing = \"jra\", using_payu = True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "##  Step 5: Handle the ocean forcing - where the magic happens\n",
-                "\n",
-                "This cuts out and interpolates the initial condition as well as all boundaries (unless you don't pass it boundaries).\n",
-                "\n",
-                "The dictionary maps the MOM6 variable names to what they're called in your ocean input file. Notice how for GLORYs, the horizontal dimensions are x and y, vs xh, yh, xq, yq for ACCESS OM2-01. This is because for an 'A' grid type tracers share the grid with velocities so there's no difference.\n",
+                "## Step 8: Run your model!\n",
                 "\n",
-                "If one of your segments is land, you can delete its string from the 'boundaries' list. You'll need to update MOM_input to reflect this though so it knows how many segments to look for, and their orientations. \n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "expt.ocean_forcing(\n",
-                "    tmpdir,  ## Path to ocean foring files\n",
-                "    {\"time\":\"time\",\n",
-                "     \"y\":\"latitude\",\n",
-                "     \"x\":\"longitude\",\n",
-                "     \"zl\":\"depth\",\n",
-                "     \"eta\":\"zos\",\n",
-                "     \"u\":\"uo\",\n",
-                "     \"v\":\"vo\",\n",
-                "     \"tracers\":{\"salt\":\"so\",\n",
-                "                \"temp\":\"thetao\"\n",
-                "                }\n",
-                "    },\n",
-                "    boundaries = [\"south\",\"north\",\"west\",\"east\"],\n",
-                "    gridtype=\"A\"\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Step 6 Run the FRE tools\n",
+                "To do this, navigate to your run directory in terminal. If you're working on NCI, you can do this via:\n",
                 "\n",
-                "This is just a wrapper for the FRE tools needed to make the mosaics and masks for the experiment. The only thing you need to tell it is the processor layout. In this case we're saying that we want a 10 by 10 grid of 100 processors. "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "expt.FRE_tools((10,10))\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Step 7: Modify the default input directory to make a (hopefully) runnable configuration out of the box\n",
+                "```\n",
+                "module load conda/analysis3\n",
+                "payu setup -f\n",
+                "payu run -f\n",
+                "```\n",
                 "\n",
-                "This cell just copies a default run directory and modifies it to match your configuration.\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "subprocess.run(f\"cp default_rundir/era5_surface/* {rundir} -r\",shell = True)\n",
-                "# subprocess.run(f\"cp default_rundir/era5_surface/* {rundir} -r\",shell = True)\n",
-                "subprocess.run(f\"ln -s {inputdir} {rundir}/inputdir\",shell=True)\n",
-                "\n",
-                "hgrid = xr.open_dataset(f\"{inputdir}/hgrid.nc\")\n",
-                "\n",
-                "## Get mask table information\n",
-                "ncpus = 10\n",
-                "mask_table = None\n",
-                "for i in os.listdir(f\"{inputdir}\"):\n",
-                "    if \"mask_table\" in i:\n",
-                "        mask_table = i\n",
-                "        a = mask_table.split(\".\")[1]\n",
-                "        b = mask_table.split(\".\")[2].split(\"x\")\n",
-                "        ncpus = int(b[0]) * int(b[1]) - int(a)\n",
-                "\n",
-                "\n",
-                "## Modify MOM_input\n",
-                "inputfile = open(f\"{rundir}/MOM_input\",'r')\n",
-                "lines = inputfile.readlines()\n",
-                "inputfile.close()\n",
-                "for i in range(len(lines)):\n",
-                "    if \"MASKTABLE\" in lines[i]:\n",
-                "        if mask_table != None:\n",
-                "            lines[i] = f'MASKTABLE = \"{mask_table}\"\\n'\n",
-                "        else:\n",
-                "            lines[i] = \"# MASKTABLE = no mask table\"\n",
-                "    if \"LAYOUT =\" in lines[i] and \"IO\" not in lines[i]:\n",
-                "        lines[i] = f'LAYOUT = {expt.layout[1]},{expt.layout[0]}\\n'\n",
-                "\n",
-                "    if \"NIGLOBAL\" in lines[i]: \n",
-                "        # lines[i] = f\"NIGLOBAL = {str(x_indices_centre[1] - x_indices_centre[0])}\\n\"\n",
-                "        lines[i] = f\"NIGLOBAL = {hgrid.nx.shape[0]//2}\\n\"\n",
-                "\n",
-                "        \n",
-                "    if \"NJGLOBAL\" in lines[i]:\n",
-                "        # lines[i] = f\"NJGLOBAL = {str(y_indices_centre[1] - y_indices_centre[0])}\\n\"\n",
-                "        lines[i] = f\"NJGLOBAL = {hgrid.ny.shape[0]//2}\\n\"\n",
-                "\n",
-                "        \n",
-                "inputfile = open(f\"{rundir}/MOM_input\",'w')\n",
-                "\n",
-                "inputfile.writelines(lines)\n",
-                "inputfile.close()\n",
-                "\n",
-                "## Modify SIS_input\n",
-                "inputfile = open(f\"{rundir}/SIS_input\",'r')\n",
-                "lines = inputfile.readlines()\n",
-                "inputfile.close()\n",
-                "for i in range(len(lines)):\n",
-                "    if \"MASKTABLE\" in lines[i]:\n",
-                "        lines[i] = f'MASKTABLE = \"{mask_table}\"\\n'\n",
-                "    if \"NIGLOBAL\" in lines[i]:\n",
-                "        # lines[i] = f\"NIGLOBAL = {str(x_indices_centre[1] - x_indices_centre[0])}\\n\"\n",
-                "        lines[i] = f\"NIGLOBAL = {hgrid.nx.shape[0]//2}\\n\"\n",
-                "    if \"LAYOUT =\" in lines[i] and \"IO\" not in lines[i]:\n",
-                "        lines[i] = f'LAYOUT = {expt.layout[1]},{expt.layout[0]}\\n'\n",
-                "    if \"NJGLOBAL\" in lines[i]:\n",
-                "        # lines[i] = f\"NJGLOBAL = {str(y_indices_centre[1] - y_indices_centre[0])}\\n\"\n",
-                "        lines[i] = f\"NJGLOBAL = {hgrid.ny.shape[0]//2}\\n\"\n",
-                "        \n",
-                "inputfile = open(f\"{rundir}/SIS_input\",'w')\n",
-                "inputfile.writelines(lines)\n",
-                "inputfile.close()\n",
-                "\n",
-                "## Modify config.yaml \n",
-                "inputfile = open(f\"{rundir}/config.yaml\",'r')\n",
-                "lines = inputfile.readlines()\n",
-                "inputfile.close()\n",
-                "for i in range(len(lines)):\n",
-                "    if \"ncpus\" in lines[i]:\n",
-                "        lines[i] = f'ncpus: {str(ncpus)}\\n'\n",
-                "    if \"jobname\" in lines[i]:\n",
-                "        lines[i] = f\"jobname: mom6_{expt_name}\\n\"\n",
-                "        \n",
-                "    if \"input:\" in lines[i]:\n",
-                "        lines[i + 1] = f\"    - {inputdir}\\n\"\n",
-                "\n",
-                "inputfile = open(f\"{rundir}/config.yaml\",'w')\n",
-                "inputfile.writelines(lines)\n",
-                "inputfile.close()\n",
-                "\n",
-                "\n",
-                "# Modify input.nml \n",
-                "inputfile = open(f\"{rundir}/input.nml\",'r')\n",
-                "lines = inputfile.readlines()\n",
-                "inputfile.close()\n",
-                "for i in range(len(lines)):\n",
-                "    if \"current_date\" in lines[i]:\n",
-                "        tmp = daterange[0].split(\" \")[0].split(\"-\")\n",
-                "        lines[i] = f\"{lines[i].split(' = ')[0]} = {int(tmp[0])},{int(tmp[1])},{int(tmp[2])},0,0,0,\\n\"\n",
-                "\n",
-                " \n",
-                "inputfile = open(f\"{rundir}/input.nml\",'w')\n",
-                "inputfile.writelines(lines)\n",
-                "inputfile.close()\n"
+                "By default `input.nml` is set to only run for 5 days as a test. If this is successful, you can modify this file to then run for longer."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### SET UP ERA5 forcing:\n",
-                "Here we assume you've already got ERA5 data stored somewhere on your system. For NCI users, you need access to the rt group. ERA5 - specific functions provided cut out the region of interest and fix up the metadata ready for MOM6.\n",
-                "\n",
-                "For this example, we are forcing for the entire year of 2015 so we just generate a single forcing file with 2015's data.\n",
-                "\n",
-                "Below is a table showing ERA5 characteristics and what needs to be done to sort it out\n",
-                "### Required ERA data:\n",
-                "Name | ERA filename | era variable name | notes\n",
-                "---|---|---|---\n",
-                "Surface Pressure | sp | sp | Pa :heavy_check_mark:\n",
-                "Surface Temperature | 2t | t2m | K :heavy_check_mark:\n",
-                "Meridional Wind | 10v | v10 | m/s :heavy_check_mark:\n",
-                "Zonal Wind | 10u | u10 | m/s :heavy_check_mark:\n",
-                "Specific Humidity | na | na | kg/kg, calculated from dewpoint temperature\n",
-                "Dewpoint Temperature | 2d | d2m | K\n",
-                "\n",
-                "\n",
-                "We can calculate specific humidity $q$ from dewpoint temperature $T_d$ and surface pressure $P$ via saturation vapour pressure $P_v$.\n",
-                "\n",
-                "$\\large P_v = 10^{8.07131 - \\frac{1730.63}{233.426 + T}} \\frac{101325}{760} $ Pascals\n",
-                "\n",
-                "$\\large q = 0.001 * 0.622  \\frac{P_v}{P}$ "
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "erapath = \"/g/data/rt52/era5/single-levels/reanalysis\"\n",
-                "\n",
-                "## Firstly just open all raw data\n",
-                "rawdata = {}\n",
-                "for fname , vname in zip([\"2t\",\"10u\",\"10v\",\"sp\",\"2d\"] , [\"t2m\",\"u10\",\"v10\",\"sp\",\"d2m\"]):\n",
-                "\n",
-                "    ## Cut out this variable to our domain size\n",
-                "    rawdata[fname] = rm.nicer_slicer(\n",
-                "        xr.open_mfdataset(f\"{erapath}/{fname}/{daterange[0].split('-')[0]}/{fname}*\",decode_times = False,chunks = {\"longitude\":100,\"latitude\":100}),\n",
-                "        xextent,\n",
-                "        \"longitude\"\n",
-                "    ).sel(\n",
-                "        latitude = slice(yextent[1],yextent[0]) ## This is because ERA5 has latitude in decreasing order (??)\n",
-                "    )\n",
-                "\n",
-                "    ## Now fix up the latitude and time dimensions\n",
-                "\n",
-                "    rawdata[fname] = rawdata[fname].isel(\n",
-                "        latitude = slice(None,None,-1) ## Flip latitude        \n",
-                "        ).assign_coords(\n",
-                "        time = np.arange(0,rawdata[fname].time.shape[0],dtype=float) ## Set the zero date of forcing to start of run\n",
-                "        )\n",
-                "    \n",
-                "\n",
-                "    \n",
-                "\n",
-                "    rawdata[fname].time.attrs = {\"calendar\":\"julian\",\"units\":f\"hours since {daterange[0]}\"} ## Fix up calendar to match\n",
-                "\n",
-                "    if fname == \"2d\":\n",
-                "        ## Calculate specific humidity from dewpoint temperature \n",
-                "        q = xr.Dataset(\n",
-                "            data_vars= {\n",
-                "                \"q\": (0.622 / rawdata[\"sp\"][\"sp\"]) * (10**(8.07131 - 1730.63 / (233.426 + rawdata[\"2d\"][\"d2m\"] - 273.15) )) * 101325 / 760\n",
-                "                }\n",
-                "\n",
-                "        )\n",
-                "        q.q.attrs = {\"long_name\":\"Specific Humidity\",\"units\": \"kg/kg\"}\n",
-                "        q.to_netcdf(f\"{inputdir}/forcing/q_ERA5\",unlimited_dims = \"time\",encoding = {\"q\":{\"dtype\":\"double\"}})\n",
-                "    else:\n",
-                "        rawdata[fname].to_netcdf(f\"{inputdir}/forcing/{fname}_ERA5\",unlimited_dims = \"time\",encoding = {vname:{\"dtype\":\"double\"}})\n",
-                "\n",
+                "## Step 9 and beyond: Fiddling, troubleshooting and fine tuning\n",
                 "\n",
-                "## Update the data table to match:\n",
+                "Hopefully your model is running. If not, the first thing you should do is reduce the timestep. You can do this by adding `#override DT=XXXX` to your `MOM_override` file. \n",
                 "\n",
-                "subprocess.run(f\"cp default_rundir/era5_surface/data_table {rundir}/data_table\",shell = True)"
+                "If there's strange behaviour on your boundaries, you could play around with the `nudging timescale` (an example is already included in the `MOM_override` file). Sometimes, if your boundary has a lot going on (like all of the eddies spinning off the ACC), it can be hard to avoid these edge effects. This is because the chaotic, submesoscale structures developed within the regional domain won't match those at the boundary. "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python [conda env:analysis3-23.04] *",
+            "display_name": "Python [conda env:analysis3-24.01]",
             "language": "python",
-            "name": "conda-env-analysis3-23.04-py"
+            "name": "conda-env-analysis3-24.01-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.17"
+            "version": "3.10.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `regional_mom6-0.2.1/docs/Makefile` & `regional_mom6-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.2.1/docs/conf.py` & `regional_mom6-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.2.1/docs/contributing.md` & `regional_mom6-0.5.0/docs/contributing.md`

 * *Files 13% similar despite different names*

```diff
@@ -26,20 +26,27 @@
 Now we need to install the package in this environment as well as `pytest`
 
 ```{code-block} bash
 python -m pip install .
 python -m pip install pytest
 ```
 
-Now we can run the test with
+Now we can run the tests with
 
 ```{code-block} bash
 python -m pytest tests/
 ```
 
+If we also want to run the doctests (tests that appear as examples in various docstrings), we
+can use
+
+```{code-block} bash
+python -m pytest --doctest-modules tests/ regional_mom6/
+```
+
 ## Documentation
 
 To build the docs from a local clone of the repository we first need to create a conda
 environment. Navigate to the `docs` directory of your local repository clone (e.g., `cd docs`)
 and then 
 
 ```{code-block} bash
```

### Comparing `regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/SIS_input` & `regional_mom6-0.5.0/demos/premade_run_directories/common_files/SIS_input`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,19 @@
 ! cosine of solar zenith angle for first radiation step
 CONSTANT_COSZEN_IC = 0.0
 ! don't call iceberg module
 DO_ICEBERGS = False
 ! time between writes of global ice diags and conservation
 ICE_STATS_INTERVAL = 0.25
 
-NIGLOBAL = 80
-NJGLOBAL = 129
-LAYOUT = 10,10
-MASKTABLE = "mask_table.18.10x10"
-
 GRID_CONFIG = "mosaic"
 GRID_FILE = "hgrid.nc"
 INPUTDIR = "INPUT"
 
-TOPO_FILE = "topog.nc"
+TOPO_FILE = "bathymetry.nc"
 
 MAXIMUM_DEPTH = 6000.0
 
 WRITE_GEOM = 0
 
 ! rotation rate of earth
 OMEGA = 7.292E-05
```

### Comparing `regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/data_table` & `regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/data_table`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-"ATM", "p_surf", "sp", "./INPUT/forcing/sp_ERA5", "bilinear", 1.0
-"ATM", "p_bot",  "sp", "./INPUT/forcing/sp_ERA5", "bilinear", 1.0
-"ATM", "t_bot",  "t2m", "./INPUT/forcing/2t_ERA5", "bilinear", 1.0
-"ATM", "sphum_bot", "q", "./INPUT/forcing/q_ERA5", "bilinear", 1.0
-"ATM", "u_bot", "u10", "./INPUT/forcing/10u_ERA5", "bicubic", 1.0
-"ATM", "v_bot", "v10", "./INPUT/forcing/10v_ERA5", "bicubic", 1.0
+"ATM", "p_surf", "sp", "./INPUT/forcing/sp_ERA5.nc", "bilinear", 1.0
+"ATM", "p_bot",  "sp", "./INPUT/forcing/sp_ERA5.nc", "bilinear", 1.0
+"ATM", "t_bot",  "t2m", "./INPUT/forcing/2t_ERA5.nc", "bilinear", 1.0
+"ATM", "sphum_bot", "q", "./INPUT/forcing/q_ERA5.nc", "bilinear", 1.0
+"ATM", "u_bot", "u10", "./INPUT/forcing/10u_ERA5.nc", "bicubic", 1.0
+"ATM", "v_bot", "v10", "./INPUT/forcing/10v_ERA5.nc", "bicubic", 1.0
 "ATM", "z_bot", "", "", "bilinear", 10.0
 "ATM", "gust", "", "", "bilinear", 1.0e-4
-"ICE", "lw_flux_dn", "rlds", "./INPUT/RYF.rlds.1990_1991.nc", "bilinear", 1.0
-"ICE", "sw_flux_vis_dir_dn", "rsds", "./INPUT/RYF.rsds.1990_1991.nc", "bilinear", 0.285
-"ICE", "sw_flux_vis_dif_dn", "rsds", "./INPUT/RYF.rsds.1990_1991.nc", "bilinear", 0.285
-"ICE", "sw_flux_nir_dir_dn", "rsds", "./INPUT/RYF.rsds.1990_1991.nc", "bilinear", 0.215
-"ICE", "sw_flux_nir_dif_dn", "rsds", "./INPUT/RYF.rsds.1990_1991.nc", "bilinear", 0.215
-"ICE", "lprec", "prrn", "./INPUT/RYF.rain.1990_1991.nc", "bilinear", 1.0
-"ICE", "fprec", "prsn", "./INPUT/RYF.snow.1990_1991.nc", "bilinear", 1.0
+"ICE", "lw_flux_dn", "", "", "bilinear", 1.0
+"ICE", "sw_flux_vis_dir_dn", "msdwswrf", "./INPUT/forcing/msdwswrf_ERA5.nc", "bilinear", 0.285
+"ICE", "sw_flux_vis_dif_dn", "msdwswrf", "./INPUT/forcing/msdwswrf_ERA5.nc", "bilinear", 0.285
+"ICE", "sw_flux_nir_dir_dn", "msdwlwrf", "./INPUT/forcing/msdwlwrf_ERA5.nc", "bilinear", 0.215
+"ICE", "sw_flux_nir_dif_dn", "msdwlwrf", "./INPUT/forcing/msdwlwrf_ERA5.nc", "bilinear", 0.215
+"ICE", "lprec", "trr", "./INPUT/forcing/trr_ERA5.nc", "bilinear", 1.0
+"ICE", "fprec", "", "", "bilinear", 0.0
 "ICE", "runoff", "", "", "none", 0.0
 "ICE", "dhdt", "", "", "none", 80.0
 "ICE", "dedt", "", "", "none", 2.0e-6
 "ICE", "drdt", "", "", "none", 10.0
 "LND", "rough_mom", "", "", "none", 0.01
-"LND", "rough_heat", "", "", "none", 0.1"""
+"LND", "rough_heat", "", "", "none", 0.1
+
```

### Comparing `regional_mom6-0.2.1/regional_mom6/default_rundir/era5_surface/input.nml` & `regional_mom6-0.5.0/demos/premade_run_directories/era5_surface/input.nml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 &MOM_input_nml
 	output_directory = '.',
 	input_filename = 'n',
 	restart_input_dir = 'INPUT',
 	restart_output_dir = 'RESTART',
-	parameter_filename = 'MOM_input', 'MOM_override'
+	parameter_filename = 'MOM_input', 'MOM_layout', 'MOM_override'
 /
 
 &SIS_input_nml
 	output_directory = '.',
 	input_filename = 'n',
 	restart_input_dir = 'INPUT',
 	restart_output_dir = 'RESTART',
-	parameter_filename = 'SIS_input'
+	parameter_filename = 'SIS_input','MOM_layout'
 /
 
 &fms_nml
 	domains_stack_size = 1600000,
 	stack_size = 0,
 	clock_grain = 'LOOP'
 /
@@ -24,18 +24,18 @@
         netcdf_default_format = "netcdf4"
 	shuffle = .true.,
 	deflate = 5
 /
 
 &coupler_nml
 	months = 0,
-	days = 5,
+	days = 1,
 	hours = 0,
-	current_date = 1991,1,1,0,0,0,
-	calendar = 'NOLEAP',
+	current_date = 2015,1,1,0,0,0,
+	calendar = 'JULIAN',
 	dt_cpld = 3600,
 	dt_atmos = 3600,
 	do_atmos = .false.,
 	do_land = .false.,
 	do_ice = .true.,
 	do_ocean = .true.,
 	do_flux = .true.,
@@ -69,15 +69,16 @@
 
 &sat_vapor_pres_nml
 	construct_table_wrt_liq = .true.,
 	construct_table_wrt_liq_and_ice = .true.
 /
 
 &surface_flux_nml
-	ncar_ocean_flux = .true.,
-	raoult_sat_vap = .true.
-/
+    ncar_ocean_flux_multilevel = .true.
+    bulk_zu = 10.
+    bulk_zt = 2.
+    bulk_zq = 2.
 
 &xgrid_nml
 	make_exchange_reproduce = .false.,
 	interp_method = 'second_order'
 /
```

### Comparing `regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/data_table` & `regional_mom6-0.5.0/demos/premade_run_directories/jra_surface/data_table`

 * *Files identical despite different names*

### Comparing `regional_mom6-0.2.1/regional_mom6/default_rundir/jra_surface/input.nml` & `regional_mom6-0.5.0/demos/premade_run_directories/common_files/input.nml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 &MOM_input_nml
 	output_directory = '.',
 	input_filename = 'n',
 	restart_input_dir = 'INPUT',
 	restart_output_dir = 'RESTART',
-	parameter_filename = 'MOM_input', 'MOM_override'
+	parameter_filename = 'MOM_input', 'MOM_layout', 'MOM_override'
 /
 
 &SIS_input_nml
 	output_directory = '.',
 	input_filename = 'n',
 	restart_input_dir = 'INPUT',
 	restart_output_dir = 'RESTART',
-	parameter_filename = 'SIS_input'
+	parameter_filename = 'SIS_input','MOM_layout'
 /
 
 &fms_nml
 	domains_stack_size = 1600000,
 	stack_size = 0,
 	clock_grain = 'LOOP'
 /
@@ -24,18 +24,18 @@
         netcdf_default_format = "netcdf4"
 	shuffle = .true.,
 	deflate = 5
 /
 
 &coupler_nml
 	months = 0,
-	days = 5,
+	days = 1,
 	hours = 0,
-	current_date = 1991,1,1,0,0,0,
-	calendar = 'NOLEAP',
+	current_date = 2015,1,1,0,0,0,
+	calendar = 'JULIAN',
 	dt_cpld = 3600,
 	dt_atmos = 3600,
 	do_atmos = .false.,
 	do_land = .false.,
 	do_ice = .true.,
 	do_ocean = .true.,
 	do_flux = .true.,
```

### Comparing `regional_mom6-0.2.1/regional_mom6/regional_mom6.py` & `regional_mom6-0.5.0/regional_mom6/regional_mom6.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,382 +1,303 @@
 import numpy as np
-from itertools import cycle
 from pathlib import Path
 import dask.array as da
-import dask.bag as db
-import numpy as np
 import xarray as xr
 import xesmf as xe
 import subprocess
 from scipy.ndimage import binary_fill_holes
 import netCDF4
-from dask.distributed import Client, worker_client
 from dask.diagnostics import ProgressBar
+import f90nml
 import datetime as dt
 import warnings
-from .utils import vecdot
+import shutil
+import os
+import importlib.resources
+
+from .utils import quadrilateral_areas
+
 
 warnings.filterwarnings("ignore")
 
 __all__ = [
-    "nicer_slicer",
-    "motu_requests",
-    "dz",
-    "angle_between",
-    "latlon_to_cartesian",
-    "quadrilateral_area",
-    "quadrilateral_areas",
+    "longitude_slicer",
+    "hyperbolictan_thickness_profile",
     "rectangular_hgrid",
     "experiment",
     "segment",
 ]
 
 
-def nicer_slicer(data, xextent, xcoords, buffer=2):
-    """Slices longitudes, handling periodicity and 'seams' where the
-    data wraps around (commonly either at -180 -> 180 or -270 -> 90)
+## Auxiliary functions
+
+
+def longitude_slicer(data, longitude_extent, longitude_coords):
+    """
+    Slice longitudes, handling periodicity and 'seams' where the
+    data wraps around (commonly either in domain [0, 360], [-180, 180], or [-270, 90]).
 
     The algorithm works in five steps:
 
-    - Determine whether we need to add or subtract 360 to get the
-      middle of the xextent to lie within data's lonitude range
-      (hereby oldx)
+    - Determine whether we need to add or subtract 360 to get the middle of the
+      ``longitude_extent`` to lie within ``data``'s longitude range (hereby ``old_lon``).
 
     - Shift the dataset so that its midpoint matches the midpoint of
-      xextent (up to a muptiple of 360). Now, the modified oldx
-      doesn't increase monotonically W to E since the 'seam' has
-      moved.
-
-    - Fix oldx to make it monotonically increasing again. This uses
-      the information we have about the way the dataset was
-      shifted/rolled
+      ``longitude_extent`` (up to a multiple of 360). Now, the modified ``old_lon``
+      does not increase monotonically from West to East since the 'seam'
+      has moved.
+
+    - Fix ``old_lon`` to make it monotonically increasing again. This uses
+      the information we have about the way the dataset was shifted/rolled.
 
-    - Slice the data index-wise. We know that ``|xextent| / 360``
+    - Slice the ``data`` index-wise. We know that ``|longitude_extent[1] - longitude_extent[0]| / 360``
       multiplied by the number of discrete longitude points will give
       the total width of our slice, and we've already set the midpoint
-      to be the middle of the target domain. Here we add a buffer
-      region on either side if we need it for interpolation.
+      to be the middle of the target domain.
 
-    - Finally re-add the right multiple of 360 so the whole domain matches the target.
+    - Finally re-add the right multiple of 360 so the whole domain matches
+      the target.
 
     Args:
-        data (xarray.Dataset): The global data you want to slice in longitude
-        xextent (Tuple[float, float]): The target longitudes you want to slice
-            to. This must be either start negative and progress to
-            positive, or be entirely positive
-        xcoords (Union[str, List[str]): The name of the longitude
-            dimension in your xarray or list of names
-
+        data (xarray.Dataset): The global data you want to slice in longitude.
+        longitude_extent (Tuple[float, float]): The target longitudes (in degrees)
+            we want to slice to. Must be in increasing order.
+        longitude_coords (Union[str, list[str]): The name or list of names of the
+            longitude coordinates(s) in ``data``.
     Returns:
-        xarray.Dataset: The data after the slicing has been performed.
-
+        xarray.Dataset: The sliced ``data``.
     """
 
-    if isinstance(xcoords, str):
-        xcoords = [xcoords]
+    if isinstance(longitude_coords, str):
+        longitude_coords = [longitude_coords]
 
-    for x in xcoords:
-        mp_target = np.mean(xextent)  ## Midpoint of target domain
+    for lon in longitude_coords:
+        central_longitude = np.mean(longitude_extent)  ## Midpoint of target domain
+
+        ## Find a corresponding value for the intended domain midpoint in our data.
+        ## It's assumed that data has equally-spaced longitude values.
+
+        λ = data[lon].data
+        dλ = λ[1] - λ[0]
+
+        assert np.allclose(
+            np.diff(λ), dλ * np.ones(np.size(λ) - 1)
+        ), "provided longitude coordinate must be uniformly spaced"
 
-        ## Find a corresponding value for the intended domain midpint in our data. Assuming here that data has equally spaced longitude values spanning 360deg
         for i in range(-1, 2, 1):
-            if data[x][0] <= mp_target + 360 * i <= data[x][-1]:
-                _mp_target = (
-                    mp_target + 360 * i
-                )  ## Shifted version of target midpoint. eg, could be -90 vs 270. i keeps track of what multiple of 360 we need to shift entire grid by to match midpoint
+            if data[lon][0] <= central_longitude + 360 * i <= data[lon][-1]:
 
-                mp_data = data[x][data[x].shape[0] // 2].values  ## Midpoint of the data
+                ## Shifted version of target midpoint; e.g., could be -90 vs 270
+                ## integer i keeps track of what how many multiples of 360 we need to shift entire
+                ## grid by to match central_longitude
+                _central_longitude = central_longitude + 360 * i
 
-                shift = -1 * (data[x].shape[0] * (_mp_target - mp_data)) // 360
+                ## Midpoint of the data
+                central_data = data[lon][data[lon].shape[0] // 2].values
+
+                ## Number of indices between the data midpoint and the target midpoint.
+                ## Sign indicates direction needed to shift.
                 shift = int(
-                    shift
-                )  ## This is the number of indices between the data midpoint, and the target midpoint. Sign indicates direction needed to shift
+                    -(data[lon].shape[0] * (_central_longitude - central_data)) // 360
+                )
 
-                new_data = data.roll(
-                    {x: 1 * shift}, roll_coords=True
-                )  ## Shifts data so that the midpoint of the target domain is the middle of the data for easy slicing
-
-                new_x = new_data[
-                    x
-                ].values  ## Create a new longitude coordinate. We'll modify this to remove any seams (jumps like -270 -> 90)
+                ## Shift data so that the midpoint of the target domain is the middle of
+                ## the data for easy slicing.
+                new_data = data.roll({lon: 1 * shift}, roll_coords=True)
+
+                ## Create a new longitude coordinate.
+                ## We'll modify this to remove any seams (i.e., jumps like -270 -> 90)
+                new_lon = new_data[lon].values
 
-                ## Take the 'seam' of the data, and either backfill or forward fill based on whether the data was shifted F or west
+                ## Take the 'seam' of the data, and either backfill or forward fill based on
+                ## whether the data was shifted F or west
                 if shift > 0:
                     new_seam_index = shift
 
-                    new_x[0:new_seam_index] -= 360
+                    new_lon[0:new_seam_index] -= 360
 
                 if shift < 0:
-                    new_seam_index = data[x].shape[0] + shift
+                    new_seam_index = data[lon].shape[0] + shift
 
-                    new_x[new_seam_index:] += 360
+                    new_lon[new_seam_index:] += 360
 
-                new_x -= (
-                    i * 360
-                )  ## Use this to recentre the midpoint to match that of target domain
+                ## new_x is used to recentre the midpoint to match that of target domain
+                new_lon -= i * 360
 
-                new_data = new_data.assign_coords({x: new_x})
+                new_data = new_data.assign_coords({lon: new_lon})
 
-                ## Choose the number of x points to take from the middle, including a buffer. Use this to index the new global dataset
-
-                num_xpoints = (
-                    int(data[x].shape[0] * (mp_target - xextent[0])) // 360 + buffer * 2
+                ## Choose the number of lon points to take from the middle, including a buffer.
+                ## Use this to index the new global dataset
+                num_lonpoints = (
+                    int(data[lon].shape[0] * (central_longitude - longitude_extent[0]))
+                    // 360
                 )
 
         data = new_data.isel(
             {
-                x: slice(
-                    data[x].shape[0] // 2 - num_xpoints,
-                    data[x].shape[0] // 2 + num_xpoints,
+                lon: slice(
+                    data[lon].shape[0] // 2 - num_lonpoints,
+                    data[lon].shape[0] // 2 + num_lonpoints,
                 )
             }
         )
 
     return data
 
 
-def motu_requests(
-    xextent,
-    yextent,
-    daterange,
-    outfolder,
-    usr,
-    pwd,
-    segs,
-    url="https://my.cmems-du.eu/motu-web/Motu",
-    serviceid="GLOBAL_MULTIYEAR_PHY_001_030-TDS",
-    productid="cmems_mod_glo_phy_my_0.083_P1D-m",
-    buffer=0.3,
-):
-    """Generates MOTU data request for each specified boundary, as
-    well as for the initial condition. By default pulls the GLORYS
-    reanalysis dataset.
+def hyperbolictan_thickness_profile(nlayers, ratio, total_depth):
+    """Generate a hyperbolic tangent thickness profile with ``nlayers`` vertical
+    layers and total depth of ``total_depth`` whose bottom layer is (about) ``ratio``
+    times larger than the top layer.
+
+    The thickness profile transitions from the top-layer thickness to
+    the bottom-layer thickness via a hyperbolic tangent proportional to
+    ``tanh(2π * (k / (nlayers - 1) - 1 / 2))``, where ``k = 0, 1, ..., nlayers - 1``
+    is the layer index with ``k = 0`` corresponding to the top-most layer.
+
+    The sum of all layer thicknesses is ``total_depth``.
+
+    Positive parameter ``ratio`` prescribes (approximately) the ratio of the thickness
+    of the bottom-most layer to the top-most layer. The final ratio of the bottom-most
+    layer to the top-most layer ends up a bit different from the prescribed ``ratio``.
+    In particular, the final ratio of the bottom over the top-most layer thickness is
+    ``(1 + ratio * exp(2π)) / (ratio + exp(2π))``. This slight departure comes about
+    because of the value of the hyperbolic tangent profile at the end-points ``tanh(π)``,
+    which is approximately 0.9963 and not 1. Note that because ``exp(2π)`` is much greater
+    than 1, the value of the actual ratio is not that different from prescribed value
+    ``ratio``, e.g., for ``ratio`` values between 1/100 and 100 the final ratio of the
+    bottom-most layer to the top-most layer only departs from the prescribed ``ratio``
+    by ±20%.
 
     Args:
-        xextent (List[float]): Extreme values of longitude coordinates for rectangular domain
-        yextent (List[float]): Extreme values of latitude coordinates for rectangular domain
-        daterange (Tuple[str]): Start and end dates of boundary forcing window. Format: ``%Y-%m-%d %H:%M:%S``
-        outfolder (str): Directory in which to receive the downloaded files
-        usr (str): MOTU authentication username
-        pwd (str): MOTU authentication password
-        segs (List[str]): List of the cardinal directions for your boundary forcing
-        url (Optional[str]): MOTU server for the request (defaults to CMEMS)
-        serviceid (Optional[str]): Service containing the desired dataset
-        productid (Optional[str]): Data product within the chosen service.
+        nlayers (int): Number of vertical layers.
+        ratio (float): The desired value of the ratio of bottom-most to
+            the top-most layer thickness. Note that the final value of
+            the ratio of bottom-most to the top-most layer thickness
+            ends up ``(1 + ratio * exp(2π)) / (ratio + exp(2π))``. Must
+            be positive.
+        total_depth (float): The total depth of grid, i.e., the sum
+            of all thicknesses.
 
     Returns:
-        str: A bash script which will call ``motuclient`` to invoke the data requests.
-
-    """
+        numpy.array: An array containing the layer thicknesses.
 
-    if type(segs) == str:
-        return f"\nprintf 'processing {segs} segment' \npython -m motuclient --motu {url} --service-id {serviceid} --product-id {productid} --longitude-min {xextent[0]} --longitude-max {xextent[1]} --latitude-min {yextent[0]} --latitude-max {yextent[1]} --date-min {daterange[0]} --date-max {daterange[1]} --depth-min 0.49 --depth-max 6000 --variable so --variable thetao --variable vo --variable zos --variable uo --out-dir {outfolder} --out-name {segs}_unprocessed --user '{usr}' --pwd '{pwd}'\n"
+    Examples:
 
-    ## Buffer pads out our boundaries a small amount to allow for interpolation
-    xextent, yextent = np.array(xextent), np.array(yextent)
-    script = "#!/bin/bash\n\n"
-    for seg in segs:
-        if seg == "east":
-            script += motu_requests(
-                [xextent[1] - buffer, xextent[1] + buffer],
-                yextent,
-                daterange,
-                outfolder,
-                usr,
-                pwd,
-                seg,
-                url=url,
-                serviceid=serviceid,
-                productid=productid,
-            )
-        if seg == "west":
-            script += motu_requests(
-                [xextent[0] - buffer, xextent[0] + buffer],
-                yextent,
-                daterange,
-                outfolder,
-                usr,
-                pwd,
-                seg,
-                url=url,
-                serviceid=serviceid,
-                productid=productid,
-            )
-        if seg == "north":
-            script += motu_requests(
-                xextent,
-                [yextent[1] - buffer, yextent[1] + buffer],
-                daterange,
-                outfolder,
-                usr,
-                pwd,
-                seg,
-                url=url,
-                serviceid=serviceid,
-                productid=productid,
-            )
-
-        if seg == "south":
-            script += motu_requests(
-                xextent,
-                [yextent[0] - buffer, yextent[0] + buffer],
-                daterange,
-                outfolder,
-                usr,
-                pwd,
-                seg,
-                url=url,
-                serviceid=serviceid,
-                productid=productid,
-            )
-    ## Now handle the initial condition
-    script += motu_requests(
-        xextent + np.array([-1 * buffer, buffer]),
-        yextent + np.array([-1 * buffer, buffer]),
-        [
-            daterange[0],
-            dt.datetime.strptime(daterange[0], "%Y-%m-%d %H:%M:%S")
-            + dt.timedelta(hours=1),
-        ],  ## For initial condition just take one day
-        outfolder,
-        usr,
-        pwd,
-        "ic",
-        url=url,
-        serviceid=serviceid,
-        productid=productid,
-    )
-    return script
-
-
-def dz(npoints, ratio, target_depth, min_dz=0.0001, tolerance=1):
-    """Generate a hyperbolic tangent thickness profile for the
-    experiment.  Iterates to find the mininum depth value which gives
-    the target depth within some tolerance
-
-    Args:
-        npoints (int): Number of vertical points
-        ratio (float): Ratio of largest to smallest layer
-            thickness. Negative values mean higher resolution is at
-            bottom rather than top of the column.
-        target_depth (float): Maximum depth of a layer
-        min_dz (float): Starting layer thickness for iteration
-        tolerance (float): Tolerance to the target depth.
-
-    Returns:
-        numpy.array: An array containing the thickness profile.
+        The spacings for a vertical grid with 20 layers, with maximum depth 1000 meters,
+        and for which the top-most layer is about 4 times thinner than the bottom-most
+        one.
+
+        >>> from regional_mom6 import hyperbolictan_thickness_profile
+        >>> nlayers, total_depth = 20, 1000
+        >>> ratio = 4
+        >>> dz = hyperbolictan_thickness_profile(nlayers, ratio, total_depth)
+        >>> dz
+        array([20.11183771, 20.2163053 , 20.41767549, 20.80399084, 21.53839043,
+               22.91063751, 25.3939941 , 29.6384327 , 36.23006369, 45.08430684,
+               54.91569316, 63.76993631, 70.3615673 , 74.6060059 , 77.08936249,
+               78.46160957, 79.19600916, 79.58232451, 79.7836947 , 79.88816229])
+        >>> dz.sum()
+        1000.0
+        >>> dz[-1] / dz[0]
+        3.9721960481753706
+
+        If we want the top layer to be thicker then we need to prescribe ``ratio < 1``.
+
+        >>> from regional_mom6 import hyperbolictan_thickness_profile
+        >>> nlayers, total_depth = 20, 1000
+        >>> ratio = 1/4
+        >>> dz = hyperbolictan_thickness_profile(nlayers, ratio, total_depth)
+        >>> dz
+        array([79.88816229, 79.7836947 , 79.58232451, 79.19600916, 78.46160957,
+               77.08936249, 74.6060059 , 70.3615673 , 63.76993631, 54.91569316,
+               45.08430684, 36.23006369, 29.6384327 , 25.3939941 , 22.91063751,
+               21.53839043, 20.80399084, 20.41767549, 20.2163053 , 20.11183771])
+        >>> dz.sum()
+        1000.0
+        >>> dz[-1] / dz[0]
+        0.25174991059652
+
+        Now how about a grid with the same total depth as above but with equally-spaced
+        layers.
+
+        >>> from regional_mom6 import hyperbolictan_thickness_profile
+        >>> nlayers, total_depth = 20, 1000
+        >>> ratio = 1
+        >>> dz = hyperbolictan_thickness_profile(nlayers, ratio, total_depth)
+        >>> dz
+        array([50., 50., 50., 50., 50., 50., 50., 50., 50., 50., 50., 50., 50.,
+               50., 50., 50., 50., 50., 50., 50.])
     """
 
-    profile = min_dz + 0.5 * (np.abs(ratio) * min_dz - min_dz) * (
-        1 + np.tanh(2 * np.pi * (np.arange(npoints) - npoints // 2) / npoints)
-    )
-    tot = np.sum(profile)
-    if np.abs(tot - target_depth) < tolerance:
-        if ratio > 0:
-            return profile
-
-        return profile[::-1]
+    assert isinstance(nlayers, int), "nlayers must be an integer"
 
-    err_ratio = target_depth / tot
+    if nlayers == 1:
+        return np.array([float(total_depth)])
 
-    return dz(npoints, ratio, target_depth, min_dz * err_ratio)
+    assert ratio > 0, "ratio must be > 0"
 
+    # The hyberbolic tangent profile below implies that the sum of
+    # all layer thicknesses is:
+    #
+    # nlayers * (top_layer_thickness + bottom_layer_thickness) / 2
+    #
+    # By choosing the top_layer_thickness appropriately we ensure that
+    # the sum of all layer thicknesses is the prescribed total_depth.
+    top_layer_thickness = 2 * total_depth / (nlayers * (1 + ratio))
 
-def angle_between(v1, v2, v3):
-    """Returns the angle v2-v1-v3 (in radians). That is the angle between vectors v1-v2 and v1-v3."""
-
-    v1xv2 = np.cross(v1, v2)
-    v1xv3 = np.cross(v1, v3)
-
-    cosangle = vecdot(v1xv2, v1xv3) / np.sqrt(
-        vecdot(v1xv2, v1xv2) * vecdot(v1xv3, v1xv3)
-    )
-
-    return np.arccos(cosangle)
-
-
-def quadrilateral_area(v1, v2, v3, v4):
-    """Returns area of a spherical quadrilateral on the unit sphere that
-    has vertices on 3-vectors `v1`, `v2`, `v3`, `v4` (counter-clockwise
-    orientation is implied). The area is computed via the excess of the
-    sum of the spherical angles of the quadrilateral from 2π."""
-
-    if not (
-        np.all(np.isclose(vecdot(v1, v1), vecdot(v2, v2)))
-        & np.all(np.isclose(vecdot(v1, v1), vecdot(v2, v2)))
-        & np.all(np.isclose(vecdot(v1, v1), vecdot(v3, v3)))
-        & np.all(np.isclose(vecdot(v1, v1), vecdot(v4, v4)))
-    ):
-        raise ValueError("vectors provided must have the same length")
-
-    R = np.sqrt(vecdot(v1, v1))
+    bottom_layer_thickness = ratio * top_layer_thickness
 
-    a1 = angle_between(v1, v2, v4)
-    a2 = angle_between(v2, v3, v1)
-    a3 = angle_between(v3, v4, v2)
-    a4 = angle_between(v4, v1, v3)
+    layer_thicknesses = top_layer_thickness + 0.5 * (
+        bottom_layer_thickness - top_layer_thickness
+    ) * (1 + np.tanh(2 * np.pi * (np.arange(nlayers) / (nlayers - 1) - 1 / 2)))
 
-    return (a1 + a2 + a3 + a4 - 2 * np.pi) * R**2
+    sum_of_thicknesses = np.sum(layer_thicknesses)
 
+    atol = np.finfo(type(sum_of_thicknesses)).eps
 
-def latlon_to_cartesian(lat, lon, R=1):
-    """Convert latitude-longitude (in degrees) to Cartesian coordinates on a sphere of radius `R`.
-    By default `R = 1`."""
+    assert np.isclose(total_depth, sum_of_thicknesses, atol=atol)  # just checking ;)
 
-    x = R * np.cos(np.deg2rad(lat)) * np.cos(np.deg2rad(lon))
-    y = R * np.cos(np.deg2rad(lat)) * np.sin(np.deg2rad(lon))
-    z = R * np.sin(np.deg2rad(lat))
-
-    return x, y, z
-
-
-def quadrilateral_areas(lat, lon, R=1):
-    """Returns area of spherical quadrilaterals on a sphere of radius `R`. By default, `R = 1`.
-    The quadrilaterals are formed by constant latitude and longitude lines on the `lat`-`lon` grid provided.
-
-    Args:
-        lat (array): Array of latitude points (in degrees)
-        lon (array): Array of longitude points (in degrees)
-
-    Returns:
-        areas (array): Array with the areas of the quadrilaterals defined by the
-                       `lat`-`lon` grid provided. If the `lat`-`lon` are `m x n`
-                       then `areas` is `(m-1) x (n-1)`.
-    """
-
-    coords = np.dstack(latlon_to_cartesian(lat, lon, R))
-
-    return quadrilateral_area(
-        coords[:-1, :-1, :], coords[:-1, 1:, :], coords[1:, 1:, :], coords[1:, :-1, :]
-    )
+    return layer_thicknesses
 
 
 def rectangular_hgrid(λ, φ):
     """
-    Construct a horizontal grid with all the metadata given an array of
-    latitudes (`φ`) and longitudes (`λ`).
+    Construct a horizontal grid with all the metadata required by MOM6 provided
+    an array of longitudes (``λ``) and latitudes (``φ``) on the supergrid.
+    Here, 'supergrid' refers to both cell edges and centres, meaning that there
+    are twice as many points along each axis than for any individual field.
 
     Caution:
-        Here, it is assumed the grid's boundaries are lines of constant latitude and
-        longitude. Rotated grids need to be handled in a different manner.
-        Also we assume here that the longitude array values are uniformly spaced.
+        It is assumed the grid's boundaries are lines of constant latitude and
+        longitude. Rotated grids need to be handled differently.
 
-        Make sure both `λ` and `φ` *must* be monotonically increasing.
+        It is also assumed here that the longitude array values are uniformly spaced.
+
+        Ensure both ``λ`` and ``φ`` are monotonically increasing.
 
     Args:
-        λ (numpy.array): All longitude points on the supergrid.
+        λ (numpy.array): All longitude points on the supergrid. Must be uniformly spaced.
         φ (numpy.array): All latitude points on the supergrid.
 
     Returns:
-        xarray.Dataset: A FMS-compatible *hgrid*, including the required attributes.
+        xarray.Dataset: An FMS-compatible horizontal grid (``hgrid``) that includes all required attributes.
     """
 
-    R = 6371e3  # mean radius of the Earth
+    assert np.all(np.diff(λ) > 0), "longitudes array λ must be monotonically increasing"
+    assert np.all(np.diff(φ) > 0), "latitudes array φ must be monotonically increasing"
+
+    R = 6371e3  # mean radius of the Earth; https://en.wikipedia.org/wiki/Earth_radius
 
-    dλ = λ[1] - λ[0]  # assuming that longitude is uniformly spaced
+    # compute longitude spacing and ensure that longitudes are uniformly spaced
+    dλ = λ[1] - λ[0]
+
+    assert np.allclose(
+        np.diff(λ), dλ * np.ones(np.size(λ) - 1)
+    ), "provided array of longitudes must be uniformly spaced"
 
     # dx = R * cos(φ) * np.deg2rad(dλ) / 2
     # Note: division by 2 because we're on the supergrid
     dx = np.broadcast_to(
         R * np.cos(np.deg2rad(φ)) * np.deg2rad(dλ) / 2,
         (λ.shape[0] - 1, φ.shape[0]),
     ).T
@@ -434,213 +355,325 @@
         }
     )
 
 
 class experiment:
     """The main class for setting up a regional experiment.
 
-    Knows everything about your regional experiment! Methods in this
-    class will generate the various input files you need to generate a
-    MOM6 experiment forced with open boundary conditions (OBCs). It's
-    written agnostic to your choice of boundary forcing, topography
-    and surface forcing - you need to tell it what your variables are
-    all called via mapping dictionaries from MOM6 variable/coordinate
-    name to the name in the input dataset.
+    Everything about the regional experiment.
+
+    Methods in this class generate the various input files needed for a MOM6
+    experiment forced with open boundary conditions (OBCs). The code is agnostic
+    to the user's choice of boundary forcing, bathymetry and surface forcing;
+    users need to prescribe what variables are all called via mapping dictionaries
+    from MOM6 variable/coordinate name to the name in the input dataset.
+
+    The class can be used to generate the grids for a new experiment, or to read in
+    an existing one by providing with ``read_existing_grids=True``.
 
     Args:
-        xextent (Tuple[float]): Extent of the region in longitude.
-        yextent (Tuple[float]): Extent of the region in latitude.
-        daterange (Tuple[str]): Start and end dates of the boundary forcing window.
+        longitude_extent (Tuple[float]): Extent of the region in longitude in degrees.
+        latitude_extent (Tuple[float]): Extent of the region in latitude in degrees.
+        date_range (Tuple[str]): Start and end dates of the boundary forcing window.
         resolution (float): Lateral resolution of the domain, in degrees.
-        vlayers (int): Number of vertical layers.
-        dz_ratio (float): Ratio of largest to smallest layer thickness, used in :func:`~dz`.
+        number_vertical_layers (int): Number of vertical layers.
+        layer_thickness_ratio (float): Ratio of largest to smallest layer thickness;
+            used as input in :func:`~hyperbolictan_thickness_profile`.
         depth (float): Depth of the domain.
         mom_run_dir (str): Path of the MOM6 control directory.
         mom_input_dir (str): Path of the MOM6 input directory, to receive the forcing files.
-        toolpath (str): Path of FREtools binaries.
-        gridtype (Optional[str]): Type of grid to generate, only ``even_spacing`` is supported.
-
+        toolpath_dir (str): Path of GFDL's FRE tools (https://github.com/NOAA-GFDL/FRE-NCtools)
+            binaries.
+        grid_type (Optional[str]): Type of horizontal grid to generate.
+            Currently, only ``'even_spacing'`` is supported.
+        repeat_year_forcing (Optional[bool]): When ``True`` the experiment runs with
+            repeat-year forcing. When ``False`` (default) then inter-annual forcing is used.
+        read_existing_grids (Optional[Bool]): When ``True``, instead of generating the grids,
+            reads the grids and ocean mask from ``mom_input_dir`` and ``mom_run_dir``. Useful
+            for modifying or troubleshooting experiments. Default: ``False``.
     """
 
     def __init__(
         self,
-        xextent,
-        yextent,
-        daterange,
+        *,
+        longitude_extent,
+        latitude_extent,
+        date_range,
         resolution,
-        vlayers,
-        dz_ratio,
+        number_vertical_layers,
+        layer_thickness_ratio,
         depth,
         mom_run_dir,
         mom_input_dir,
-        toolpath,
-        gridtype="even_spacing",
+        toolpath_dir,
+        grid_type="even_spacing",
+        repeat_year_forcing=False,
+        read_existing_grids=False,
     ):
+        ## in case list was given, convert to tuples
+        self.longitude_extent = tuple(longitude_extent)
+        self.latitude_extent = tuple(latitude_extent)
+        self.date_range = tuple(date_range)
+
         self.mom_run_dir = Path(mom_run_dir)
         self.mom_input_dir = Path(mom_input_dir)
 
         self.mom_run_dir.mkdir(exist_ok=True)
         self.mom_input_dir.mkdir(exist_ok=True)
 
-        self.xextent = xextent
-        self.yextent = yextent
-        self.daterange = [
-            dt.datetime.strptime(daterange[0], "%Y-%m-%d %H:%M:%S"),
-            dt.datetime.strptime(daterange[1], "%Y-%m-%d %H:%M:%S"),
+        self.date_range = [
+            dt.datetime.strptime(date_range[0], "%Y-%m-%d %H:%M:%S"),
+            dt.datetime.strptime(date_range[1], "%Y-%m-%d %H:%M:%S"),
         ]
-        self.res = resolution
-        self.vlayers = vlayers
-        self.dz_ratio = dz_ratio
+        self.resolution = resolution
+        self.number_vertical_layers = number_vertical_layers
+        self.layer_thickness_ratio = layer_thickness_ratio
         self.depth = depth
-        self.toolpath = toolpath
-        self.hgrid = self._make_hgrid(gridtype)
-        self.vgrid = self._make_vgrid()
-        self.gridtype = gridtype
-
+        self.toolpath_dir = Path(toolpath_dir)
+        self.grid_type = grid_type
+        self.repeat_year_forcing = repeat_year_forcing
+        self.ocean_mask = None
+        if read_existing_grids:
+            try:
+                self.hgrid = xr.open_dataset(self.mom_input_dir / "hgrid.nc")
+                self.vgrid = xr.open_dataset(self.mom_input_dir / "vcoord.nc")
+            except:
+                print(
+                    "Error in reading in existing grids. Make sure you've got files called `hgrid.nc` and `vcoord.nc` in {self.mom_input_dir}"
+                )
+                raise ValueError
+        else:
+            self.hgrid = self._make_hgrid()
+            self.vgrid = self._make_vgrid()
         # create additional directories and links
         (self.mom_input_dir / "weights").mkdir(exist_ok=True)
         (self.mom_input_dir / "forcing").mkdir(exist_ok=True)
 
         run_inputdir = self.mom_run_dir / "inputdir"
         if not run_inputdir.exists():
             run_inputdir.symlink_to(self.mom_input_dir.resolve())
         input_rundir = self.mom_input_dir / "rundir"
         if not input_rundir.exists():
             input_rundir.symlink_to(self.mom_run_dir.resolve())
 
-    def _make_hgrid(self, gridtype):
-        """Sets up hgrid based on users specification of
-        domain. Default behaviour leaves latitude and longitude evenly
-        spaced. This is very simple but suitable for small domains.
+    def __getattr__(self, name):
+        available_methods = [
+            method for method in dir(self) if not method.startswith("__")
+        ]
+        error_message = (
+            f"'{name}' method not found. Available methods are: {available_methods}"
+        )
+        raise AttributeError(error_message)
+
+    def _make_hgrid(self):
+        """
+        Set up a horizontal grid based on user's specification of the domain.
+        The default behaviour provides with a grid evenly spaced both in
+        longitude and in latitude.
+
+        The latitudinal resolution is scaled with the cosine of the central latitude of
+        the domain, i.e., ``Δφ = cos(φ_central) * Δλ``, where ``Δλ`` is the longitudinal
+        spacing. This way, and given that the domain is small enough, the linear
+        distances between grid points are nearly identical: ``Δx = R * cos(φ) * Δλ``
+        and ``Δy = R * Δφ = R * cos(φ_central) * Δλ``. That is, given that the domain is
+        small enough so that so that ``cos(φ_North_Side)`` is not much different from
+        ``cos(φ_South_Side)`` then ``Δx`` and ``Δy`` are similar.
 
         Note:
-            The intention is for the hgrid generation to be very flexible. For now there is only one implemented horizontal grid included in the package, but you can customise it by simply overwriting the `hgrid.nc` file that's deposited in your `rundir` after initialising an `experiment`. To conserve the metadata, it might be easiest to read the file in, then modify the fields before re-saving.
+            The intention is for the horizontal grid (``hgrid``) generation to be very flexible.
+            For now, there is only one implemented horizontal grid included in the package,
+            but you can customise it by simply overwriting the ``hgrid.nc`` file in the ``rundir``
+            after initialising an ``experiment``. To conserve the metadata, it might be easiest
+            to read the file in, then modify the fields before re-saving.
         """
 
-        if gridtype == "even_spacing":
-            # longitudes will just be evenly spaced, based only on resolution and bounds
-            nx = int((self.xextent[1] - self.xextent[0]) / (self.res / 2))
+        assert (
+            self.grid_type == "even_spacing"
+        ), "only even_spacing grid type is implemented"
+
+        if self.grid_type == "even_spacing":
+
+            # longitudes are evenly spaced based on resolution and bounds
+            nx = int(
+                (self.longitude_extent[1] - self.longitude_extent[0])
+                / (self.resolution / 2)
+            )
             if nx % 2 != 1:
                 nx += 1
 
-            x = np.linspace(self.xextent[0], self.xextent[1], nx)
+            λ = np.linspace(
+                self.longitude_extent[0], self.longitude_extent[1], nx
+            )  # longitudes in degrees
+
+            # Latitudes evenly spaced by dx * cos(central_latitude)
+            central_latitude = np.mean(self.latitude_extent)  # degrees
+            latitudinal_resolution = self.resolution * np.cos(
+                np.deg2rad(central_latitude)
+            )
 
-            # Latitudes evenly spaced by dx * cos(mean_lat)
-            res_y = self.res * np.cos(np.mean(self.yextent) * np.pi / 180)
+            ny = (
+                int(
+                    (self.latitude_extent[1] - self.latitude_extent[0])
+                    / (latitudinal_resolution / 2)
+                )
+                + 1
+            )
 
-            ny = int((self.yextent[1] - self.yextent[0]) / (res_y / 2)) + 1
             if ny % 2 != 1:
                 ny += 1
 
-            y = np.linspace(self.yextent[0], self.yextent[1], ny)
-            hgrid = rectangular_hgrid(x, y)
+            φ = np.linspace(
+                self.latitude_extent[0], self.latitude_extent[1], ny
+            )  # latitudes in degrees
+
+            hgrid = rectangular_hgrid(λ, φ)
             hgrid.to_netcdf(self.mom_input_dir / "hgrid.nc")
 
             return hgrid
 
     def _make_vgrid(self):
-        """Generates a vertical grid based on the number of layers
-        and vertical ratio specified at the class level.
-
+        """
+        Generate a vertical grid based on the number of layers ``nlayers`` and
+        the prescribed ratio of the vertical layer thicknesses (``layer_thickness_ratio``)
+        specified at the class level.
         """
 
-        thickness = dz(self.vlayers + 1, self.dz_ratio, self.depth)
-        vcoord = xr.Dataset(
-            {
-                "zi": ("zi", np.cumsum(thickness)),
-                "zl": ("zl", (np.cumsum(thickness) + 0.5 * thickness)[0:-1]),
-            }  ## THIS MIGHT BE WRONG REVISIT
+        thicknesses = hyperbolictan_thickness_profile(
+            self.number_vertical_layers, self.layer_thickness_ratio, self.depth
         )
+
+        zi = np.cumsum(thicknesses)
+        zi = np.insert(zi, 0, 0.0)  # add zi = 0.0 as first interface
+
+        zl = zi[0:-1] + thicknesses / 2  # the mid-points between interfaces zi
+
+        vcoord = xr.Dataset({"zi": ("zi", zi), "zl": ("zl", zl)})
+
         vcoord["zi"].attrs = {"units": "meters"}
+        vcoord["zl"].attrs = {"units": "meters"}
+
         vcoord.to_netcdf(self.mom_input_dir / "vcoord.nc")
 
         return vcoord
 
-    def ocean_forcing(
-        self, path, varnames, boundaries=None, gridtype="A", vcoord_type="height"
-    ):
-        """Reads in the forcing files that force the ocean at
-        boundaries (if specified) and for initial condition
+    def initial_condition(self, ic_path, varnames, gridtype="A", vcoord_type="height"):
+        """
+        Read the initial condition files, interpolates to the model grid fixes
+        up metadata and saves to the input directory.
 
         Args:
-            path (Union[str, Path]): Path to directory containing the forcing
-                files. Files should be named
-                ``north_segment_unprocessed`` for each boundary (for
-                the cardinal directions) and ``ic_unprocessed`` for the
-                initial conditions.
-            varnames (Dict[str, str]): Mapping from MOM6
-                variable/coordinate names to the name in the input
-                dataset.
-            boundaries (List[str]): Cardinal directions of included boundaries, in anticlockwise order
-            gridtype (Optional[str]): Arakawa grid staggering of input, one of ``A``, ``B`` or ``C``
-            vcoord_type (Optional[str]): The type of vertical
-                coordinate used in the forcing files. Either
-                ``height`` or ``thickness``.
-
+            ic_path (Union[str, Path]): Path to initial condition file.
+            varnames (Dict[str, str]): Mapping from MOM6 variable/coordinate names to the names
+                in the input dataset. For example, ``{'xq': 'lonq', 'yh': 'lath', 'salt': 'so', ...}``.
+            gridtype (Optional[str]): Arakawa grid staggering of input; either ``'A'``, ``'B'``,
+                or ``'C'``.
+            vcoord_type (Optional[str]): The type of vertical coordinate used in the forcing files.
+                Either ``'height'`` or ``'thickness'``.
         """
 
-        path = Path(path)
-
-        ## Do initial condition
-
-        ## pull out the initial velocity on MOM5's Bgrid
-        ic_raw = xr.open_dataset(path / "ic_unprocessed")
+        # Remove time dimension if present in the IC. Assume that the first time dim is the intended on if more than one is present
 
+        ic_raw = xr.open_dataset(ic_path)
         if varnames["time"] in ic_raw.dims:
             ic_raw = ic_raw.isel({varnames["time"]: 0})
+        if varnames["time"] in ic_raw.coords:
+            ic_raw = ic_raw.drop(varnames["time"])
 
-        ## Separate out tracers from two velocity fields of IC
+        # Separate out tracers from two velocity fields of IC
         try:
             ic_raw_tracers = ic_raw[
                 [varnames["tracers"][i] for i in varnames["tracers"]]
             ]
         except:
-            print("Error in reading in initial condition tracers. Terminating")
-            raise ValueError
+            raise ValueError(
+                "Error in reading in initial condition tracers. Terminating"
+            )
         try:
             ic_raw_u = ic_raw[varnames["u"]]
             ic_raw_v = ic_raw[varnames["v"]]
         except:
-            print("Error in reading in initial condition velocities. Terminating")
-            raise ValueError
+            raise ValueError(
+                "Error in reading in initial condition tracers. Terminating"
+            )
+
         try:
             ic_raw_eta = ic_raw[varnames["eta"]]
         except:
-            print("Error in reading in initial condition tracers. Terminating")
-            raise ValueError
-
-        ## Rename all coordinates to cgrid convention
-        if gridtype == "A":
-            ic_raw_tracers = ic_raw_tracers.rename(
-                {varnames["x"]: "lon", varnames["y"]: "lat"}
+            raise ValueError(
+                "Error in reading in initial condition tracers. Terminating"
             )
-            ic_raw_u = ic_raw_u.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
-            ic_raw_v = ic_raw_v.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
-            ic_raw_eta = ic_raw_eta.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
 
+        # Rename all coordinates to have 'lon' and 'lat' to work with the xesmf regridder
+        if gridtype == "A":
+            if (
+                "xh" in varnames.keys() and "yh" in varnames.keys()
+            ):  ## Handle case where user has provided xh and yh rather than x & y
+                # Rename xh with x in dictionary
+                varnames["x"] = varnames["xh"]
+                varnames["y"] = varnames["yh"]
+
+            if "x" in varnames.keys() and "y" in varnames.keys():
+                ic_raw_tracers = ic_raw_tracers.rename(
+                    {varnames["x"]: "lon", varnames["y"]: "lat"}
+                )
+                ic_raw_u = ic_raw_u.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
+                ic_raw_v = ic_raw_v.rename({varnames["x"]: "lon", varnames["y"]: "lat"})
+                ic_raw_eta = ic_raw_eta.rename(
+                    {varnames["x"]: "lon", varnames["y"]: "lat"}
+                )
+            else:
+                raise ValueError(
+                    "Can't find required coordinates in initial condition. Given that gridtype is 'A' the 'x' and 'y' coordinates should be provided in the varnames dictionary. E.g., {'x': 'lon','y': 'lat'}. Terminating"
+                )
         if gridtype == "B":
-            ic_raw_tracers = ic_raw_tracers.rename(
-                {varnames["xh"]: "lon", varnames["yh"]: "lat"}
-            )
-            ic_raw_eta = ic_raw_eta.rename(
-                {varnames["xh"]: "lon", varnames["yh"]: "lat"}
-            )
-            ic_raw_u = ic_raw_u.rename({varnames["xq"]: "lon", varnames["yq"]: "lat"})
-            ic_raw_v = ic_raw_v.rename({varnames["xq"]: "lon", varnames["yq"]: "lat"})
-
+            if (
+                "xq" in varnames.keys()
+                and "yq" in varnames.keys()
+                and "xh" in varnames.keys()
+                and "yh" in varnames.keys()
+            ):
+                ic_raw_tracers = ic_raw_tracers.rename(
+                    {varnames["xh"]: "lon", varnames["yh"]: "lat"}
+                )
+                ic_raw_eta = ic_raw_eta.rename(
+                    {varnames["xh"]: "lon", varnames["yh"]: "lat"}
+                )
+                ic_raw_u = ic_raw_u.rename(
+                    {varnames["xq"]: "lon", varnames["yq"]: "lat"}
+                )
+                ic_raw_v = ic_raw_v.rename(
+                    {varnames["xq"]: "lon", varnames["yq"]: "lat"}
+                )
+            else:
+                raise ValueError(
+                    "Can't find coordinates in initial condition. Given that gridtype is 'B' the names of the cell centre ('xh' & 'yh') as well as the cell edge ('xq' & 'yq') coordinates should be provided in the varnames dictionary. E.g {'xh':'lonh','yh':'lath' etc }. Terminating"
+                )
         if gridtype == "C":
-            ic_raw_tracers = ic_raw_tracers.rename(
-                {varnames["xh"]: "lon", varnames["yh"]: "lat"}
-            )
-            ic_raw_eta = ic_raw_eta.rename(
-                {varnames["xh"]: "lon", varnames["yh"]: "lat"}
-            )
-            ic_raw_u = ic_raw_u.rename({varnames["xq"]: "lon", varnames["yh"]: "lat"})
-            ic_raw_v = ic_raw_v.rename({varnames["xh"]: "lon", varnames["yq"]: "lat"})
-
+            if (
+                "xq" in varnames.keys()
+                and "yq" in varnames.keys()
+                and "xh" in varnames.keys()
+                and "yh" in varnames.keys()
+            ):
+                ic_raw_tracers = ic_raw_tracers.rename(
+                    {varnames["xh"]: "lon", varnames["yh"]: "lat"}
+                )
+                ic_raw_eta = ic_raw_eta.rename(
+                    {varnames["xh"]: "lon", varnames["yh"]: "lat"}
+                )
+                ic_raw_u = ic_raw_u.rename(
+                    {varnames["xq"]: "lon", varnames["yh"]: "lat"}
+                )
+                ic_raw_v = ic_raw_v.rename(
+                    {varnames["xh"]: "lon", varnames["yq"]: "lat"}
+                )
+            else:
+                raise ValueError(
+                    "Can't find coordinates in initial condition. Given that gridtype is 'C' the names of the cell centre ('xh' & 'yh') as well as the cell edge ('xq' & 'yq') coordinates should be provided in the varnames dictionary. E.g {'xh':'lonh','yh':'lath' etc }. Terminating"
+                )
         ## Construct the xq,yh and xh yq grids
         ugrid = (
             self.hgrid[["x", "y"]]
             .isel(nxp=slice(None, None, 2), nyp=slice(1, None, 2))
             .rename({"x": "lon", "y": "lat"})
             .set_coords(["lat", "lon"])
         )
@@ -662,15 +695,15 @@
                     ["lat"],
                     self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
                 ),
             }
         )
 
         ### Drop NaNs to be re-added later
-        # NaNs are from the land mask. When we interpolate onto a new grid, need to put in the new land mask. If NaNs left in, land mask stays the same
+        # NaNs might be here from the land mask of the model that the IC has come from. If they're not removed then the coastlines from this other grid will be retained!
         ic_raw_tracers = (
             ic_raw_tracers.interpolate_na("lon", method="linear")
             .ffill("lon")
             .bfill("lon")
             .ffill("lat")
             .bfill("lat")
             .ffill(varnames["zl"])
@@ -767,35 +800,27 @@
         eta_out.attrs = ic_raw_eta.attrs
 
         if np.min(tracers_out["temp"].isel({"zl": 0})) > 100:
             tracers_out["temp"] -= 273.15
 
         ## Regrid the fields vertically
 
-        ### NEED TO FIX THE HANDLING OF THICKNESS INPUT. will result in smaller number of vertical layers
-
-        if vcoord_type == "thickness":
+        if (
+            vcoord_type == "thickness"
+        ):  ## In this case construct the vertical profile by summing thickness
             tracers_out["zl"] = tracers_out["zl"].diff("zl")
             dz = tracers_out[self.z].diff(self.z)
             dz.name = "dz"
             dz = xr.concat([dz, dz[-1]], dim=self.z)
 
         tracers_out = tracers_out.interp({"zl": self.vgrid.zl.values})
         vel_out = vel_out.interp({"zl": self.vgrid.zl.values})
 
         print("Saving outputs... ", end="")
 
-        ## Remove time IF it exists. Users may already have done so for us
-        if "time" in vel_out.dims:
-            vel_out = vel_out.isel(time=0).drop("time")
-        if "time" in tracers_out.dims:
-            tracers_out = tracers_out.isel(time=0).drop("time")
-        if "time" in eta_out.dims:
-            eta_out = eta_out.isel(time=0).drop("time")
-
         vel_out.fillna(0).to_netcdf(
             self.mom_input_dir / "forcing/init_vel.nc",
             mode="w",
             encoding={
                 "u": {"_FillValue": netCDF4.default_fillvals["f4"]},
                 "v": {"_FillValue": netCDF4.default_fillvals["f4"]},
             },
@@ -817,233 +842,333 @@
             mode="w",
             encoding={
                 "xh": {"_FillValue": None},
                 "yh": {"_FillValue": None},
                 "eta_t": {"_FillValue": None},
             },
         )
-        print("done.")
+        print("done setting up initial condition.")
 
         self.ic_eta = eta_out
         self.ic_tracers = tracers_out
         self.ic_vels = vel_out
+        return
 
-        if boundaries is None:
-            return
+    def rectangular_boundary(
+        self, path_to_bc, varnames, orientation, segment_number, arakawa_grid="A"
+    ):
+        """
+        Setup a boundary forcing file for a given orientation. Here the term 'rectangular'
+        implies boundaries along lines of constant latitude or longitude.
 
-        print("BRUSHCUT BOUNDARIES")
+        Args:
+            path_to_bc (str): Path to boundary forcing file. Ideally this should be a pre cut-out
+                netCDF file containing only the boundary region and 3 extra boundary points on either
+                side. Users can also provide a large dataset containing their entire domain but this
+                will be slower.
+            varnames (Dict[str, str]): Mapping from MOM6 variable/coordinate names to the name in the
+                input dataset.
+            orientation (str): Orientation of boundary forcing file, i.e., ``'east'``, ``'west'``,
+                ``'north'``, or ``'south'``.
+            segment_number (int): Number the segments according to how they'll be specified in
+                the ``MOM_input``.
+            arakawa_grid (Optional[str]): Arakawa grid staggering of input; either ``'A'``, ``'B'``,
+                or ``'C'``.
+        """
 
-        ## Generate a rectangular OBC domain. This is the default
-        ## configuration. For fancier domains, need to use the segment
-        ## class manually
-        for i, o in enumerate(boundaries):
-            print(f"Processing {o}...", end="")
-            seg = segment(
-                self.hgrid,
-                path / f"{o.lower()}_unprocessed",  # location of raw boundary
-                self.mom_input_dir,
-                varnames,
-                "segment_{:03d}".format(i + 1),
-                o.lower(),  # orienataion
-                self.daterange[0],
-                gridtype,
-                vcoord_type,
-            )
+        print("Processing {} boundary...".format(orientation), end="")
 
-            seg.brushcut()
-            print("Done.")
+        seg = segment(
+            self.hgrid,
+            path_to_bc,  # location of raw boundary
+            self.mom_input_dir,
+            varnames,
+            "segment_{:03d}".format(segment_number),
+            orientation,  # orienataion
+            self.date_range[0],
+            gridtype=arakawa_grid,
+            repeat_year_forcing=self.repeat_year_forcing,
+        )
+
+        seg.rectangular_brushcut()
+        print("Done.")
+        return
 
-    def bathymetry(
+    def setup_bathymetry(
         self,
-        bathy_path,
-        varnames,
+        *,
+        bathymetry_path,
+        longitude_coordinate_name="lat",
+        latitude_coordinate_name="lon",
+        vertical_coordinate_name="elevation",
         fill_channels=False,
         minimum_layers=3,
-        maketopog=True,
-        positivedown=False,
+        positive_down=False,
         chunks="auto",
     ):
-        """Cuts out and interpolates chosen bathymetry, then fills
-        inland lakes.
+        """
+        Cut out and interpolate the chosen bathymetry and then fill inland lakes.
+
+        It's also possible to optionally fill narrow channels (see ``fill_channels``
+        below), although narrow channels are less of an issue for models that are
+        discretized on an Arakawa C grid, like MOM6.
 
-        It's also possible to optionally fill narrow channels, although this
-        is less of an issue for models on a C-grid, like MOM6. Output
-        saved to the input folder for your experiment.
+        Output is saved in the input directory of the experiment.
 
         Args:
-            bathy_path (str): Path to chosen bathymetry file netCDF file
-            varnames (Dict[str, str]): Mapping of coordinate and
-                variable names between the input and output.
+            bathymetry_path (str): Path to the netCDF file with the bathymetry.
+            longitude_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
+                dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'lon'`` (default).
+            latitude_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
+                dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'lat'`` (default).
+            vertical_coordinate_name (Optional[str]): The name of the longitude coordinate in the bathymetry
+                dataset at ``bathymetry_path``. For example, for GEBCO bathymetry: ``'elevation'`` (default).
             fill_channels (Optional[bool]): Whether or not to fill in
                 diagonal channels. This removes more narrow inlets,
-                but can also connect extra islands to land.
-            minimum layers (Optional[int]): The minimum depth allowed
-                as an integer number of layers. The default of 3
-                layers means that anything shallower than the 3rd
-                layer is deemed land.
-            maketopog (Optional[bool]): Whether to use FREtools to
-                make topography (if true), or read an existing file.
-            positivedown (Optional[bool]): If true, assumes that
-                bathymetry vertical coordinate is positive down.
-            chunks (Optional Dict[str, str]): Chunking scheme for bathymetry, eg {"lon": 100, "lat": 100}. Use lat/lon rather than the coordinate names in the input file.
-
-
+                but can also connect extra islands to land. Default: ``False``.
+            minimum_layers (Optional[int]): The minimum depth allowed as an integer
+                number of layers. Anything shallower than the ``minimum_layers``
+                (as specified by the vertical coordinate file ``vcoord.nc``) is deemed land.
+                Default: 3.
+            positive_down (Optional[bool]): If ``True``, it assumes that
+                bathymetry vertical coordinate is positive down. Default: ``False``.
+            chunks (Optional Dict[str, str]): Horizontal chunking scheme for the bathymetry, e.g.,
+                ``{"longitude": 100, "latitude": 100}``. Use ``'longitude'`` and ``'latitude'`` rather
+                than the actual coordinate names in the input file.
         """
 
-        if maketopog == True:
-            if chunks != "auto":
-                chunks = {varnames["xh"]: chunks["lon"], varnames["yh"]: chunks["lat"]}
+        ## Convert the provided coordinate names into a dictionary mapping to the
+        ## coordinate names that MOM6 expects.
+        coordinate_names = {
+            "xh": longitude_coordinate_name,
+            "yh": latitude_coordinate_name,
+            "elevation": vertical_coordinate_name,
+        }
+        if chunks != "auto":
+            chunks = {
+                coordinate_names["xh"]: chunks["longitude"],
+                coordinate_names["yh"]: chunks["latitude"],
+            }
 
-            bathy = xr.open_dataset(bathy_path, chunks=chunks)[varnames["elevation"]]
+        bathymetry = xr.open_dataset(bathymetry_path, chunks=chunks)[
+            coordinate_names["elevation"]
+        ]
 
-            bathy = bathy.sel(
-                {
-                    varnames["yh"]: slice(self.yextent[0] - 1, self.yextent[1] + 1)
-                }  #! Hardcoded 1 degree buffer around bathymetry selection. TODO: automatically select buffer
-            ).astype("float")
-
-            ## Here need to make a decision as to whether to slice 'normally' or with nicer slicer for 360 degree domain.
-
-            horizontal_resolution = bathy[varnames["xh"]][1] - bathy[varnames["xh"]][0]
-            horizontal_extent = (
-                bathy[varnames["xh"]][-1]
-                - bathy[varnames["xh"]][0]
-                + horizontal_resolution
-            )
-
-            if np.isclose(horizontal_extent, 360):
-                ## Assume that we're dealing with a global grid, in which case we use nicer slicer
-                bathy = nicer_slicer(
-                    bathy,
-                    np.array(self.xextent)
-                    + np.array(
-                        [-0.1, 0.1]
-                    ),  #! Hardcoded 0.1 degree buffer around bathymetry selection. TODO: automatically select buffer
-                    varnames["xh"],
+        bathymetry = bathymetry.sel(
+            {
+                coordinate_names["yh"]: slice(
+                    self.latitude_extent[0] - 0.5, self.latitude_extent[1] + 0.5
                 )
-            else:
-                ## Otherwise just slice normally
-                bathy = bathy.sel(
-                    {
-                        varnames["xh"]: slice(self.xextent[0] - 1, self.xextent[1] + 1)
-                    }  #! Hardcoded 1 degree buffer around bathymetry selection. TODO: automatically select buffer
-                )
-
-            bathy.attrs[
-                "missing_value"
-            ] = -1e20  # This is what FRE tools expects I guess?
-            bathyout = xr.Dataset({"elevation": bathy})
-            bathy.close()
-
-            bathyout = bathyout.rename({varnames["xh"]: "lon", varnames["yh"]: "lat"})
-            bathyout.lon.attrs["units"] = "degrees_east"
-            bathyout.lat.attrs["units"] = "degrees_north"
-            bathyout.elevation.attrs["_FillValue"] = -1e20
-            bathyout.elevation.attrs["units"] = "m"
-            bathyout.elevation.attrs[
-                "standard_name"
-            ] = "height_above_reference_ellipsoid"
-            bathyout.elevation.attrs["long_name"] = "Elevation relative to sea level"
-            bathyout.elevation.attrs["coordinates"] = "lon lat"
-            bathyout.to_netcdf(
-                self.mom_input_dir / "bathy_original.nc", mode="w", engine="netcdf4"
-            )
+            }  # 0.5 degree latitude buffer (hardcoded) for regridding
+        ).astype("float")
 
-            tgrid = xr.Dataset(
+        ## Check if the original bathymetry provided has a longitude extent that goes around the globe
+        ## to take care of the longitude seam when we slice out the regional domain.
+
+        horizontal_resolution = (
+            bathymetry[coordinate_names["xh"]][1]
+            - bathymetry[coordinate_names["xh"]][0]
+        )
+
+        horizontal_extent = (
+            bathymetry[coordinate_names["xh"]][-1]
+            - bathymetry[coordinate_names["xh"]][0]
+            + horizontal_resolution
+        )
+
+        longitude_buffer = 0.5  # 0.5 degree longitude buffer (hardcoded) for regridding
+
+        if np.isclose(horizontal_extent, 360):
+            ## longitude extent that goes around the globe -- use longitude_slicer
+            bathymetry = longitude_slicer(
+                bathymetry,
+                np.array(self.longitude_extent)
+                + np.array([-longitude_buffer, longitude_buffer]),
+                coordinate_names["xh"],
+            )
+        else:
+            ## otherwise, slice normally
+            bathymetry = bathymetry.sel(
                 {
-                    "lon": (
-                        ["lon"],
-                        self.hgrid.x.isel(nxp=slice(1, None, 2), nyp=1).values,
-                    ),
-                    "lat": (
-                        ["lat"],
-                        self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
-                    ),
+                    coordinate_names["xh"]: slice(
+                        self.longitude_extent[0] - longitude_buffer,
+                        self.longitude_extent[1] + longitude_buffer,
+                    )
                 }
             )
-            tgrid = xr.Dataset(
-                data_vars={
-                    "elevation": (
-                        ["lat", "lon"],
-                        np.zeros(
-                            self.hgrid.x.isel(
-                                nxp=slice(1, None, 2), nyp=slice(1, None, 2)
-                            ).shape
-                        ),
-                    )
-                },
-                coords={
-                    "lon": (
-                        ["lon"],
-                        self.hgrid.x.isel(nxp=slice(1, None, 2), nyp=1).values,
-                    ),
-                    "lat": (
-                        ["lat"],
-                        self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
+
+        bathymetry.attrs["missing_value"] = -1e20  # missing value expected by FRE tools
+        bathymetry_output = xr.Dataset({"elevation": bathymetry})
+        bathymetry.close()
+
+        bathymetry_output = bathymetry_output.rename(
+            {coordinate_names["xh"]: "lon", coordinate_names["yh"]: "lat"}
+        )
+        bathymetry_output.lon.attrs["units"] = "degrees_east"
+        bathymetry_output.lat.attrs["units"] = "degrees_north"
+        bathymetry_output.elevation.attrs["_FillValue"] = -1e20
+        bathymetry_output.elevation.attrs["units"] = "m"
+        bathymetry_output.elevation.attrs["standard_name"] = (
+            "height_above_reference_ellipsoid"
+        )
+        bathymetry_output.elevation.attrs["long_name"] = (
+            "Elevation relative to sea level"
+        )
+        bathymetry_output.elevation.attrs["coordinates"] = "lon lat"
+        bathymetry_output.to_netcdf(
+            self.mom_input_dir / "bathymetry_original.nc", mode="w", engine="netcdf4"
+        )
+
+        tgrid = xr.Dataset(
+            {
+                "lon": (
+                    ["lon"],
+                    self.hgrid.x.isel(nxp=slice(1, None, 2), nyp=1).values,
+                ),
+                "lat": (
+                    ["lat"],
+                    self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
+                ),
+            }
+        )
+        tgrid = xr.Dataset(
+            data_vars={
+                "elevation": (
+                    ["lat", "lon"],
+                    np.zeros(
+                        self.hgrid.x.isel(
+                            nxp=slice(1, None, 2), nyp=slice(1, None, 2)
+                        ).shape
                     ),
-                },
-            )
+                )
+            },
+            coords={
+                "lon": (
+                    ["lon"],
+                    self.hgrid.x.isel(nxp=slice(1, None, 2), nyp=1).values,
+                ),
+                "lat": (
+                    ["lat"],
+                    self.hgrid.y.isel(nxp=1, nyp=slice(1, None, 2)).values,
+                ),
+            },
+        )
 
-            # rewrite chunks to use lat/lon now for use with xesmf
-            if chunks != "auto":
-                chunks = {"lon": chunks[varnames["xh"]], "lat": chunks[varnames["yh"]]}
+        # rewrite chunks to use lat/lon now for use with xesmf
+        if chunks != "auto":
+            chunks = {
+                "lon": chunks[coordinate_names["xh"]],
+                "lat": chunks[coordinate_names["yh"]],
+            }
 
-            tgrid = tgrid.chunk(chunks)
-            tgrid.lon.attrs["units"] = "degrees_east"
-            tgrid.lon.attrs["_FillValue"] = 1e20
-            tgrid.lat.attrs["units"] = "degrees_north"
-            tgrid.to_netcdf(
-                self.mom_input_dir / "topog_raw.nc", mode="w", engine="netcdf4"
-            )
-            tgrid.close()
+        tgrid = tgrid.chunk(chunks)
+        tgrid.lon.attrs["units"] = "degrees_east"
+        tgrid.lon.attrs["_FillValue"] = 1e20
+        tgrid.lat.attrs["units"] = "degrees_north"
+        tgrid.lat.attrs["_FillValue"] = 1e20
+        tgrid.elevation.attrs["units"] = "m"
+        tgrid.elevation.attrs["coordinates"] = "lon lat"
+        tgrid.to_netcdf(
+            self.mom_input_dir / "bathymetry_unfinished.nc", mode="w", engine="netcdf4"
+        )
+        tgrid.close()
 
-            ## Replace subprocess run with regular regridder
-            print(
-                "Starting to regrid bathymetry. If this process hangs you might be better off calling ESMF directly from a terminal with appropriate computational resources using \n\n mpirun ESMF_Regrid -s bathy_original.nc -d topog_raw.nc -m bilinear --src_var elevation --dst_var elevation --netcdf4 --src_regional --dst_regional\n\nThis is better for larger domains.\n\n"
-            )
+        ## Replace subprocess run with regular regridder
+        print(
+            "Begin regridding bathymetry...\n\n"
+            + "If this process hangs it means that the chosen domain might be too big to handle this way. "
+            + "After ensuring access to appropriate computational resources, try calling ESMF "
+            + "directly from a terminal in the input directory via\n\n"
+            + "mpirun ESMF_Regrid -s bathymetry_original.nc -d bathymetry_unfinished.nc -m bilinear --src_var elevation --dst_var elevation --netcdf4 --src_regional --dst_regional\n\n"
+            + "For details see https://xesmf.readthedocs.io/en/latest/large_problems_on_HPC.html\n\n"
+            + "Aftewards, we run 'tidy_bathymetry' method to skip the expensive interpolation step, and finishing metadata, encoding and cleanup."
+        )
+
+        # If we have a domain large enough for chunks, we'll run regridder with parallel=True
+        parallel = True
+        if len(tgrid.chunks) != 2:
+            parallel = False
+        print(f"Regridding in parallel: {parallel}")
+        bathymetry_output = bathymetry_output.chunk(chunks)
+        # return
+        regridder = xe.Regridder(
+            bathymetry_output, tgrid, "bilinear", parallel=parallel
+        )
+
+        bathymetry = regridder(bathymetry_output)
+        bathymetry.to_netcdf(
+            self.mom_input_dir / "bathymetry_unfinished.nc", mode="w", engine="netcdf4"
+        )
+        print(
+            "Regridding finished. Now calling `tidy_bathymetry` method for some finishing touches..."
+        )
 
-            # If we have a domain large enough for chunks, we'll run regridder with parallel=True
-            parallel = True
-            if len(tgrid.chunks) != 2:
-                parallel = False
-            regridder = xe.Regridder(bathyout, tgrid, "bilinear", parallel=parallel)
+        self.tidy_bathymetry(fill_channels, minimum_layers, positive_down)
 
-            topog = regridder(bathyout)
-            topog.to_netcdf(
-                self.mom_input_dir / "topog_raw.nc", mode="w", engine="netcdf4"
-            )
+    def tidy_bathymetry(
+        self, fill_channels=False, minimum_layers=3, positive_down=True
+    ):
+        """
+        An auxiliary function for bathymetry used to fix up the metadata and remove inland
+        lakes after regridding the bathymetry. Having `tidy_bathymetry` as a separate
+        method from :func:`~setup_bathymetry` allows for the regridding to be done separately,
+        since regridding can be really expensive for large domains.
+
+        If the bathymetry is already regridded and what is left to be done is fixing the metadata,
+        or fill in some channels then call this function directly to read in the existing
+        ``bathymetry_unfinished.nc`` file that should be in the input directory.
+
+        Args:
+            fill_channels (Optional[bool]): Whether or not to fill in
+                diagonal channels. This removes more narrow inlets,
+                but can also connect extra islands to land. Default: ``False``.
+            minimum_layers (Optional[int]): The minimum depth allowed
+                as an integer number of layers. The default value of ``3``
+                layers means that anything shallower than the 3rd
+                layer (as specified by the ``vcoord``) is deemed land.
+            positive_down (Optional[bool]): If ``True`` (default), it assumes that
+                bathymetry vertical coordinate is positive down.
+        """
 
-        ## reopen topography to modify
+        ## reopen bathymetry to modify
         print("Reading in regridded bathymetry to fix up metadata...", end="")
-        topog = xr.open_dataset(self.mom_input_dir / "topog_raw.nc", engine="netcdf4")
+        bathymetry = xr.open_dataset(
+            self.mom_input_dir / "bathymetry_unfinished.nc", engine="netcdf4"
+        )
 
         ## Ensure correct encoding
-        topog = xr.Dataset({"depth": (["ny", "nx"], topog["elevation"].values)})
-        topog.attrs["depth"] = "meters"
-        topog.attrs["standard_name"] = "topographic depth at T-cell centers"
-        topog.attrs["coordinates"] = "zi"
+        bathymetry = xr.Dataset(
+            {"depth": (["ny", "nx"], bathymetry["elevation"].values)}
+        )
+        bathymetry.attrs["depth"] = "meters"
+        bathymetry.attrs["standard_name"] = "bathymetryraphic depth at T-cell centers"
+        bathymetry.attrs["coordinates"] = "zi"
 
-        topog.expand_dims("tiles", 0)
+        bathymetry.expand_dims("tiles", 0)
 
-        if not positivedown:
+        if not positive_down:
             ## Ensure that coordinate is positive down!
-            topog["depth"] *= -1
+            bathymetry["depth"] *= -1
 
         ## REMOVE INLAND LAKES
 
         min_depth = self.vgrid.zi[minimum_layers]
 
-        ocean_mask = topog.copy(deep=True).depth.where(topog.depth <= min_depth, 1)
+        ocean_mask = bathymetry.copy(deep=True).depth.where(
+            bathymetry.depth <= min_depth, 1
+        )
         land_mask = np.abs(ocean_mask - 1)
+
         changed = True  ## keeps track of whether solution has converged or not
 
         forward = True  ## only useful for iterating through diagonal channel removal. Means iteration goes SW -> NE
 
         while changed == True:
-            ## First fill in all lakes. This uses a scipy function where it fills holes made of 0's within a field of 1's
+            ## First fill in all lakes.
+            ## scipy.ndimage.binary_fill_holes fills holes made of 0's within a field of 1's
             land_mask[:, :] = binary_fill_holes(land_mask.data)
             ## Get the ocean mask instead of land- easier to remove channels this way
             ocean_mask = np.abs(land_mask - 1)
 
             ## Now fill in all one-cell-wide channels
             newmask = xr.where(
                 ocean_mask * (land_mask.shift(nx=1) + land_mask.shift(nx=-1)) == 2, 1, 0
@@ -1157,121 +1282,404 @@
 
                     forward = True
 
             newmask = xr.where(newmask > 0, 1, 0)
             changed = np.max(newmask) == 1
             land_mask += newmask
 
-        ocean_mask = np.abs(land_mask - 1)
+        self.ocean_mask = np.abs(land_mask - 1)
 
-        topog["depth"] *= ocean_mask
+        bathymetry["depth"] *= self.ocean_mask
 
-        topog["depth"] = topog["depth"].where(topog["depth"] != 0, np.nan)
+        bathymetry["depth"] = bathymetry["depth"].where(
+            bathymetry["depth"] != 0, np.nan
+        )
 
-        topog.expand_dims({"ntiles": 1}).to_netcdf(
-            self.mom_input_dir / "topog_deseas.nc",
+        bathymetry.expand_dims({"ntiles": 1}).to_netcdf(
+            self.mom_input_dir / "bathymetry.nc",
             mode="w",
             encoding={"depth": {"_FillValue": None}},
         )
 
-        (self.mom_input_dir / "topog_deseas.nc").rename(self.mom_input_dir / "topog.nc")
         print("done.")
-        self.topog = topog
+        self.bathymetry = bathymetry
 
-    def FRE_tools(self, layout):
-        """
-        Just a wrapper for FRE Tools check_mask, make_solo_mosaic and make_quick_mosaic. User provides processor layout tuple of processing units.
+    def FRE_tools(self, layout=None):
+        """A wrapper for FRE Tools ``check_mask``, ``make_solo_mosaic``, and ``make_quick_mosaic``.
+        User provides processor ``layout`` tuple of processing units.
         """
 
-        if not (self.mom_input_dir / "topog.nc").exists():
-            print("No topography file! Need to run make_bathymetry first")
+        print(
+            "Running GFDL's FRE Tools. The following information is all printed by the FRE tools themselves"
+        )
+        if not (self.mom_input_dir / "bathymetry.nc").exists():
+            print("No bathymetry file! Need to run .setup_bathymetry method first")
             return
 
         for p in self.mom_input_dir.glob("mask_table*"):
             p.unlink()
 
         print(
-            "MAKE SOLO MOSAIC",
+            "OUTPUT FROM MAKE SOLO MOSAIC:",
             subprocess.run(
-                self.toolpath
-                + "make_solo_mosaic/make_solo_mosaic --num_tiles 1 --dir . --mosaic_name ocean_mosaic --tile_file hgrid.nc",
+                str(self.toolpath_dir / "make_solo_mosaic/make_solo_mosaic")
+                + " --num_tiles 1 --dir . --mosaic_name ocean_mosaic --tile_file hgrid.nc",
                 shell=True,
                 cwd=self.mom_input_dir,
             ),
             sep="\n\n",
         )
 
         print(
-            "QUICK MOSAIC",
+            "OUTPUT FROM QUICK MOSAIC:",
             subprocess.run(
-                self.toolpath
-                + "make_quick_mosaic/make_quick_mosaic --input_mosaic ocean_mosaic.nc --mosaic_name grid_spec --ocean_topog topog.nc",
+                str(self.toolpath_dir / "make_quick_mosaic/make_quick_mosaic")
+                + " --input_mosaic ocean_mosaic.nc --mosaic_name grid_spec --ocean_topog bathymetry.nc",
                 shell=True,
                 cwd=self.mom_input_dir,
             ),
             sep="\n\n",
         )
 
+        if layout != None:
+            self.cpu_layout(layout)
+
+    def cpu_layout(self, layout):
+        """
+        Wrapper for the ``check_mask`` function of GFDL's FRE Tools. User provides processor
+        ``layout`` tuple of processing units.
+        """
+
         print(
-            "CHECK MASK",
+            "OUTPUT FROM CHECK MASK:\n\n",
             subprocess.run(
-                self.toolpath
-                + f"check_mask/check_mask --grid_file ocean_mosaic.nc --ocean_topog topog.nc --layout {layout[0]},{layout[1]} --halo 4",
+                str(self.toolpath_dir / "check_mask/check_mask")
+                + f" --grid_file ocean_mosaic.nc --ocean_topog bathymetry.nc --layout {layout[0]},{layout[1]} --halo 4",
                 shell=True,
                 cwd=self.mom_input_dir,
             ),
         )
         self.layout = layout
+        return
+
+    def setup_run_directory(
+        self,
+        surface_forcing=None,
+        using_payu=False,
+        overwrite=False,
+    ):
+        """
+        Setup the run directory for MOM6. Either copy a pre-made set of files, or modify
+        existing files in the 'rundir' directory for the experiment.
+
+        Args:
+            regional_mom6_path (str): Path to the regional MOM6 source code that was cloned
+                from GitHub. Default is current path, ``'.'``.
+            surface_forcing (Optional[str]): Specify the choice of surface forcing, one
+                of: ``'jra'`` or ``'era5'``. If not prescribed then constant fluxes are used.
+            using_payu (Optional[bool]): Whether or not to use payu (https://github.com/payu-org/payu)
+                to run the model. If ``True``, a payu configuration file will be created.
+                Default: ``False``.
+            overwrite (Optional[bool]): Whether or not to overwrite existing files in the
+                run directory. If ``False`` (default), will only modify the ``MOM_layout`` file and will
+                not re-copy across the rest of the default files.
+        """
+
+        ## Get the path to the regional_mom package on this computer
+        premade_rundir_path = Path(
+            importlib.resources.files("regional_mom6") / "demos/premade_run_directories"
+        )
+
+        # Define the locations of the directories we'll copy files across from. Base contains most of the files, and overwrite replaces files in the base directory.
+        base_run_dir = premade_rundir_path / "common_files"
+        if not premade_rundir_path.exists():
+            raise ValueError(
+                f"Cannot find the premade run directory files at \n{premade_rundir_path}\n. Something is not right about how the package has been installed as these files are missing!"
+            )
+        if surface_forcing:
+            overwrite_run_dir = premade_rundir_path / f"{surface_forcing}_surface"
+            if not overwrite_run_dir.exists():
+                available = [x for x in premade_rundir_path.iterdir() if x.is_dir()]
+                raise ValueError(
+                    f"Surface forcing {surface_forcing} not available. Please choose from {str(available)}"  ##Here print all available run directories
+                )
+        else:
+            ## In case there is additional forcing (e.g., tides) then we need to modify the run dir to include the additional forcing.
+            overwrite_run_dir = False
+
+        # 3 different cases to handle:
+        #   1. User is creating a new run directory from scratch. Here we copy across all files and modify.
+        #   2. User has already created a run directory, and wants to modify it. Here we only modify the MOM_layout file.
+        #   3. User has already created a run directory, and wants to overwrite it. Here we copy across all files and modify. This requires overwrite = True
+
+        if not overwrite:
+            for file in base_run_dir.glob(
+                "*"
+            ):  ## copy each file individually if it doesn't already exist OR overwrite = True
+                if not os.path.exists(self.mom_run_dir / file.name):
+                    ## Check whether this file exists in an override directory or not
+                    if (
+                        overwrite_run_dir != False
+                        and (overwrite_run_dir / file.name).exists()
+                    ):
+                        shutil.copy(overwrite_run_dir / file.name, self.mom_run_dir)
+                    else:
+                        shutil.copy(base_run_dir / file.name, self.mom_run_dir)
+        else:
+            shutil.copytree(base_run_dir, self.mom_run_dir, dirs_exist_ok=True)
+            if overwrite_run_dir != False:
+                shutil.copy(base_run_dir / file, self.mom_run_dir)
+
+        ## Make symlinks between run and input directories
+        inputdir_in_rundir = self.mom_run_dir / "inputdir"
+        rundir_in_inputdir = self.mom_input_dir / "rundir"
+
+        inputdir_in_rundir.unlink(missing_ok=True)
+        inputdir_in_rundir.symlink_to(self.mom_input_dir)
+
+        rundir_in_inputdir.unlink(missing_ok=True)
+        rundir_in_inputdir.symlink_to(self.mom_run_dir)
+
+        ## Get mask table information
+        mask_table = None
+        for p in self.mom_input_dir.glob("mask_table.*"):
+            if mask_table != None:
+                print(
+                    f"WARNING: Multiple mask tables found. Defaulting to {mask_table}. If this is not what you want, remove it from the run directory and try again."
+                )
+                break
+
+            _, masked, layout = p.name.split(".")
+            mask_table = p.name
+            x, y = (int(v) for v in layout.split("x"))
+            ncpus = (x * y) - int(masked)
+        if mask_table == None:
+            print(
+                "No mask table found! This suggests the domain is mostly water, so there are no `non compute` cells that are entirely land. If this doesn't seem right, ensure you've already run .FRE_tools()."
+            )
+            if not hasattr(self, "layout"):
+                raise AttributeError(
+                    "No layout information found. This suggests you haven't run .FRE_tools() yet. Please do so first so I know how many processors you'd like to use."
+                )
+            ncpus = self.layout[0] * self.layout[1]
+        print("Number of CPUs required: ", ncpus)
+
+        ## Modify the input namelists to give the correct layouts
+        # TODO Re-implement with package that works for this file type? or at least tidy up code
+        with open(self.mom_run_dir / "MOM_layout", "r") as file:
+            lines = file.readlines()
+            for jj in range(len(lines)):
+                if "MASKTABLE" in lines[jj]:
+                    if mask_table != None:
+                        lines[jj] = f'MASKTABLE = "{mask_table}"\n'
+                    else:
+                        lines[jj] = "# MASKTABLE = no mask table"
+                if "LAYOUT =" in lines[jj] and "IO" not in lines[jj]:
+                    lines[jj] = f"LAYOUT = {self.layout[1]},{self.layout[0]}\n"
+
+                if "NIGLOBAL" in lines[jj]:
+                    lines[jj] = f"NIGLOBAL = {self.hgrid.nx.shape[0]//2}\n"
+
+                if "NJGLOBAL" in lines[jj]:
+                    lines[jj] = f"NJGLOBAL = {self.hgrid.ny.shape[0]//2}\n"
+
+        with open(self.mom_run_dir / "MOM_layout", "w") as f:
+            f.writelines(lines)
+
+        ## If using payu to run the model, create a payu configuration file
+        if not using_payu and os.path.exists(f"{self.mom_run_dir}/config.yaml"):
+            os.remove(f"{self.mom_run_dir}/config.yaml")
+
+        else:
+            with open(f"{self.mom_run_dir}/config.yaml", "r") as file:
+                lines = file.readlines()
+
+                inputfile = open(f"{self.mom_run_dir}/config.yaml", "r")
+                lines = inputfile.readlines()
+                inputfile.close()
+                for i in range(len(lines)):
+                    if "ncpus" in lines[i]:
+                        lines[i] = f"ncpus: {str(ncpus)}\n"
+                    if "jobname" in lines[i]:
+                        lines[i] = f"jobname: mom6_{self.mom_input_dir.name}\n"
+
+                    if "input:" in lines[i]:
+                        lines[i + 1] = f"    - {self.mom_input_dir}\n"
+
+            with open(f"{self.mom_run_dir}/config.yaml", "w") as file:
+                file.writelines(lines)
+
+        # Modify input.nml
+        nml = f90nml.read(self.mom_run_dir / "input.nml")
+        nml["coupler_nml"]["current_date"] = [
+            self.date_range[0].year,
+            self.date_range[0].month,
+            self.date_range[0].day,
+            0,
+            0,
+            0,
+        ]
+        nml.write(self.mom_run_dir / "input.nml", force=True)
+
+    def setup_era5(self, era5_path):
+        """
+        Setup the ERA5 forcing files for the experiment. This assumes that
+        all of the ERA5 data in the prescribed date range are downloaded.
+        We need the following fields: "2t", "10u", "10v", "sp", "2d", "msdwswrf",
+        "msdwlwrf", "lsrr", and "crr".
+
+        Args:
+            era5_path (str): Path to the ERA5 forcing files. Specifically, the single-level
+                reanalysis product. For example, ``'SOMEPATH/era5/single-levels/reanalysis'``
+        """
+
+        ## Firstly just open all raw data
+        rawdata = {}
+        for fname, vname in zip(
+            ["2t", "10u", "10v", "sp", "2d", "msdwswrf", "msdwlwrf", "lsrr", "crr"],
+            ["t2m", "u10", "v10", "sp", "d2m", "msdwswrf", "msdwlwrf", "lsrr", "crr"],
+        ):
+            ## Load data from all relevant years
+            years = [
+                i for i in range(self.date_range[0].year, self.date_range[1].year + 1)
+            ]
+            # Loop through each year and read the corresponding files
+            for year in years:
+                ds = xr.open_mfdataset(
+                    f"{era5_path}/{fname}/{year}/{fname}*",
+                    decode_times=False,
+                    chunks={"longitude": 100, "latitude": 100},
+                )
+
+                ## Cut out this variable to our domain size
+                rawdata[fname] = longitude_slicer(
+                    ds,
+                    self.longitude_extent,
+                    "longitude",
+                ).sel(
+                    latitude=slice(
+                        self.longitude_extent[1], self.longitude_extent[0]
+                    )  ## This is because ERA5 has latitude in decreasing order (??)
+                )
+
+                ## Now fix up the latitude and time dimensions
+
+                rawdata[fname] = (
+                    rawdata[fname]
+                    .isel(latitude=slice(None, None, -1))  ## Flip latitude
+                    .assign_coords(
+                        time=np.arange(
+                            0, rawdata[fname].time.shape[0], dtype=float
+                        )  ## Set the zero date of forcing to start of run
+                    )
+                )
+
+                rawdata[fname].time.attrs = {
+                    "calendar": "julian",
+                    "units": f"hours since {self.date_range[0].strftime('%Y-%m-%d %H:%M:%S')}",
+                }  ## Fix up calendar to match
+
+                if fname == "2d":
+                    ## Calculate specific humidity from dewpoint temperature
+                    dewpoint = 8.07131 - 1730.63 / (
+                        233.426 + rawdata["2d"]["d2m"] - 273.15
+                    )
+                    humidity = (
+                        (0.622 / rawdata["sp"]["sp"]) * (10**dewpoint) * 101325 / 760
+                    )
+                    q = xr.Dataset(data_vars={"q": humidity})
+
+                    q.q.attrs = {"long_name": "Specific Humidity", "units": "kg/kg"}
+                    q.to_netcdf(
+                        f"{self.mom_input_dir}/forcing/q_ERA5.nc",
+                        unlimited_dims="time",
+                        encoding={"q": {"dtype": "double"}},
+                    )
+                elif fname == "crr":
+                    ## Calculate total rain rate from convective and total
+                    trr = xr.Dataset(
+                        data_vars={
+                            "trr": rawdata["crr"]["crr"] + rawdata["lsrr"]["lsrr"]
+                        }
+                    )
+
+                    trr.trr.attrs = {
+                        "long_name": "Total Rain Rate",
+                        "units": "kg m**-2 s**-1",
+                    }
+                    trr.to_netcdf(
+                        f"{self.mom_input_dir}/forcing/trr_ERA5-{year}.nc",
+                        unlimited_dims="time",
+                        encoding={"trr": {"dtype": "double"}},
+                    )
+
+                elif fname == "lsrr":
+                    ## This is handled by crr as both are added together to calculate total rain rate.
+                    pass
+                else:
+                    rawdata[fname].to_netcdf(
+                        f"{self.mom_input_dir}/forcing/{fname}_ERA5-{year}.nc",
+                        unlimited_dims="time",
+                        encoding={vname: {"dtype": "double"}},
+                    )
 
 
 class segment:
-    """Class to turn raw boundary segment data into MOM6 boundary
+    """
+    Class to turn raw boundary segment data into MOM6 boundary
     segments.
 
     Boundary segments should only contain the necessary data for that
     segment. No horizontal chunking is done here, so big fat segments
     will process slowly.
 
     Data should be at daily temporal resolution, iterating upwards
     from the provided startdate. Function ignores the time metadata
     and puts it on Julian calendar.
 
+    Only supports z-star (z*) vertical coordinate!
 
     Args:
-        hgrid (xarray.Dataset): The horizontal grid used for domain
-        infile (Union[str, Path]): Path to the raw, unprocessed boundary segment
-        outfolder (Union[str, Path]): Path to folder where the model inputs will be stored
-        varnames (Dict[str, str]): Mapping between the
-            variable/dimension names and standard naming convension of
-            this pipeline, e.g. ``{"xq":"longitude, "yh":"latitude",
-            "salt":"salinity...}``. Key "tracers" points to nested
-            dictionary of tracers to include in boundary
-        seg_name (str): Name of the segment. Something like ``segment_001``
-        orientation (str): Cardinal direction (lowercase) of the boundary segment
-        startdate (str): The starting date to use in the segment calendar
-        gridtype (Optional[str]): Arakawa staggering of input grid, one of ``A``, ``B`` or ``C``
-        vcoord_type (Optional[str]): Vertical coordinate, either
-            interfacial ``height`` or layer ``thickness``
-        time_units (str): The units used by raw forcing file,
-            e.g. ``hours``, ``days`` (default)
-
+        hgrid (xarray.Dataset): The horizontal grid used for domain.
+        infile (Union[str, Path]): Path to the raw, unprocessed boundary segment.
+        outfolder (Union[str, Path]): Path to folder where the model inputs will
+            be stored.
+        varnames (Dict[str, str]): Mapping between the variable/dimension names and
+            standard naming convension of this pipeline, e.g., ``{"xq": "longitude,
+            "yh": "latitude", "salt": "salinity", ...}``. Key "tracers" points to nested
+            dictionary of tracers to include in boundary.
+        seg_name (str): Name of the segment, e.g., ``'segment_001'``.
+        orientation (str): Cardinal direction (lowercase) of the boundary segment.
+        startdate (str): The starting date to use in the segment calendar.
+        gridtype (Optional[str]): Arakawa staggering of input grid, one of ``'A'``, ``'B'``,
+            or ``'C'``
+        time_units (str): The units used by the raw forcing files, e.g., ``hours``,
+            ``days`` (default).
+        tidal_constituents (Optional[int]): An integer determining the number of tidal
+            constituents to be included from the list: *M*:sub:`2`, *S*:sub:`2`, *N*:sub:`2`,
+            *K*:sub:`2`, *K*:sub:`1`, *O*:sub:`2`, *P*:sub:`1`, *Q*:sub:`1`, *Mm*,
+            *Mf*, and *M*:sub:`4`. For example, specifying ``1`` only includes *M*:sub:`2`;
+            specifying ``2`` includes *M*:sub:`2` and *S*:sub:`2`, etc. Default: ``None``.
+        repeat_year_forcing (Optional[bool]): When ``True`` the experiment runs with repeat-year
+            forcing. When ``False`` (default) then inter-annual forcing is used.
     """
 
     def __init__(
         self,
         hgrid,
         infile,
         outfolder,
         varnames,
         seg_name,
         orientation,
         startdate,
         gridtype="A",
-        vcoord_type="height",
         time_units="days",
+        tidal_constituents=None,
+        repeat_year_forcing=False,
     ):
         ## Store coordinate names
         if gridtype == "A":
             self.x = varnames["x"]
             self.y = varnames["y"]
 
         elif gridtype in ("B", "C"):
@@ -1283,75 +1691,83 @@
         ## Store velocity names
         self.u = varnames["u"]
         self.v = varnames["v"]
         self.z = varnames["zl"]
         self.eta = varnames["eta"]
         self.time = varnames["time"]
         self.startdate = startdate
+
         ## Store tracer names
         self.tracers = varnames["tracers"]
         self.time_units = time_units
 
         ## Store other data
         self.infile = infile
         self.outfolder = outfolder
         self.orientation = orientation.lower()  ## might not be needed? NSEW
         self.grid = gridtype
         self.hgrid = hgrid
         self.seg_name = seg_name
-        self.vcoord_type = vcoord_type
-
-    def brushcut(self, ryf=False):
-        ### Implement brushcutter scheme on single segment ###
-        rawseg = xr.open_dataset(self.infile, decode_times=False, engine="netcdf4")
+        self.tidal_constituents = tidal_constituents
+        self.repeat_year_forcing = repeat_year_forcing
 
-        ## Depending on the orientation of the segment, cut out the right bit of the hgrid
-        ## and define which coordinate is along or into the segment
+    def rectangular_brushcut(self):
+        """
+        Cut out and interpolates tracers. This method assumes that the boundary
+        is a simple Northern, Southern, Eastern, or Western boundary. Cuts out
+        and interpolates tracers.
+        """
         if self.orientation == "north":
-            hgrid_seg = self.hgrid.isel(nyp=[-1])
-            perpendicular = "ny"
-            parallel = "nx"
+            self.hgrid_seg = self.hgrid.isel(nyp=[-1])
+            self.perpendicular = "ny"
+            self.parallel = "nx"
 
         if self.orientation == "south":
-            hgrid_seg = self.hgrid.isel(nyp=[0])
-            perpendicular = "ny"
-            parallel = "nx"
+            self.hgrid_seg = self.hgrid.isel(nyp=[0])
+            self.perpendicular = "ny"
+            self.parallel = "nx"
 
         if self.orientation == "east":
-            hgrid_seg = self.hgrid.isel(nxp=[-1])
-            perpendicular = "nx"
-            parallel = "ny"
+            self.hgrid_seg = self.hgrid.isel(nxp=[-1])
+            self.perpendicular = "nx"
+            self.parallel = "ny"
 
         if self.orientation == "west":
-            hgrid_seg = self.hgrid.isel(nxp=[0])
-            perpendicular = "nx"
-            parallel = "ny"
+            self.hgrid_seg = self.hgrid.isel(nxp=[0])
+            self.perpendicular = "nx"
+            self.parallel = "ny"
 
         ## Need to keep track of which axis the 'main' coordinate corresponds to for later on when re-adding the 'secondary' axis
-        if perpendicular == "ny":
-            axis1 = 3
-            axis2 = 2
+        if self.perpendicular == "ny":
+            self.axis_to_expand = 2
         else:
-            axis1 = 2
-            axis2 = 3
+            self.axis_to_expand = 3
 
         ## Grid for interpolating our fields
-        interp_grid = xr.Dataset(
+        self.interp_grid = xr.Dataset(
             {
-                "lat": ([f"{parallel}_{self.seg_name}"], hgrid_seg.y.squeeze().data),
-                "lon": ([f"{parallel}_{self.seg_name}"], hgrid_seg.x.squeeze().data),
+                "lat": (
+                    [f"{self.parallel}_{self.seg_name}"],
+                    self.hgrid_seg.y.squeeze().data,
+                ),
+                "lon": (
+                    [f"{self.parallel}_{self.seg_name}"],
+                    self.hgrid_seg.x.squeeze().data,
+                ),
             }
         ).set_coords(["lat", "lon"])
 
+        rawseg = xr.open_dataset(self.infile, decode_times=False, engine="netcdf4")
+
         if self.grid == "A":
             rawseg = rawseg.rename({self.x: "lon", self.y: "lat"})
             ## In this case velocities and tracers all on same points
             regridder = xe.Regridder(
                 rawseg[self.u],
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_velocity_weights_{self.orientation}.nc",
             )
 
@@ -1366,25 +1782,25 @@
                 ]
             )
 
         if self.grid == "B":
             ## All tracers on one grid, all velocities on another
             regridder_velocity = xe.Regridder(
                 rawseg[self.u].rename({self.xq: "lon", self.yq: "lat"}),
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_velocity_weights_{self.orientation}.nc",
             )
 
             regridder_tracer = xe.Regridder(
                 rawseg[self.tracers["salt"]].rename({self.xh: "lon", self.yh: "lat"}),
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_tracer_weights_{self.orientation}.nc",
             )
 
@@ -1403,35 +1819,35 @@
                 ]
             )
 
         if self.grid == "C":
             ## All tracers on one grid, all velocities on another
             regridder_uvelocity = xe.Regridder(
                 rawseg[self.u].rename({self.xq: "lon", self.yh: "lat"}),
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_uvelocity_weights_{self.orientation}.nc",
             )
 
             regridder_vvelocity = xe.Regridder(
                 rawseg[self.v].rename({self.xh: "lon", self.yq: "lat"}),
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_vvelocity_weights_{self.orientation}.nc",
             )
 
             regridder_tracer = xe.Regridder(
                 rawseg[self.tracers["salt"]].rename({self.xh: "lon", self.yh: "lat"}),
-                interp_grid,
+                self.interp_grid,
                 "bilinear",
                 locstream_out=True,
                 reuse_weights=False,
                 filename=self.outfolder
                 / f"weights/bilinear_tracer_weights_{self.orientation}.nc",
             )
 
@@ -1456,43 +1872,31 @@
             > 100
         ):
             segment_out[self.tracers["temp"]] -= 273.15
 
         # fill in NaNs
         segment_out = (
             segment_out.ffill(self.z)
-            .interpolate_na(f"{parallel}_{self.seg_name}")
-            .ffill(f"{parallel}_{self.seg_name}")
-            .bfill(f"{parallel}_{self.seg_name}")
+            .interpolate_na(f"{self.parallel}_{self.seg_name}")
+            .ffill(f"{self.parallel}_{self.seg_name}")
+            .bfill(f"{self.parallel}_{self.seg_name}")
         )
 
-        ##### FIX UP COORDINATE METADATA #####
-        ## OLD: Use 1950 reference
-        # start_jd50 = (self.startdate - dt.datetime.strptime("1950-01-01 00:00:00","%Y-%m-%d %H:%M:%S")).days
-        # time = np.arange(
-        #     start_jd50,
-        #     start_jd50 + rawseg[self.time].shape[0]  ## Time is just range of days from start of window until end in Julian day offset from 1950 epoch
-        # )
-
-        #! This only works for RYF or shorter IAF runs.
-        #  We'd need a better way to split up forcing files into separate chunks if you wanted to run one year at a time.
         time = np.arange(
             0,  #! Indexing everything from start of experiment = simple but maybe counterintutive?
             segment_out[self.time].shape[
                 0
             ],  ## Time is indexed from start date of window
             dtype=float,
         )
 
         segment_out = segment_out.assign_coords({"time": time})
-
         segment_out.time.attrs = {
             "calendar": "julian",
             "units": f"{self.time_units} since {self.startdate}",
-            "modulo": " ",
         }
         # Dictionary we built for encoding the netcdf at end
         encoding_dict = {
             "time": {
                 "dtype": "double",
             },
             f"nx_{self.seg_name}": {
@@ -1500,23 +1904,17 @@
             },
             f"ny_{self.seg_name}": {
                 "dtype": "int32",
             },
         }
 
         ### Generate our dz variable. This needs to be in layer thicknesses
-        if self.vcoord_type == "height":
-            dz = segment_out[self.z].diff(self.z)
-            dz.name = "dz"
-            dz = xr.concat([dz, dz[-1]], dim=self.z)
-
-        else:
-            dz = segment_out[self.z]
-            dz.name = "dz"
-        del segment_out[self.z]
+        dz = segment_out[self.z].diff(self.z)
+        dz.name = "dz"
+        dz = xr.concat([dz, dz[-1]], dim=self.z)
 
         # Here, keep in mind that 'var' keeps track of the mom6 variable names we want, and self.tracers[var] will return the name of the variable from the original data
 
         allfields = {
             **self.tracers,
             "u": self.u,
             "v": self.v,
@@ -1539,15 +1937,15 @@
             ## Replace the old depth coordinates with incremental integers
             segment_out[f"nz_{self.seg_name}_{var}"] = np.arange(
                 segment_out[f"nz_{self.seg_name}_{var}"].size
             )
 
             ## Re-add the secondary dimension (even though it represents one value..)
             segment_out[v] = segment_out[v].expand_dims(
-                f"{perpendicular}_{self.seg_name}", axis=axis2
+                f"{self.perpendicular}_{self.seg_name}", axis=self.axis_to_expand
             )
 
             ## Add the layer thicknesses
             segment_out[f"dz_{v}"] = (
                 ["time", f"nz_{v}", f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
                 da.broadcast_to(
                     dz.data[None, :, None, None],
@@ -1578,36 +1976,47 @@
         ## Treat eta separately since it has no vertical coordinate. Do the same things as for the surface variables above
         segment_out = segment_out.rename({self.eta: f"eta_{self.seg_name}"})
         encoding_dict[f"eta_{self.seg_name}"] = {
             "_FillValue": netCDF4.default_fillvals["f8"],
         }
         segment_out[f"eta_{self.seg_name}"] = segment_out[
             f"eta_{self.seg_name}"
-        ].expand_dims(f"{perpendicular}_{self.seg_name}", axis=axis2 - 1)
+        ].expand_dims(
+            f"{self.perpendicular}_{self.seg_name}", axis=self.axis_to_expand - 1
+        )
 
         # Overwrite the actual lat/lon values in the dimensions, replace with incrementing integers
-        segment_out[f"{parallel}_{self.seg_name}"] = np.arange(
-            segment_out[f"{parallel}_{self.seg_name}"].size
+        segment_out[f"{self.parallel}_{self.seg_name}"] = np.arange(
+            segment_out[f"{self.parallel}_{self.seg_name}"].size
         )
-        segment_out[f"{perpendicular}_{self.seg_name}"] = [0]
+        segment_out[f"{self.perpendicular}_{self.seg_name}"] = [0]
 
         # Store actual lat/lon values here as variables rather than coordinates
         segment_out[f"lon_{self.seg_name}"] = (
             [f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
-            hgrid_seg.x.data,
+            self.hgrid_seg.x.data,
         )
         segment_out[f"lat_{self.seg_name}"] = (
             [f"ny_{self.seg_name}", f"nx_{self.seg_name}"],
-            hgrid_seg.y.data,
+            self.hgrid_seg.y.data,
         )
 
+        # Add units to the lat / lon to keep the `categorize_axis_from_units` checker happy
+        segment_out[f"lat_{self.seg_name}"].attrs = {
+            "units": "degrees_north",
+        }
+        segment_out[f"lon_{self.seg_name}"].attrs = {
+            "units": "degrees_east",
+        }
+
+        # If repeat-year forcing, add modulo coordinate
+        if self.repeat_year_forcing:
+            segment_out["time"] = segment_out["time"].assign_attrs({"modulo": " "})
+
         with ProgressBar():
-            segment_out["time"] = segment_out["time"].assign_attrs(
-                {"modulo": " "}
-            )  ## Add modulo attribute for MOM6 to treat as repeat forcing
             segment_out.load().to_netcdf(
                 self.outfolder / f"forcing/forcing_obc_{self.seg_name}.nc",
                 encoding=encoding_dict,
                 unlimited_dims="time",
             )
 
         return segment_out, encoding_dict
```

