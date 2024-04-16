# Comparing `tmp/factory_farm-1.1.3.tar.gz` & `tmp/factory_farm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factory_farm-1.1.3.tar", max compression
+gzip compressed data, was "factory_farm-1.2.0.tar", max compression
```

## Comparing `factory_farm-1.1.3.tar` & `factory_farm-1.2.0.tar`

### file list

```diff
@@ -1,703 +1,710 @@
--rw-r--r--   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.1.3/license.S.HTML
--rw-r--r--   0        0        0     1203 2024-04-16 02:56:25.710342 factory_farm-1.1.3/pyproject.toml
--rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.1.3/readme.md
--rw-r--r--   0        0        0     2227 2024-04-16 02:40:00.549573 factory_farm-1.1.3/venue.S.HTML
--rw-r--r--   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.1.3/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
--rw-r--r--   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     3866 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.1.3/venues/stages/factory_farm/__bin/factory_farm_1
--rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.1.3/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_book/book.s.HTML
--rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.1.3/venues/stages/factory_farm/_clique/__init__.py
--rw-r--r--   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.1.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.1.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.1.3/venues/stages/factory_farm/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.1.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.1.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/--statuspy.py
--rwxr-xr-x   0        0        0   518746 2024-04-16 02:45:28.933836 factory_farm-1.1.3/venues/stages/factory_farm/_status/DB/records.json
--rw-r--r--   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.1.3/venues/stages/factory_farm/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
--rw-r--r--   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
--rw-r--r--   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
--rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    63413 2024-04-16 02:45:28.897836 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.1.3/venues/stages/factory_farm/_status/status.proc.py
--rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/architecture.s.HTML
--rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.1.3/venues/stages/factory_farm/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.1.3/venues/stages/factory_farm/license.S.HTML
--rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.1.3/venues/stages/factory_farm/module.s.HTML
--rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.1.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.1.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     1146 2024-04-16 02:40:51.696992 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      562 2024-04-16 02:39:38.309829 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      890 2024-04-16 02:41:24.580618 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      588 2024-04-16 02:39:33.821881 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
--rwxr-xr-x   0        0        0      877 2024-04-16 02:41:20.608663 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     2005 2024-04-14 05:33:00.731251 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
--rwxr-xr-x   0        0        0     1956 2024-04-14 05:33:07.555211 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
--rw-r--r--   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
--rw-r--r--   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
--rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
--rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
--rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2281 2024-04-16 02:30:30.372188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
--rw-r--r--   0        0        0     2813 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
--rw-r--r--   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1081 2024-04-16 02:30:30.372188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rw-r--r--   0        0        0     2218 2024-04-16 02:30:30.376188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rw-r--r--   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rw-r--r--   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rw-r--r--   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     1282 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
--rw-r--r--   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
--rw-r--r--   0        0        0     2991 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
--rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
--rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
--rwxr-xr-x   0        0        0     1131 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-16 02:30:30.372188 factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     6643 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-16 02:30:29.476199 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
--rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__init__.py
--rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
--rw-r--r--   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
--rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.1.3/venues/stages/factory_farm/procedures/processes.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/topics/exceptions.py
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.1.3/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.1.3/venues/stages/factory_farm/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.1.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.1.3/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/one.py
--rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.1.3/venues/stages/factory_farm/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.1.3/venues/stages/factory_farm/variables/__init__.py
--rw-r--r--   0        0        0     5536 1970-01-01 00:00:00.000000 factory_farm-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.2.0/license.S.HTML
+-rw-r--r--   0        0        0     1232 2024-04-16 03:42:14.879645 factory_farm-1.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.2.0/readme.md
+-rw-r--r--   0        0        0     2064 2024-04-16 03:42:28.111496 factory_farm-1.2.0/venue.S.HTML
+-rw-r--r--   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.2.0/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rw-r--r--   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     3866 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.2.0/venues/stages/factory_farm/__bin/factory_farm_1
+-rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.2.0/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__init__.py
+-rw-r--r--   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/--statuspy.py
+-rwxr-xr-x   0        0        0   623712 2024-04-16 03:41:36.588076 factory_farm-1.2.0/venues/stages/factory_farm/_status/DB/records.json
+-rw-r--r--   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.2.0/venues/stages/factory_farm/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/status_1.py
+-rw-r--r--   0        0        0      367 2024-04-16 03:23:58.043895 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1065 2024-04-16 03:36:15.519687 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/status_1.py
+-rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
+-rw-r--r--   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
+-rw-r--r--   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
+-rwxr-xr-x   0        0        0    63715 2024-04-16 03:41:28.864163 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.2.0/venues/stages/factory_farm/_status/status.proc.py
+-rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/architecture.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.2.0/venues/stages/factory_farm/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.2.0/venues/stages/factory_farm/license.S.HTML
+-rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.2.0/venues/stages/factory_farm/module.s.HTML
+-rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
+-rw-r--r--   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     1146 2024-04-16 02:40:51.696992 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      562 2024-04-16 02:39:38.309829 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      890 2024-04-16 02:41:24.580618 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      588 2024-04-16 02:39:33.821881 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:41:20.608663 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2005 2024-04-14 05:33:00.731251 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1956 2024-04-14 05:33:07.555211 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
+-rw-r--r--   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
+-rw-r--r--   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
+-rw-r--r--   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
+-rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
+-rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
+-rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2379 2024-04-16 03:23:57.115905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
+-rw-r--r--   0        0        0     3030 2024-04-16 03:21:03.897796 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
+-rw-r--r--   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     1232 2024-04-16 03:23:57.111905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rw-r--r--   0        0        0     2561 2024-04-16 03:40:58.876501 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rw-r--r--   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rw-r--r--   0        0        0      860 2024-04-16 03:35:16.680347 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rw-r--r--   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rw-r--r--   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     1678 2024-04-16 03:23:14.884368 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
+-rw-r--r--   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
+-rw-r--r--   0        0        0     3638 2024-04-16 03:41:47.775951 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
+-rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
+-rw-r--r--   0        0        0     1077 2024-04-16 03:35:13.940378 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py
+-rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
+-rwxr-xr-x   0        0        0     1213 2024-04-16 03:20:38.414072 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-16 03:23:57.111905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     6719 2024-04-16 03:40:15.480990 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__init__.py
+-rw-r--r--   0        0        0     3217 2024-04-16 03:40:58.048510 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
+-rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__.py
+-rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
+-rw-r--r--   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
+-rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/processes.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/one.py
+-rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.2.0/venues/stages/factory_farm/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.2.0/venues/stages/factory_farm/variables/__init__.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 factory_farm-1.2.0/PKG-INFO
```

### Comparing `factory_farm-1.1.3/pyproject.toml` & `factory_farm-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 
 
 
 
 [tool.poetry]
 name = "factory_farm"
-version = "1.1.3"
-description = "Ensuring that your prod-uctions are absolutely stunning"
+version = "1.2.0"
+description = "The automated cybentic herb harvest factory of plantary towns yet to be established."
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "factory_farm", from = "venues/stages" }
 ]
 exclude = []
```

### Comparing `factory_farm-1.1.3/readme.md` & `factory_farm-1.2.0/readme.md`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venue.S.HTML` & `factory_farm-1.2.0/venue.S.HTML`

 * *Files 8% similar despite different names*

```diff
@@ -65,26 +65,21 @@
 
 		
 		#
 		#	statuses
 		#
 		python3 /factory_farm/venues/stages/factory_farm/_status/status.proc.py
 		
-		#
-		#	readme
-		#
-		cp /factory_farm/venues/stages/factory_farm/room.md /factory_farm/readme.md
+
 		
 		#
 		#	poetry auth
 		#
-		
 		rm -rf dist && poetry build --verbose && poetry publish --verbose;
 		
-		# rm -rf stages_pip && pip install factory_farm -t stages_pip
 
 	<h2>important</h2>
 		poetry show --tree
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg` & `factory_farm-1.2.0/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/itinerary.S.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/maybes.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout/start.py` & `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py` & `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html` & `factory_farm-1.2.0/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_book/advanced tutorial.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_book/book.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_book/relevant.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_clique/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/establish.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/establish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/0_start/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/1/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/2/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/6_various/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/7/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975247524752475%*

 * *Differences: {"'_default'": "{'202': OrderedDict([('paths', [OrderedDict([('path', 'guarantee_1.py'), ('empty', "*

 * *               "False), ('parsed', True), ('stats', OrderedDict([('passes', 1), ('alarms', 0)])), "*

 * *               "('checks', [OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[3.339999238960445e-06, 'seconds'])])])])]), ('alarms', []), ('stats', "*

 * *               "OrderedDict([('alarms', 0), ('empty', 0), ('checks', OrderedDict([('passes', 1), "*

 * *               "('alarms', 0 […]*

```diff
@@ -3676,14 +3676,46 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "202": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.339999238960445e-06,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "guarantee_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 0,
+                    "passes": 1
+                },
+                "empty": 0
+            }
+        },
         "21": {
             "alarms": [],
             "paths": [
                 {
                     "checks": [
                         {
                             "check": "check 1",
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status/status.proc.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json` & `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/_status_advanced/status.proc.py` & `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/architecture.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/module.s.HTML` & `factory_farm-1.2.0/venues/stages/factory_farm/module.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/on.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/on.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 02:23:09 2024 UTC, .py size: 2813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0de1 1d66 fd0a 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 9fee 1d66 d60b 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 0100 6400 6401 6c07  m.Z.m.Z...d.d.l.
 00000060: 5a07 6400 6401 6c08 5a08 6400 6401 6c09  Z.d.d.l.Z.d.d.l.
 00000070: 5a09 6400 6403 6c0a 6d0b 5a0b 6d0c 5a0c  Z.d.d.l.m.Z.m.Z.
@@ -54,90 +54,96 @@
 00000350: 6170 6163 6974 79da 0662 6566 6f72 65da  apacity..before.
 00000360: 0561 6674 6572 da0f 696e 7472 6f5f 7661  .after..intro_va
 00000370: 7269 6162 6c65 73da 1074 6865 5f69 6e74  riables..the_int
 00000380: 726f 5f68 6172 626f 72da 0c69 6e74 726f  ro_harbor..intro
 00000390: 5f68 6172 626f 72da 0379 6573 da17 696e  _harbor..yes..in
 000003a0: 7465 726e 616c 5f73 7461 7475 7365 735f  ternal_statuses_
 000003b0: 6275 696c 7463 0100 0000 0000 0000 0000  builtc..........
-000003c0: 0000 0200 0000 0600 0000 1300 0000 7348  ..............sH
-000003d0: 0000 0074 007c 0088 0188 0264 0188 0069  ...t.|.....d...i
-000003e0: 0164 029c 0464 038d 017d 0174 0183 0001  .d...d...}.t....
-000003f0: 0074 0164 047c 0183 0201 0074 0183 0001  .t.d.|.....t....
-00000400: 007c 0174 0264 0519 0074 037c 0088 0283  .|.t.d...t.|....
-00000410: 0219 0064 063c 007c 0153 0029 074e da04  ...d.<.|.S.).N..
-00000420: 706f 7274 2904 da11 7374 6174 7573 5f63  port)...status_c
-00000430: 6865 636b 5f70 6174 6872 1100 0000 7212  heck_pathr....r.
-00000440: 0000 00da 1269 6d70 6c69 6369 745f 7072  .....implicit_pr
-00000450: 6f63 6564 7572 6529 01da 0670 6163 6b65  ocedure)...packe
-00000460: 747a 0974 6865 5f73 6361 6e3a da11 696e  tz.the_scan:..in
-00000470: 7465 726e 616c 5f73 7461 7475 7365 73da  ternal_statuses.
-00000480: 0770 726f 6365 7373 2904 7208 0000 00da  .process).r.....
-00000490: 0570 7269 6e74 7209 0000 0072 0b00 0000  .printr....r....
-000004a0: 2902 721d 0000 00da 0874 6865 5f73 6361  ).r......the_sca
-000004b0: 6e29 03da 1769 6d70 6c69 6369 745f 7072  n)...implicit_pr
-000004c0: 6f63 6564 7572 655f 706f 7274 7211 0000  ocedure_portr...
-000004d0: 0072 1200 0000 a900 fa68 2f66 6163 746f  .r.......h/facto
-000004e0: 7279 5f66 6172 6d2f 7665 6e75 6573 2f73  ry_farm/venues/s
-000004f0: 7461 6765 732f 6661 6374 6f72 795f 6661  tages/factory_fa
-00000500: 726d 2f70 726f 6365 6475 7265 732f 696d  rm/procedures/im
-00000510: 706c 6963 6974 5f70 726f 6365 6475 7265  plicit_procedure
-00000520: 2f70 726f 6365 7373 2f6b 6567 2f73 7061  /process/keg/spa
-00000530: 6365 732f 7061 7468 735f 7061 7463 682e  ces/paths_patch.
-00000540: 7079 da07 7665 6e74 7572 6558 0000 0073  py..ventureX...s
-00000550: 2800 0000 0201 0202 0202 0201 0403 02ff  (...............
-00000560: 04fa 06ff 060d 0a01 0601 0209 02fa 0201  ................
-00000570: 02ff 0803 02fd 0205 02fb 0409 7a31 7061  ............z1pa
-00000580: 7468 735f 7061 7463 682e 3c6c 6f63 616c  ths_patch.<local
-00000590: 733e 2e70 6174 6873 5f70 6174 6368 2e3c  s>.paths_patch.<
-000005a0: 6c6f 6361 6c73 3e2e 7665 6e74 7572 6529  locals>.venture)
-000005b0: 03da 0863 6170 6163 6974 79da 0569 7465  ...capacity..ite
-000005c0: 6d73 da04 6d6f 7665 7a20 7175 6575 655f  ms..movez queue_
-000005d0: 6361 7061 6369 7479 5f6c 696d 6974 6572  capacity_limiter
-000005e0: 2070 726f 6365 6564 733a da08 7265 6365   proceeds:..rece
-000005f0: 6976 6564 290b 7222 0000 00da 046a 736f  ived).r".....jso
-00000600: 6eda 056c 6f61 6473 7206 0000 0072 0f00  n..loadsr....r..
-00000610: 0000 da06 6465 636f 6465 da04 7269 6368  ....decode..rich
-00000620: da0a 7072 696e 745f 6a73 6f6e 7209 0000  ..print_jsonr...
-00000630: 0072 0a00 0000 7207 0000 0029 09da 0a74  .r....r....)...t
-00000640: 6865 5f70 6163 6b65 7472 1000 0000 7213  he_packetr....r.
-00000650: 0000 0072 1400 0000 7215 0000 0072 1600  ...r....r....r..
-00000660: 0000 7227 0000 00da 0870 726f 6365 6564  ..r'.....proceed
-00000670: 7372 1d00 0000 a901 7224 0000 0029 0272  sr......r$...).r
-00000680: 1100 0000 7212 0000 0072 2600 0000 da0b  ....r....r&.....
-00000690: 7061 7468 735f 7061 7463 681d 0000 0073  paths_patch....s
-000006a0: 4600 0000 0802 0203 1210 0401 0401 08ff  F...............
-000006b0: 0806 0802 0801 0802 0801 0802 0801 0804  ................
-000006c0: 0c01 0204 0203 0201 0201 04fe 0804 1006  ................
-000006d0: 0420 0201 0201 0201 0201 06fd 0a06 0206  . ..............
-000006e0: 0404 08f9 0a01 0202 0404 7a20 7061 7468  ..........z path
-000006f0: 735f 7061 7463 682e 3c6c 6f63 616c 733e  s_patch.<locals>
-00000700: 2e70 6174 6873 5f70 6174 6368 2901 da05  .paths_patch)...
-00000710: 726f 7574 6529 03da 0361 7070 7224 0000  route)...appr$..
-00000720: 0072 3400 0000 7225 0000 0072 3300 0000  .r4...r%...r3...
-00000730: 7226 0000 0072 3400 0000 1800 0000 7304  r&...r4.......s.
-00000740: 0000 000e 0512 0172 3400 0000 2901 4e29  .......r4...).N)
-00000750: 1872 2c00 0000 da07 7061 7468 6c69 62da  .r,.....pathlib.
-00000760: 026f 73da 076f 732e 7061 7468 7202 0000  .os..os.pathr...
-00000770: 0072 0300 0000 7204 0000 00da 0373 7973  .r....r......sys
-00000780: da09 7468 7265 6164 696e 67da 0474 696d  ..threading..tim
-00000790: 65da 0566 6c61 736b 7205 0000 0072 0600  e..flaskr....r..
-000007a0: 0000 722f 0000 00da 3166 6163 746f 7279  ..r/....1factory
-000007b0: 5f66 6172 6d2e 746f 7069 6373 2e71 7565  _farm.topics.que
-000007c0: 7565 732e 7175 6575 655f 6361 7061 6369  ues.queue_capaci
-000007d0: 7479 5f6c 696d 6974 6572 7207 0000 00da  ty_limiterr.....
-000007e0: 2666 6163 746f 7279 5f66 6172 6d2e 7072  &factory_farm.pr
-000007f0: 6f63 6564 7572 6573 2e68 6561 6c74 685f  ocedures.health_
-00000800: 7363 616e 2e6f 6e72 0800 0000 da3c 6661  scan.onr.....<fa
-00000810: 6374 6f72 795f 6661 726d 2e70 726f 6365  ctory_farm.proce
-00000820: 6475 7265 732e 696d 706c 6963 6974 5f70  dures.implicit_p
-00000830: 726f 6365 6475 7265 2e70 726f 6365 7373  rocedure.process
-00000840: 2e76 6172 6961 626c 6573 7209 0000 0072  .variablesr....r
-00000850: 0a00 0000 da44 6661 6374 6f72 795f 6661  .....Dfactory_fa
-00000860: 726d 2e70 726f 6365 6475 7265 732e 696d  rm.procedures.im
-00000870: 706c 6963 6974 5f70 726f 6365 6475 7265  plicit_procedure
-00000880: 2e70 726f 6365 7373 2e6d 6f76 6573 2e66  .process.moves.f
-00000890: 6f72 6d61 745f 7061 7468 720b 0000 0072  ormat_pathr....r
-000008a0: 3400 0000 7225 0000 0072 2500 0000 7225  4...r%...r%...r%
-000008b0: 0000 0072 2600 0000 da08 3c6d 6f64 756c  ...r&.....<modul
-000008c0: 653e 0100 0000 731e 0000 0008 0308 0108  e>....s.........
-000008d0: 0114 0108 0108 0108 0110 0308 010c 020c  ................
-000008e0: 0110 020c 0102 070e fd                   .........
+000003c0: 0000 0300 0000 0600 0000 1300 0000 736e  ..............sn
+000003d0: 0000 0074 0074 01a0 01a1 0083 017d 0174  ...t.t.......}.t
+000003e0: 027c 0088 0188 0264 0188 0069 0164 029c  .|.....d...i.d..
+000003f0: 0464 038d 017d 0274 0383 0001 0074 0364  .d...}.t.....t.d
+00000400: 047c 0283 0201 0074 0383 0001 007c 0274  .|.....t.....|.t
+00000410: 0464 0519 0074 057c 0088 0283 0219 0064  .d...t.|.......d
+00000420: 063c 007c 0174 0464 0519 0074 057c 0088  .<.|.t.d...t.|..
+00000430: 0283 0219 0064 0719 0064 083c 007c 0253  .....d...d.<.|.S
+00000440: 0029 094e da04 706f 7274 2904 da11 7374  .).N..port)...st
+00000450: 6174 7573 5f63 6865 636b 5f70 6174 6872  atus_check_pathr
+00000460: 1100 0000 7212 0000 00da 1269 6d70 6c69  ....r......impli
+00000470: 6369 745f 7072 6f63 6564 7572 6529 01da  cit_procedure)..
+00000480: 0670 6163 6b65 747a 0974 6865 5f73 6361  .packetz.the_sca
+00000490: 6e3a da11 696e 7465 726e 616c 5f73 7461  n:..internal_sta
+000004a0: 7475 7365 73da 0770 726f 6365 7373 da05  tuses..process..
+000004b0: 7469 6d65 73da 0773 7461 7274 6564 2906  times..started).
+000004c0: da03 7374 72da 0474 696d 6572 0800 0000  ..str..timer....
+000004d0: da05 7072 696e 7472 0900 0000 720b 0000  ..printr....r...
+000004e0: 0029 0372 1d00 0000 da0a 7374 6172 745f  .).r......start_
+000004f0: 7469 6d65 da08 7468 655f 7363 616e 2903  time..the_scan).
+00000500: da17 696d 706c 6963 6974 5f70 726f 6365  ..implicit_proce
+00000510: 6475 7265 5f70 6f72 7472 1100 0000 7212  dure_portr....r.
+00000520: 0000 00a9 00fa 682f 6661 6374 6f72 795f  ......h/factory_
+00000530: 6661 726d 2f76 656e 7565 732f 7374 6167  farm/venues/stag
+00000540: 6573 2f66 6163 746f 7279 5f66 6172 6d2f  es/factory_farm/
+00000550: 7072 6f63 6564 7572 6573 2f69 6d70 6c69  procedures/impli
+00000560: 6369 745f 7072 6f63 6564 7572 652f 7072  cit_procedure/pr
+00000570: 6f63 6573 732f 6b65 672f 7370 6163 6573  ocess/keg/spaces
+00000580: 2f70 6174 6873 5f70 6174 6368 2e70 79da  /paths_patch.py.
+00000590: 0776 656e 7475 7265 5800 0000 733e 0000  .ventureX...s>..
+000005a0: 000c 0102 0202 0202 0202 0104 0302 ff04  ................
+000005b0: fa06 ff06 0d0a 0106 0102 0902 fa02 0102  ................
+000005c0: ff08 0302 fd02 0502 fb02 1102 f802 0102  ................
+000005d0: ff08 0302 fd02 0502 fb02 0702 f904 0a7a  ...............z
+000005e0: 3170 6174 6873 5f70 6174 6368 2e3c 6c6f  1paths_patch.<lo
+000005f0: 6361 6c73 3e2e 7061 7468 735f 7061 7463  cals>.paths_patc
+00000600: 682e 3c6c 6f63 616c 733e 2e76 656e 7475  h.<locals>.ventu
+00000610: 7265 2903 da08 6361 7061 6369 7479 da05  re)...capacity..
+00000620: 6974 656d 73da 046d 6f76 657a 2071 7565  items..movez que
+00000630: 7565 5f63 6170 6163 6974 795f 6c69 6d69  ue_capacity_limi
+00000640: 7465 7220 7072 6f63 6565 6473 3ada 0872  ter proceeds:..r
+00000650: 6563 6569 7665 6429 0b72 2600 0000 da04  eceived).r&.....
+00000660: 6a73 6f6e da05 6c6f 6164 7372 0600 0000  json..loadsr....
+00000670: 720f 0000 00da 0664 6563 6f64 65da 0472  r......decode..r
+00000680: 6963 68da 0a70 7269 6e74 5f6a 736f 6e72  ich..print_jsonr
+00000690: 0900 0000 720a 0000 0072 0700 0000 2909  ....r....r....).
+000006a0: da0a 7468 655f 7061 636b 6574 7210 0000  ..the_packetr...
+000006b0: 0072 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
+000006c0: 7216 0000 0072 2c00 0000 da08 7072 6f63  r....r,.....proc
+000006d0: 6565 6473 721d 0000 00a9 0172 2900 0000  eedsr......r)...
+000006e0: 2902 7211 0000 0072 1200 0000 722b 0000  ).r....r....r+..
+000006f0: 00da 0b70 6174 6873 5f70 6174 6368 1d00  ...paths_patch..
+00000700: 0000 7346 0000 0008 0202 0312 1004 0104  ..sF............
+00000710: 0108 ff08 0608 0208 0108 0208 0108 0208  ................
+00000720: 0108 040c 0102 0402 0302 0102 0104 fe08  ................
+00000730: 0410 0604 2c02 0102 0102 0102 0106 fd0a  ....,...........
+00000740: 0602 0604 0408 f90a 0102 0204 047a 2070  .............z p
+00000750: 6174 6873 5f70 6174 6368 2e3c 6c6f 6361  aths_patch.<loca
+00000760: 6c73 3e2e 7061 7468 735f 7061 7463 6829  ls>.paths_patch)
+00000770: 01da 0572 6f75 7465 2903 da03 6170 7072  ...route)...appr
+00000780: 2900 0000 7239 0000 0072 2a00 0000 7238  )...r9...r*...r8
+00000790: 0000 0072 2b00 0000 7239 0000 0018 0000  ...r+...r9......
+000007a0: 0073 0400 0000 0e05 1201 7239 0000 0029  .s........r9...)
+000007b0: 014e 2918 7231 0000 00da 0770 6174 686c  .N).r1.....pathl
+000007c0: 6962 da02 6f73 da07 6f73 2e70 6174 6872  ib..os..os.pathr
+000007d0: 0200 0000 7203 0000 0072 0400 0000 da03  ....r....r......
+000007e0: 7379 73da 0974 6872 6561 6469 6e67 7225  sys..threadingr%
+000007f0: 0000 00da 0566 6c61 736b 7205 0000 0072  .....flaskr....r
+00000800: 0600 0000 7234 0000 00da 3166 6163 746f  ....r4....1facto
+00000810: 7279 5f66 6172 6d2e 746f 7069 6373 2e71  ry_farm.topics.q
+00000820: 7565 7565 732e 7175 6575 655f 6361 7061  ueues.queue_capa
+00000830: 6369 7479 5f6c 696d 6974 6572 7207 0000  city_limiterr...
+00000840: 00da 2666 6163 746f 7279 5f66 6172 6d2e  ..&factory_farm.
+00000850: 7072 6f63 6564 7572 6573 2e68 6561 6c74  procedures.healt
+00000860: 685f 7363 616e 2e6f 6e72 0800 0000 da3c  h_scan.onr.....<
+00000870: 6661 6374 6f72 795f 6661 726d 2e70 726f  factory_farm.pro
+00000880: 6365 6475 7265 732e 696d 706c 6963 6974  cedures.implicit
+00000890: 5f70 726f 6365 6475 7265 2e70 726f 6365  _procedure.proce
+000008a0: 7373 2e76 6172 6961 626c 6573 7209 0000  ss.variablesr...
+000008b0: 0072 0a00 0000 da44 6661 6374 6f72 795f  .r.....Dfactory_
+000008c0: 6661 726d 2e70 726f 6365 6475 7265 732e  farm.procedures.
+000008d0: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
+000008e0: 7265 2e70 726f 6365 7373 2e6d 6f76 6573  re.process.moves
+000008f0: 2e66 6f72 6d61 745f 7061 7468 720b 0000  .format_pathr...
+00000900: 0072 3900 0000 722a 0000 0072 2a00 0000  .r9...r*...r*...
+00000910: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
+00000920: 756c 653e 0100 0000 731e 0000 0008 0308  ule>....s.......
+00000930: 0108 0114 0108 0108 0108 0110 0308 010c  ................
+00000940: 020c 0110 020c 0102 070e fd              ...........
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py`

 * *Files 16% similar despite different names*

```diff
@@ -82,14 +82,16 @@
 		implicit_procedure_variables ["internal_statuses_built"] = "yes"
 		#
 		# ----
 		
 		
 		
 		def venture (status_check_path):
+			start_time = str (time.time ())
+		
 			the_scan = turn_on_health_check (
 				packet = {
 					"status_check_path": status_check_path,
 					
 					"module_paths": module_paths,
 					"relative_path": relative_path,
 					
@@ -109,14 +111,24 @@
 			] [ 
 				format_path (status_check_path, relative_path) 
 			] [ 
 				"process" 
 			] = the_scan
 		
 		
+			implicit_procedure_variables [
+				"internal_statuses"
+			] [ 
+				format_path (status_check_path, relative_path) 
+			] [
+				"times"
+			] [
+				"started"
+			] = start_time
+		
 			return the_scan;
 		
 		
 		
 		if (simultaneous):
 			proceeds = queue_capacity_limiter (
 				capacity = simultaneous_capacity,
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 02:23:09 2024 UTC, .py size: 1282 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0de1 1d66 0205 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 22ef 1d66 8e06 0000  o......."..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6402 6c08 5a08 6401 6402 6c09 5a09 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c0a 5a0a 6401 6404 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
@@ -16,53 +16,62 @@
 000000f0: 6a6f 696e da08 6e6f 726d 7061 7468 2902  join..normpath).
 00000100: da05 466c 6173 6bda 0772 6571 7565 7374  ..Flask..request
 00000110: 2901 da1c 696d 706c 6963 6974 5f70 726f  )...implicit_pro
 00000120: 6365 6475 7265 5f76 6172 6961 626c 6573  cedure_variables
 00000130: e901 0000 0029 01da 0f61 6767 7265 6761  .....)...aggrega
 00000140: 7465 5f73 7461 7473 da00 6301 0000 0000  te_stats..c.....
 00000150: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
-00000160: 0000 0073 8000 0000 7c00 6401 1900 7d01  ...s....|.d...}.
+00000160: 0000 0073 dc00 0000 7c00 6401 1900 7d01  ...s....|.d...}.
 00000170: 7c00 6402 1900 7d02 7c00 6403 1900 7d03  |.d...}.|.d...}.
 00000180: 0900 7400 6404 7401 6405 1900 7c01 1900  ..t.d.t.d...|...
 00000190: 6406 1900 6406 1900 8302 0100 6401 7c01  d...d.......d.|.
 000001a0: 6901 7c02 a501 7d04 6407 7401 6405 1900  i.|...}.d.t.d...
 000001b0: 7c01 1900 6408 1900 6409 3c00 7c04 7401  |...d...d.<.|.t.
-000001c0: 6405 1900 7c01 1900 640a 3c00 7401 6405  d...|...d.<.t.d.
-000001d0: 1900 7c01 1900 6406 1900 6406 1900 a002  ..|...d...d.....
-000001e0: a100 0100 6400 5300 290b 4eda 0470 6174  ....d.S.).N..pat
-000001f0: 68da 0672 6573 756c 74da 0370 6964 7a09  h..result..pidz.
-00000200: 7374 6f70 7069 6e67 3ada 1169 6e74 6572  stopping:..inter
-00000210: 6e61 6c5f 7374 6174 7573 6573 da07 7072  nal_statuses..pr
-00000220: 6f63 6573 73da 0464 6f6e 65da 0673 7461  ocess..done..sta
-00000230: 7475 73da 0473 6361 6eda 0f72 6573 756c  tus..scan..resul
-00000240: 7473 5f6f 665f 7363 616e 2903 da05 7072  ts_of_scan)...pr
-00000250: 696e 7472 0700 0000 da09 7465 726d 696e  intr......termin
-00000260: 6174 6529 05da 0a74 6865 5f70 6163 6b65  ate)...the_packe
-00000270: 74da 0874 6865 5f70 6174 68da 0a74 6865  t..the_path..the
-00000280: 5f72 6573 756c 74da 0774 6865 5f70 6964  _result..the_pid
-00000290: 7211 0000 00a9 0072 1a00 0000 fa66 2f66  r......r.....f/f
-000002a0: 6163 746f 7279 5f66 6172 6d2f 7665 6e75  actory_farm/venu
-000002b0: 6573 2f73 7461 6765 732f 6661 6374 6f72  es/stages/factor
-000002c0: 795f 6661 726d 2f70 726f 6365 6475 7265  y_farm/procedure
-000002d0: 732f 696d 706c 6963 6974 5f70 726f 6365  s/implicit_proce
-000002e0: 6475 7265 2f70 726f 6365 7373 2f6d 6f76  dure/process/mov
-000002f0: 6573 2f64 6f6e 655f 7769 7468 5f73 6361  es/done_with_sca
-00000300: 6e2e 7079 da13 646f 6e65 5f77 6974 685f  n.py..done_with_
-00000310: 7363 616e 5f6d 6f76 651a 0000 0073 1800  scan_move....s..
-00000320: 0000 0803 0801 0801 0202 1a09 0404 02ff  ................
-00000330: 0202 04fe 1407 1001 1c07 721c 0000 0029  ..........r....)
-00000340: 0172 0a00 0000 2913 da07 5f5f 646f 635f  .r....)...__doc_
-00000350: 5fda 046a 736f 6eda 0770 6174 686c 6962  _..json..pathlib
-00000360: da02 6f73 da07 6f73 2e70 6174 6872 0200  ..os..os.pathr..
-00000370: 0000 7203 0000 0072 0400 0000 da03 7379  ..r....r......sy
-00000380: 73da 0974 6872 6561 6469 6e67 da04 7469  s..threading..ti
-00000390: 6d65 da05 666c 6173 6b72 0500 0000 7206  me..flaskr....r.
-000003a0: 0000 00da 0472 6963 68da 3c66 6163 746f  .....rich.<facto
-000003b0: 7279 5f66 6172 6d2e 7072 6f63 6564 7572  ry_farm.procedur
-000003c0: 6573 2e69 6d70 6c69 6369 745f 7072 6f63  es.implicit_proc
-000003d0: 6564 7572 652e 7072 6f63 6573 732e 7661  edure.process.va
-000003e0: 7269 6162 6c65 7372 0700 0000 7209 0000  riablesr....r...
-000003f0: 0072 1c00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000400: 721a 0000 0072 1b00 0000 da08 3c6d 6f64  r....r......<mod
-00000410: 756c 653e 0100 0000 731c 0000 0004 0208  ule>....s.......
-00000420: 0408 0108 0114 0108 0108 0108 0110 0208  ................
-00000430: 020c 030c 0202 050e ff                   .........
+000001c0: 6405 1900 7c01 1900 640a 3c00 7402 7403  d...|...d.<.t.t.
+000001d0: a003 a100 8301 7401 6405 1900 7c01 1900  ......t.d...|...
+000001e0: 640b 1900 640c 3c00 7404 7401 6405 1900  d...d.<.t.t.d...
+000001f0: 7c01 1900 640b 1900 640c 1900 8301 7404  |...d...d.....t.
+00000200: 7401 6405 1900 7c01 1900 640b 1900 640d  t.d...|...d...d.
+00000210: 1900 8301 1800 7401 6405 1900 7c01 1900  ......t.d...|...
+00000220: 640b 1900 640e 3c00 7401 6405 1900 7c01  d...d.<.t.d...|.
+00000230: 1900 6406 1900 6406 1900 a005 a100 0100  ..d...d.........
+00000240: 6400 5300 290f 4eda 0470 6174 68da 0672  d.S.).N..path..r
+00000250: 6573 756c 74da 0370 6964 7a09 7374 6f70  esult..pidz.stop
+00000260: 7069 6e67 3ada 1169 6e74 6572 6e61 6c5f  ping:..internal_
+00000270: 7374 6174 7573 6573 da07 7072 6f63 6573  statuses..proces
+00000280: 73da 0464 6f6e 65da 0673 7461 7475 73da  s..done..status.
+00000290: 0473 6361 6eda 0f72 6573 756c 7473 5f6f  .scan..results_o
+000002a0: 665f 7363 616e da05 7469 6d65 73da 0565  f_scan..times..e
+000002b0: 6e64 6564 da07 7374 6172 7465 64da 0765  nded..started..e
+000002c0: 6c61 7073 6564 2906 da05 7072 696e 7472  lapsed)...printr
+000002d0: 0700 0000 da03 7374 72da 0474 696d 65da  ......str..time.
+000002e0: 0566 6c6f 6174 da09 7465 726d 696e 6174  .float..terminat
+000002f0: 6529 05da 0a74 6865 5f70 6163 6b65 74da  e)...the_packet.
+00000300: 0874 6865 5f70 6174 68da 0a74 6865 5f72  .the_path..the_r
+00000310: 6573 756c 74da 0774 6865 5f70 6964 7211  esult..the_pidr.
+00000320: 0000 00a9 0072 2100 0000 fa66 2f66 6163  .....r!....f/fac
+00000330: 746f 7279 5f66 6172 6d2f 7665 6e75 6573  tory_farm/venues
+00000340: 2f73 7461 6765 732f 6661 6374 6f72 795f  /stages/factory_
+00000350: 6661 726d 2f70 726f 6365 6475 7265 732f  farm/procedures/
+00000360: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
+00000370: 7265 2f70 726f 6365 7373 2f6d 6f76 6573  re/process/moves
+00000380: 2f64 6f6e 655f 7769 7468 5f73 6361 6e2e  /done_with_scan.
+00000390: 7079 da13 646f 6e65 5f77 6974 685f 7363  py..done_with_sc
+000003a0: 616e 5f6d 6f76 651a 0000 0073 2200 0000  an_move....s"...
+000003b0: 0803 0801 0801 0202 1a09 0404 02ff 0202  ................
+000003c0: 04fe 1407 1001 1c02 1603 1601 02ff 12ff  ................
+000003d0: 1c09 7223 0000 0029 0172 0a00 0000 2913  ..r#...).r....).
+000003e0: da07 5f5f 646f 635f 5fda 046a 736f 6eda  ..__doc__..json.
+000003f0: 0770 6174 686c 6962 da02 6f73 da07 6f73  .pathlib..os..os
+00000400: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
+00000410: 0400 0000 da03 7379 73da 0974 6872 6561  ......sys..threa
+00000420: 6469 6e67 721a 0000 00da 0566 6c61 736b  dingr......flask
+00000430: 7205 0000 0072 0600 0000 da04 7269 6368  r....r......rich
+00000440: da3c 6661 6374 6f72 795f 6661 726d 2e70  .<factory_farm.p
+00000450: 726f 6365 6475 7265 732e 696d 706c 6963  rocedures.implic
+00000460: 6974 5f70 726f 6365 6475 7265 2e70 726f  it_procedure.pro
+00000470: 6365 7373 2e76 6172 6961 626c 6573 7207  cess.variablesr.
+00000480: 0000 0072 0900 0000 7223 0000 0072 2100  ...r....r#...r!.
+00000490: 0000 7221 0000 0072 2100 0000 7222 0000  ..r!...r!...r"..
+000004a0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000004b0: 1c00 0000 0402 0804 0801 0801 1401 0801  ................
+000004c0: 0801 0801 1002 0802 0c03 0c02 0205 0eff  ................
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 02:23:09 2024 UTC, .py size: 2991 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,161 @@
-00000000: 6f0d 0d0a 0000 0000 0de1 1d66 af0b 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 46f3 1d66 360e 0000  o.......F..f6...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
+00000020: 0002 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c08 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
-00000070: 6407 6c09 6d09 5a09 0100 6408 6409 8400  d.l.m.Z...d.d...
-00000080: 5a0a 640a 640b 8400 5a0b 640c 640d 8400  Z.d.d...Z.d.d...
-00000090: 5a0c 6402 5300 290e 7a23 0a09 7468 655f  Z.d.S.).z#..the_
-000000a0: 7363 616e 205b 2270 726f 6365 7373 225d  scan ["process"]
-000000b0: 2e69 735f 616c 6976 6520 2829 0ae9 0000  .is_alive ()....
-000000c0: 0000 4e29 01da 1c69 6d70 6c69 6369 745f  ..N)...implicit_
-000000d0: 7072 6f63 6564 7572 655f 7661 7269 6162  procedure_variab
-000000e0: 6c65 7329 01da 0f69 6d70 6c69 6369 745f  les)...implicit_
-000000f0: 7468 7265 6164 e901 0000 0029 01da 0973  thread.....)...s
-00000100: 656e 645f 646f 6e65 2901 da0f 6167 6772  end_done)...aggr
-00000110: 6567 6174 655f 7374 6174 7363 0000 0000  egate_statsc....
-00000120: 0000 0000 0000 0000 0600 0000 0b00 0000  ................
-00000130: 4300 0000 73dc 0000 0074 0064 0119 007d  C...s....t.d...}
-00000140: 0069 007d 0167 007d 027c 0044 005d 4c7d  .i.}.g.}.|.D.]L}
-00000150: 0364 027d 047a 2174 0164 037c 007c 0319  .d.}.z!t.d.|.|..
-00000160: 0083 0201 007c 007c 0319 0064 0419 0064  .....|.|...d...d
-00000170: 0419 00a0 02a1 0064 056b 0272 2e64 067d  .......d.k.r.d.}
-00000180: 0464 0674 0064 0119 007c 0319 0064 0719  .d.t.d...|...d..
-00000190: 0064 043c 0057 006e 1904 0074 0379 4801  .d.<.W.n...t.yH.
-000001a0: 007d 0501 007a 0d74 0164 0874 04a0 05a1  .}...z.t.d.t....
-000001b0: 0083 0201 0057 0059 0064 007d 057e 056e  .....W.Y.d.}.~.n
-000001c0: 0564 007d 057e 0577 0177 007c 007c 0319  .d.}.~.w.w.|.|..
-000001d0: 0064 0719 0064 0919 007c 0464 0a9c 027c  .d...d...|.d...|
-000001e0: 017c 033c 0071 0a09 007c 0144 005d 0f7d  .|.<.q...|.D.].}
-000001f0: 037c 017c 0319 0064 0419 0064 066b 0372  .|.|...d...d.k.r
-00000200: 697c 02a0 067c 03a1 0101 0071 5a7c 017c  i|...|.....qZ|.|
-00000210: 0267 0253 0029 0b4e da11 696e 7465 726e  .g.S.).N..intern
-00000220: 616c 5f73 7461 7475 7365 73da 0770 656e  al_statuses..pen
-00000230: 6469 6e67 7a18 6368 6563 6b69 6e67 2070  dingz.checking p
-00000240: 726f 6365 7373 2073 7461 7475 733a da07  rocess status:..
-00000250: 7072 6f63 6573 7346 da04 646f 6e65 da06  processF..done..
-00000260: 7374 6174 7573 7a1a 7061 7273 6520 616e  statusz.parse an
-00000270: 6420 6368 6563 6b20 6578 6365 7074 696f  d check exceptio
-00000280: 6e3a da04 7363 616e 2902 720c 0000 0072  n:..scan).r....r
-00000290: 0900 0000 2907 7202 0000 00da 0570 7269  ....).r......pri
-000002a0: 6e74 da08 6973 5f61 6c69 7665 da09 4578  nt..is_alive..Ex
-000002b0: 6365 7074 696f 6eda 0974 7261 6365 6261  ception..traceba
-000002c0: 636b da0a 666f 726d 6174 5f65 7863 da06  ck..format_exc..
-000002d0: 6170 7065 6e64 2906 7207 0000 00da 0873  append).r......s
-000002e0: 7461 7475 7365 73da 0a75 6e66 696e 6973  tatuses..unfinis
-000002f0: 6865 64da 0b73 7461 7475 735f 7061 7468  hed..status_path
-00000300: da0e 7072 6f63 6573 735f 7374 6174 7573  ..process_status
-00000310: da01 45a9 0072 1800 0000 fa77 2f66 6163  ..E..r.....w/fac
-00000320: 746f 7279 5f66 6172 6d2f 7665 6e75 6573  tory_farm/venues
-00000330: 2f73 7461 6765 732f 6661 6374 6f72 795f  /stages/factory_
-00000340: 6661 726d 2f70 726f 6365 6475 7265 732f  farm/procedures/
-00000350: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
-00000360: 7265 2f70 726f 6365 7373 2f6d 6f76 6573  re/process/moves
-00000370: 2f70 7269 6e74 5f69 735f 646f 6e65 5f73  /print_is_done_s
-00000380: 7461 7475 735f 7265 7065 7469 7665 6c79  tatus_repetively
-00000390: 2e70 79da 2470 6172 7365 5f61 6e64 5f63  .py.$parse_and_c
-000003a0: 6865 636b 5f69 735f 616c 6976 655f 6f66  heck_is_alive_of
-000003b0: 5f73 7461 7475 7365 7311 0000 0073 3200  _statuses....s2.
-000003c0: 0000 0801 0402 0401 0801 0401 0201 0e01  ................
-000003d0: 1801 0407 1401 0480 0e02 0e01 0c02 0880  ................
-000003e0: 02fd 0e06 0201 0cfe 0205 0805 1001 0a01  ................
-000003f0: 0280 0802 721a 0000 0063 0100 0000 0000  ....r....c......
-00000400: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
-00000410: 0000 7364 0000 0074 007c 0083 0164 016b  ..sd...t.|...d.k
-00000420: 0572 0864 0053 0009 0074 0164 0219 007d  .r.d.S...t.d...}
-00000430: 017c 0144 005d 0f7d 027c 017c 0219 0064  .|.D.].}.|.|...d
-00000440: 0319 0064 0419 0064 056b 0372 1e01 0064  ...d...d.k.r...d
-00000450: 0053 0071 0f09 0074 0274 0164 0619 0064  .S.q...t.t.d...d
-00000460: 0719 0074 0164 0619 0064 0819 0074 0383  ...t.d...d...t..
-00000470: 0064 098d 0301 0064 0053 0029 0a4e 7204  .d.....d.S.).Nr.
-00000480: 0000 0072 0700 0000 720b 0000 0072 0900  ...r....r....r..
-00000490: 0000 720a 0000 00da 0c69 6e74 726f 5f68  ..r......intro_h
-000004a0: 6172 626f 72da 0468 6f73 74da 0470 6f72  arbor..host..por
-000004b0: 7429 0372 1c00 0000 721d 0000 00da 0870  t).r....r......p
-000004c0: 726f 6365 6564 7329 04da 036c 656e 7202  roceeds)...lenr.
-000004d0: 0000 0072 0500 0000 7206 0000 0029 0372  ...r....r....).r
-000004e0: 1400 0000 da15 7468 655f 696e 7465 726e  ......the_intern
-000004f0: 616c 5f73 7461 7475 7365 73da 0f69 6e74  al_statuses..int
-00000500: 6572 6e61 6c5f 7374 6174 7573 7218 0000  ernal_statusr...
-00000510: 0072 1800 0000 7219 0000 00da 1573 656e  .r....r......sen
-00000520: 645f 646f 6e65 5f69 665f 6669 6e69 7368  d_done_if_finish
-00000530: 6564 3a00 0000 731c 0000 000c 0104 0102  ed:...s.........
-00000540: 0208 0308 0114 0d06 0102 ff02 0402 030a  ................
-00000550: 010a 0104 020a fc72 2200 0000 6300 0000  .......r"...c...
-00000560: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000570: 0003 0000 0073 3000 0000 7400 6401 1900  .....s0...t.d...
-00000580: 8900 0900 6406 8700 6601 6402 6403 8409  ....d...f.d.d...
-00000590: 7d00 7401 7c00 6404 8d01 7d01 7c01 6405  }.t.|.d...}.|.d.
-000005a0: 1900 8300 0100 6400 5300 2907 4eda 0764  ......d.S.).N..d
-000005b0: 6574 6169 6c73 6301 0000 0000 0000 0000  etailsc.........
-000005c0: 0000 0003 0000 0003 0000 0013 0000 0073  ...............s
-000005d0: 6c00 0000 7c00 a000 a100 7334 0900 7401  l...|.....s4..t.
-000005e0: 6401 1900 6402 6b03 720c 7100 7402 8300  d...d.k.r.q.t...
-000005f0: 5c02 7d01 7d02 8800 6403 6b05 721d 7403  \.}.}...d.k.r.t.
-00000600: 6a04 6404 7c01 6901 6405 8d01 0100 7403  j.d.|.i.d.....t.
-00000610: 6a04 6406 7c02 6901 6405 8d01 0100 7405  j.d.|.i.d.....t.
-00000620: 7c02 8301 0100 7406 a007 6407 a101 0100  |.....t...d.....
-00000630: 7c00 a000 a100 7204 6400 5300 6400 5300  |.....r.d.S.d.S.
-00000640: 2908 4eda 1769 6e74 6572 6e61 6c5f 7374  ).N..internal_st
-00000650: 6174 7573 6573 5f62 7569 6c74 da03 7965  atuses_built..ye
-00000660: 73e9 0200 0000 7a12 696e 7465 726e 616c  s.....z.internal
-00000670: 5f73 7461 7475 7365 733a 2901 da04 6461  _statuses:)...da
-00000680: 7461 7a0c 7761 6974 696e 6720 666f 723a  taz.waiting for:
-00000690: 7204 0000 0029 08da 0669 735f 7365 7472  r....)...is_setr
-000006a0: 0200 0000 721a 0000 00da 0472 6963 68da  ....r......rich.
-000006b0: 0a70 7269 6e74 5f6a 736f 6e72 2200 0000  .print_jsonr"...
-000006c0: da04 7469 6d65 da05 736c 6565 7029 03da  ..time..sleep)..
-000006d0: 0a73 746f 705f 6576 656e 7472 0700 0000  .stop_eventr....
-000006e0: 7214 0000 00a9 0172 2300 0000 7218 0000  r......r#...r...
-000006f0: 0072 1900 0000 da04 7461 736b 6100 0000  .r......taska...
-00000700: 7322 0000 0008 0302 010c 0302 010a 0208  s"..............
-00000710: 0204 0104 0202 ff06 ff04 0604 0202 ff06  ................
-00000720: ff08 060a 0210 e87a 2d70 7269 6e74 5f69  .......z-print_i
-00000730: 735f 646f 6e65 5f73 7461 7475 735f 7265  s_done_status_re
-00000740: 7065 7469 7665 6c79 2e3c 6c6f 6361 6c73  petively.<locals
-00000750: 3e2e 7461 736b 2901 722f 0000 00da 026f  >.task).r/.....o
-00000760: 6e29 014e 2902 7202 0000 0072 0300 0000  n).N).r....r....
-00000770: 2902 722f 0000 00da 0874 6865 5f74 6173  ).r/.....the_tas
-00000780: 6b72 1800 0000 722e 0000 0072 1900 0000  kr....r....r....
-00000790: da1f 7072 696e 745f 6973 5f64 6f6e 655f  ..print_is_done_
-000007a0: 7374 6174 7573 5f72 6570 6574 6976 656c  status_repetivel
-000007b0: 795e 0000 0073 0e00 0000 0801 0203 0eff  y^...s..........
-000007c0: 0220 0201 06ff 0e03 7232 0000 0029 0dda  . ......r2...)..
-000007d0: 075f 5f64 6f63 5f5f 722b 0000 0072 1000  .__doc__r+...r..
-000007e0: 0000 7229 0000 00da 3c66 6163 746f 7279  ..r)....<factory
-000007f0: 5f66 6172 6d2e 7072 6f63 6564 7572 6573  _farm.procedures
-00000800: 2e69 6d70 6c69 6369 745f 7072 6f63 6564  .implicit_proced
-00000810: 7572 652e 7072 6f63 6573 732e 7661 7269  ure.process.vari
-00000820: 6162 6c65 7372 0200 0000 da23 6661 6374  ablesr.....#fact
-00000830: 6f72 795f 6661 726d 2e74 6f70 6963 732e  ory_farm.topics.
-00000840: 696d 706c 6963 6974 2e74 6872 6561 6472  implicit.threadr
-00000850: 0300 0000 7205 0000 0072 0600 0000 721a  ....r....r....r.
-00000860: 0000 0072 2200 0000 7232 0000 0072 1800  ...r"...r2...r..
-00000870: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000880: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00000890: 1600 0000 0402 0804 0801 0802 0c01 0c01  ................
-000008a0: 0c02 0c01 0802 0829 0c24                 .......).$
+00000070: 6407 6c09 6d09 5a09 0100 6405 6408 6c0a  d.l.m.Z...d.d.l.
+00000080: 6d0a 5a0a 0100 6409 640a 8400 5a0b 640b  m.Z...d.d...Z.d.
+00000090: 640c 8400 5a0c 640d 640e 8400 5a0d 6402  d...Z.d.d...Z.d.
+000000a0: 5300 290f 7a23 0a09 7468 655f 7363 616e  S.).z#..the_scan
+000000b0: 205b 2270 726f 6365 7373 225d 2e69 735f   ["process"].is_
+000000c0: 616c 6976 6520 2829 0ae9 0000 0000 4e29  alive ()......N)
+000000d0: 01da 1c69 6d70 6c69 6369 745f 7072 6f63  ...implicit_proc
+000000e0: 6564 7572 655f 7661 7269 6162 6c65 7329  edure_variables)
+000000f0: 01da 0f69 6d70 6c69 6369 745f 7468 7265  ...implicit_thre
+00000100: 6164 e901 0000 0029 01da 0973 656e 645f  ad.....)...send_
+00000110: 646f 6e65 2901 da0f 6167 6772 6567 6174  done)...aggregat
+00000120: 655f 7374 6174 7329 01da 0c73 746f 705f  e_stats)...stop_
+00000130: 7072 6f63 6573 7363 0000 0000 0000 0000  processc........
+00000140: 0000 0000 0700 0000 0b00 0000 4300 0000  ............C...
+00000150: 7382 0100 0074 0064 0119 007d 0074 0064  s....t.d...}.t.d
+00000160: 0219 0064 0319 007d 0169 007d 0267 007d  ...d...}.i.}.g.}
+00000170: 037c 0044 005d 997d 0464 047d 0509 007a  .|.D.].}.d.}...z
+00000180: 287c 007c 0419 0064 0519 0064 0519 00a0  (|.|...d...d....
+00000190: 01a1 0064 066b 0272 3c74 02a0 02a1 0074  ...d.k.r<t.....t
+000001a0: 037c 007c 0419 0064 0719 0064 0819 0083  .|.|...d...d....
+000001b0: 0118 0074 037c 0183 016b 0572 3c74 047c  ...t.|...k.r<t.|
+000001c0: 0464 0964 0a69 0164 0b8d 0201 0057 006e  .d.d.i.d.....W.n
+000001d0: 1904 0074 0579 5601 007d 0601 007a 0d74  ...t.yV..}...z.t
+000001e0: 0664 0c74 07a0 08a1 0083 0201 0057 0059  .d.t.........W.Y
+000001f0: 0064 007d 067e 066e 0564 007d 067e 0677  .d.}.~.n.d.}.~.w
+00000200: 0177 007a 1a7c 007c 0419 0064 0519 0064  .w.z.|.|...d...d
+00000210: 0519 00a0 01a1 0064 0d6b 0272 7064 0e7d  .......d.k.rpd.}
+00000220: 0564 0e74 0064 0119 007c 0419 0064 0f19  .d.t.d...|...d..
+00000230: 0064 053c 0057 006e 2a04 0074 0579 8a01  .d.<.W.n*..t.y..
+00000240: 007d 0601 007a 0d74 0664 1074 07a0 08a1  .}...z.t.d.t....
+00000250: 0083 0201 0057 0059 0064 007d 067e 066e  .....W.Y.d.}.~.n
+00000260: 1664 007d 067e 0677 0104 0074 0579 9b01  .d.}.~.w...t.y..
+00000270: 007d 0601 007a 0657 0059 0064 007d 067e  .}...z.W.Y.d.}.~
+00000280: 066e 0564 007d 067e 0677 0177 007c 007c  .n.d.}.~.w.w.|.|
+00000290: 0419 0064 0f19 0064 1119 007c 0564 129c  ...d...d...|.d..
+000002a0: 027c 027c 043c 0071 1009 007c 0244 005d  .|.|.<.q...|.D.]
+000002b0: 0f7d 047c 027c 0419 0064 0519 0064 0e6b  .}.|.|...d...d.k
+000002c0: 0372 bc7c 03a0 097c 04a1 0101 0071 ad7c  .r.|...|.....q.|
+000002d0: 027c 0367 0253 0029 134e da11 696e 7465  .|.g.S.).N..inte
+000002e0: 726e 616c 5f73 7461 7475 7365 73da 0f69  rnal_statuses..i
+000002f0: 6e74 726f 5f76 6172 6961 626c 6573 da0a  ntro_variables..
+00000300: 7469 6d65 5f6c 696d 6974 da07 7065 6e64  time_limit..pend
+00000310: 696e 67da 0770 726f 6365 7373 54da 0574  ing..processT..t
+00000320: 696d 6573 da07 7374 6172 7465 64da 0561  imes..started..a
+00000330: 6c61 726d 7a13 7469 6d65 206c 696d 6974  larmz.time limit
+00000340: 2065 7863 6565 6465 6429 01da 0673 7461   exceeded)...sta
+00000350: 7475 737a 1b74 696d 6520 6c69 6d69 7420  tusz.time limit 
+00000360: 6368 6563 6b20 6578 6365 7074 696f 6e3a  check exception:
+00000370: 46da 0464 6f6e 6572 1000 0000 7a1a 7061  F..doner....z.pa
+00000380: 7273 6520 616e 6420 6368 6563 6b20 6578  rse and check ex
+00000390: 6365 7074 696f 6e3a da04 7363 616e 2902  ception:..scan).
+000003a0: 7212 0000 0072 0c00 0000 290a 7202 0000  r....r....).r...
+000003b0: 00da 0869 735f 616c 6976 65da 0474 696d  ...is_alive..tim
+000003c0: 65da 0566 6c6f 6174 7207 0000 00da 0945  e..floatr......E
+000003d0: 7863 6570 7469 6f6e da05 7072 696e 74da  xception..print.
+000003e0: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
+000003f0: 6174 5f65 7863 da06 6170 7065 6e64 2907  at_exc..append).
+00000400: 7208 0000 0072 0a00 0000 da08 7374 6174  r....r......stat
+00000410: 7573 6573 da0a 756e 6669 6e69 7368 6564  uses..unfinished
+00000420: da0b 7374 6174 7573 5f70 6174 68da 0e70  ..status_path..p
+00000430: 726f 6365 7373 5f73 7461 7475 73da 0145  rocess_status..E
+00000440: a900 7220 0000 00fa 772f 6661 6374 6f72  ..r ....w/factor
+00000450: 795f 6661 726d 2f76 656e 7565 732f 7374  y_farm/venues/st
+00000460: 6167 6573 2f66 6163 746f 7279 5f66 6172  ages/factory_far
+00000470: 6d2f 7072 6f63 6564 7572 6573 2f69 6d70  m/procedures/imp
+00000480: 6c69 6369 745f 7072 6f63 6564 7572 652f  licit_procedure/
+00000490: 7072 6f63 6573 732f 6d6f 7665 732f 7072  process/moves/pr
+000004a0: 696e 745f 6973 5f64 6f6e 655f 7374 6174  int_is_done_stat
+000004b0: 7573 5f72 6570 6574 6976 656c 792e 7079  us_repetively.py
+000004c0: da24 7061 7273 655f 616e 645f 6368 6563  .$parse_and_chec
+000004d0: 6b5f 6973 5f61 6c69 7665 5f6f 665f 7374  k_is_alive_of_st
+000004e0: 6174 7573 6573 1200 0000 7356 0000 0008  atuses....sV....
+000004f0: 010c 0104 0204 0108 0104 0102 0302 0318  ................
+00000500: 0124 0102 0102 0104 0202 ff06 fe04 800e  .$..............
+00000510: 060e 010c 0108 8002 fe02 0418 0204 0714  ................
+00000520: 0104 800e 020e 010c 0108 800e 060c 0108  ................
+00000530: 8002 ff0e 0502 010c fe02 0508 0510 010a  ................
+00000540: 0102 8008 0272 2200 0000 6301 0000 0000  .....r"...c.....
+00000550: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
+00000560: 0000 0073 6400 0000 7400 7c00 8301 6401  ...sd...t.|...d.
+00000570: 6b05 7208 6400 5300 0900 7401 6402 1900  k.r.d.S...t.d...
+00000580: 7d01 7c01 4400 5d0f 7d02 7c01 7c02 1900  }.|.D.].}.|.|...
+00000590: 6403 1900 6404 1900 6405 6b03 721e 0100  d...d...d.k.r...
+000005a0: 6400 5300 710f 0900 7402 7401 6406 1900  d.S.q...t.t.d...
+000005b0: 6407 1900 7401 6406 1900 6408 1900 7403  d...t.d...d...t.
+000005c0: 8300 6409 8d03 0100 6400 5300 290a 4e72  ..d.....d.S.).Nr
+000005d0: 0400 0000 7208 0000 0072 1000 0000 720c  ....r....r....r.
+000005e0: 0000 0072 1100 0000 da0c 696e 7472 6f5f  ...r......intro_
+000005f0: 6861 7262 6f72 da04 686f 7374 da04 706f  harbor..host..po
+00000600: 7274 2903 7224 0000 0072 2500 0000 da08  rt).r$...r%.....
+00000610: 7072 6f63 6565 6473 2904 da03 6c65 6e72  proceeds)...lenr
+00000620: 0200 0000 7205 0000 0072 0600 0000 2903  ....r....r....).
+00000630: 721c 0000 00da 1574 6865 5f69 6e74 6572  r......the_inter
+00000640: 6e61 6c5f 7374 6174 7573 6573 da0f 696e  nal_statuses..in
+00000650: 7465 726e 616c 5f73 7461 7475 7372 2000  ternal_statusr .
+00000660: 0000 7220 0000 0072 2100 0000 da15 7365  ..r ...r!.....se
+00000670: 6e64 5f64 6f6e 655f 6966 5f66 696e 6973  nd_done_if_finis
+00000680: 6865 6455 0000 0073 1c00 0000 0c01 0401  hedU...s........
+00000690: 0202 0803 0801 140d 0601 02ff 0204 0203  ................
+000006a0: 0a01 0a01 0402 0afc 722a 0000 0063 0000  ........r*...c..
+000006b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000006c0: 0000 0300 0000 7330 0000 0074 0064 0119  ......s0...t.d..
+000006d0: 0089 0009 0064 0687 0066 0164 0264 0384  .....d...f.d.d..
+000006e0: 097d 0074 017c 0064 048d 017d 017c 0164  .}.t.|.d...}.|.d
+000006f0: 0519 0083 0001 0064 0053 0029 074e da07  .......d.S.).N..
+00000700: 6465 7461 696c 7363 0100 0000 0000 0000  detailsc........
+00000710: 0000 0000 0300 0000 0300 0000 1300 0000  ................
+00000720: 736c 0000 007c 00a0 00a1 0073 3409 0074  sl...|.....s4..t
+00000730: 0164 0119 0064 026b 0372 0c71 0074 0283  .d...d.k.r.q.t..
+00000740: 005c 027d 017d 0288 0064 036b 0572 1d74  .\.}.}...d.k.r.t
+00000750: 036a 0464 047c 0169 0164 058d 0101 0074  .j.d.|.i.d.....t
+00000760: 036a 0464 067c 0269 0164 058d 0101 0074  .j.d.|.i.d.....t
+00000770: 057c 0283 0101 0074 06a0 0764 07a1 0101  .|.....t...d....
+00000780: 007c 00a0 00a1 0072 0464 0053 0064 0053  .|.....r.d.S.d.S
+00000790: 0029 084e da17 696e 7465 726e 616c 5f73  .).N..internal_s
+000007a0: 7461 7475 7365 735f 6275 696c 74da 0379  tatuses_built..y
+000007b0: 6573 e903 0000 007a 1269 6e74 6572 6e61  es.....z.interna
+000007c0: 6c5f 7374 6174 7573 6573 3a29 01da 0464  l_statuses:)...d
+000007d0: 6174 617a 0c77 6169 7469 6e67 2066 6f72  ataz.waiting for
+000007e0: 3a72 0400 0000 2908 da06 6973 5f73 6574  :r....)...is_set
+000007f0: 7202 0000 0072 2200 0000 da04 7269 6368  r....r".....rich
+00000800: da0a 7072 696e 745f 6a73 6f6e 722a 0000  ..print_jsonr*..
+00000810: 0072 1400 0000 da05 736c 6565 7029 03da  .r......sleep)..
+00000820: 0a73 746f 705f 6576 656e 7472 0800 0000  .stop_eventr....
+00000830: 721c 0000 00a9 0172 2b00 0000 7220 0000  r......r+...r ..
+00000840: 0072 2100 0000 da04 7461 736b 7c00 0000  .r!.....task|...
+00000850: 7322 0000 0008 0302 010c 0302 010a 0208  s"..............
+00000860: 0204 0104 0202 ff06 ff04 0604 0202 ff06  ................
+00000870: ff08 060a 0210 e87a 2d70 7269 6e74 5f69  .......z-print_i
+00000880: 735f 646f 6e65 5f73 7461 7475 735f 7265  s_done_status_re
+00000890: 7065 7469 7665 6c79 2e3c 6c6f 6361 6c73  petively.<locals
+000008a0: 3e2e 7461 736b 2901 7236 0000 00da 026f  >.task).r6.....o
+000008b0: 6e29 014e 2902 7202 0000 0072 0300 0000  n).N).r....r....
+000008c0: 2902 7236 0000 00da 0874 6865 5f74 6173  ).r6.....the_tas
+000008d0: 6b72 2000 0000 7235 0000 0072 2100 0000  kr ...r5...r!...
+000008e0: da1f 7072 696e 745f 6973 5f64 6f6e 655f  ..print_is_done_
+000008f0: 7374 6174 7573 5f72 6570 6574 6976 656c  status_repetivel
+00000900: 7979 0000 0073 0e00 0000 0801 0203 0eff  yy...s..........
+00000910: 0220 0201 06ff 0e03 7239 0000 0029 0eda  . ......r9...)..
+00000920: 075f 5f64 6f63 5f5f 7214 0000 0072 1800  .__doc__r....r..
+00000930: 0000 7231 0000 00da 3c66 6163 746f 7279  ..r1....<factory
+00000940: 5f66 6172 6d2e 7072 6f63 6564 7572 6573  _farm.procedures
+00000950: 2e69 6d70 6c69 6369 745f 7072 6f63 6564  .implicit_proced
+00000960: 7572 652e 7072 6f63 6573 732e 7661 7269  ure.process.vari
+00000970: 6162 6c65 7372 0200 0000 da23 6661 6374  ablesr.....#fact
+00000980: 6f72 795f 6661 726d 2e74 6f70 6963 732e  ory_farm.topics.
+00000990: 696d 706c 6963 6974 2e74 6872 6561 6472  implicit.threadr
+000009a0: 0300 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+000009b0: 0000 0072 2200 0000 722a 0000 0072 3900  ...r"...r*...r9.
+000009c0: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
+000009d0: 0072 2100 0000 da08 3c6d 6f64 756c 653e  .r!.....<module>
+000009e0: 0100 0000 7318 0000 0004 0208 0408 0108  ....s...........
+000009f0: 020c 010c 010c 020c 010c 0108 0208 430c  ..............C.
+00000a00: 24                                       $
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,16 +47,22 @@
 		** the_result
 	}
 	#implicit_procedure_variables ["paths_statuses"].append (status)
 	
 	
 	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["status"] ["scan"] = "done"
 	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["results_of_scan"] = status
-	
+
+	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"] = str (time.time ());
+
+	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["elapsed"] = (
+		float (implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["ended"]) - 
+		float (implicit_procedure_variables ["internal_statuses"] [ the_path ] ["times"] ["started"])
+	);
 	
 	#
 	#	Once the status of the scan has been established,
 	# 	then the scan process can be stopped.
 	#
 	implicit_procedure_variables ["internal_statuses"] [ the_path ] ["process"] ["process"].terminate ()
 	
-
+
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,39 +9,66 @@
 
 import rich
 from factory_farm.procedures.implicit_procedure.process.variables import implicit_procedure_variables
 from factory_farm.topics.implicit.thread import implicit_thread
 
 from .send_done import send_done
 from .aggregate_stats import aggregate_stats
+from .stop_process import stop_process
 
 def parse_and_check_is_alive_of_statuses ():
 	internal_statuses = implicit_procedure_variables ["internal_statuses"]
+	time_limit = implicit_procedure_variables ["intro_variables"] ["time_limit"]
 
 	statuses = {}
 	unfinished = []
 	for status_path in internal_statuses:
 		process_status = "pending"
+		
+		
+		'''
+			if over the time limit, stop the process
+		'''
 		try:
-			print ("checking process status:", internal_statuses [ status_path ])		
+			if (internal_statuses [ status_path ] ["process"] ["process"].is_alive () == True):
+				if (time.time () - float (internal_statuses [ status_path ] ["times"] ["started"]) >= float (time_limit)):
+					stop_process (
+						status_path,
+						status = {
+							"alarm": "time limit exceeded"
+						}
+					)
+		except Exception as E:
+			print ("time limit check exception:", traceback.format_exc ())
+			pass;
+		
+		try:
+			#print ("checking process status:", internal_statuses [ status_path ])		
 			if (internal_statuses [ status_path ] ["process"] ["process"].is_alive () == False):				
 				#
 				#	
 				#
 				#	check if the scan is done, if not the process exitted 
 				#	and 
 				#
 				process_status = "done"
 				implicit_procedure_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
 			print ("parse and check exception:", traceback.format_exc ())
+			pass;
+
+		
+				
+			
 		
+		except Exception as E:
 			pass;
-	
+			
+
 		statuses [ status_path ] = {
 			"scan": internal_statuses [ status_path ] ["status"] ["scan"],
 			"process": process_status
 		}
 	
 	'''
 		loop through again,
@@ -102,15 +129,15 @@
 				check if internal_statuses_built
 			'''
 			if (implicit_procedure_variables ["internal_statuses_built"] != "yes"):
 				continue;
 		
 			[ internal_statuses, unfinished ] = parse_and_check_is_alive_of_statuses ()
 			
-			if (details >= 2):
+			if (details >= 3):
 				rich.print_json (
 					data = {
 						"internal_statuses:": internal_statuses
 					}
 				)
 			
 			rich.print_json (
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 	"intro_variables": {},
 	
 	#
 	#	This is the list of statuses
 	#
 	#"paths_statuses": [],
 	
-	"details": 1,
+	"details": 2,
 	
 	#
 	#
 	#
 	"internal_statuses": {},
 	"internal_statuses_built": "no"
 }
@@ -62,14 +62,21 @@
 ):
 	for status_check_path in status_check_paths:		
 		implicit_procedure_variables ["internal_statuses"] [ format_path (status_check_path, relative_path) ] = {
 			"status": {
 				"scan": "pending",
 				"process": "pending"
 			},
+			
+			"times": {
+				"started": "",
+				"ended": "",
+				"elapsed": ""
+			},
+			
 			"process": None,
 			"results_of_scan": None
 		}
 			
 			
 	return;
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 	
 	relative_path = False,
 	module_paths = [],
 	
 	simultaneous = False,
 	simultaneous_capacity = 10,
 	
+	time_limit = "99999999999999999999999",
+	
 	before = False,
 	after = False
 ):
 	#regulators_on.on ()
 	#return;
 
 
@@ -145,14 +147,16 @@
 			"simultaneous_capacity": simultaneous_capacity,
 			
 			"before": before,
 			"after": after,
 			
 			"aggregation_format": aggregation_format,
 			
+			"time_limit": time_limit,
+			
 			"the_intro_harbor": {
 				"port": intro_port,
 				"host": "0.0.0.0"
 			}
 		}
 	)
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 02:23:09 2024 UTC, .py size: 6643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,198 +1,202 @@
-00000000: 6f0d 0d0a 0000 0000 0de1 1d66 f319 0000  o..........f....
+00000000: 6f0d 0d0a 0000 0000 1ff3 1d66 3f1a 0000  o..........f?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000d 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6402 6c08 5a08 6401 6402 6c09 5a09 6401  d.l.Z.d.d.l.Z.d.
 00000070: 6402 6c0a 5a0a 6401 6404 6c0b 6d0c 5a0c  d.l.Z.d.d.l.m.Z.
 00000080: 6d0d 5a0d 0100 6401 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
 00000090: 0100 6401 6406 6c10 6d11 5a11 0100 6401  ..d.d.l.m.Z...d.
 000000a0: 6407 6c12 6d13 5a13 0100 6401 6408 6c14  d.l.m.Z...d.d.l.
 000000b0: 6d15 5a15 0100 6401 6409 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
 000000c0: 0100 6401 6402 6c18 5a18 0900 640a 640b  ..d.d.l.Z...d.d.
 000000d0: 640c 640d 640e 640f 640e 640f 6700 640f  d.d.d.d.d.d.g.d.
-000000e0: 6410 640f 640f 660d 6411 6412 8401 5a19  d.d.d.f.d.d...Z.
-000000f0: 6402 5300 2913 6103 0100 000a 0969 6d70  d.S.).a......imp
-00000100: 6f72 7420 7061 7468 6c69 620a 0966 726f  ort pathlib..fro
-00000110: 6d20 6f73 2e70 6174 6820 696d 706f 7274  m os.path import
-00000120: 2064 6972 6e61 6d65 2c20 6a6f 696e 2c20   dirname, join, 
-00000130: 6e6f 726d 7061 7468 0a09 0a09 7468 6973  normpath....this
-00000140: 5f66 6f6c 6465 7220 3d20 7061 7468 6c69  _folder = pathli
-00000150: 622e 5061 7468 2028 5f5f 6669 6c65 5f5f  b.Path (__file__
-00000160: 292e 7061 7265 6e74 2e72 6573 6f6c 7665  ).parent.resolve
-00000170: 2028 290a 0973 6561 7263 6820 3d20 6e6f   ()..search = no
-00000180: 726d 7061 7468 2028 6a6f 696e 2028 7468  rmpath (join (th
-00000190: 6973 5f66 6f6c 6465 722c 2022 2e2e 2f2e  is_folder, "../.
-000001a0: 2e22 2929 0a0a 0969 6d70 6f72 7420 6661  ."))...import fa
-000001b0: 6374 6f72 795f 6661 726d 0a09 6661 6374  ctory_farm..fact
-000001c0: 6f72 795f 6661 726d 2e73 7461 7274 2028  ory_farm.start (
-000001d0: 0a09 0967 6c6f 625f 7374 7269 6e67 203d  ...glob_string =
-000001e0: 2073 6561 7263 6820 2b20 272f 2a2a 2f2a   search + '/**/*
-000001f0: 7374 6174 7573 2e70 7927 0a09 290a e900  status.py'..)...
-00000200: 0000 004e 2903 da07 6469 726e 616d 65da  ...N)...dirname.
-00000210: 046a 6f69 6eda 086e 6f72 6d70 6174 6829  .join..normpath)
-00000220: 02da 0654 696e 7944 42da 0551 7565 7279  ...TinyDB..Query
-00000230: 2901 da0f 7072 696e 746f 7574 5f70 6173  )...printout_pas
-00000240: 7365 7329 01da 1569 6d70 6c69 6369 745f  ses)...implicit_
-00000250: 7072 6f63 6564 7572 655f 6f6e 2901 da0b  procedure_on)...
-00000260: 6f70 656e 5f68 6172 626f 7229 01da 1e61  open_harbor)...a
-00000270: 7761 6974 5f69 6d70 6c69 6369 745f 7072  wait_implicit_pr
-00000280: 6f63 6564 7572 655f 6973 5f6f 6e29 01da  ocedure_is_on)..
-00000290: 0a73 656e 645f 7061 7468 73da 0069 d2cc  .send_paths..i..
-000002a0: 0000 69d3 cc00 0054 e901 0000 0046 e90a  ..i....T.....F..
-000002b0: 0000 0063 0d00 0000 0000 0000 0000 0000  ...c............
-000002c0: 1a00 0000 0d00 0000 0300 0000 73be 0100  ............s...
-000002d0: 0074 006a 007c 0064 0164 028d 027d 0d74  .t.j.|.d.d...}.t
-000002e0: 017c 0783 017d 077c 0464 036b 0572 1e74  .|...}.|.d.k.r.t
-000002f0: 0283 0001 0074 0264 0483 0101 0074 0264  .....t.d.....t.d
-00000300: 057c 0083 0201 0074 0283 0001 007c 0464  .|.....t.....|.d
-00000310: 036b 0572 3474 0283 0001 0074 0264 067c  .k.r4t.....t.d.|
-00000320: 0d83 0201 0074 0264 0774 037c 0d83 0183  .....t.d.t.|....
-00000330: 0201 0074 0283 0001 0074 04a0 05a1 0089  ...t.....t......
-00000340: 0169 0089 0087 0087 0166 0264 0864 0984  .i.......f.d.d..
-00000350: 087d 0e74 067c 017c 0e64 0a8d 025c 017d  .}.t.|.|.d...\.}
-00000360: 0f7c 0fa0 07a1 0001 0074 087c 0269 0064  .|.......t.|.i.d
-00000370: 0b8d 027d 1009 0074 097c 0264 0c8d 0101  ...}...t.|.d....
-00000380: 0074 0264 0d83 0101 0074 0a7c 027c 0d7c  .t.d.....t.|.|.|
-00000390: 077c 087c 097c 0a7c 0b7c 0c7c 067c 0164  .|.|.|.|.|.|.|.d
-000003a0: 0e64 0f9c 0264 109c 0964 0b8d 0201 0074  .d...d...d.....t
-000003b0: 0283 0001 0074 0264 1183 0101 0074 0283  .....t.d.....t..
-000003c0: 0001 0088 01a0 0ba1 0001 0074 0283 0001  ...........t....
-000003d0: 0074 0264 1283 0101 0074 0283 0001 007c  .t.d.....t.....|
-000003e0: 0fa0 0ca1 0001 0074 0264 1383 0101 0074  .......t.d.....t
-000003f0: 0264 147c 1083 0201 007c 1064 1519 00a0  .d.|.....|.d....
-00000400: 0da1 0001 0074 0264 147c 1083 0201 0074  .....t.d.|.....t
-00000410: 0e6a 0f64 1688 0069 0164 178d 0101 0074  .j.d...i.d.....t
-00000420: 107c 0583 0174 016b 0272 d274 116a 127c  .|...t.k.r.t.j.|
-00000430: 0564 0164 188d 0201 0074 1374 147c 0564  .d.d.....t.t.|.d
-00000440: 1983 0283 017d 1174 157c 1183 017d 127c  .....}.t.|...}.|
-00000450: 12a0 1688 0064 1a19 0088 0064 1b19 0088  .....d.....d....
-00000460: 0064 1c19 0064 1d9c 03a1 0101 007c 12a0  .d...d.......|..
-00000470: 17a1 0001 0088 0088 0064 1a19 0088 0064  .........d.....d
-00000480: 1b19 0088 0064 1c19 0064 1e9c 0453 0029  .....d...d...S.)
-00000490: 1f4e 5429 01da 0972 6563 7572 7369 7665  .NT)...recursive
-000004a0: e902 0000 007a 1a73 6561 7263 6869 6e67  .....z.searching
-000004b0: 2066 6f72 2067 6c6f 625f 7374 7269 6e67   for glob_string
-000004c0: 3afa 0109 7a07 0966 696e 6473 3a7a 0d09  :...z..finds:z..
-000004d0: 6669 6e64 7320 636f 756e 743a 6301 0000  finds count:c...
-000004e0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-000004f0: 0013 0000 0073 1000 0000 7c00 8900 8801  .....s....|.....
-00000500: a000 a100 0100 6400 5300 2901 4e29 01da  ......d.S.).N)..
-00000510: 0373 6574 2901 da0a 7468 655f 7061 636b  .set)...the_pack
-00000520: 6574 a902 da10 7468 655f 7363 616e 5f72  et....the_scan_r
-00000530: 6573 756c 7473 da1c 7761 6974 5f75 6e74  esults..wait_unt
-00000540: 696c 5f68 6561 6c74 685f 7363 616e 735f  il_health_scans_
-00000550: 646f 6e65 a900 fa45 2f66 6163 746f 7279  done...E/factory
-00000560: 5f66 6172 6d2f 7665 6e75 6573 2f73 7461  _farm/venues/sta
-00000570: 6765 732f 6661 6374 6f72 795f 6661 726d  ges/factory_farm
-00000580: 2f70 726f 6365 6475 7265 732f 696e 7472  /procedures/intr
-00000590: 6f2f 5f5f 696e 6974 5f5f 2e70 79da 1168  o/__init__.py..h
-000005a0: 6561 6c74 685f 7363 616e 735f 646f 6e65  ealth_scans_done
-000005b0: 6200 0000 7304 0000 0004 030c 057a 2073  b...s........z s
-000005c0: 7461 7274 2e3c 6c6f 6361 6c73 3e2e 6865  tart.<locals>.he
-000005d0: 616c 7468 5f73 6361 6e73 5f64 6f6e 6529  alth_scans_done)
-000005e0: 02da 0470 6f72 7472 1900 0000 2902 721a  ...portr....).r.
-000005f0: 0000 00da 0670 6163 6b65 7429 0172 1a00  .....packet).r..
-00000600: 0000 7a22 7468 6520 696d 706c 6963 6974  ..z"the implicit
-00000610: 2070 726f 6365 6475 7265 2068 6173 2073   procedure has s
-00000620: 7461 7274 6564 7a07 302e 302e 302e 3029  tartedz.0.0.0.0)
-00000630: 0272 1a00 0000 da04 686f 7374 2909 da12  .r......host)...
-00000640: 7374 6174 7573 5f63 6865 636b 5f70 6174  status_check_pat
-00000650: 6873 da0d 7265 6c61 7469 7665 5f70 6174  hs..relative_pat
-00000660: 68da 0c6d 6f64 756c 655f 7061 7468 73da  h..module_paths.
-00000670: 0c73 696d 756c 7461 6e65 6f75 73da 1573  .simultaneous..s
-00000680: 696d 756c 7461 6e65 6f75 735f 6361 7061  imultaneous_capa
-00000690: 6369 7479 da06 6265 666f 7265 da05 6166  city..before..af
-000006a0: 7465 72da 1261 6767 7265 6761 7469 6f6e  ter..aggregation
-000006b0: 5f66 6f72 6d61 74da 1074 6865 5f69 6e74  _format..the_int
-000006c0: 726f 5f68 6172 626f 727a 2d70 6174 6873  ro_harborz-paths
-000006d0: 2073 656e 742c 2077 6169 7469 6e67 2075   sent, waiting u
-000006e0: 6e74 696c 2074 6865 2073 6361 6e73 2061  ntil the scans a
-000006f0: 7265 2064 6f6e 652e 7a1a 646f 6e65 2061  re done.z.done a
-00000700: 7761 6974 696e 6720 6865 616c 7468 2073  waiting health s
-00000710: 6361 6e73 7a13 696e 7472 6f20 6861 7262  cansz.intro harb
-00000720: 6f72 2069 7320 6f66 667a 1774 6865 5f69  or is offz.the_i
-00000730: 6d70 6c69 6369 745f 7072 6f63 6564 7572  mplicit_procedur
-00000740: 653a da07 7072 6f63 6573 737a 1769 6e74  e:..processz.int
-00000750: 726f 3a20 7468 655f 7363 616e 5f72 6573  ro: the_scan_res
-00000760: 756c 7473 2901 da04 6461 7461 2901 da08  ults)...data)...
-00000770: 6578 6973 745f 6f6b 7a0c 7265 636f 7264  exist_okz.record
-00000780: 732e 6a73 6f6e da05 7061 7468 73da 0661  s.json..paths..a
-00000790: 6c61 726d 73da 0573 7461 7473 2903 7229  larms..stats).r)
-000007a0: 0000 0072 2a00 0000 722b 0000 0029 04da  ...r*...r+...)..
-000007b0: 0673 7461 7475 7372 2900 0000 722a 0000  .statusr)...r*..
-000007c0: 0072 2b00 0000 2920 da04 676c 6f62 da03  .r+...) ..glob..
-000007d0: 7374 72da 0570 7269 6e74 da03 6c65 6eda  str..print..len.
-000007e0: 0974 6872 6561 6469 6e67 da05 4576 656e  .threading..Even
-000007f0: 7472 0900 0000 da05 7374 6172 7472 0800  tr......startr..
-00000800: 0000 720a 0000 0072 0b00 0000 da04 7761  ..r....r......wa
-00000810: 6974 da04 7374 6f70 da09 7465 726d 696e  it..stop..termin
-00000820: 6174 65da 0472 6963 68da 0a70 7269 6e74  ate..rich..print
-00000830: 5f6a 736f 6eda 0474 7970 65da 026f 73da  _json..type..os.
-00000840: 086d 616b 6564 6972 7372 0400 0000 7203  .makedirsr....r.
-00000850: 0000 0072 0500 0000 da06 696e 7365 7274  ...r......insert
-00000860: da05 636c 6f73 65da 0b74 7572 6e5f 6f6e  ..close..turn_on
-00000870: 5f6f 6e65 da04 6a73 6f6e da05 6475 6d70  _one..json..dump
-00000880: 73da 1674 7572 6e5f 6f6e 5f73 696d 756c  s..turn_on_simul
-00000890: 7461 6e65 6f75 736c 79da 1474 7572 6e5f  taneously..turn_
-000008a0: 6f6e 5f73 6571 7565 6e74 6961 6c6c 79da  on_sequentially.
-000008b0: 0961 6767 7265 6761 7465 da0c 616c 6172  .aggregate..alar
-000008c0: 6d5f 7061 7273 6572 7207 0000 0029 1ada  m_parserr....)..
-000008d0: 0b67 6c6f 625f 7374 7269 6e67 da0a 696e  .glob_string..in
-000008e0: 7472 6f5f 706f 7274 da17 696d 706c 6963  tro_port..implic
-000008f0: 6974 5f70 726f 6365 6475 7265 5f70 6f72  it_procedure_por
-00000900: 74da 0c70 7269 6e74 5f61 6c61 726d 73da  t..print_alarms.
-00000910: 0772 6563 6f72 6473 da0c 6462 5f64 6972  .records..db_dir
-00000920: 6563 746f 7279 7224 0000 0072 1e00 0000  ectoryr$...r....
-00000930: 721f 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-00000940: 2200 0000 7223 0000 00da 0566 696e 6473  "...r#.....finds
-00000950: 7219 0000 00da 0c69 6e74 726f 5f68 6172  r......intro_har
-00000960: 626f 72da 1674 6865 5f69 6d70 6c69 6369  bor..the_implici
-00000970: 745f 7072 6f63 6564 7572 65da 0764 625f  t_procedure..db_
-00000980: 6669 6c65 da02 6462 da14 6265 666f 7265  file..db..before
-00000990: 5f70 6174 685f 7374 6174 7573 6573 da0d  _path_statuses..
-000009a0: 7061 7468 5f73 7461 7475 7365 73da 1361  path_statuses..a
-000009b0: 6674 6572 5f70 6174 685f 7374 6174 7573  fter_path_status
-000009c0: 6573 722c 0000 0072 2b00 0000 7229 0000  esr,...r+...r)..
-000009d0: 0072 2a00 0000 7217 0000 0072 1400 0000  .r*...r....r....
-000009e0: 7218 0000 0072 3300 0000 3100 0000 7396  r....r3...1...s.
-000009f0: 0000 000e 1d08 0108 0206 0108 010a 0106  ................
-00000a00: 0108 0206 010a 010e 0106 0108 0204 030e  ................
-00000a10: 0202 0e02 0102 0108 fe08 0402 0202 0102  ................
-00000a20: 0106 fe02 0802 0302 0106 ff08 0302 0402  ................
-00000a30: 0102 0202 0202 0102 0202 0102 0202 0102  ................
-00000a40: 0202 0302 0104 fe04 f206 fe06 1708 0106  ................
-00000a50: 0108 0206 0208 0106 0108 0208 010a 020c  ................
-00000a60: 020a 0204 0204 0202 ff06 ff0c 060e 010e  ................
-00000a70: 0108 0104 0206 0106 0106 0108 fd08 0602  ................
-00000a80: 0306 0206 0106 0106 fb72 3300 0000 291a  .........r3...).
-00000a90: da07 5f5f 646f 635f 5f72 2d00 0000 723f  ..__doc__r-...r?
-00000aa0: 0000 00da 0770 6174 686c 6962 da07 6f73  .....pathlib..os
-00000ab0: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
-00000ac0: 0400 0000 723a 0000 00da 0474 696d 6572  ....r:.....timer
-00000ad0: 3700 0000 da06 7469 6e79 6462 7205 0000  7.....tinydbr...
-00000ae0: 0072 0600 0000 da23 6661 6374 6f72 795f  .r.....#factory_
-00000af0: 6661 726d 2e74 6f70 6963 732e 7072 696e  farm.topics.prin
-00000b00: 746f 7574 2e70 6173 7365 7372 0700 0000  tout.passesr....
-00000b10: da2d 6661 6374 6f72 795f 6661 726d 2e70  .-factory_farm.p
-00000b20: 726f 6365 6475 7265 732e 696d 706c 6963  rocedures.implic
-00000b30: 6974 5f70 726f 6365 6475 7265 2e6f 6e72  it_procedure.onr
-00000b40: 0800 0000 da21 6661 6374 6f72 795f 6661  .....!factory_fa
-00000b50: 726d 2e70 726f 6365 6475 7265 732e 696e  rm.procedures.in
-00000b60: 7472 6f2e 6b65 6772 0900 0000 da38 6661  tro.kegr.....8fa
-00000b70: 6374 6f72 795f 6661 726d 2e70 726f 6365  ctory_farm.proce
-00000b80: 6475 7265 732e 696e 7472 6f2e 636f 6d73  dures.intro.coms
-00000b90: 2e69 6d70 6c69 6369 745f 7072 6f63 6564  .implicit_proced
-00000ba0: 7572 652e 6f6e 720a 0000 00da 4066 6163  ure.onr.....@fac
-00000bb0: 746f 7279 5f66 6172 6d2e 7072 6f63 6564  tory_farm.proced
-00000bc0: 7572 6573 2e69 6e74 726f 2e63 6f6d 732e  ures.intro.coms.
-00000bd0: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
-00000be0: 7265 2e73 656e 645f 7061 7468 7372 0b00  re.send_pathsr..
-00000bf0: 0000 7231 0000 0072 3300 0000 7217 0000  ..r1...r3...r...
-00000c00: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
-00000c10: da08 3c6d 6f64 756c 653e 0100 0000 733c  ..<module>....s<
-00000c20: 0000 0004 0108 0f08 0108 0114 0108 0108  ................
-00000c30: 0108 0210 010c 0a0c 040c 020c 010c 0108  ................
-00000c40: 0202 0102 0402 0502 0102 0202 0102 0102  ................
-00000c50: 0202 0202 0102 0202 0102 0202 010e ea    ...............
+000000e0: 6410 6411 640f 640f 660e 6412 6413 8401  d.d.d.d.f.d.d...
+000000f0: 5a19 6402 5300 2914 6103 0100 000a 0969  Z.d.S.).a......i
+00000100: 6d70 6f72 7420 7061 7468 6c69 620a 0966  mport pathlib..f
+00000110: 726f 6d20 6f73 2e70 6174 6820 696d 706f  rom os.path impo
+00000120: 7274 2064 6972 6e61 6d65 2c20 6a6f 696e  rt dirname, join
+00000130: 2c20 6e6f 726d 7061 7468 0a09 0a09 7468  , normpath....th
+00000140: 6973 5f66 6f6c 6465 7220 3d20 7061 7468  is_folder = path
+00000150: 6c69 622e 5061 7468 2028 5f5f 6669 6c65  lib.Path (__file
+00000160: 5f5f 292e 7061 7265 6e74 2e72 6573 6f6c  __).parent.resol
+00000170: 7665 2028 290a 0973 6561 7263 6820 3d20  ve ()..search = 
+00000180: 6e6f 726d 7061 7468 2028 6a6f 696e 2028  normpath (join (
+00000190: 7468 6973 5f66 6f6c 6465 722c 2022 2e2e  this_folder, "..
+000001a0: 2f2e 2e22 2929 0a0a 0969 6d70 6f72 7420  /.."))...import 
+000001b0: 6661 6374 6f72 795f 6661 726d 0a09 6661  factory_farm..fa
+000001c0: 6374 6f72 795f 6661 726d 2e73 7461 7274  ctory_farm.start
+000001d0: 2028 0a09 0967 6c6f 625f 7374 7269 6e67   (...glob_string
+000001e0: 203d 2073 6561 7263 6820 2b20 272f 2a2a   = search + '/**
+000001f0: 2f2a 7374 6174 7573 2e70 7927 0a09 290a  /*status.py'..).
+00000200: e900 0000 004e 2903 da07 6469 726e 616d  .....N)...dirnam
+00000210: 65da 046a 6f69 6eda 086e 6f72 6d70 6174  e..join..normpat
+00000220: 6829 02da 0654 696e 7944 42da 0551 7565  h)...TinyDB..Que
+00000230: 7279 2901 da0f 7072 696e 746f 7574 5f70  ry)...printout_p
+00000240: 6173 7365 7329 01da 1569 6d70 6c69 6369  asses)...implici
+00000250: 745f 7072 6f63 6564 7572 655f 6f6e 2901  t_procedure_on).
+00000260: da0b 6f70 656e 5f68 6172 626f 7229 01da  ..open_harbor)..
+00000270: 1e61 7761 6974 5f69 6d70 6c69 6369 745f  .await_implicit_
+00000280: 7072 6f63 6564 7572 655f 6973 5f6f 6e29  procedure_is_on)
+00000290: 01da 0a73 656e 645f 7061 7468 73da 0069  ...send_paths..i
+000002a0: d2cc 0000 69d3 cc00 0054 e901 0000 0046  ....i....T.....F
+000002b0: e90a 0000 00da 1739 3939 3939 3939 3939  .......999999999
+000002c0: 3939 3939 3939 3939 3939 3939 3939 630e  99999999999999c.
+000002d0: 0000 0000 0000 0000 0000 001b 0000 000e  ................
+000002e0: 0000 0003 0000 0073 c001 0000 7400 6a00  .......s....t.j.
+000002f0: 7c00 6401 6402 8d02 7d0e 7401 7c07 8301  |.d.d...}.t.|...
+00000300: 7d07 7c04 6403 6b05 721e 7402 8300 0100  }.|.d.k.r.t.....
+00000310: 7402 6404 8301 0100 7402 6405 7c00 8302  t.d.....t.d.|...
+00000320: 0100 7402 8300 0100 7c04 6403 6b05 7234  ..t.....|.d.k.r4
+00000330: 7402 8300 0100 7402 6406 7c0e 8302 0100  t.....t.d.|.....
+00000340: 7402 6407 7403 7c0e 8301 8302 0100 7402  t.d.t.|.......t.
+00000350: 8300 0100 7404 a005 a100 8901 6900 8900  ....t.......i...
+00000360: 8700 8701 6602 6408 6409 8408 7d0f 7406  ....f.d.d...}.t.
+00000370: 7c01 7c0f 640a 8d02 5c01 7d10 7c10 a007  |.|.d...\.}.|...
+00000380: a100 0100 7408 7c02 6900 640b 8d02 7d11  ....t.|.i.d...}.
+00000390: 0900 7409 7c02 640c 8d01 0100 7402 640d  ..t.|.d.....t.d.
+000003a0: 8301 0100 740a 7c02 7c0e 7c07 7c08 7c09  ....t.|.|.|.|.|.
+000003b0: 7c0a 7c0c 7c0d 7c06 7c0b 7c01 640e 640f  |.|.|.|.|.|.d.d.
+000003c0: 9c02 6410 9c0a 640b 8d02 0100 7402 8300  ..d...d.....t...
+000003d0: 0100 7402 6411 8301 0100 7402 8300 0100  ..t.d.....t.....
+000003e0: 8801 a00b a100 0100 7402 8300 0100 7402  ........t.....t.
+000003f0: 6412 8301 0100 7402 8300 0100 7c10 a00c  d.....t.....|...
+00000400: a100 0100 7402 6413 8301 0100 7402 6414  ....t.d.....t.d.
+00000410: 7c11 8302 0100 7c11 6415 1900 a00d a100  |.....|.d.......
+00000420: 0100 7402 6414 7c11 8302 0100 740e 6a0f  ..t.d.|.....t.j.
+00000430: 6416 8800 6901 6417 8d01 0100 7410 7c05  d...i.d.....t.|.
+00000440: 8301 7401 6b02 72d3 7411 6a12 7c05 6401  ..t.k.r.t.j.|.d.
+00000450: 6418 8d02 0100 7413 7414 7c05 6419 8302  d.....t.t.|.d...
+00000460: 8301 7d12 7415 7c12 8301 7d13 7c13 a016  ..}.t.|...}.|...
+00000470: 8800 641a 1900 8800 641b 1900 8800 641c  ..d.....d.....d.
+00000480: 1900 641d 9c03 a101 0100 7c13 a017 a100  ..d.......|.....
+00000490: 0100 8800 8800 641a 1900 8800 641b 1900  ......d.....d...
+000004a0: 8800 641c 1900 641e 9c04 5300 291f 4e54  ..d...d...S.).NT
+000004b0: 2901 da09 7265 6375 7273 6976 65e9 0200  )...recursive...
+000004c0: 0000 7a1a 7365 6172 6368 696e 6720 666f  ..z.searching fo
+000004d0: 7220 676c 6f62 5f73 7472 696e 673a fa01  r glob_string:..
+000004e0: 097a 0709 6669 6e64 733a 7a0d 0966 696e  .z..finds:z..fin
+000004f0: 6473 2063 6f75 6e74 3a63 0100 0000 0000  ds count:c......
+00000500: 0000 0000 0000 0100 0000 0200 0000 1300  ................
+00000510: 0000 7310 0000 007c 0089 0088 01a0 00a1  ..s....|........
+00000520: 0001 0064 0053 0029 014e 2901 da03 7365  ...d.S.).N)...se
+00000530: 7429 01da 0a74 6865 5f70 6163 6b65 74a9  t)...the_packet.
+00000540: 02da 1074 6865 5f73 6361 6e5f 7265 7375  ...the_scan_resu
+00000550: 6c74 73da 1c77 6169 745f 756e 7469 6c5f  lts..wait_until_
+00000560: 6865 616c 7468 5f73 6361 6e73 5f64 6f6e  health_scans_don
+00000570: 65a9 00fa 452f 6661 6374 6f72 795f 6661  e...E/factory_fa
+00000580: 726d 2f76 656e 7565 732f 7374 6167 6573  rm/venues/stages
+00000590: 2f66 6163 746f 7279 5f66 6172 6d2f 7072  /factory_farm/pr
+000005a0: 6f63 6564 7572 6573 2f69 6e74 726f 2f5f  ocedures/intro/_
+000005b0: 5f69 6e69 745f 5f2e 7079 da11 6865 616c  _init__.py..heal
+000005c0: 7468 5f73 6361 6e73 5f64 6f6e 6564 0000  th_scans_doned..
+000005d0: 0073 0400 0000 0403 0c05 7a20 7374 6172  .s........z star
+000005e0: 742e 3c6c 6f63 616c 733e 2e68 6561 6c74  t.<locals>.healt
+000005f0: 685f 7363 616e 735f 646f 6e65 2902 da04  h_scans_done)...
+00000600: 706f 7274 721a 0000 0029 0272 1b00 0000  portr....).r....
+00000610: da06 7061 636b 6574 2901 721b 0000 007a  ..packet).r....z
+00000620: 2274 6865 2069 6d70 6c69 6369 7420 7072  "the implicit pr
+00000630: 6f63 6564 7572 6520 6861 7320 7374 6172  ocedure has star
+00000640: 7465 647a 0730 2e30 2e30 2e30 2902 721b  tedz.0.0.0.0).r.
+00000650: 0000 00da 0468 6f73 7429 0ada 1273 7461  .....host)...sta
+00000660: 7475 735f 6368 6563 6b5f 7061 7468 73da  tus_check_paths.
+00000670: 0d72 656c 6174 6976 655f 7061 7468 da0c  .relative_path..
+00000680: 6d6f 6475 6c65 5f70 6174 6873 da0c 7369  module_paths..si
+00000690: 6d75 6c74 616e 656f 7573 da15 7369 6d75  multaneous..simu
+000006a0: 6c74 616e 656f 7573 5f63 6170 6163 6974  ltaneous_capacit
+000006b0: 79da 0662 6566 6f72 65da 0561 6674 6572  y..before..after
+000006c0: da12 6167 6772 6567 6174 696f 6e5f 666f  ..aggregation_fo
+000006d0: 726d 6174 da0a 7469 6d65 5f6c 696d 6974  rmat..time_limit
+000006e0: da10 7468 655f 696e 7472 6f5f 6861 7262  ..the_intro_harb
+000006f0: 6f72 7a2d 7061 7468 7320 7365 6e74 2c20  orz-paths sent, 
+00000700: 7761 6974 696e 6720 756e 7469 6c20 7468  waiting until th
+00000710: 6520 7363 616e 7320 6172 6520 646f 6e65  e scans are done
+00000720: 2e7a 1a64 6f6e 6520 6177 6169 7469 6e67  .z.done awaiting
+00000730: 2068 6561 6c74 6820 7363 616e 737a 1369   health scansz.i
+00000740: 6e74 726f 2068 6172 626f 7220 6973 206f  ntro harbor is o
+00000750: 6666 7a17 7468 655f 696d 706c 6963 6974  ffz.the_implicit
+00000760: 5f70 726f 6365 6475 7265 3ada 0770 726f  _procedure:..pro
+00000770: 6365 7373 7a17 696e 7472 6f3a 2074 6865  cessz.intro: the
+00000780: 5f73 6361 6e5f 7265 7375 6c74 7329 01da  _scan_results)..
+00000790: 0464 6174 6129 01da 0865 7869 7374 5f6f  .data)...exist_o
+000007a0: 6b7a 0c72 6563 6f72 6473 2e6a 736f 6eda  kz.records.json.
+000007b0: 0570 6174 6873 da06 616c 6172 6d73 da05  .paths..alarms..
+000007c0: 7374 6174 7329 0372 2b00 0000 722c 0000  stats).r+...r,..
+000007d0: 0072 2d00 0000 2904 da06 7374 6174 7573  .r-...)...status
+000007e0: 722b 0000 0072 2c00 0000 722d 0000 0029  r+...r,...r-...)
+000007f0: 20da 0467 6c6f 62da 0373 7472 da05 7072   ..glob..str..pr
+00000800: 696e 74da 036c 656e da09 7468 7265 6164  int..len..thread
+00000810: 696e 67da 0545 7665 6e74 7209 0000 00da  ing..Eventr.....
+00000820: 0573 7461 7274 7208 0000 0072 0a00 0000  .startr....r....
+00000830: 720b 0000 00da 0477 6169 74da 0473 746f  r......wait..sto
+00000840: 70da 0974 6572 6d69 6e61 7465 da04 7269  p..terminate..ri
+00000850: 6368 da0a 7072 696e 745f 6a73 6f6e da04  ch..print_json..
+00000860: 7479 7065 da02 6f73 da08 6d61 6b65 6469  type..os..makedi
+00000870: 7273 7204 0000 0072 0300 0000 7205 0000  rsr....r....r...
+00000880: 00da 0669 6e73 6572 74da 0563 6c6f 7365  ...insert..close
+00000890: da0b 7475 726e 5f6f 6e5f 6f6e 65da 046a  ..turn_on_one..j
+000008a0: 736f 6eda 0564 756d 7073 da16 7475 726e  son..dumps..turn
+000008b0: 5f6f 6e5f 7369 6d75 6c74 616e 656f 7573  _on_simultaneous
+000008c0: 6c79 da14 7475 726e 5f6f 6e5f 7365 7175  ly..turn_on_sequ
+000008d0: 656e 7469 616c 6c79 da09 6167 6772 6567  entially..aggreg
+000008e0: 6174 65da 0c61 6c61 726d 5f70 6172 7365  ate..alarm_parse
+000008f0: 7272 0700 0000 291b da0b 676c 6f62 5f73  rr....)...glob_s
+00000900: 7472 696e 67da 0a69 6e74 726f 5f70 6f72  tring..intro_por
+00000910: 74da 1769 6d70 6c69 6369 745f 7072 6f63  t..implicit_proc
+00000920: 6564 7572 655f 706f 7274 da0c 7072 696e  edure_port..prin
+00000930: 745f 616c 6172 6d73 da07 7265 636f 7264  t_alarms..record
+00000940: 73da 0c64 625f 6469 7265 6374 6f72 7972  s..db_directoryr
+00000950: 2500 0000 721f 0000 0072 2000 0000 7221  %...r....r ...r!
+00000960: 0000 0072 2200 0000 7226 0000 0072 2300  ...r"...r&...r#.
+00000970: 0000 7224 0000 00da 0566 696e 6473 721a  ..r$.....findsr.
+00000980: 0000 00da 0c69 6e74 726f 5f68 6172 626f  .....intro_harbo
+00000990: 72da 1674 6865 5f69 6d70 6c69 6369 745f  r..the_implicit_
+000009a0: 7072 6f63 6564 7572 65da 0764 625f 6669  procedure..db_fi
+000009b0: 6c65 da02 6462 da14 6265 666f 7265 5f70  le..db..before_p
+000009c0: 6174 685f 7374 6174 7573 6573 da0d 7061  ath_statuses..pa
+000009d0: 7468 5f73 7461 7475 7365 73da 1361 6674  th_statuses..aft
+000009e0: 6572 5f70 6174 685f 7374 6174 7573 6573  er_path_statuses
+000009f0: 722e 0000 0072 2d00 0000 722b 0000 0072  r....r-...r+...r
+00000a00: 2c00 0000 7218 0000 0072 1500 0000 7219  ,...r....r....r.
+00000a10: 0000 0072 3500 0000 3100 0000 7398 0000  ...r5...1...s...
+00000a20: 000e 1f08 0108 0206 0108 010a 0106 0108  ................
+00000a30: 0206 010a 010e 0106 0108 0204 030e 0202  ................
+00000a40: 0e02 0102 0108 fe08 0402 0202 0102 0106  ................
+00000a50: fe02 0802 0302 0106 ff08 0302 0402 0102  ................
+00000a60: 0202 0202 0102 0202 0102 0202 0102 0202  ................
+00000a70: 0202 0302 0104 fe04 f006 fe06 1908 0106  ................
+00000a80: 0108 0206 0208 0106 0108 0208 010a 020c  ................
+00000a90: 020a 0204 0204 0202 ff06 ff0c 060e 010e  ................
+00000aa0: 0108 0104 0206 0106 0106 0108 fd08 0602  ................
+00000ab0: 0306 0206 0106 0106 fb72 3500 0000 291a  .........r5...).
+00000ac0: da07 5f5f 646f 635f 5f72 2f00 0000 7241  ..__doc__r/...rA
+00000ad0: 0000 00da 0770 6174 686c 6962 da07 6f73  .....pathlib..os
+00000ae0: 2e70 6174 6872 0200 0000 7203 0000 0072  .pathr....r....r
+00000af0: 0400 0000 723c 0000 00da 0474 696d 6572  ....r<.....timer
+00000b00: 3900 0000 da06 7469 6e79 6462 7205 0000  9.....tinydbr...
+00000b10: 0072 0600 0000 da23 6661 6374 6f72 795f  .r.....#factory_
+00000b20: 6661 726d 2e74 6f70 6963 732e 7072 696e  farm.topics.prin
+00000b30: 746f 7574 2e70 6173 7365 7372 0700 0000  tout.passesr....
+00000b40: da2d 6661 6374 6f72 795f 6661 726d 2e70  .-factory_farm.p
+00000b50: 726f 6365 6475 7265 732e 696d 706c 6963  rocedures.implic
+00000b60: 6974 5f70 726f 6365 6475 7265 2e6f 6e72  it_procedure.onr
+00000b70: 0800 0000 da21 6661 6374 6f72 795f 6661  .....!factory_fa
+00000b80: 726d 2e70 726f 6365 6475 7265 732e 696e  rm.procedures.in
+00000b90: 7472 6f2e 6b65 6772 0900 0000 da38 6661  tro.kegr.....8fa
+00000ba0: 6374 6f72 795f 6661 726d 2e70 726f 6365  ctory_farm.proce
+00000bb0: 6475 7265 732e 696e 7472 6f2e 636f 6d73  dures.intro.coms
+00000bc0: 2e69 6d70 6c69 6369 745f 7072 6f63 6564  .implicit_proced
+00000bd0: 7572 652e 6f6e 720a 0000 00da 4066 6163  ure.onr.....@fac
+00000be0: 746f 7279 5f66 6172 6d2e 7072 6f63 6564  tory_farm.proced
+00000bf0: 7572 6573 2e69 6e74 726f 2e63 6f6d 732e  ures.intro.coms.
+00000c00: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
+00000c10: 7265 2e73 656e 645f 7061 7468 7372 0b00  re.send_pathsr..
+00000c20: 0000 7233 0000 0072 3500 0000 7218 0000  ..r3...r5...r...
+00000c30: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000c40: da08 3c6d 6f64 756c 653e 0100 0000 733e  ..<module>....s>
+00000c50: 0000 0004 0108 0f08 0108 0114 0108 0108  ................
+00000c60: 0108 0210 010c 0a0c 040c 020c 010c 0108  ................
+00000c70: 0202 0102 0402 0502 0102 0202 0102 0102  ................
+00000c80: 0202 0202 0102 0202 0102 0202 0202 010e  ................
+00000c90: e8                                       .
```

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/thread/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/printout/passes.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/venues/stages/factory_farm/topics/start--/simultaneously.py` & `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.1.3/PKG-INFO` & `factory_farm-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: factory_farm
-Version: 1.1.3
-Summary: Ensuring that your prod-uctions are absolutely stunning
+Version: 1.2.0
+Summary: The automated cybentic herb harvest factory of plantary towns yet to be established.
 License: GPL-3.0-only
 Keywords: neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

