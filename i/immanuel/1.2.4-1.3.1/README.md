# Comparing `tmp/immanuel-1.2.4.tar.gz` & `tmp/immanuel-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immanuel-1.2.4.tar", last modified: Tue Mar 19 16:30:48 2024, max compression
+gzip compressed data, was "immanuel-1.3.1.tar", last modified: Tue Apr 16 01:32:34 2024, max compression
```

## Comparing `immanuel-1.2.4.tar` & `immanuel-1.3.1.tar`

### file list

```diff
@@ -1,70 +1,78 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.660117 immanuel-1.2.4/
--rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.2.4/LICENSE.md
--rw-r--r--   0 robert     (501) staff       (20)       21 2023-12-02 01:56:03.000000 immanuel-1.2.4/MANIFEST.in
--rw-r--r--   0 robert     (501) staff       (20)    46396 2024-03-19 16:30:48.659832 immanuel-1.2.4/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     8403 2024-03-19 16:26:21.000000 immanuel-1.2.4/README.md
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.593307 immanuel-1.2.4/immanuel/
--rw-r--r--   0 robert     (501) staff       (20)    19034 2024-02-05 00:09:40.000000 immanuel-1.2.4/immanuel/charts.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.595270 immanuel-1.2.4/immanuel/classes/
--rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/classes/serialize.py
--rw-r--r--   0 robert     (501) staff       (20)    10808 2024-02-03 23:33:10.000000 immanuel-1.2.4/immanuel/classes/wrap.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.596920 immanuel-1.2.4/immanuel/const/
--rw-r--r--   0 robert     (501) staff       (20)     2325 2024-01-20 20:33:35.000000 immanuel-1.2.4/immanuel/const/calc.py
--rw-r--r--   0 robert     (501) staff       (20)     2613 2023-12-15 16:02:49.000000 immanuel-1.2.4/immanuel/const/chart.py
--rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/const/data.py
--rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/const/dignities.py
--rw-r--r--   0 robert     (501) staff       (20)     5692 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/const/names.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.598380 immanuel-1.2.4/immanuel/reports/
--rw-r--r--   0 robert     (501) staff       (20)     4658 2024-01-30 17:26:50.000000 immanuel-1.2.4/immanuel/reports/aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     7581 2024-01-20 00:30:03.000000 immanuel-1.2.4/immanuel/reports/dignity.py
--rw-r--r--   0 robert     (501) staff       (20)     2132 2024-01-20 00:32:00.000000 immanuel-1.2.4/immanuel/reports/pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/reports/weighting.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.591399 immanuel-1.2.4/immanuel/resources/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.641405 immanuel-1.2.4/immanuel/resources/ephemeris/
--rw-r--r--   0 robert     (501) staff       (20)   225863 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/seas_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   225440 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/seas_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   225108 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/seas_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1306782 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/semo_12.se1
--rw-r--r--   0 robert     (501) staff       (20)  1305686 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/semo_18.se1
--rw-r--r--   0 robert     (501) staff       (20)  1309017 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/semo_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1326257 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/semo_36.se1
--rw-r--r--   0 robert     (501) staff       (20)  1339659 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/semo_42.se1
--rw-r--r--   0 robert     (501) staff       (20)   483763 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/sepl_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   484065 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/sepl_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   483399 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/sepl_24.se1
--rw-r--r--   0 robert     (501) staff       (20)   484686 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/sepl_36.se1
--rw-r--r--   0 robert     (501) staff       (20)   483628 2023-12-02 01:56:03.000000 immanuel-1.2.4/immanuel/resources/ephemeris/sepl_42.se1
--rw-r--r--   0 robert     (501) staff       (20)    11277 2024-01-21 02:46:23.000000 immanuel-1.2.4/immanuel/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.649444 immanuel-1.2.4/immanuel/tools/
--rw-r--r--   0 robert     (501) staff       (20)     3197 2024-02-02 15:17:22.000000 immanuel-1.2.4/immanuel/tools/calculate.py
--rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/tools/convert.py
--rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.2.4/immanuel/tools/date.py
--rw-r--r--   0 robert     (501) staff       (20)    20967 2024-01-20 00:27:15.000000 immanuel-1.2.4/immanuel/tools/ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     5702 2024-01-20 00:28:24.000000 immanuel-1.2.4/immanuel/tools/find.py
--rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/tools/forecast.py
--rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/tools/midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2786 2024-01-16 22:54:01.000000 immanuel-1.2.4/immanuel/tools/position.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.659417 immanuel-1.2.4/immanuel.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)    46396 2024-03-19 16:30:48.000000 immanuel-1.2.4/immanuel.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     1601 2024-03-19 16:30:48.000000 immanuel-1.2.4/immanuel.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2024-03-19 16:30:48.000000 immanuel-1.2.4/immanuel.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       60 2024-03-19 16:30:48.000000 immanuel-1.2.4/immanuel.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)        9 2024-03-19 16:30:48.000000 immanuel-1.2.4/immanuel.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)     1070 2024-03-19 16:25:56.000000 immanuel-1.2.4/pyproject.toml
--rw-r--r--   0 robert     (501) staff       (20)       38 2024-03-19 16:30:48.660162 immanuel-1.2.4/setup.cfg
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-03-19 16:30:48.659228 immanuel-1.2.4/tests/
--rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.2.4/tests/se01181s.se1
--rw-r--r--   0 robert     (501) staff       (20)     3920 2024-01-19 14:41:23.000000 immanuel-1.2.4/tests/test_aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     3530 2024-01-20 00:34:00.000000 immanuel-1.2.4/tests/test_calculate.py
--rw-r--r--   0 robert     (501) staff       (20)    23296 2024-02-05 00:14:17.000000 immanuel-1.2.4/tests/test_charts.py
--rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.2.4/tests/test_convert.py
--rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.2.4/tests/test_date.py
--rw-r--r--   0 robert     (501) staff       (20)     9602 2024-01-19 14:31:30.000000 immanuel-1.2.4/tests/test_dignity.py
--rw-r--r--   0 robert     (501) staff       (20)    15020 2024-01-21 00:36:19.000000 immanuel-1.2.4/tests/test_ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.2.4/tests/test_find.py
--rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.2.4/tests/test_forecast.py
--rw-r--r--   0 robert     (501) staff       (20)     5374 2024-01-20 20:36:20.000000 immanuel-1.2.4/tests/test_midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.2.4/tests/test_pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     5109 2024-01-21 00:35:39.000000 immanuel-1.2.4/tests/test_position.py
--rw-r--r--   0 robert     (501) staff       (20)     3240 2024-02-03 02:11:39.000000 immanuel-1.2.4/tests/test_setup.py
--rw-r--r--   0 robert     (501) staff       (20)     2286 2024-01-20 20:36:05.000000 immanuel-1.2.4/tests/test_weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.694680 immanuel-1.3.1/
+-rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.3.1/LICENSE.md
+-rw-r--r--   0 robert     (501) staff       (20)       21 2023-12-02 01:56:03.000000 immanuel-1.3.1/MANIFEST.in
+-rw-r--r--   0 robert     (501) staff       (20)    49211 2024-04-16 01:32:34.694393 immanuel-1.3.1/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)    11218 2024-04-16 01:30:39.000000 immanuel-1.3.1/README.md
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.629694 immanuel-1.3.1/immanuel/
+-rw-r--r--   0 robert     (501) staff       (20)       66 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    18861 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/charts.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.634036 immanuel-1.3.1/immanuel/classes/
+-rw-r--r--   0 robert     (501) staff       (20)      619 2024-04-01 00:34:17.000000 immanuel-1.3.1/immanuel/classes/cache.py
+-rw-r--r--   0 robert     (501) staff       (20)     2158 2024-04-16 01:25:04.000000 immanuel-1.3.1/immanuel/classes/localize.py
+-rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/classes/serialize.py
+-rw-r--r--   0 robert     (501) staff       (20)    12561 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/classes/wrap.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.639209 immanuel-1.3.1/immanuel/const/
+-rw-r--r--   0 robert     (501) staff       (20)     2325 2024-01-20 20:33:35.000000 immanuel-1.3.1/immanuel/const/calc.py
+-rw-r--r--   0 robert     (501) staff       (20)     2613 2023-12-15 16:02:49.000000 immanuel-1.3.1/immanuel/const/chart.py
+-rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/const/data.py
+-rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/const/dignities.py
+-rw-r--r--   0 robert     (501) staff       (20)      255 2024-04-08 01:17:15.000000 immanuel-1.3.1/immanuel/const/genders.py
+-rw-r--r--   0 robert     (501) staff       (20)     5692 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/const/names.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.626393 immanuel-1.3.1/immanuel/locales/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.640114 immanuel-1.3.1/immanuel/locales/pt_BR/
+-rw-r--r--   0 robert     (501) staff       (20)     2045 2024-04-15 00:27:49.000000 immanuel-1.3.1/immanuel/locales/pt_BR/mappings.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.642463 immanuel-1.3.1/immanuel/reports/
+-rw-r--r--   0 robert     (501) staff       (20)     4658 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/reports/aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     7581 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/reports/dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)     2186 2024-04-16 01:27:34.000000 immanuel-1.3.1/immanuel/reports/pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/reports/weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.626597 immanuel-1.3.1/immanuel/resources/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.676464 immanuel-1.3.1/immanuel/resources/ephemeris/
+-rw-r--r--   0 robert     (501) staff       (20)   225863 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/seas_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225440 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/seas_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225108 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/seas_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1306782 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/semo_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1305686 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/semo_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1309017 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/semo_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1326257 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/semo_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1339659 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/semo_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483763 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/sepl_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484065 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/sepl_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483399 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/sepl_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484686 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/sepl_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483628 2024-03-29 02:29:31.000000 immanuel-1.3.1/immanuel/resources/ephemeris/sepl_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)    11845 2024-04-16 01:24:46.000000 immanuel-1.3.1/immanuel/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.683530 immanuel-1.3.1/immanuel/tools/
+-rw-r--r--   0 robert     (501) staff       (20)     3197 2024-02-02 15:17:22.000000 immanuel-1.3.1/immanuel/tools/calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/tools/convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.3.1/immanuel/tools/date.py
+-rw-r--r--   0 robert     (501) staff       (20)    21046 2024-04-01 00:06:06.000000 immanuel-1.3.1/immanuel/tools/ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     5702 2024-04-09 19:59:42.000000 immanuel-1.3.1/immanuel/tools/find.py
+-rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/tools/forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/tools/midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2786 2024-01-16 22:54:01.000000 immanuel-1.3.1/immanuel/tools/position.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.693886 immanuel-1.3.1/immanuel.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)    49211 2024-04-16 01:32:34.000000 immanuel-1.3.1/immanuel.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     1765 2024-04-16 01:32:34.000000 immanuel-1.3.1/immanuel.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-16 01:32:34.000000 immanuel-1.3.1/immanuel.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       60 2024-04-16 01:32:34.000000 immanuel-1.3.1/immanuel.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)        9 2024-04-16 01:32:34.000000 immanuel-1.3.1/immanuel.egg-info/top_level.txt
+-rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-16 01:29:35.000000 immanuel-1.3.1/pyproject.toml
+-rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-16 01:32:34.694728 immanuel-1.3.1/setup.cfg
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-16 01:32:34.693676 immanuel-1.3.1/tests/
+-rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.3.1/tests/se01181s.se1
+-rw-r--r--   0 robert     (501) staff       (20)     3920 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     3530 2024-01-20 00:34:00.000000 immanuel-1.3.1/tests/test_calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)    23308 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_charts.py
+-rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.3.1/tests/test_convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.3.1/tests/test_date.py
+-rw-r--r--   0 robert     (501) staff       (20)     9521 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)    15068 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.3.1/tests/test_find.py
+-rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.3.1/tests/test_forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)    18927 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_localization.py
+-rw-r--r--   0 robert     (501) staff       (20)     5374 2024-01-20 20:36:20.000000 immanuel-1.3.1/tests/test_midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.3.1/tests/test_pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     5157 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_position.py
+-rw-r--r--   0 robert     (501) staff       (20)     3169 2024-04-16 01:27:34.000000 immanuel-1.3.1/tests/test_setup.py
+-rw-r--r--   0 robert     (501) staff       (20)     2286 2024-04-01 00:40:36.000000 immanuel-1.3.1/tests/test_weighting.py
```

### Comparing `immanuel-1.2.4/LICENSE.md` & `immanuel-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/PKG-INFO` & `immanuel-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.2.4
+Version: 1.3.1
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -648,15 +648,25 @@
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.2.4/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+
+## Translations
+
+Immanuel is currently available in the following locales / languages:
+
+* **en_US:** (default) US English
+* **pt_BR:** Brazilian Portuguese
+* Coming soon: Spanish translation
+
+See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -679,16 +689,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House
-Moon 16°19'29" in Scorpio, 8th House
+Sun 10°37'26" in Capricorn, 11th House, Direct
+Moon 16°19'29" in Scorpio, 8th House, Direct
+Mercury 02°16'43" in Capricorn, 10th House, Direct
+Venus 01°52'05" in Sagittarius, 9th House, Direct
+Mars 28°09'26" in Aquarius, 12th House, Direct
+Jupiter 25°15'48" in Aries, 2nd House, Direct
+Saturn 10°23'27" in Taurus, 2nd House, Retrograde
+Uranus 14°49'19" in Aquarius, 12th House, Direct
+Neptune 03°12'07" in Aquarius, 12th House, Direct
+Pluto 11°27'49" in Sagittarius, 9th House, Direct
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -708,15 +726,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House
+Ceres 04°30'28" in Libra, 7th House, Direct
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -767,15 +785,21 @@
         "direction": "+",
         "degrees": 10,
         "minutes": 37,
         "seconds": 26
     },
     "sign": {
         "number": 10,
-        "name": "Capricorn"
+        "name": "Capricorn",
+        "element": "Earth",
+        "modality": "Cardinal"
+    },
+    "decan": {
+        "number": 2,
+        "name": "2nd Decan"
     },
     "house": {
         "index": 2000011,
         "number": 11,
         "name": "11th House"
     },
     "distance": 0.9833259257690341,
@@ -884,10 +908,34 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
+
+## Contributions
+
+New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
+
+* Fork the repo.
+* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
+* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
+* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
+* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
+```
+msgctxt "masculine"
+msgid "Applicative"
+msgstr "Aplicativo"
+
+msgctxt "feminine"
+msgid "Applicative"
+msgstr "Aplicativa"
+```
+* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
+* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
+* If everything looks good, I will merge to master & prep a new release!
+
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.2.4/README.md` & `immanuel-1.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,25 @@
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.2.4/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+
+## Translations
+
+Immanuel is currently available in the following locales / languages:
+
+* **en_US:** (default) US English
+* **pt_BR:** Brazilian Portuguese
+* Coming soon: Spanish translation
+
+See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -42,16 +52,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House
-Moon 16°19'29" in Scorpio, 8th House
+Sun 10°37'26" in Capricorn, 11th House, Direct
+Moon 16°19'29" in Scorpio, 8th House, Direct
+Mercury 02°16'43" in Capricorn, 10th House, Direct
+Venus 01°52'05" in Sagittarius, 9th House, Direct
+Mars 28°09'26" in Aquarius, 12th House, Direct
+Jupiter 25°15'48" in Aries, 2nd House, Direct
+Saturn 10°23'27" in Taurus, 2nd House, Retrograde
+Uranus 14°49'19" in Aquarius, 12th House, Direct
+Neptune 03°12'07" in Aquarius, 12th House, Direct
+Pluto 11°27'49" in Sagittarius, 9th House, Direct
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -71,15 +89,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House
+Ceres 04°30'28" in Libra, 7th House, Direct
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -130,15 +148,21 @@
         "direction": "+",
         "degrees": 10,
         "minutes": 37,
         "seconds": 26
     },
     "sign": {
         "number": 10,
-        "name": "Capricorn"
+        "name": "Capricorn",
+        "element": "Earth",
+        "modality": "Cardinal"
+    },
+    "decan": {
+        "number": 2,
+        "name": "2nd Decan"
     },
     "house": {
         "index": 2000011,
         "number": 11,
         "name": "11th House"
     },
     "distance": 0.9833259257690341,
@@ -247,10 +271,34 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
+
+## Contributions
+
+New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
+
+* Fork the repo.
+* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
+* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
+* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
+* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
+```
+msgctxt "masculine"
+msgid "Applicative"
+msgstr "Aplicativo"
+
+msgctxt "feminine"
+msgid "Applicative"
+msgstr "Aplicativa"
+```
+* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
+* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
+* If everything looks good, I will merge to master & prep a new release!
+
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.2.4/immanuel/charts.py` & `immanuel-1.3.1/immanuel/charts.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 """
 
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 from immanuel.classes import wrap
+from immanuel.classes.localize import _
 from immanuel.const import chart, names
-from immanuel.reports import aspect, pattern, weighting
+from immanuel.reports import aspect, pattern
 from immanuel.setup import settings
 from immanuel.tools import calculate, convert, date, ephemeris, forecast, midpoint, position
 
 
 class Subject:
     """ Simple class to model a chart subject - essentially just
     a time and place. """
@@ -38,19 +39,19 @@
                 lon=self.longitude,
                 is_dst=time_is_dst
             )
         self.date_time_ambiguous = date.ambiguous(self.date_time) and time_is_dst is None
         self.julian_date = date.to_jd(self.date_time)
 
 
-class Chart():
+class Chart:
     """ Base chart class. This acts as an abstract class for the actual chart
     classes to inherit from. """
     def __init__(self, type: int, aspects_to: 'Chart' = None) -> None:
-        self.type = names.CHART_TYPES[type]
+        self.type = _(names.CHART_TYPES[type])
         self._type = type
         self._aspects_to = aspects_to
         self.generate()
         self.wrap()
 
     def house_for(self, object: wrap.Object) -> int:
         """ Returns the index of the house where any passed arbitrary object
@@ -77,18 +78,18 @@
                 getattr(self, method)()
 
     # Base class provides wrappers for properties common to all classes.
     def set_wrapped_native(self) -> None:
         self.native = wrap.Subject(self._native)
 
     def set_wrapped_house_system(self) -> None:
-        self.house_system = names.HOUSE_SYSTEMS[settings.house_system]
+        self.house_system = _(names.HOUSE_SYSTEMS[settings.house_system])
 
     def set_wrapped_shape(self) -> None:
-        self.shape = names.CHART_SHAPES[pattern.chart_shape(self._objects)]
+        self.shape = _(names.CHART_SHAPES[pattern.chart_shape(self._objects)])
 
     def set_wrapped_diurnal(self) -> None:
         self.diurnal = self._diurnal
 
     def set_wrapped_moon_phase(self) -> None:
         self.moon_phase = wrap.MoonPhase(self._moon_phase)
 
@@ -113,19 +114,15 @@
         self.houses = {index: wrap.Object(object=house) for index, house in self._houses.items()}
 
     def set_wrapped_aspects(self) -> None:
         aspects = aspect.all(self._objects) if self._aspects_to is None else aspect.synastry(self._objects, self._aspects_to._objects)
         self.aspects = {index: {object_index: wrap.Aspect(aspect=object_aspect, objects=self._objects) for object_index, object_aspect in aspect_list.items()} for index, aspect_list in aspects.items()}
 
     def set_wrapped_weightings(self) -> None:
-        self.weightings = {
-            'elements': wrap.Elements(weighting.elements(self._objects)),
-            'modalities': wrap.Modalities(weighting.modalities(self._objects)),
-            'quadrants': wrap.Quadrants(weighting.quadrants(self._objects, self._houses)),
-        }
+        self.weightings = wrap.Weightings(self._objects, self._houses)
 
 
 class Natal(Chart):
     """ Standard natal chart generates data straight from the passed
     native information. """
     def __init__(self, native: Subject, aspects_to: Chart = None) -> None:
         self._native = native
@@ -293,15 +290,15 @@
                 dt=self._progressed_jd,
                 armc=self._progressed_armc_longitude,
                 latitude=self._native.latitude,
                 longitude=self._native.longitude,
             )
 
     def set_wrapped_progression_method(self) -> None:
-        self.progression_method = names.PROGRESSION_METHODS[settings.mc_progression_method]
+        self.progression_method = _(names.PROGRESSION_METHODS[settings.mc_progression_method])
 
 
 class Composite(Chart):
     """ Generates a midpoint chart based on the two passed sets of data. """
     def __init__(self, native: Subject, partner: Subject, aspects_to: Chart = None) -> None:
         self._native = native
         self._partner = partner
```

### Comparing `immanuel-1.2.4/immanuel/classes/serialize.py` & `immanuel-1.3.1/immanuel/classes/serialize.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/classes/wrap.py` & `immanuel-1.3.1/immanuel/classes/wrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     JSON keys are defined here, either explicitly or as class members.
 
 """
 
 from datetime import datetime
 
 from immanuel.const import calc, chart, dignities, names
-from immanuel.reports import dignity
+from immanuel.reports import dignity, weighting
 from immanuel.setup import settings
 from immanuel.tools import calculate, convert, date, ephemeris, position
+from immanuel.classes.localize import gender, _
 
 
 class Angle:
     def __init__(self, angle: float, format: int = convert.FORMAT_DMS) -> None:
         self.raw = angle
         self.formatted = convert.dec_to_string(angle, format)
         self.direction = None
@@ -33,42 +34,49 @@
 
 class Aspect:
     def __init__(self, aspect: dict, objects: dict) -> None:
         self._active_name = objects[aspect['active']]['name']
         self._passive_name = objects[aspect['passive']]['name']
         self.active = aspect['active']
         self.passive = aspect['passive']
-        self.type = names.ASPECTS[aspect['aspect']]
+        self.type = _(names.ASPECTS[aspect['aspect']])
         self.aspect = aspect['aspect']
         self.orb = aspect['orb']
         self.distance = Angle(aspect['distance'])
         self.difference = Angle(aspect['difference'])
-        self.movement = AspectMovement(aspect['movement'])
-        self.condition = AspectCondition(aspect['condition'])
+        self.movement = AspectMovement(aspect)
+        self.condition = AspectCondition(aspect)
 
     def __str__(self) -> str:
-        return f'{self._active_name} {self._passive_name} {self.type} within {self.difference} ({self.movement}, {self.condition})'
+        return _('{active} {passive} {type} within {difference} ({movement}, {condition})').format(
+                active=self._active_name,
+                passive=self._passive_name,
+                type=self.type,
+                difference = self.difference,
+                movement = self.movement,
+                condition = self.condition,
+            )
 
 
 class AspectCondition:
-    def __init__(self, condition: int) -> None:
-        self.associate = condition == calc.ASSOCIATE
-        self.dissociate = condition == calc.DISSOCIATE
-        self.formatted = names.ASPECT_CONDITIONS[condition]
+    def __init__(self, aspect: dict) -> None:
+        self.associate = aspect['condition'] == calc.ASSOCIATE
+        self.dissociate = aspect['condition'] == calc.DISSOCIATE
+        self.formatted = _(names.ASPECT_CONDITIONS[aspect['condition']], gender(aspect['aspect']))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class AspectMovement:
-    def __init__(self, movement: int) -> None:
-        self.applicative = movement == calc.APPLICATIVE
-        self.exact = movement == calc.EXACT
-        self.separative = movement == calc.SEPARATIVE
-        self.formatted = names.ASPECT_MOVEMENTS[movement]
+    def __init__(self, aspect: dict) -> None:
+        self.applicative = aspect['movement'] == calc.APPLICATIVE
+        self.exact = aspect['movement'] == calc.EXACT
+        self.separative = aspect['movement'] == calc.SEPARATIVE
+        self.formatted = _(names.ASPECT_MOVEMENTS[aspect['movement']], gender(aspect['aspect']))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class Coordinates:
     def __init__(self, latitude: float, longitude: float) -> None:
@@ -87,51 +95,60 @@
         self.julian = date.to_jd(dt)
         self.deltat = ephemeris.deltat(self.julian)
 
         if armc is not None:
             self.sidereal_time = convert.dec_to_string(calculate.sidereal_time(armc), convert.FORMAT_TIME)
 
     def __str__(self) -> str:
-        str = f'{self.datetime.strftime("%a %b %d %Y %I:%M:%S %p")} {self.timezone}'
+        str = f"{self.datetime.strftime('%a %b %d %Y %H:%M:%S')} {self.timezone}"
 
         if self.ambiguous:
-            str += ' (ambiguous)'
+            str += f" ({_('ambiguous')})"
 
         return str
 
 
+class Decan:
+    def __init__(self, number: int) -> None:
+        self.number = number
+        self.name = _(names.DECANS[self.number])
+
+    def __str__(self) -> str:
+        return self.name
+
+
 class DignityState:
-    def __init__(self, dignity_state: dict) -> None:
+    def __init__(self, object: dict, dignity_state: dict) -> None:
         self.ruler = dignity_state[dignities.RULER]
         self.exalted = dignity_state[dignities.EXALTED]
         self.triplicity_ruler = dignity_state[dignities.TRIPLICITY_RULER]
         self.term_ruler = dignity_state[dignities.TERM_RULER]
         self.face_ruler = dignity_state[dignities.FACE_RULER]
         self.mutual_reception_ruler = dignity_state[dignities.MUTUAL_RECEPTION_RULER]
         self.mutual_reception_exalted = dignity_state[dignities.MUTUAL_RECEPTION_EXALTED]
         self.mutual_reception_triplicity_ruler = dignity_state[dignities.MUTUAL_RECEPTION_TRIPLICITY_RULER]
         self.mutual_reception_term_ruler = dignity_state[dignities.MUTUAL_RECEPTION_TERM_RULER]
         self.mutual_reception_face_ruler = dignity_state[dignities.MUTUAL_RECEPTION_FACE_RULER]
         self.detriment = dignity_state[dignities.DETRIMENT]
         self.fall = dignity_state[dignities.FALL]
         self.peregrine = dignity_state[dignities.PEREGRINE]
-        self.formatted = [names.DIGNITIES[dignity] for dignity, active in dignity_state.items() if active]
+        self.formatted = [_(names.DIGNITIES[dignity], gender(object['index'])) for dignity, active in dignity_state.items() if active]
 
     def __str__(self) -> str:
         return ', '.join(self.formatted)
 
 
 class EclipseType:
     def __init__(self, eclipse_type: int) -> None:
         self.total = eclipse_type == chart.TOTAL
         self.annular = eclipse_type == chart.ANNULAR
         self.partial = eclipse_type == chart.PARTIAL
         self.annular_total = eclipse_type == chart.ANNULAR_TOTAL
         self.penumbral = eclipse_type == chart.PENUMBRAL
-        self.formatted = names.ECLIPSE_TYPES[eclipse_type]
+        self.formatted = _(names.ECLIPSE_TYPES[eclipse_type])
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class House:
     def __init__(self, house: dict) -> None:
@@ -149,15 +166,15 @@
         self.waxing_crescent = moon_phase == calc.WAXING_CRESCENT
         self.first_quarter = moon_phase == calc.FIRST_QUARTER
         self.waxing_gibbous = moon_phase == calc.WAXING_GIBBOUS
         self.full_moon = moon_phase == calc.FULL_MOON
         self.disseminating = moon_phase == calc.DISSEMINATING
         self.third_quarter = moon_phase == calc.THIRD_QUARTER
         self.balsamic = moon_phase == calc.BALSAMIC
-        self.formatted = names.MOON_PHASES[moon_phase]
+        self.formatted = _(names.MOON_PHASES[moon_phase])
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class Object:
     def __init__(self, object: dict, objects: dict = None, houses: dict = None, is_daytime: bool = None, obliquity: float = None) -> None:
@@ -177,14 +194,15 @@
 
         if 'lat' in object:
             self.latitude = Angle(object['lat'])
 
         self.longitude = Angle(object['lon'])
         self.sign_longitude = Angle(position.sign_longitude(object))
         self.sign = Sign(position.sign(object))
+        self.decan = Decan(position.decan(object))
 
         if houses is not None:
             self.house = House(position.house(object, houses))
 
         if 'dist' in object:
             self.distance = object['dist']
 
@@ -200,51 +218,60 @@
                 self.out_of_bounds = calculate.is_out_of_bounds(object=object, obliquity=obliquity)
 
         if 'size' in object:
             self.size = object['size']
 
         if objects is not None and object['type'] == chart.PLANET and is_daytime is not None and calc.PLANETS.issubset(objects):
             dignity_state = dignity.all(object=object, objects=objects, is_daytime=is_daytime)
-            self.dignities = DignityState(dignity_state)
+            self.dignities = DignityState(object=object, dignity_state=dignity_state)
             self.score = dignity.score(dignity_state)
 
     def __str__(self) -> str:
-        str = f'{self.name} {self.sign_longitude} in {self.sign}'
+        formatted = _('{name} {longitude} in {sign}').format(
+                name=self.name,
+                longitude=self.sign_longitude,
+                sign=self.sign,
+            )
 
         if hasattr(self, 'house'):
-            str += f', {self.house.name}'
+            formatted += f', {_(self.house)}'
 
-        return str
+        if hasattr(self, 'movement'):
+            formatted += f', {_(self.movement)}'
+
+        return formatted
 
 
 class ObjectMovement:
     def __init__(self, object: dict) -> None:
         self._movement = calculate.object_movement(object)
         self.direct = self._movement == calc.DIRECT
         self.stationary = self._movement == calc.STATIONARY
         self.retrograde = self._movement == calc.RETROGRADE
-        self.formatted = names.OBJECT_MOVEMENTS[self._movement]
+        self.formatted = _(names.OBJECT_MOVEMENTS[self._movement], gender(object['index']))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class ObjectType:
     def __init__(self, type: int) -> None:
         self.index = type
-        self.name = names.OBJECTS[type]
+        self.name = _(names.OBJECTS[type])
 
     def __str__(self) -> str:
         return self.name
 
 
 class Sign:
     def __init__(self, number: int) -> None:
         self.number = number
-        self.name = names.SIGNS[self.number]
+        self.name = _(names.SIGNS[self.number])
+        self.element = _(names.ELEMENTS[position.element((self.number-1) * 30)])
+        self.modality = _(names.MODALITIES[position.modality((self.number-1) * 30)])
 
     def __str__(self) -> str:
         return self.name
 
 
 class Subject:
     def __init__(self, subject: 'Subject') -> None:
@@ -264,40 +291,54 @@
             )
         self.coordinates = Coordinates(
                 latitude=subject.latitude,
                 longitude=subject.longitude,
             )
 
     def __str__(self) -> str:
-        return f'{self.date_time} at {self.coordinates}'
+        return _('{date_time} at {lat}, {lon}').format(
+                date_time=self.date_time,
+                lat=self.coordinates.latitude,
+                lon=self.coordinates.longitude,
+            )
+
+
+class Weightings:
+    def __init__(self, objects: dict, houses: dict) -> None:
+        self.elements = Elements(weighting.elements(objects))
+        self.modalities = Modalities(weighting.modalities(objects))
+        self.quadrants = Quadrants(weighting.quadrants(objects, houses))
+
+    def __str__(self) -> str:
+        return f'{self.elements}\n{self.modalities}\n{self.quadrants}'
 
 
 class Elements:
     def __init__(self, elements: dict) -> None:
         self.fire = elements[chart.FIRE]
         self.earth = elements[chart.EARTH]
         self.air = elements[chart.AIR]
         self.water = elements[chart.WATER]
 
     def __str__(self) -> str:
-        return f'Fire: {len(self.fire)}, Earth: {len(self.earth)}, Air: {len(self.air)}, Water: {len(self.water)}'
+        return f"{_('Fire')}: {len(self.fire)}, {_('Earth')}: {len(self.earth)}, {_('Air')}: {len(self.air)}, {_('Water')}: {len(self.water)}"
 
 
 class Modalities:
     def __init__(self, modalities: dict) -> None:
         self.cardinal = modalities[chart.CARDINAL]
         self.fixed = modalities[chart.FIXED]
         self.mutable = modalities[chart.MUTABLE]
 
     def __str__(self) -> str:
-        return f'Cardinal: {len(self.cardinal)}, Fixed: {len(self.fixed)}, Mutable: {len(self.mutable)}'
+        return f"{_('Cardinal')}: {len(self.cardinal)}, {_('Fixed')}: {len(self.fixed)}, {_('Mutable')}: {len(self.mutable)}"
 
 
 class Quadrants:
     def __init__(self, quadrants: dict) -> None:
         self.first = quadrants[1]
         self.second = quadrants[2]
         self.third = quadrants[3]
         self.fourth = quadrants[4]
 
     def __str__(self) -> str:
-        return f'First: {len(self.first)}, Second: {len(self.second)}, Third: {len(self.third)}, Fourth: {len(self.fourth)}'
+        return f"{_('First')}: {len(self.first)}, {_('Second')}: {len(self.second)}, {_('Third')}: {len(self.third)}, {_('Fourth')}: {len(self.fourth)}"
```

### Comparing `immanuel-1.2.4/immanuel/const/calc.py` & `immanuel-1.3.1/immanuel/const/calc.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/const/chart.py` & `immanuel-1.3.1/immanuel/const/chart.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/const/data.py` & `immanuel-1.3.1/immanuel/const/data.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/const/dignities.py` & `immanuel-1.3.1/immanuel/const/dignities.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/const/names.py` & `immanuel-1.3.1/immanuel/const/names.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/reports/aspect.py` & `immanuel-1.3.1/immanuel/reports/aspect.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/reports/dignity.py` & `immanuel-1.3.1/immanuel/reports/dignity.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/reports/pattern.py` & `immanuel-1.3.1/immanuel/reports/pattern.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 def chart_shape(objects: dict) -> int:
     """ Returns which of the predetermined shapes the passed
     chart objects form. """
     # Filter objects
     objects = { k: v for k, v in objects.items() if k in settings.chart_shape_objects }
 
+    if len(objects) <= 1:
+        return calc.SPLASH
+
     # Sort objects by longitude
     longitudes = sorted([v['lon'] for v in objects.values()])
     diffs = [swe.difdegn(_next(longitudes, k), v) for k, v in enumerate(longitudes)]
     max_diff = max(diffs)
 
     # All planets within 120º can only be a bundle
     if max_diff >= 240-settings.chart_shape_orb:
```

### Comparing `immanuel-1.2.4/immanuel/reports/weighting.py` & `immanuel-1.3.1/immanuel/reports/weighting.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/seas_12.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/seas_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/seas_18.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/seas_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/seas_24.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/seas_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/semo_12.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/semo_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/semo_18.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/semo_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/semo_24.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/semo_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/semo_36.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/semo_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/semo_42.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/semo_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/sepl_12.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/sepl_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/sepl_18.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/sepl_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/sepl_24.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/sepl_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/sepl_36.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/sepl_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/resources/ephemeris/sepl_42.se1` & `immanuel-1.3.1/immanuel/resources/ephemeris/sepl_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/setup.py` & `immanuel-1.3.1/immanuel/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 """
 
 import os
 from typing import Any
 
 import swisseph as swe
 
+from immanuel.classes.localize import Localize
 from immanuel.const import calc, chart, data, dignities
 
 
 class BaseSettings:
     def __init__(self) -> None:
+        """ Set locale. """
+        self._locale = None
+
         """ Default ephemeris file path. """
-        self._file_path = None
-        self.add_filepath(f'{os.path.dirname(__file__)}{os.sep}resources{os.sep}ephemeris')
+        self._file_path = f'{os.path.dirname(__file__)}{os.sep}resources{os.sep}ephemeris'
 
         """ Data that should be included for each chart type's output. """
         self.chart_data = {
             chart.NATAL: [
                 data.NATIVE,
                 data.HOUSE_SYSTEM,
                 data.SHAPE,
@@ -196,14 +199,23 @@
         self._default_aspect_rule = {}
         self._planet_aspect_rule = {}
         self._point_aspect_rule = {}
         self._aspect_rules = {}
         self._orbs = {}
 
     @property
+    def locale(self) -> str:
+        return self._locale
+
+    @locale.setter
+    def locale(self, lcid: str) -> None:
+        self._locale = lcid
+        Localize.set_locale(lcid)
+
+    @property
     def default_aspect_rule(self) -> dict:
         """ Cascading setting - default aspects allowed for objects. """
         return  {
             'initiate': self.aspects,
             'receive': self.aspects,
         } | self._default_aspect_rule
 
@@ -303,32 +315,42 @@
 
     @orbs.setter
     def orbs(self, value: dict) -> None:
         self._orbs = value
 
     def add_filepath(self, path: str, default: bool = False) -> None:
         """ Add an ephemeris file path. """
-        if default or self._file_path is None:
+        if default:
             self._file_path = path
         else:
             extra_path = f'{os.pathsep}{path}'
 
             if self._file_path.endswith(extra_path):
                 return
 
             self._file_path += extra_path
 
+        self.set_swe_filepath()
+
+    def set_swe_filepath(self) -> None:
+        """ Pass defined path(s) to swisseph. """
         swe.set_ephe_path(self._file_path)
 
 
 class StaticSingleton(type):
     """ Metaclass to ensure singleton behavior & route everything to
     our BaseSettings instance to emulate static behavior. """
     _instance = BaseSettings()
 
+    def reset(cls) -> None:
+        """ Reset all settings to default. """
+        StaticSingleton._instance = BaseSettings()
+        StaticSingleton._instance.set_swe_filepath()
+        Localize.reset()
+
     def set(cls, values: dict) -> None:
         """ Helper mass-set method. """
         for key, value in values.items():
             setattr(StaticSingleton._instance, key, value)
 
     def __getattr__(cls, name: str) -> Any:
         return getattr(StaticSingleton._instance, name)
```

### Comparing `immanuel-1.2.4/immanuel/tools/calculate.py` & `immanuel-1.3.1/immanuel/tools/calculate.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/convert.py` & `immanuel-1.3.1/immanuel/tools/convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/date.py` & `immanuel-1.3.1/immanuel/tools/date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/ephemeris.py` & `immanuel-1.3.1/immanuel/tools/ephemeris.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
     Many of the functions here, including angle, house and vertex functions,
     have an "armc_"-prefixed alternative if they are required to calculate
     from an ARMC.
 
 """
 
-from functools import cache
-
 import swisseph as swe
 
 from immanuel.const import chart, names
+from immanuel.classes.cache import cache
 from immanuel.tools import calculate, find
+from immanuel.classes.localize import _
 
 
 ALL = -1
 
 _SWE = {
     chart.ALCABITUS: b'B',
     chart.AZIMUTHAL: b'H',
@@ -369,15 +369,15 @@
     ec_res = swe.calc_ut(jd, _SWE[index])[0]
     eq_res = swe.cotrans((ec_res[0], ec_res[1], ec_res[2]), -obliquity(jd))
     asteroid = _type(index) == chart.ASTEROID
 
     return {
         'index': index,
         'type': chart.ASTEROID if asteroid else chart.PLANET,
-        'name': names.ASTEROIDS[index] if asteroid else names.PLANETS[index],
+        'name': _(names.ASTEROIDS[index] if asteroid else names.PLANETS[index]),
         'lon': ec_res[0],
         'lat': ec_res[1],
         'dist': ec_res[2],
         'speed': ec_res[3],
         'dec': eq_res[1],
     }
 
@@ -445,15 +445,15 @@
             ec_res = swe.calc_ut(eclipse_jd, swe.MOON)[0]
 
     eq_res = swe.cotrans((ec_res[0], ec_res[1], ec_res[2]), -obliquity(jd))
 
     return {
         'index': index,
         'type': chart.ECLIPSE,
-        'name': names.ECLIPSES[index],
+        'name': _(names.ECLIPSES[index]),
         'eclipse_type': eclipse_type,
         'jd': eclipse_jd,
         'lon': ec_res[0],
         'lat': ec_res[1],
         'dist': ec_res[2],
         'speed': 0.0,
         'dec': eq_res[1],
@@ -539,27 +539,27 @@
         lon = ascmc[_SWE[i]]
         speed = ascmcspeed[_SWE[i]]
         dec = swe.cotrans((lon, 0, 0), -obliquity)[1]
 
         angles[i] = {
             'index': i,
             'type': chart.ANGLE,
-            'name': names.ANGLES[i],
+            'name': _(names.ANGLES[i]),
             'lon': lon,
             'speed': speed,
             'dec': dec,
         }
 
         if i in (chart.ASC, chart.MC):
             index = chart.DESC if i == chart.ASC else chart.IC
 
             angles[index] = {
                 'index': index,
                 'type': chart.ANGLE,
-                'name': names.ANGLES[index],
+                'name': _(names.ANGLES[index]),
                 'lon': swe.degnorm(lon - 180),
                 'speed': speed,
                 'dec': dec * -1,
             }
 
     houses = {}
 
@@ -568,30 +568,30 @@
         size = swe.difdeg2n(cusps[i if i < 12 else 0], lon)
         speed = cuspsspeed[i-1]
         dec = swe.cotrans((lon, 0, 0), -obliquity)[1]
 
         houses[index] = {
             'index': index,
             'type': chart.HOUSE,
-            'name': names.HOUSES[index],
+            'name': _(names.HOUSES[index]),
             'number': i,
             'lon': lon,
             'size': size,
             'speed': speed,
             'dec': dec,
         }
 
     vertex_lon = ascmc[_SWE[chart.VERTEX]]
     vertex_speed = ascmcspeed[_SWE[chart.VERTEX]]
     vertex_dec = swe.cotrans((vertex_lon, 0, 0), -obliquity)[1]
 
     vertex = {
         'index': chart.VERTEX,
         'type': chart.POINT,
-        'name': names.POINTS[chart.VERTEX],
+        'name': _(names.POINTS[chart.VERTEX]),
         'lon': vertex_lon,
         'speed': vertex_speed,
         'dec': vertex_dec,
     }
 
     return {
         'angles': angles,
@@ -609,15 +609,15 @@
     distance = swe.difdeg2n(moon['lon'], sun['lon'])
     syzygy_jd = find.previous_new_moon(jd) if distance > 0 else find.previous_full_moon(jd)
     syzygy_moon = planet(chart.MOON, syzygy_jd)
 
     return {
         'index': chart.SYZYGY,
         'type': chart.POINT,
-        'name': names.POINTS[chart.SYZYGY],
+        'name': _(names.POINTS[chart.SYZYGY]),
         'lon': syzygy_moon['lon'],
         'lat': syzygy_moon['lat'],
         'speed': syzygy_moon['speed'],
         'dec': syzygy_moon['dec'],
     }
 
 
@@ -631,15 +631,15 @@
     asc = angle(chart.ASC, jd, lat, lon, chart.PLACIDUS) if armc is None else armc_angle(chart.ASC, armc, lat, armc_obliquity, chart.PLACIDUS)
     lon = calculate.pars_fortuna_longitude(sun, moon, asc, formula)
     dec = swe.cotrans((lon, 0, 0), -obliquity(jd))[1]
 
     return {
         'index': chart.PARS_FORTUNA,
         'type': chart.POINT,
-        'name': names.POINTS[chart.PARS_FORTUNA],
+        'name': _(names.POINTS[chart.PARS_FORTUNA]),
         'lon': lon,
         'lat': 0.0,
         'speed': 0.0,
         'dec': dec,
     }
 
 
@@ -651,15 +651,15 @@
     lat = res[1] if index not in (chart.NORTH_NODE, chart.TRUE_NORTH_NODE, chart.SOUTH_NODE, chart.TRUE_SOUTH_NODE) else 0.0
     speed = res[3]
     dec = swe.cotrans((lon, lat, 0), -obliquity(jd))[1]
 
     return {
         'index': index,
         'type': chart.POINT,
-        'name': names.POINTS[index],
+        'name': _(names.POINTS[index]),
         'lon': lon,
         'lat': lat,
         'speed': speed,
         'dec': dec,
     }
```

### Comparing `immanuel-1.2.4/immanuel/tools/find.py` & `immanuel-1.3.1/immanuel/tools/find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/forecast.py` & `immanuel-1.3.1/immanuel/tools/forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/midpoint.py` & `immanuel-1.3.1/immanuel/tools/midpoint.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel/tools/position.py` & `immanuel-1.3.1/immanuel/tools/position.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/immanuel.egg-info/PKG-INFO` & `immanuel-1.3.1/immanuel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.2.4
+Version: 1.3.1
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -648,15 +648,25 @@
 
 Data for natal charts, solar returns, progressions, and composites are available, as well as the ability to point the aspects from any one chart instance to the planets in another, creating a flexible method to build synastries.
 
 Simply pass in a date and coordinates to one of the available chart classes, and the returned instance will contain all data necessary to construct a full astrological chart. A serializer is bundled to easily output all data as JSON, or it can simply be printed out as human-readable text.
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.2.4/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+
+## Translations
+
+Immanuel is currently available in the following locales / languages:
+
+* **en_US:** (default) US English
+* **pt_BR:** Brazilian Portuguese
+* Coming soon: Spanish translation
+
+See [the documentation](https://github.com/theriftlab/immanuel-python/tree/v1.3.1/docs/5-settings.md#locale) on how to switch. The documentation itself is not currently available in other translations. To contribute translations, see [below](#contributions).
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -679,16 +689,24 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
 
 ```
-Sun 10°37'26" in Capricorn, 11th House
-Moon 16°19'29" in Scorpio, 8th House
+Sun 10°37'26" in Capricorn, 11th House, Direct
+Moon 16°19'29" in Scorpio, 8th House, Direct
+Mercury 02°16'43" in Capricorn, 10th House, Direct
+Venus 01°52'05" in Sagittarius, 9th House, Direct
+Mars 28°09'26" in Aquarius, 12th House, Direct
+Jupiter 25°15'48" in Aries, 2nd House, Direct
+Saturn 10°23'27" in Taurus, 2nd House, Retrograde
+Uranus 14°49'19" in Aquarius, 12th House, Direct
+Neptune 03°12'07" in Aquarius, 12th House, Direct
+Pluto 11°27'49" in Sagittarius, 9th House, Direct
 ...
 ```
 
 Add asteroid Ceres into the mix:
 
 ```python
 from immanuel import charts
@@ -708,15 +726,15 @@
 for object in natal.objects.values():
     print(object)
 ```
 
 Now you will see this appended to the list:
 
 ```
-Ceres 04°30'28" in Libra, 7th House
+Ceres 04°30'28" in Libra, 7th House, Direct
 ```
 
 More on the settings & constants in the full documentation - for now, we can see much more data by serializing the chart's `objects` property to JSON like this:
 
 ```python
 import json
 
@@ -767,15 +785,21 @@
         "direction": "+",
         "degrees": 10,
         "minutes": 37,
         "seconds": 26
     },
     "sign": {
         "number": 10,
-        "name": "Capricorn"
+        "name": "Capricorn",
+        "element": "Earth",
+        "modality": "Cardinal"
+    },
+    "decan": {
+        "number": 2,
+        "name": "2nd Decan"
     },
     "house": {
         "index": 2000011,
         "number": 11,
         "name": "11th House"
     },
     "distance": 0.9833259257690341,
@@ -884,10 +908,34 @@
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the [GNU Affero General Public License](LICENSE.md) for more details.
 
 ## Credits
 
 Immanuel is forever indebted to the pioneering work of Alois Treindl and Dieter Koch at Astrodienst, and to João Ventura for the incredibly detailed [flatlib](https://github.com/flatangle/flatlib) which first inspired the development of this package.
 
+A big thank-you goes to Nathan Octavio who suggested translations, and who translated Immanuel into Brazilian Portuguese.
+
+## Contributions
+
+New translations for Immanuel's output are always welcome, although it is currently geared to Western-European languages. If you would like to contribute a translation, follow these steps:
+
+* Fork the repo.
+* Create a branch named after the locale, eg. `translations/pr_BR` - locale names for various languages can be found online, for example [here](https://learn.microsoft.com/en-us/openspecs/office_standards/ms-oe376/6c085406-a698-4e12-9d4d-c3b0ee3dbc4a), although you should use an underscore rather than a hyphen.
+* Create a subdirectory in `/immanuel/locales` named after your locale code, and another sub-directory under this called `LC_MESSAGES`.
+* Copy `locales/immanuel.pot` into the new `LC_MESSAGES` sub-directory and rename it `immanuel.po`.
+* Within `immanuel.po`, for every English word or sentence in a `msgid` string, if there is a direct translation in your language, enter it in the following empty `msgstr`. For gendered adjectives, you will need to add all gendered variants using `msgctxt` like this:
+```
+msgctxt "masculine"
+msgid "Applicative"
+msgstr "Aplicativo"
+
+msgctxt "feminine"
+msgid "Applicative"
+msgstr "Aplicativa"
+```
+* To map genders, a file `mappings.py` will need to be created under your new locale directory alongside `LC_MESSAGES`. See existing mapping files for an example of how to assign all of Immanuel's objects a gender for your language.
+* Once all translations and gender-mapping is complete, you can either compile your `.po` file to an `.mo` file or simply leave this out and I will compile it. Commit your changes and create a pull request.
+* If everything looks good, I will merge to master & prep a new release!
+
 ## Contact
 
 Please post any issues, feature requests, PRs etc. on GitHub. For anything else email robert@theriftlab.com.
```

### Comparing `immanuel-1.2.4/immanuel.egg-info/SOURCES.txt` & `immanuel-1.3.1/immanuel.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
+immanuel/__init__.py
 immanuel/charts.py
 immanuel/setup.py
 immanuel.egg-info/PKG-INFO
 immanuel.egg-info/SOURCES.txt
 immanuel.egg-info/dependency_links.txt
 immanuel.egg-info/requires.txt
 immanuel.egg-info/top_level.txt
+immanuel/classes/cache.py
+immanuel/classes/localize.py
 immanuel/classes/serialize.py
 immanuel/classes/wrap.py
 immanuel/const/calc.py
 immanuel/const/chart.py
 immanuel/const/data.py
 immanuel/const/dignities.py
+immanuel/const/genders.py
 immanuel/const/names.py
+immanuel/locales/pt_BR/mappings.py
 immanuel/reports/aspect.py
 immanuel/reports/dignity.py
 immanuel/reports/pattern.py
 immanuel/reports/weighting.py
 immanuel/resources/ephemeris/seas_12.se1
 immanuel/resources/ephemeris/seas_18.se1
 immanuel/resources/ephemeris/seas_24.se1
@@ -47,12 +52,13 @@
 tests/test_charts.py
 tests/test_convert.py
 tests/test_date.py
 tests/test_dignity.py
 tests/test_ephemeris.py
 tests/test_find.py
 tests/test_forecast.py
+tests/test_localization.py
 tests/test_midpoint.py
 tests/test_pattern.py
 tests/test_position.py
 tests/test_setup.py
 tests/test_weighting.py
```

### Comparing `immanuel-1.2.4/pyproject.toml` & `immanuel-1.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "immanuel"
-version = "1.2.4"
+version = "1.3.1"
 description = "Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com."
 authors = [
   { name = "Robert Davies", email = "robert@theriftlab.com" },
 ]
 license = { file = "LICENSE.md" }
 readme = "README.md"
 keywords = ["astrology", "api", "pyswisseph", "swisseph", "swiss ephemeris", "astro.com", "astro gold"]
```

### Comparing `immanuel-1.2.4/tests/se01181s.se1` & `immanuel-1.3.1/tests/se01181s.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_aspect.py` & `immanuel-1.3.1/tests/test_aspect.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_calculate.py` & `immanuel-1.3.1/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_charts.py` & `immanuel-1.3.1/tests/test_charts.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 @fixture
 def pdt():
     # We compare against astro.com which assumes UTC for progressions date
     # so we knock 8 hours off midnight 2023-06-21 to account for Pacific Time
     return '2025-06-20 17:00:00'
 
 
+def teardown_function():
+    settings.reset()
+
+
 def test_subject(dob, lat, lon, native, julian_date):
     date_time = datetime.fromisoformat(f'{dob} -08:00')
     latitude, longitude = (convert.string_to_dec(v) for v in (lat, lon))
     assert native.date_time.year == date_time.year
     assert native.date_time.month == date_time.month
     assert native.date_time.day == date_time.day
     assert native.date_time.hour == date_time.hour
@@ -145,17 +149,17 @@
     assert natal_chart.aspects[chart.SUN][chart.MOON].aspect == calc.SEXTILE
 
     assert chart.MOON in natal_chart.aspects
     assert chart.SATURN in natal_chart.aspects[chart.MOON]
     assert natal_chart.aspects[chart.MOON][chart.SATURN].aspect == calc.OPPOSITION
 
     # Spot-check for correct weightings against astro.com
-    assert chart.JUPITER in natal_chart.weightings['elements'].fire
-    assert chart.JUPITER in natal_chart.weightings['modalities'].cardinal
-    assert chart.JUPITER in natal_chart.weightings['quadrants'].first
+    assert chart.JUPITER in natal_chart.weightings.elements.fire
+    assert chart.JUPITER in natal_chart.weightings.modalities.cardinal
+    assert chart.JUPITER in natal_chart.weightings.quadrants.first
 
 
 def test_solar_return(native, lat, lon, solar_return_year):
     solar_return_chart = charts.SolarReturn(native, solar_return_year)
 
     assert solar_return_chart.type == names.CHART_TYPES[chart.SOLAR_RETURN]
 
@@ -211,17 +215,17 @@
     assert solar_return_chart.aspects[chart.SUN][chart.SATURN].aspect == calc.TRINE
 
     assert chart.MOON in solar_return_chart.aspects
     assert chart.NEPTUNE in solar_return_chart.aspects[chart.MOON]
     assert solar_return_chart.aspects[chart.MOON][chart.NEPTUNE].aspect == calc.TRINE
 
     # Spot-check for correct weightings against astro.com
-    assert chart.JUPITER in solar_return_chart.weightings['elements'].water
-    assert chart.JUPITER in solar_return_chart.weightings['modalities'].fixed
-    assert chart.JUPITER in solar_return_chart.weightings['quadrants'].second
+    assert chart.JUPITER in solar_return_chart.weightings.elements.water
+    assert chart.JUPITER in solar_return_chart.weightings.modalities.fixed
+    assert chart.JUPITER in solar_return_chart.weightings.quadrants.second
 
 
 def test_progressed(native, lat, lon, pdt):
     settings.mc_progression_method = calc.NAIBOD
     progressed_chart = charts.Progressed(native, pdt)
 
     assert progressed_chart.type == names.CHART_TYPES[chart.PROGRESSED]
@@ -285,17 +289,17 @@
     assert progressed_chart.aspects[chart.SUN][chart.SATURN].aspect == calc.SQUARE
 
     assert chart.MOON in progressed_chart.aspects
     assert chart.URANUS in progressed_chart.aspects[chart.MOON]
     assert progressed_chart.aspects[chart.MOON][chart.URANUS].aspect == calc.TRINE
 
     # Spot-check for correct weightings against astro.com
-    assert chart.VENUS in progressed_chart.weightings['elements'].earth
-    assert chart.VENUS in progressed_chart.weightings['modalities'].cardinal
-    assert chart.VENUS in progressed_chart.weightings['quadrants'].third
+    assert chart.VENUS in progressed_chart.weightings.elements.earth
+    assert chart.VENUS in progressed_chart.weightings.modalities.cardinal
+    assert chart.VENUS in progressed_chart.weightings.quadrants.third
 
 
 def test_composite(native, lat, lon, partner, partner_lat, partner_lon):
     composite_chart = charts.Composite(native, partner)
 
     assert composite_chart.type == names.CHART_TYPES[chart.COMPOSITE]
 
@@ -357,17 +361,17 @@
     assert composite_chart.aspects[chart.SUN][chart.MOON].aspect == calc.SEXTILE
 
     assert chart.MOON in composite_chart.aspects
     assert chart.VENUS in composite_chart.aspects[chart.MOON]
     assert composite_chart.aspects[chart.MOON][chart.VENUS].aspect == calc.SEXTILE
 
     # Spot-check for correct weightings against astro.com
-    assert chart.JUPITER in composite_chart.weightings['elements'].earth
-    assert chart.JUPITER in composite_chart.weightings['modalities'].fixed
-    assert chart.JUPITER in composite_chart.weightings['quadrants'].first
+    assert chart.JUPITER in composite_chart.weightings.elements.earth
+    assert chart.JUPITER in composite_chart.weightings.modalities.fixed
+    assert chart.JUPITER in composite_chart.weightings.quadrants.first
 
     # Ensure more quirky house systems work
     settings.house_system = chart.EQUAL
 
     composite_chart = charts.Composite(native, partner)
 
     assert composite_chart.objects[chart.ASC].sign.name == names.SIGNS[chart.AQUARIUS]
```

### Comparing `immanuel-1.2.4/tests/test_convert.py` & `immanuel-1.3.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_date.py` & `immanuel-1.3.1/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_dignity.py` & `immanuel-1.3.1/tests/test_dignity.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,15 @@
 
 @fixture
 def is_daytime(jd, coords):
     return ephemeris.is_daytime(jd, *coords)
 
 
 def teardown_function():
-    settings.include_participatory_triplicities = False
-    settings.include_mutual_receptions = True
+    settings.reset()
 
 
 def test_ruler(objects):
     # Uranus is ruler of its sign
     assert dignity.ruler(objects[chart.SUN]) is False
     assert dignity.ruler(objects[chart.URANUS]) is True
```

### Comparing `immanuel-1.2.4/tests/test_ephemeris.py` & `immanuel-1.3.1/tests/test_ephemeris.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,18 @@
             'dec': '19°45\'29"',
             'eclipse_type': chart.TOTAL,
             'date': '20 January',
         },
     }
 
 
+def teardown_function():
+    settings.reset()
+
+
 """ These tests simply check the correct chart objects are being
 returned. Data is checked separately afterwards. """
 def test_objects(jd, coords):
     chart_objects = (chart.SUN, chart.MOON, chart.PARS_FORTUNA, chart.SYZYGY, chart.NORTH_NODE, chart.ASC)
     objects = ephemeris.objects(chart_objects, jd, *coords, chart.PLACIDUS, calc.DAY_NIGHT_FORMULA)
     assert tuple(objects.keys()) == chart_objects
```

### Comparing `immanuel-1.2.4/tests/test_find.py` & `immanuel-1.3.1/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_forecast.py` & `immanuel-1.3.1/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_midpoint.py` & `immanuel-1.3.1/tests/test_midpoint.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_pattern.py` & `immanuel-1.3.1/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.2.4/tests/test_position.py` & `immanuel-1.3.1/tests/test_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 """
 
 import os
 
 from pytest import fixture
 
-from immanuel.setup import settings
 from immanuel.const import calc, chart
+from immanuel.setup import settings
 from immanuel.tools import convert, date, ephemeris, position
 
 
 @fixture
 def coords():
     # San Diego coords as used by astro.com
     return [convert.string_to_dec(v) for v in ('32n43', '117w09')]
@@ -119,14 +119,18 @@
             'decan': chart.DECAN1,
             'element': chart.FIRE,
             'modality': chart.MUTABLE,
         },
     }
 
 
+def teardown_function():
+    settings.reset()
+
+
 def test_sign(data, astro):
     for key, object in data.items():
         assert position.sign(object) == astro[key]['sign']
 
 
 def test_sign_longitude(data, astro):
     for key, object in data.items():
```

### Comparing `immanuel-1.2.4/tests/test_setup.py` & `immanuel-1.3.1/tests/test_setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,34 +5,37 @@
 
     Tests for the settings class. This class is designed to act like a module
     containing global variables, but due to some settings cascading into each
     other it requires slightly more complex machinery under the hood.
 
 """
 
-import random, os
-from datetime import datetime
+import os
 
 import swisseph as swe
 import pytest
 from pytest import fixture
 
 from immanuel import charts
+from immanuel.classes.cache import FunctionCache
 from immanuel.const import calc, chart
 from immanuel.setup import settings
 
 
 @fixture
 def native():
     return charts.Subject('2000-01-01 10:00', '32N43.0', '117W9.0')
 
 
+def teardown_function():
+    settings.reset()
+    FunctionCache.clear_all()
+
+
 def test_attributes():
-    # Standard setting
-    assert settings.house_system == chart.PLACIDUS
     settings.house_system = chart.POLICH_PAGE
     assert settings.house_system == chart.POLICH_PAGE
 
     # Cascading setting
     assert calc.CONJUNCTION in settings.aspects
     assert calc.CONJUNCTION in settings.aspect_rules[chart.SUN]['initiate']
 
@@ -92,16 +95,14 @@
 
 def test_add_filepath(native):
     settings.add_filepath(os.path.dirname(__file__))
     settings.objects.append(1181)
     natal = charts.Natal(native)
     assert 1181 in natal.objects
 
-    # Cache-bust
-    settings.add_filepath(os.path.dirname(__file__), True)
-    date_time = datetime.now()
-    latitude = random.random() * 180 - 90
-    longitude = random.random() * 360 - 180
-    native2 = charts.Subject(date_time, latitude, longitude)
+    settings.add_filepath('', True)
+    FunctionCache.clear_all()
 
     with pytest.raises(swe.Error):
-        charts.Natal(native2)
+        charts.Natal(native)
+
+    settings.add_filepath(f'{os.path.dirname(__file__)}{os.sep}..{os.sep}resources{os.sep}ephemeris')
```

### Comparing `immanuel-1.2.4/tests/test_weighting.py` & `immanuel-1.3.1/tests/test_weighting.py`

 * *Files identical despite different names*

