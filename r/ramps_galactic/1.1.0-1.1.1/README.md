# Comparing `tmp/ramps_galactic-1.1.0.tar.gz` & `tmp/ramps_galactic-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramps_galactic-1.1.0.tar", last modified: Mon Mar 18 04:12:18 2024, max compression
+gzip compressed data, was "ramps_galactic-1.1.1.tar", max compression
```

## Comparing `ramps_galactic-1.1.0.tar` & `ramps_galactic-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,67 @@
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     2063 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/PKG-INFO
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.674812 ramps_galactic-1.1.0/modules/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.674812 ramps_galactic-1.1.0/modules/ramps_galactic/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     2085 2024-02-23 22:28:28.000000 ramps_galactic-1.1.0/modules/ramps_galactic/__init__.py
--rw-r--r--   0 calculator  (1000) calculator  (1000)     5345 2024-02-23 22:28:28.000000 ramps_galactic-1.1.0/modules/ramps_galactic/__init__v1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_clique/
--rw-r--r--   0 calculator  (1000) calculator  (1000)      297 2023-12-11 06:07:46.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_clique/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_clique/group/
--rw-r--r--   0 calculator  (1000) calculator  (1000)      294 2023-12-01 19:53:30.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_clique/group/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_licenses/
--rw-r--r--   0 calculator  (1000) calculator  (1000)    37279 2023-12-01 20:51:04.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_licenses/gpl-3.0-standalone.html
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_status/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     1395 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_status/status.proc.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.674812 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/1/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1590 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/1/status_1.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)    32206 2024-02-07 21:25:16.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/1/yahoo-finance--BTC-USD.CSV
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/2/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1615 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/2/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/3/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1684 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/3/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/charts/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1984 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/VLOCH.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/charts/annotations/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1058 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/annotations/vline.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      427 2024-02-23 22:28:28.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/galactic_line.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/charts/shapes/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       20 2024-02-10 22:59:24.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/shapes/rectangle.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      634 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/shapes/vline.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      641 2024-02-23 22:28:28.000000 ramps_galactic-1.1.0/modules/ramps_galactic/charts/trend_side_circles.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/example_data/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      343 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/example_data/read.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)    32206 2024-02-07 21:25:16.000000 ramps_galactic-1.1.0/modules/ramps_galactic/example_data/yahoo-finance--BTC-USD.CSV
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/CSV/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1128 2024-02-10 23:03:09.000000 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/CSV/read.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/DF/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      126 2024-02-07 22:57:26.000000 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/DF/reverse.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      549 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/furniture/places.py
--rw-r--r--   0 calculator  (1000) calculator  (1000)     1837 2024-03-18 04:11:41.000000 ramps_galactic-1.1.0/modules/ramps_galactic/module.MD
--rw-r--r--   0 calculator  (1000) calculator  (1000)       62 2023-12-11 06:14:40.000000 ramps_galactic-1.1.0/modules/ramps_galactic/status_1.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.674812 ramps_galactic-1.1.0/modules/ramps_galactic/tendencies/
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/tendencies/galactic/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     4511 2024-02-23 22:28:28.000000 ramps_galactic-1.1.0/modules/ramps_galactic/tendencies/galactic/__init__.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     2529 2024-03-18 03:41:22.000000 ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/purchase_treasure_at_inclines.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)      266 2024-02-23 22:27:38.000000 ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/purchase_treasure_over_span.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     2031 2024-02-23 22:28:29.000000 ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/ramp_v1.py
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1940 2024-02-23 22:28:29.000000 ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/ramp_v2.py
-drwxrwxr-x   0 calculator  (1000) calculator  (1000)        0 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/
--rw-r--r--   0 calculator  (1000) calculator  (1000)     2063 2024-03-18 04:12:18.000000 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/PKG-INFO
--rw-rw-r--   0 calculator  (1000) calculator  (1000)     1629 2024-03-18 04:12:18.000000 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/SOURCES.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)        1 2024-03-18 04:12:18.000000 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/dependency_links.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       34 2024-03-18 04:12:18.000000 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/requires.txt
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       15 2024-03-18 04:12:18.000000 ramps_galactic-1.1.0/modules/ramps_galactic.egg-info/top_level.txt
--rw-r--r--   0 calculator  (1000) calculator  (1000)      960 2024-03-18 04:11:54.000000 ramps_galactic-1.1.0/pyproject.toml
--rw-rw-r--   0 calculator  (1000) calculator  (1000)       38 2024-03-18 04:12:18.678812 ramps_galactic-1.1.0/setup.cfg
+-rwxr-xr-x   0        0        0      206 2024-02-23 22:27:05.795130 ramps_galactic-1.1.1/license.s.HTML
+-rwxr-xr-x   0        0        0      833 2024-04-16 17:37:19.723903 ramps_galactic-1.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1535 2024-02-11 01:36:46.692134 ramps_galactic-1.1.1/readme.md
+-rwxr-xr-x   0        0        0      859 2024-04-16 17:29:44.182363 ramps_galactic-1.1.1/venue.S.HTML
+-rwxr-xr-x   0        0        0      386 2024-04-16 17:22:29.439902 ramps_galactic-1.1.1/venues/stages/ramps_galactic/___perf/ramps_galactic_1
+-rwxr-xr-x   0        0        0     2574 2024-04-16 17:44:58.690918 ramps_galactic-1.1.1/venues/stages/ramps_galactic/__init__.py
+-rwxr-xr-x   0        0        0     5345 2024-02-23 22:28:28.402158 ramps_galactic-1.1.1/venues/stages/ramps_galactic/__init__v1.py
+-rwxr-xr-x   0        0        0       62 2024-04-16 17:24:29.680744 ramps_galactic-1.1.1/venues/stages/ramps_galactic/__itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      519 2024-02-08 03:01:03.475844 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_book/indexes.s.HTML
+-rwxr-xr-x   0        0        0      297 2023-12-11 06:07:46.193124 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/__init__.py
+-rwxr-xr-x   0        0        0      759 2024-02-23 22:28:04.542439 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1166 2023-12-01 19:55:35.306618 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      766 2024-02-23 22:28:04.542439 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_licenses/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0    76465 2024-04-16 17:56:02.968704 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1290 2024-04-16 17:04:51.780354 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/status.proc.py
+-rw-r--r--   0        0        0     1687 2024-04-16 17:56:00.972721 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/1/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1506 2024-04-16 17:55:55.908767 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/1/status_1.py
+-rwxr-xr-x   0        0        0    32206 2024-02-07 21:25:16.770278 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/1/yahoo-finance--BTC-USD.CSV
+-rw-r--r--   0        0        0     1721 2024-04-16 17:56:00.956722 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/2/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1527 2024-04-16 17:55:51.160809 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/2/status_1.py
+-rwxr-xr-x   0        0        0    17389 2024-02-07 23:05:44.345602 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/2/yahoo-finance--SPXU.csv
+-rw-r--r--   0        0        0     1765 2024-04-16 17:56:00.956722 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/3/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1692 2024-04-16 17:55:46.424852 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/3/status_1.py
+-rwxr-xr-x   0        0        0    17478 2024-02-08 04:42:12.819877 ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/3/yahoo-finance--UPRO.csv
+-rwxr-xr-x   0        0        0     1984 2024-02-23 22:27:38.426746 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/VLOCH.py
+-rwxr-xr-x   0        0        0     1384 2024-02-23 22:28:05.086432 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/VLOCH.cpython-310.pyc
+-rwxr-xr-x   0        0        0      756 2024-02-23 22:29:14.777613 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/galactic_line.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-23 22:28:28.930152 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/majestic_line.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-07 23:40:57.321456 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/pivots.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-08 04:48:09.385109 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/superb_line.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-23 22:27:38.238748 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/__pycache__/trend_side_circles.cpython-310.pyc
+-rwxr-xr-x   0        0        0      900 2024-02-23 22:28:05.146432 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/annotations/__pycache__/vline.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1058 2024-02-23 22:27:38.310747 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/annotations/vline.py
+-rwxr-xr-x   0        0        0      427 2024-02-23 22:28:28.946152 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/galactic_line.py
+-rwxr-xr-x   0        0        0      708 2024-02-23 22:28:05.146432 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/shapes/__pycache__/vline.cpython-310.pyc
+-rwxr-xr-x   0        0        0       20 2024-02-10 22:59:24.506330 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/shapes/rectangle.py
+-rwxr-xr-x   0        0        0      634 2024-02-23 22:27:38.390746 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/shapes/vline.py
+-rwxr-xr-x   0        0        0      641 2024-02-23 22:28:28.962152 ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/trend_side_circles.py
+-rw-r--r--   0        0        0     1196 2024-04-16 17:53:28.742094 ramps_galactic-1.1.1/venues/stages/ramps_galactic/clouds/Yahoo/VLOCH.py
+-rw-r--r--   0        0        0     1123 2024-04-16 17:53:31.826066 ramps_galactic-1.1.1/venues/stages/ramps_galactic/clouds/Yahoo/__pycache__/VLOCH.cpython-310.pyc
+-rwxr-xr-x   0        0        0      774 2024-02-23 22:28:04.546439 ramps_galactic-1.1.1/venues/stages/ramps_galactic/example_data/__pycache__/read.cpython-310.pyc
+-rwxr-xr-x   0        0        0      343 2024-02-23 22:27:38.462746 ramps_galactic-1.1.1/venues/stages/ramps_galactic/example_data/read.py
+-rwxr-xr-x   0        0        0    32206 2024-02-07 21:25:16.770278 ramps_galactic-1.1.1/venues/stages/ramps_galactic/example_data/yahoo-finance--BTC-USD.CSV
+-rwxr-xr-x   0        0        0     1218 2024-02-23 22:28:04.546439 ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/CSV/__pycache__/read.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1128 2024-02-10 23:03:09.927878 ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/CSV/read.py
+-rwxr-xr-x   0        0        0      126 2024-02-07 22:57:26.961624 ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/DF/reverse.py
+-rwxr-xr-x   0        0        0        4 2024-02-08 04:48:09.569108 ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/__pycache__/places.cpython-310.pyc
+-rwxr-xr-x   0        0        0      549 2024-02-23 22:27:38.502745 ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/places.py
+-rwxr-xr-x   0        0        0      229 2024-02-07 17:50:22.400178 ramps_galactic-1.1.1/venues/stages/ramps_galactic/license.s.HTML
+-rwxr-xr-x   0        0        0     1913 2024-03-18 19:01:24.086348 ramps_galactic-1.1.1/venues/stages/ramps_galactic/module.MD
+-rwxr-xr-x   0        0        0      148 2024-03-18 03:31:20.644589 ramps_galactic-1.1.1/venues/stages/ramps_galactic/module.s.HTML
+-rwxr-xr-x   0        0        0       62 2023-12-11 06:14:40.025640 ramps_galactic-1.1.1/venues/stages/ramps_galactic/status_1.py
+-rwxr-xr-x   0        0        0     4510 2024-03-18 04:14:47.812879 ramps_galactic-1.1.1/venues/stages/ramps_galactic/tendencies/galactic/__init__.py
+-rwxr-xr-x   0        0        0     2787 2024-03-18 19:26:55.945757 ramps_galactic-1.1.1/venues/stages/ramps_galactic/tendencies/galactic/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-07 23:40:57.365455 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/__pycache__/holding.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1666 2024-03-18 03:41:24.844514 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/__pycache__/purchase_treasure_at_inclines.cpython-310.pyc
+-rwxr-xr-x   0        0        0      595 2024-02-23 22:28:04.546439 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/__pycache__/purchase_treasure_over_span.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-23 22:27:38.654743 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/__pycache__/ramp.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-02-23 22:27:38.690743 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/__pycache__/treasure_purchase.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2529 2024-03-18 03:41:22.888529 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/purchase_treasure_at_inclines.py
+-rwxr-xr-x   0        0        0      266 2024-02-23 22:27:38.726742 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/purchase_treasure_over_span.py
+-rwxr-xr-x   0        0        0     2031 2024-02-23 22:28:29.046151 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/ramp_v1.py
+-rwxr-xr-x   0        0        0     1940 2024-02-23 22:28:29.058150 ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/ramp_v2.py
+-rw-r--r--   0        0        0     2391 1970-01-01 00:00:00.000000 ramps_galactic-1.1.1/PKG-INFO
```

### Comparing `ramps_galactic-1.1.0/PKG-INFO` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/module.MD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: ramps_galactic
-Version: 1.1.0
-License: GPL 3.0
-Description-Content-Type: text/markdown
-Requires-Dist: bracelet
-Requires-Dist: click
-Requires-Dist: pandas
-Requires-Dist: plotly
-Requires-Dist: rich
-
 
 
 
 
 
 ******
 
@@ -39,14 +28,23 @@
 pip install ramps_galactic
 ```
 
 --
 
 ## usage
 ```
+"date string": "",
+"high": "",
+"low": "",
+"open": "",
+"close": ""
+```
+
+
+```
 from datetime import datetime
 import json
 import pprint
 
 import pandas
 import rich	
 
@@ -95,8 +93,8 @@
 	If you would like to open the chart:
 '''
 if (True):
 	ramps_galactic.chart_the_data (
 		enhanced_trend_DF,
 		victory_multiplier_if_riding
 	)
-```
+```
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/__init__.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/2/status_1.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,99 +1,61 @@
 
-
-
-
-'''
-	based on:
-		https://stackoverflow.com/questions/44935269/supertendency-code-using-pandas-python
-'''
-
-
-from ._clique import clique
-
-
 '''
-	pivot indicates a band change.
-	
-	The place 1 place after the pivot
-	is where the purchase or sale event
-	can occur at the open price.
-	
-		"galactic incline": "yes",
-		"galactic decline": "no",
+	python3 status.proc.py "_status/vows/2/status_1.py"
 '''
 
 '''
-	import ramps_galactic
-	enhanced_tendency_DF = galactic.calc ([{
-		"high": "",
-		"low": "",
-		"open": "",
-		"close": ""
-	}])	
+	https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
 '''
 
+from datetime import datetime
+import json
+import pprint
 
-
-from ramps_galactic.tendencies.galactic import calc
-
-
-'''
-	This charts the data
-'''
-import rich
+import pandas
+import rich	
 
 import ramps_galactic
 import ramps_galactic.victory_multiplier.purchase_treasure_at_inclines as purchase_treasure_at_inclines_VM	
 import ramps_galactic.victory_multiplier.purchase_treasure_over_span as purchase_treasure_over_span_VM
 import ramps_galactic.furniture.CSV.read as read_CSV
-def chart_the_data (
-	enhanced_trend_DF = None,
-	treasure_at_inclines_VM = None
-):
-	import ramps_galactic.charts.VLOCH as VLOCH
-	chart = VLOCH.show (
-		DF = enhanced_trend_DF
-	)
-	import ramps_galactic.charts.galactic_line as galactic_line
-	galactic_line.attach (
-		chart = chart,
-		DF = enhanced_trend_DF
-	)	
-	import ramps_galactic.charts.shapes.vline as vline_shape	
-	import ramps_galactic.charts.annotations.vline as vline_annotation
-	relevant = treasure_at_inclines_VM ["relevant"]
-	for place in relevant:
-		multiplier = "()"
-		if (type (place ["change"]) == float):
-			multiplier = "(" + str (round (place ["aggregate change"], 3)) + ")";
-		
-		open = place ["open"]
-	
-		vline_shape.show (
-			chart,
-			DF = enhanced_trend_DF,
-			x = place ["date string"]
-		)
-		vline_annotation.show (
-			chart,
-			DF = enhanced_trend_DF,
-			x = place ["date string"],
-			
-			text = f"{ multiplier }"
-		)
-
-	#rich.print_json (data = treasure_at_inclines_VM ["relevant"])
-	
-	columns = list (relevant[0].keys())
-
-	import plotly.graph_objects as go
-	chart.append_trace ( 
-		go.Table (
-			header = dict(values=columns),
-			cells = dict(values=list(zip(*[data.values() for data in relevant])))
-		),
-		row = 2,
-		col = 1
+	
+
+def relative_path (path):
+	import pathlib
+	from os.path import dirname, join, normpath
+	import sys
+
+	this_directory_path = pathlib.Path (__file__).parent.resolve ()	
+	return str (normpath (join (this_directory_path, path)))
+
+def check_1 ():
+	
+	'''
+		This parses the data from the CSV.
+	'''
+	trend = read_CSV.start (relative_path ("yahoo-finance--SPXU.csv"))	
+	trend_DF = pandas.DataFrame (trend)	
+	
+	enhanced_trend_DF = ramps_galactic.calc (
+		trend_DF,
+		period = 14,
+		multiplier = 3
 	)
+	enhanced_list = enhanced_trend_DF.to_dict ('records')
+
+	
+	'''
+		This calculates the multipliers
+	'''
+	treasure_at_inclines_VM = purchase_treasure_at_inclines_VM.calc (enhanced_trend_DF)
+	rich.print_json (data = treasure_at_inclines_VM)	
+	assert (treasure_at_inclines_VM ["treasure purchase victory multiplier"] == 0.9198514681826051)
+	
+	open_price_at_spans_VM = purchase_treasure_over_span_VM.calc (enhanced_trend_DF)
+	assert (open_price_at_spans_VM == 0.5551523947750363)
+
+	
 	
-	chart.show ()
+checks = {
+	"check 1": check_1
+}
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/__init__v1.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/__init__v1.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/_licenses/gpl-3.0-standalone.html` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/1/status_1.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/3/status_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 '''
-	python3 status.proc.py "_status/vows/1/status_1.py"
+	python3 status.proc.py "_status/vows/3/status_1.py"
 '''
 
 '''
 	https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
 '''
 
 from datetime import datetime
@@ -14,49 +14,63 @@
 import pandas
 import rich	
 
 import ramps_galactic
 import ramps_galactic.victory_multiplier.purchase_treasure_at_inclines as purchase_treasure_at_inclines_VM	
 import ramps_galactic.victory_multiplier.purchase_treasure_over_span as purchase_treasure_over_span_VM
 import ramps_galactic.furniture.CSV.read as read_CSV
+	
 
 def relative_path (path):
 	import pathlib
 	from os.path import dirname, join, normpath
 	import sys
 
 	this_directory_path = pathlib.Path (__file__).parent.resolve ()	
 	return str (normpath (join (this_directory_path, path)))
-	
 
-	
 def check_1 ():
-	trend = read_CSV.start (relative_path ("yahoo-finance--BTC-USD.CSV"))
+	
+	'''
+		This parses the data from the CSV.
+	'''
+	trend = read_CSV.start (relative_path ("yahoo-finance--UPRO.csv"))	
 	trend_DF = pandas.DataFrame (trend)	
 	
 	enhanced_trend_DF = ramps_galactic.calc (
 		trend_DF,
 		period = 14,
 		multiplier = 3
 	)
 	enhanced_list = enhanced_trend_DF.to_dict ('records')
 
 	
 	'''
 		This calculates the multipliers
 	'''
-	treasure_at_inclines_VM = purchase_treasure_at_inclines_VM.calc (enhanced_trend_DF)
+	treasure_at_inclines_VM = purchase_treasure_at_inclines_VM.calc (
+		enhanced_trend_DF,
+		include_last_change = True
+	)
+	
 	rich.print_json (data = treasure_at_inclines_VM)	
-	assert (treasure_at_inclines_VM ["treasure purchase victory multiplier"] == 1.7192114362604047)
+	assert (
+		treasure_at_inclines_VM ["treasure purchase victory multiplier"] == 1.54871822964367
+	)
 	
 	open_price_at_spans_VM = purchase_treasure_over_span_VM.calc (enhanced_trend_DF)
-	assert (open_price_at_spans_VM == 1.8934619186292894), open_price_at_spans_VM
-	
+	assert (
+		open_price_at_spans_VM == 1.5598574915872383
+	), open_price_at_spans_VM
 	
+	'''
 	ramps_galactic.chart_the_data (
 		enhanced_trend_DF,
 		treasure_at_inclines_VM
 	)
+	'''
+	
+	
 	
 checks = {
 	"check 1": check_1
 }
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/1/yahoo-finance--BTC-USD.CSV` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/1/yahoo-finance--BTC-USD.CSV`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/2/status_1.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/1/status_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 '''
-	python3 status.proc.py "_status/vows/2/status_1.py"
+	python3 status.proc.py "_status/vows/1/status_1.py"
 '''
 
 '''
 	https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
 '''
 
 from datetime import datetime
@@ -14,30 +14,27 @@
 import pandas
 import rich	
 
 import ramps_galactic
 import ramps_galactic.victory_multiplier.purchase_treasure_at_inclines as purchase_treasure_at_inclines_VM	
 import ramps_galactic.victory_multiplier.purchase_treasure_over_span as purchase_treasure_over_span_VM
 import ramps_galactic.furniture.CSV.read as read_CSV
-	
 
 def relative_path (path):
 	import pathlib
 	from os.path import dirname, join, normpath
 	import sys
 
 	this_directory_path = pathlib.Path (__file__).parent.resolve ()	
 	return str (normpath (join (this_directory_path, path)))
+	
 
-def check_1 ():
 	
-	'''
-		This parses the data from the CSV.
-	'''
-	trend = read_CSV.start (relative_path ("yahoo-finance--SPXU.csv"))	
+def check_1 ():
+	trend = read_CSV.start (relative_path ("yahoo-finance--BTC-USD.CSV"))
 	trend_DF = pandas.DataFrame (trend)	
 	
 	enhanced_trend_DF = ramps_galactic.calc (
 		trend_DF,
 		period = 14,
 		multiplier = 3
 	)
@@ -45,23 +42,17 @@
 
 	
 	'''
 		This calculates the multipliers
 	'''
 	treasure_at_inclines_VM = purchase_treasure_at_inclines_VM.calc (enhanced_trend_DF)
 	rich.print_json (data = treasure_at_inclines_VM)	
-	assert (treasure_at_inclines_VM ["treasure purchase victory multiplier"] == 0.9198514681826051)
+	assert (treasure_at_inclines_VM ["treasure purchase victory multiplier"] == 1.7192114362604047)
 	
 	open_price_at_spans_VM = purchase_treasure_over_span_VM.calc (enhanced_trend_DF)
-	assert (open_price_at_spans_VM == 0.5551523947750363)
-	
-	
-	ramps_galactic.chart_the_data (
-		enhanced_trend_DF,
-		treasure_at_inclines_VM
-	)
-	
+	assert (open_price_at_spans_VM == 1.8934619186292894), open_price_at_spans_VM
 	
 	
+
 checks = {
 	"check 1": check_1
 }
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/_status/vows/3/status_1.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/_status/vows/2/__pycache__/status_1.cpython-310.pyc`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,108 @@
-00000000: 0a27 2727 0a09 7079 7468 6f6e 3320 7374  .'''..python3 st
-00000010: 6174 7573 2e70 726f 632e 7079 2022 5f73  atus.proc.py "_s
-00000020: 7461 7475 732f 766f 7773 2f33 2f73 7461  tatus/vows/3/sta
-00000030: 7475 735f 312e 7079 220a 2727 270a 0a27  tus_1.py".'''..'
-00000040: 2727 0a09 6874 7470 733a 2f2f 7061 6e64  ''..https://pand
-00000050: 6173 2e70 7964 6174 612e 6f72 672f 7061  as.pydata.org/pa
-00000060: 6e64 6173 2d64 6f63 732f 7374 6162 6c65  ndas-docs/stable
-00000070: 2f72 6566 6572 656e 6365 2f61 7069 2f70  /reference/api/p
-00000080: 616e 6461 732e 7265 6164 5f63 7376 2e68  andas.read_csv.h
-00000090: 746d 6c0a 2727 270a 0a66 726f 6d20 6461  tml.'''..from da
-000000a0: 7465 7469 6d65 2069 6d70 6f72 7420 6461  tetime import da
-000000b0: 7465 7469 6d65 0a69 6d70 6f72 7420 6a73  tetime.import js
-000000c0: 6f6e 0a69 6d70 6f72 7420 7070 7269 6e74  on.import pprint
-000000d0: 0a0a 696d 706f 7274 2070 616e 6461 730a  ..import pandas.
-000000e0: 696d 706f 7274 2072 6963 6809 0a0a 696d  import rich...im
-000000f0: 706f 7274 2072 616d 7073 5f67 616c 6163  port ramps_galac
-00000100: 7469 630a 696d 706f 7274 2072 616d 7073  tic.import ramps
-00000110: 5f67 616c 6163 7469 632e 7669 6374 6f72  _galactic.victor
-00000120: 795f 6d75 6c74 6970 6c69 6572 2e70 7572  y_multiplier.pur
-00000130: 6368 6173 655f 7472 6561 7375 7265 5f61  chase_treasure_a
-00000140: 745f 696e 636c 696e 6573 2061 7320 7075  t_inclines as pu
-00000150: 7263 6861 7365 5f74 7265 6173 7572 655f  rchase_treasure_
-00000160: 6174 5f69 6e63 6c69 6e65 735f 564d 090a  at_inclines_VM..
-00000170: 696d 706f 7274 2072 616d 7073 5f67 616c  import ramps_gal
-00000180: 6163 7469 632e 7669 6374 6f72 795f 6d75  actic.victory_mu
-00000190: 6c74 6970 6c69 6572 2e70 7572 6368 6173  ltiplier.purchas
-000001a0: 655f 7472 6561 7375 7265 5f6f 7665 725f  e_treasure_over_
-000001b0: 7370 616e 2061 7320 7075 7263 6861 7365  span as purchase
-000001c0: 5f74 7265 6173 7572 655f 6f76 6572 5f73  _treasure_over_s
-000001d0: 7061 6e5f 564d 0a69 6d70 6f72 7420 7261  pan_VM.import ra
-000001e0: 6d70 735f 6761 6c61 6374 6963 2e66 7572  mps_galactic.fur
-000001f0: 6e69 7475 7265 2e43 5356 2e72 6561 6420  niture.CSV.read 
-00000200: 6173 2072 6561 645f 4353 560a 090a 0a64  as read_CSV....d
-00000210: 6566 2072 656c 6174 6976 655f 7061 7468  ef relative_path
-00000220: 2028 7061 7468 293a 0a09 696d 706f 7274   (path):..import
-00000230: 2070 6174 686c 6962 0a09 6672 6f6d 206f   pathlib..from o
-00000240: 732e 7061 7468 2069 6d70 6f72 7420 6469  s.path import di
-00000250: 726e 616d 652c 206a 6f69 6e2c 206e 6f72  rname, join, nor
-00000260: 6d70 6174 680a 0969 6d70 6f72 7420 7379  mpath..import sy
-00000270: 730a 0a09 7468 6973 5f64 6972 6563 746f  s...this_directo
-00000280: 7279 5f70 6174 6820 3d20 7061 7468 6c69  ry_path = pathli
-00000290: 622e 5061 7468 2028 5f5f 6669 6c65 5f5f  b.Path (__file__
-000002a0: 292e 7061 7265 6e74 2e72 6573 6f6c 7665  ).parent.resolve
-000002b0: 2028 2909 0a09 7265 7475 726e 2073 7472   ()...return str
-000002c0: 2028 6e6f 726d 7061 7468 2028 6a6f 696e   (normpath (join
-000002d0: 2028 7468 6973 5f64 6972 6563 746f 7279   (this_directory
-000002e0: 5f70 6174 682c 2070 6174 6829 2929 0a0a  _path, path)))..
-000002f0: 6465 6620 6368 6563 6b5f 3120 2829 3a0a  def check_1 ():.
-00000300: 090a 0927 2727 0a09 0954 6869 7320 7061  ...'''...This pa
-00000310: 7273 6573 2074 6865 2064 6174 6120 6672  rses the data fr
-00000320: 6f6d 2074 6865 2043 5356 2e0a 0927 2727  om the CSV...'''
-00000330: 0a09 7472 656e 6420 3d20 7265 6164 5f43  ..trend = read_C
-00000340: 5356 2e73 7461 7274 2028 7265 6c61 7469  SV.start (relati
-00000350: 7665 5f70 6174 6820 2822 7961 686f 6f2d  ve_path ("yahoo-
-00000360: 6669 6e61 6e63 652d 2d55 5052 4f2e 6373  finance--UPRO.cs
-00000370: 7622 2929 090a 0974 7265 6e64 5f44 4620  v"))...trend_DF 
-00000380: 3d20 7061 6e64 6173 2e44 6174 6146 7261  = pandas.DataFra
-00000390: 6d65 2028 7472 656e 6429 090a 090a 0965  me (trend).....e
-000003a0: 6e68 616e 6365 645f 7472 656e 645f 4446  nhanced_trend_DF
-000003b0: 203d 2072 616d 7073 5f67 616c 6163 7469   = ramps_galacti
-000003c0: 632e 6361 6c63 2028 0a09 0974 7265 6e64  c.calc (...trend
-000003d0: 5f44 462c 0a09 0970 6572 696f 6420 3d20  _DF,...period = 
-000003e0: 3134 2c0a 0909 6d75 6c74 6970 6c69 6572  14,...multiplier
-000003f0: 203d 2033 0a09 290a 0965 6e68 616e 6365   = 3..)..enhance
-00000400: 645f 6c69 7374 203d 2065 6e68 616e 6365  d_list = enhance
-00000410: 645f 7472 656e 645f 4446 2e74 6f5f 6469  d_trend_DF.to_di
-00000420: 6374 2028 2772 6563 6f72 6473 2729 0a0a  ct ('records')..
-00000430: 090a 0927 2727 0a09 0954 6869 7320 6361  ...'''...This ca
-00000440: 6c63 756c 6174 6573 2074 6865 206d 756c  lculates the mul
-00000450: 7469 706c 6965 7273 0a09 2727 270a 0974  tipliers..'''..t
-00000460: 7265 6173 7572 655f 6174 5f69 6e63 6c69  reasure_at_incli
-00000470: 6e65 735f 564d 203d 2070 7572 6368 6173  nes_VM = purchas
-00000480: 655f 7472 6561 7375 7265 5f61 745f 696e  e_treasure_at_in
-00000490: 636c 696e 6573 5f56 4d2e 6361 6c63 2028  clines_VM.calc (
-000004a0: 0a09 0965 6e68 616e 6365 645f 7472 656e  ...enhanced_tren
-000004b0: 645f 4446 2c0a 0909 696e 636c 7564 655f  d_DF,...include_
-000004c0: 6c61 7374 5f63 6861 6e67 6520 3d20 5472  last_change = Tr
-000004d0: 7565 0a09 290a 090a 0972 6963 682e 7072  ue..)....rich.pr
-000004e0: 696e 745f 6a73 6f6e 2028 6461 7461 203d  int_json (data =
-000004f0: 2074 7265 6173 7572 655f 6174 5f69 6e63   treasure_at_inc
-00000500: 6c69 6e65 735f 564d 2909 0a09 6173 7365  lines_VM)...asse
-00000510: 7274 2028 0a09 0974 7265 6173 7572 655f  rt (...treasure_
-00000520: 6174 5f69 6e63 6c69 6e65 735f 564d 205b  at_inclines_VM [
-00000530: 2274 7265 6173 7572 6520 7075 7263 6861  "treasure purcha
-00000540: 7365 2076 6963 746f 7279 206d 756c 7469  se victory multi
-00000550: 706c 6965 7222 5d20 3d3d 2031 2e35 3438  plier"] == 1.548
-00000560: 3731 3832 3239 3634 3336 370a 0929 0a09  71822964367..)..
-00000570: 0a09 6f70 656e 5f70 7269 6365 5f61 745f  ..open_price_at_
-00000580: 7370 616e 735f 564d 203d 2070 7572 6368  spans_VM = purch
-00000590: 6173 655f 7472 6561 7375 7265 5f6f 7665  ase_treasure_ove
-000005a0: 725f 7370 616e 5f56 4d2e 6361 6c63 2028  r_span_VM.calc (
-000005b0: 656e 6861 6e63 6564 5f74 7265 6e64 5f44  enhanced_trend_D
-000005c0: 4629 0a09 6173 7365 7274 2028 0a09 096f  F)..assert (...o
-000005d0: 7065 6e5f 7072 6963 655f 6174 5f73 7061  pen_price_at_spa
-000005e0: 6e73 5f56 4d20 3d3d 2031 2e35 3539 3835  ns_VM == 1.55985
-000005f0: 3734 3931 3538 3732 3338 330a 0929 2c20  74915872383..), 
-00000600: 6f70 656e 5f70 7269 6365 5f61 745f 7370  open_price_at_sp
-00000610: 616e 735f 564d 0a09 0a09 0a09 7261 6d70  ans_VM......ramp
-00000620: 735f 6761 6c61 6374 6963 2e63 6861 7274  s_galactic.chart
-00000630: 5f74 6865 5f64 6174 6120 280a 0909 656e  _the_data (...en
-00000640: 6861 6e63 6564 5f74 7265 6e64 5f44 462c  hanced_trend_DF,
-00000650: 0a09 0974 7265 6173 7572 655f 6174 5f69  ...treasure_at_i
-00000660: 6e63 6c69 6e65 735f 564d 0a09 290a 090a  nclines_VM..)...
-00000670: 090a 090a 6368 6563 6b73 203d 207b 0a09  ....checks = {..
-00000680: 2263 6865 636b 2031 223a 2063 6865 636b  "check 1": check
-00000690: 5f31 0a7d                                _1.}
+00000000: 6f0d 0d0a 0000 0000 a7bb 1e66 f705 0000  o..........f....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0002 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
+00000030: 5a00 0900 6401 6402 6c01 6d01 5a01 0100  Z...d.d.l.m.Z...
+00000040: 6401 6403 6c02 5a02 6401 6403 6c03 5a03  d.d.l.Z.d.d.l.Z.
+00000050: 6401 6403 6c04 5a04 6401 6403 6c05 5a05  d.d.l.Z.d.d.l.Z.
+00000060: 6401 6403 6c06 5a06 6401 6403 6c07 6d08  d.d.l.Z.d.d.l.m.
+00000070: 0200 0100 6d09 5a0a 0100 6401 6403 6c0b  ....m.Z...d.d.l.
+00000080: 6d08 0200 0100 6d0c 5a0d 0100 6401 6403  m.....m.Z...d.d.
+00000090: 6c0e 6d0f 0200 0100 6d10 0200 0100 6d11  l.m.....m.....m.
+000000a0: 5a12 0100 6404 6405 8400 5a13 6406 6407  Z...d.d...Z.d.d.
+000000b0: 8400 5a14 6408 6514 6901 5a15 6403 5300  ..Z.d.e.i.Z.d.S.
+000000c0: 2909 7a36 0a09 7079 7468 6f6e 3320 7374  ).z6..python3 st
+000000d0: 6174 7573 2e70 726f 632e 7079 2022 5f73  atus.proc.py "_s
+000000e0: 7461 7475 732f 766f 7773 2f32 2f73 7461  tatus/vows/2/sta
+000000f0: 7475 735f 312e 7079 220a e900 0000 0029  tus_1.py"......)
+00000100: 01da 0864 6174 6574 696d 654e 6301 0000  ...datetimeNc...
+00000110: 0000 0000 0000 0000 0007 0000 0005 0000  ................
+00000120: 0043 0000 0073 4600 0000 6401 6400 6c00  .C...sF...d.d.l.
+00000130: 7d01 6401 6402 6c01 6d02 7d02 6d03 7d03  }.d.d.l.m.}.m.}.
+00000140: 6d04 7d04 0100 6401 6400 6c05 7d05 7c01  m.}...d.d.l.}.|.
+00000150: a006 7407 a101 6a08 a009 a100 7d06 740a  ..t...j.....}.t.
+00000160: 7c04 7c03 7c06 7c00 8302 8301 8301 5300  |.|.|.|.......S.
+00000170: 2903 4e72 0100 0000 2903 da07 6469 726e  ).Nr....)...dirn
+00000180: 616d 65da 046a 6f69 6eda 086e 6f72 6d70  ame..join..normp
+00000190: 6174 6829 0bda 0770 6174 686c 6962 da07  ath)...pathlib..
+000001a0: 6f73 2e70 6174 6872 0300 0000 7204 0000  os.pathr....r...
+000001b0: 0072 0500 0000 da03 7379 73da 0450 6174  .r......sys..Pat
+000001c0: 68da 085f 5f66 696c 655f 5fda 0670 6172  h..__file__..par
+000001d0: 656e 74da 0772 6573 6f6c 7665 da03 7374  ent..resolve..st
+000001e0: 7229 07da 0470 6174 6872 0600 0000 7203  r)...pathr....r.
+000001f0: 0000 0072 0400 0000 7205 0000 0072 0800  ...r....r....r..
+00000200: 0000 da13 7468 6973 5f64 6972 6563 746f  ....this_directo
+00000210: 7279 5f70 6174 68a9 0072 1000 0000 fa47  ry_path..r.....G
+00000220: 2f72 616d 7073 5f67 616c 6163 7469 632f  /ramps_galactic/
+00000230: 7665 6e75 6573 2f73 7461 6765 732f 7261  venues/stages/ra
+00000240: 6d70 735f 6761 6c61 6374 6963 2f5f 7374  mps_galactic/_st
+00000250: 6174 7573 2f76 6f77 732f 322f 7374 6174  atus/vows/2/stat
+00000260: 7573 5f31 2e70 79da 0d72 656c 6174 6976  us_1.py..relativ
+00000270: 655f 7061 7468 1700 0000 730a 0000 0008  e_path....s.....
+00000280: 0114 0108 0110 0212 0172 1200 0000 6300  .........r....c.
+00000290: 0000 0000 0000 0000 0000 0006 0000 0005  ................
+000002a0: 0000 0043 0000 0073 7400 0000 7400 a001  ...C...st...t...
+000002b0: 7402 6401 8301 a101 7d00 7403 a004 7c00  t.d.....}.t...|.
+000002c0: a101 7d01 7405 6a06 7c01 6402 6403 6404  ..}.t.j.|.d.d.d.
+000002d0: 8d03 7d02 7c02 a007 6405 a101 7d03 0900  ..}.|...d...}...
+000002e0: 7408 a006 7c02 a101 7d04 7409 6a0a 7c04  t...|...}.t.j.|.
+000002f0: 6406 8d01 0100 7c04 6407 1900 6408 6b02  d.....|.d...d.k.
+00000300: 732d 4a00 8201 740b a006 7c02 a101 7d05  s-J...t...|...}.
+00000310: 7c05 6409 6b02 7338 4a00 8201 640a 5300  |.d.k.s8J...d.S.
+00000320: 290b 7a27 0a09 0954 6869 7320 7061 7273  ).z'...This pars
+00000330: 6573 2074 6865 2064 6174 6120 6672 6f6d  es the data from
+00000340: 2074 6865 2043 5356 2e0a 097a 1779 6168   the CSV...z.yah
+00000350: 6f6f 2d66 696e 616e 6365 2d2d 5350 5855  oo-finance--SPXU
+00000360: 2e63 7376 e90e 0000 00e9 0300 0000 2902  .csv..........).
+00000370: da06 7065 7269 6f64 da0a 6d75 6c74 6970  ..period..multip
+00000380: 6c69 6572 da07 7265 636f 7264 7329 01da  lier..records)..
+00000390: 0464 6174 617a 2474 7265 6173 7572 6520  .dataz$treasure 
+000003a0: 7075 7263 6861 7365 2076 6963 746f 7279  purchase victory
+000003b0: 206d 756c 7469 706c 6965 7267 30b3 a058   multiplierg0..X
+000003c0: 6c6f ed3f 6708 5b7b f4ce c3e1 3f4e 290c  lo.?g.[{....?N).
+000003d0: da08 7265 6164 5f43 5356 da05 7374 6172  ..read_CSV..star
+000003e0: 7472 1200 0000 da06 7061 6e64 6173 da09  tr......pandas..
+000003f0: 4461 7461 4672 616d 65da 0e72 616d 7073  DataFrame..ramps
+00000400: 5f67 616c 6163 7469 63da 0463 616c 63da  _galactic..calc.
+00000410: 0774 6f5f 6469 6374 da20 7075 7263 6861  .to_dict. purcha
+00000420: 7365 5f74 7265 6173 7572 655f 6174 5f69  se_treasure_at_i
+00000430: 6e63 6c69 6e65 735f 564d da04 7269 6368  nclines_VM..rich
+00000440: da0a 7072 696e 745f 6a73 6f6e da1e 7075  ..print_json..pu
+00000450: 7263 6861 7365 5f74 7265 6173 7572 655f  rchase_treasure_
+00000460: 6f76 6572 5f73 7061 6e5f 564d 2906 da05  over_span_VM)...
+00000470: 7472 656e 64da 0874 7265 6e64 5f44 46da  trend..trend_DF.
+00000480: 1165 6e68 616e 6365 645f 7472 656e 645f  .enhanced_trend_
+00000490: 4446 da0d 656e 6861 6e63 6564 5f6c 6973  DF..enhanced_lis
+000004a0: 74da 1774 7265 6173 7572 655f 6174 5f69  t..treasure_at_i
+000004b0: 6e63 6c69 6e65 735f 564d da16 6f70 656e  nclines_VM..open
+000004c0: 5f70 7269 6365 5f61 745f 7370 616e 735f  _price_at_spans_
+000004d0: 564d 7210 0000 0072 1000 0000 7211 0000  VMr....r....r...
+000004e0: 00da 0763 6865 636b 5f31 1f00 0000 731c  ...check_1....s.
+000004f0: 0000 000e 050a 0104 0202 0102 0102 0106  ................
+00000500: fd0a 0502 030a 030c 0110 010a 0210 0172  ...............r
+00000510: 2a00 0000 7a07 6368 6563 6b20 3129 16da  *...z.check 1)..
+00000520: 075f 5f64 6f63 5f5f 7202 0000 00da 046a  .__doc__r......j
+00000530: 736f 6eda 0670 7072 696e 7472 1b00 0000  son..pprintr....
+00000540: 7221 0000 0072 1d00 0000 da3f 7261 6d70  r!...r.....?ramp
+00000550: 735f 6761 6c61 6374 6963 2e76 6963 746f  s_galactic.victo
+00000560: 7279 5f6d 756c 7469 706c 6965 722e 7075  ry_multiplier.pu
+00000570: 7263 6861 7365 5f74 7265 6173 7572 655f  rchase_treasure_
+00000580: 6174 5f69 6e63 6c69 6e65 73da 1276 6963  at_inclines..vic
+00000590: 746f 7279 5f6d 756c 7469 706c 6965 72da  tory_multiplier.
+000005a0: 1d70 7572 6368 6173 655f 7472 6561 7375  .purchase_treasu
+000005b0: 7265 5f61 745f 696e 636c 696e 6573 7220  re_at_inclinesr 
+000005c0: 0000 00da 3d72 616d 7073 5f67 616c 6163  ....=ramps_galac
+000005d0: 7469 632e 7669 6374 6f72 795f 6d75 6c74  tic.victory_mult
+000005e0: 6970 6c69 6572 2e70 7572 6368 6173 655f  iplier.purchase_
+000005f0: 7472 6561 7375 7265 5f6f 7665 725f 7370  treasure_over_sp
+00000600: 616e da1b 7075 7263 6861 7365 5f74 7265  an..purchase_tre
+00000610: 6173 7572 655f 6f76 6572 5f73 7061 6e72  asure_over_spanr
+00000620: 2300 0000 da21 7261 6d70 735f 6761 6c61  #....!ramps_gala
+00000630: 6374 6963 2e66 7572 6e69 7475 7265 2e43  ctic.furniture.C
+00000640: 5356 2e72 6561 64da 0966 7572 6e69 7475  SV.read..furnitu
+00000650: 7265 da03 4353 56da 0472 6561 6472 1900  re..CSV..readr..
+00000660: 0000 7212 0000 0072 2a00 0000 da06 6368  ..r....r*.....ch
+00000670: 6563 6b73 7210 0000 0072 1000 0000 7210  ecksr....r....r.
+00000680: 0000 0072 1100 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000690: 653e 0100 0000 731e 0000 0004 0102 040c  e>....s.........
+000006a0: 0408 0108 0108 0208 0108 0212 0112 0118  ................
+000006b0: 0108 0308 0804 1d08 ff                   .........
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/charts/VLOCH.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/VLOCH.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/charts/annotations/vline.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/annotations/vline.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/charts/shapes/vline.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/shapes/vline.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/charts/trend_side_circles.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/charts/trend_side_circles.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/example_data/yahoo-finance--BTC-USD.CSV` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/example_data/yahoo-finance--BTC-USD.CSV`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/furniture/CSV/read.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/CSV/read.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/furniture/places.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/furniture/places.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/tendencies/galactic/__init__.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/tendencies/galactic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 def calc (
 	DF,
 	
 	period = 14,
 	multiplier = 3
 ):
-
 	DF ['TR 1'] = abs (DF ["high"] - DF ["low"])
 	DF ['TR 2'] = abs (DF ["high"] - DF ["close"].shift (1))
 	DF ['TR 3'] = abs (DF ["low"]- DF ["close"].shift (1))
 	DF ["TR"] = round (DF [[ 'TR 1', 'TR 2', 'TR 3' ]].max (axis = 1), 2)
 	
 	DF ["ATR"] = 0.00
```

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/purchase_treasure_at_inclines.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/purchase_treasure_at_inclines.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/ramp_v1.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/ramp_v1.py`

 * *Files identical despite different names*

### Comparing `ramps_galactic-1.1.0/modules/ramps_galactic/victory_multiplier/ramp_v2.py` & `ramps_galactic-1.1.1/venues/stages/ramps_galactic/victory_multiplier/ramp_v2.py`

 * *Files identical despite different names*

