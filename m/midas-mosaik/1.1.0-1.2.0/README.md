# Comparing `tmp/midas-mosaik-1.1.0.tar.gz` & `tmp/midas-mosaik-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-mosaik-1.1.0.tar", last modified: Tue Oct 17 09:14:03 2023, max compression
+gzip compressed data, was "midas-mosaik-1.2.0.tar", last modified: Tue Apr 16 06:36:57 2024, max compression
```

## Comparing `midas-mosaik-1.1.0.tar` & `midas-mosaik-1.2.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.770799 midas-mosaik-1.1.0/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/LICENSE
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      210 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/MANIFEST.in
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5383 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/PKG-INFO
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4405 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/README.md
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        5 2023-10-17 09:11:45.000000 midas-mosaik-1.1.0/VERSION
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.754133 midas-mosaik-1.1.0/docs/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      634 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/Makefile
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2195 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/conf.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10624 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/configuration.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2009 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/getting_started.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      517 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/index.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6519 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/installation.rst
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      795 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/make.bat
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/docs/modules/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8610 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/comdata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)  3895886 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/dlp_season.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    10891 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/dlpdata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   228112 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/facilitys.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      420 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/index.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    11576 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/powergrid.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   703409 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/smart_nord_lands.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     8750 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/sndata.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     4868 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/store.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)    86633 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/time_weather.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     6048 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/timesim.rst
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   195881 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   213876 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png
--rw-r--r--   0 sbalduin  (1000) wheel      (998)   205192 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    17181 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/docs/next_steps.rst
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.750799 midas-mosaik-1.1.0/midas/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/midas/api/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      218 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/__init__.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5668 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/fnc_analyze.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13756 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/fnc_configure.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4257 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/fnc_download.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      470 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/fnc_list.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1873 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/fnc_run.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     9478 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/api/midasctl.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/midas/scenario/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/__init__.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/midas/scenario/config/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5701 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/benchmark.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7730 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/bremerhaven.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1357 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/constrainted_grids.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1724 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/four_bus.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1914 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/grid_example.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3453 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/midaslv.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3725 2023-10-17 08:12:38.000000 midas-mosaik-1.1.0/midas/scenario/config/midasmv.yml
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      874 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/no_grid.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      640 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/config/sbrural3.yml
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8865 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/midas/scenario/configurator.py
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13631 2023-07-14 11:51:02.000000 midas-mosaik-1.1.0/midas/scenario/scenario.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/midas_mosaik.egg-info/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     5383 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/PKG-INFO
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     1516 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/SOURCES.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/dependency_links.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       53 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/entry_points.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)      386 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/requires.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2023-10-17 09:14:03.000000 midas-mosaik-1.1.0/midas_mosaik.egg-info/top_level.txt
--rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2023-10-17 09:14:03.770799 midas-mosaik-1.1.0/setup.cfg
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2173 2023-10-17 09:05:29.000000 midas-mosaik-1.1.0/setup.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.750799 midas-mosaik-1.1.0/tests/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/tests/system/
--rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      129 2023-09-22 07:38:16.000000 midas-mosaik-1.1.0/tests/system/debug_script.py
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.750799 midas-mosaik-1.1.0/tests/unit/
-drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2023-10-17 09:14:03.767466 midas-mosaik-1.1.0/tests/unit/scenario/
--rw-r--r--   0 sbalduin  (1000) wheel      (998)     2135 2023-07-12 12:35:52.000000 midas-mosaik-1.1.0/tests/unit/scenario/test_configurator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/LICENSE
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      210 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/MANIFEST.in
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5034 2024-04-16 06:35:27.000000 midas-mosaik-1.2.0/README.md
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)        5 2024-04-16 06:35:19.000000 midas-mosaik-1.2.0/VERSION
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.053247 midas-mosaik-1.2.0/docs/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      634 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/Makefile
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2195 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/conf.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    10624 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/configuration.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2009 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/getting_started.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      517 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/index.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6504 2023-10-17 09:34:59.000000 midas-mosaik-1.2.0/docs/installation.rst
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      795 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/make.bat
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.056580 midas-mosaik-1.2.0/docs/modules/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8610 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/comdata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)  3895886 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/dlp_season.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    10891 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/dlpdata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   228112 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/facilitys.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      420 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/index.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    11576 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/powergrid.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   703409 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/smart_nord_lands.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     8750 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/sndata.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     4868 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/store.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)    86633 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/time_weather.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6048 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/timesim.rst
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   195881 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   213876 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)   205192 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    17182 2023-10-18 11:13:52.000000 midas-mosaik-1.2.0/docs/next_steps.rst
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.053247 midas-mosaik-1.2.0/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.056580 midas-mosaik-1.2.0/midas/api/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      218 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     5668 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/fnc_analyze.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13756 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/fnc_configure.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     4257 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/fnc_download.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      470 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/fnc_list.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1873 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/fnc_run.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     9478 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/api/midasctl.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.056580 midas-mosaik-1.2.0/midas/scenario/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/__init__.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/midas/scenario/config/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     5701 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/benchmark.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7730 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/bremerhaven.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1357 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/constrainted_grids.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1739 2024-04-08 06:46:37.000000 midas-mosaik-1.2.0/midas/scenario/config/four_bus.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1914 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/grid_example.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3453 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/midaslv.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     3725 2024-03-19 15:44:34.000000 midas-mosaik-1.2.0/midas/scenario/config/midasmv.yml
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      874 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/no_grid.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      640 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/config/sbrural3.yml
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8865 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/midas/scenario/configurator.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)    13631 2023-07-14 11:51:02.000000 midas-mosaik-1.2.0/midas/scenario/scenario.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/midas_mosaik.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     6013 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     1516 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       53 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/entry_points.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      366 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2024-04-16 06:36:57.000000 midas-mosaik-1.2.0/midas_mosaik.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2161 2024-04-16 06:33:55.000000 midas-mosaik-1.2.0/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.053247 midas-mosaik-1.2.0/tests/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/tests/system/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      129 2023-09-22 07:38:16.000000 midas-mosaik-1.2.0/tests/system/debug_script.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.053247 midas-mosaik-1.2.0/tests/unit/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-04-16 06:36:57.059913 midas-mosaik-1.2.0/tests/unit/scenario/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2135 2023-07-12 12:35:52.000000 midas-mosaik-1.2.0/tests/unit/scenario/test_configurator.py
```

### Comparing `midas-mosaik-1.1.0/LICENSE` & `midas-mosaik-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/PKG-INFO` & `midas-mosaik-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-mosaik
-Version: 1.1.0
+Version: 1.2.0
 Summary: MultI-DomAin test Scenario for smart grid co-simulation.
 Home-page: https://gitlab.com/midas-mosaik/midas
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 License-File: LICENSE
 
 # MIDAS
 
 The MultI-DomAin test Scenario (MIDAS) is a collection of mosaik simulators (https://gitlab.com/mosaik) for smart grid co-simulation and contains a semi-automatic scenario configuration tool.
 The latest documentation is always available at https://midas-mosaik.gitlab.io/midas.
 
-Version: 1.0
+Version: 1.2
 
 ## Requirements
 
 All required Python packages will be pulled during installation.
 However, there are some additional requirements which you have to setup up manually.
 
 First of all, you need a working Python installation >= 3.8. 
@@ -143,7 +143,31 @@
 
 to run the *midasmv* scenario in the docker. 
 Replace `PATH_TO_MIDAS_DATA` with the absolute path to your MIDAS data directory (usually located at ~/.config/midas/midas_data).
 Replace `PATH_TO_OUTPUT_DIR` with the location where the outputs should be stored.
 
 If you create a runtime config in the same directory as the Dockerfile before run the build command, this file will be included.
 However, you should not change the output_path and the data_path, otherwise you will have to adapt the run command as well.
+
+## Citation
+
+If you want to use Midas in your research, you can cite this publication:
+
+```
+@InProceedings{10.1007/978-3-031-43824-0_10,
+    author="Balduin, Stephan
+    and Veith, Eric M. S. P.
+    and Lehnhoff, Sebastian",
+    editor="Wagner, Gerd
+    and Werner, Frank
+    and De Rango, Floriano",
+    title="Midas: An Open-Source Framework for Simulation-Based Analysis of Energy Systems",
+    booktitle="Simulation and Modeling Methodologies, Technologies and Applications",
+    year="2023",
+    publisher="Springer International Publishing",
+    address="Cham",
+    pages="177--194",
+    isbn="978-3-031-43824-0"
+}
+
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `midas-mosaik-1.1.0/README.md` & `midas-mosaik-1.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # MIDAS
 
 The MultI-DomAin test Scenario (MIDAS) is a collection of mosaik simulators (https://gitlab.com/mosaik) for smart grid co-simulation and contains a semi-automatic scenario configuration tool.
 The latest documentation is always available at https://midas-mosaik.gitlab.io/midas.
 
-Version: 1.0
+Version: 1.2
 
 ## Requirements
 
 All required Python packages will be pulled during installation.
 However, there are some additional requirements which you have to setup up manually.
 
 First of all, you need a working Python installation >= 3.8. 
@@ -118,7 +118,31 @@
 
 to run the *midasmv* scenario in the docker. 
 Replace `PATH_TO_MIDAS_DATA` with the absolute path to your MIDAS data directory (usually located at ~/.config/midas/midas_data).
 Replace `PATH_TO_OUTPUT_DIR` with the location where the outputs should be stored.
 
 If you create a runtime config in the same directory as the Dockerfile before run the build command, this file will be included.
 However, you should not change the output_path and the data_path, otherwise you will have to adapt the run command as well.
+
+## Citation
+
+If you want to use Midas in your research, you can cite this publication:
+
+```
+@InProceedings{10.1007/978-3-031-43824-0_10,
+    author="Balduin, Stephan
+    and Veith, Eric M. S. P.
+    and Lehnhoff, Sebastian",
+    editor="Wagner, Gerd
+    and Werner, Frank
+    and De Rango, Floriano",
+    title="Midas: An Open-Source Framework for Simulation-Based Analysis of Energy Systems",
+    booktitle="Simulation and Modeling Methodologies, Technologies and Applications",
+    year="2023",
+    publisher="Springer International Publishing",
+    address="Cham",
+    pages="177--194",
+    isbn="978-3-031-43824-0"
+}
+
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `midas-mosaik-1.1.0/docs/Makefile` & `midas-mosaik-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/conf.py` & `midas-mosaik-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/configuration.rst` & `midas-mosaik-1.2.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/getting_started.rst` & `midas-mosaik-1.2.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/index.rst` & `midas-mosaik-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/installation.rst` & `midas-mosaik-1.2.0/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 We recommend to use a `virtualenv`__ to avoid messing up your system environment.
 Use your distributions' package manager to install pip and virtualenv.
 Make sure which python version is linked to the `python` command (in some distros this may still be python2).
 To be sure, specify the python interpreter when creating the env:
 
 .. code-block:: bash
 
-  $ virtualenv -p /usr/bin/python3 ~/.virtualenvs/midas
+  $ python3 -m venv ~/.virtualenvs/midas
   $ source ~/.virtualenv/midas/bin/activate
 
 Now you can install *midas-mosaik* from the pypi package repository
 
 .. code-block:: bash
 
   (midas) $ pip install midas-mosaik
```

### Comparing `midas-mosaik-1.1.0/docs/make.bat` & `midas-mosaik-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/comdata.rst` & `midas-mosaik-1.2.0/docs/modules/comdata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/dlp_season.png` & `midas-mosaik-1.2.0/docs/modules/dlp_season.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/dlpdata.rst` & `midas-mosaik-1.2.0/docs/modules/dlpdata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/facilitys.png` & `midas-mosaik-1.2.0/docs/modules/facilitys.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/powergrid.rst` & `midas-mosaik-1.2.0/docs/modules/powergrid.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/smart_nord_lands.png` & `midas-mosaik-1.2.0/docs/modules/smart_nord_lands.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/sndata.rst` & `midas-mosaik-1.2.0/docs/modules/sndata.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/store.rst` & `midas-mosaik-1.2.0/docs/modules/store.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/time_weather.png` & `midas-mosaik-1.2.0/docs/modules/time_weather.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/timesim.rst` & `midas-mosaik-1.2.0/docs/modules/timesim.rst`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png` & `midas-mosaik-1.2.0/docs/modules/two_grid_example-Powergrid__0_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png` & `midas-mosaik-1.2.0/docs/modules/two_grid_example-Powergrid__1_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png` & `midas-mosaik-1.2.0/docs/mymidasdb-Powergrid__0_0-buses_vmpu.png`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/docs/next_steps.rst` & `midas-mosaik-1.2.0/docs/next_steps.rst`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 Before we add the final two modules for this guide, we'll have a short look at the simulation results.
 You'll find them in the *_outputs* folder. 
 During the simulation, a HDF5 database will be created and saved to *mymidasdb.hdf5*.
 Although you can open this file with any HDF5 viewer, the easiest to get some generic results is to use *midasctl* again:
 
 .. code-block:: bash
 
-    midasctl analyze _outputs/mymidsdb.hdf5
+    midasctl analyze _outputs/mymidasdb.hdf5
 
 
 This takes a few seconds. 
 Afterwards, you'll find a new folder *_outputs/mymidasdb* containing results of the analysis.
 There is another folder *_outputs/mymidasdb/Powergrid_0* that contains a few .png files, one of them is the average voltage magnitude per unit of the buses in our scenario:
 
 .. image:: mymidasdb-Powergrid__0_0-buses_vmpu.png
```

### Comparing `midas-mosaik-1.1.0/midas/api/fnc_analyze.py` & `midas-mosaik-1.2.0/midas/api/fnc_analyze.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/api/fnc_configure.py` & `midas-mosaik-1.2.0/midas/api/fnc_configure.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/api/fnc_download.py` & `midas-mosaik-1.2.0/midas/api/fnc_download.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/api/fnc_run.py` & `midas-mosaik-1.2.0/midas/api/fnc_run.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/api/midasctl.py` & `midas-mosaik-1.2.0/midas/api/midasctl.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/benchmark.yml` & `midas-mosaik-1.2.0/midas/scenario/config/benchmark.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/bremerhaven.yml` & `midas-mosaik-1.2.0/midas/scenario/config/bremerhaven.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/constrainted_grids.yml` & `midas-mosaik-1.2.0/midas/scenario/config/constrainted_grids.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/four_bus.yml` & `midas-mosaik-1.2.0/midas/scenario/config/four_bus.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   modules:
     - store
     - powergrid
     - sndata
   step_size: 15*60
   start_date: 2009-01-01 00:00:00+0100
   end: 1*24*60*60
+  silent: true
   store_params:
     filename: fourbus.hdf5
   powergrid_params:
     four_bus:
       gridfile: simple_four_bus_system
   sndata_params:
     four_bus:
```

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/grid_example.yml` & `midas-mosaik-1.2.0/midas/scenario/config/grid_example.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/midaslv.yml` & `midas-mosaik-1.2.0/midas/scenario/config/midaslv.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/midasmv.yml` & `midas-mosaik-1.2.0/midas/scenario/config/midasmv.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/no_grid.yml` & `midas-mosaik-1.2.0/midas/scenario/config/no_grid.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/config/sbrural3.yml` & `midas-mosaik-1.2.0/midas/scenario/config/sbrural3.yml`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/configurator.py` & `midas-mosaik-1.2.0/midas/scenario/configurator.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas/scenario/scenario.py` & `midas-mosaik-1.2.0/midas/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/midas_mosaik.egg-info/PKG-INFO` & `midas-mosaik-1.2.0/midas_mosaik.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-mosaik
-Version: 1.1.0
+Version: 1.2.0
 Summary: MultI-DomAin test Scenario for smart grid co-simulation.
 Home-page: https://gitlab.com/midas-mosaik/midas
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -24,15 +24,15 @@
 License-File: LICENSE
 
 # MIDAS
 
 The MultI-DomAin test Scenario (MIDAS) is a collection of mosaik simulators (https://gitlab.com/mosaik) for smart grid co-simulation and contains a semi-automatic scenario configuration tool.
 The latest documentation is always available at https://midas-mosaik.gitlab.io/midas.
 
-Version: 1.0
+Version: 1.2
 
 ## Requirements
 
 All required Python packages will be pulled during installation.
 However, there are some additional requirements which you have to setup up manually.
 
 First of all, you need a working Python installation >= 3.8. 
@@ -143,7 +143,31 @@
 
 to run the *midasmv* scenario in the docker. 
 Replace `PATH_TO_MIDAS_DATA` with the absolute path to your MIDAS data directory (usually located at ~/.config/midas/midas_data).
 Replace `PATH_TO_OUTPUT_DIR` with the location where the outputs should be stored.
 
 If you create a runtime config in the same directory as the Dockerfile before run the build command, this file will be included.
 However, you should not change the output_path and the data_path, otherwise you will have to adapt the run command as well.
+
+## Citation
+
+If you want to use Midas in your research, you can cite this publication:
+
+```
+@InProceedings{10.1007/978-3-031-43824-0_10,
+    author="Balduin, Stephan
+    and Veith, Eric M. S. P.
+    and Lehnhoff, Sebastian",
+    editor="Wagner, Gerd
+    and Werner, Frank
+    and De Rango, Floriano",
+    title="Midas: An Open-Source Framework for Simulation-Based Analysis of Energy Systems",
+    booktitle="Simulation and Modeling Methodologies, Technologies and Applications",
+    year="2023",
+    publisher="Springer International Publishing",
+    address="Cham",
+    pages="177--194",
+    isbn="978-3-031-43824-0"
+}
+
+
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `midas-mosaik-1.1.0/midas_mosaik.egg-info/SOURCES.txt` & `midas-mosaik-1.2.0/midas_mosaik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midas-mosaik-1.1.0/setup.py` & `midas-mosaik-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,33 @@
     VERSION = freader.readline().strip()
 
 with open("README.md") as freader:
     README = freader.read()
 
 install_requirements = [
     "click",
-    "mosaik==3.1.1",
-    "mosaik-api==3.0.3",
-    "midas-util>=1.0.5",
+    "mosaik",
+    "mosaik-api",
+    "midas-util>=1.1.2",
     "midas-comdata>=1.0.0rc5",
     "midas-dlpdata>=1.0.0rc6",
     "midas-goa>=1.0.0rc6",
     "midas-powergrid>=1.0.10",
     "midas-pwdata>=1.0.0",
     "midas-sbdata>=1.0.1",
     "midas-sndata>=1.0.2",
     "midas-store>=1.0.0",
     "midas-timesim>=1.0.0rc5",
-    "midas-weather>=1.1.0",
-    "pysimmods>=0.10.2",
+    "midas-weather>=1.1.4",
+    "pysimmods>=0.11.1",
     "ruamel.yaml",
 ]
 
 development_requirements = [
-    "numba",
+    # "numba",
     "flake8",
     "pytest",
     "tox",
     "coverage",
     "black==22.3.0",
     "setuptools",
     "twine",
```

### Comparing `midas-mosaik-1.1.0/tests/unit/scenario/test_configurator.py` & `midas-mosaik-1.2.0/tests/unit/scenario/test_configurator.py`

 * *Files identical despite different names*

