# Comparing `tmp/factory_farm-1.2.1.tar.gz` & `tmp/factory_farm-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factory_farm-1.2.1.tar", max compression
+gzip compressed data, was "factory_farm-1.2.3.tar", max compression
```

## Comparing `factory_farm-1.2.1.tar` & `factory_farm-1.2.3.tar`

### file list

```diff
@@ -1,710 +1,710 @@
--rw-r--r--   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.2.1/license.S.HTML
--rw-r--r--   0        0        0     1232 2024-04-16 04:43:42.649723 factory_farm-1.2.1/pyproject.toml
--rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.2.1/readme.md
--rw-r--r--   0        0        0     2064 2024-04-16 03:42:28.111496 factory_farm-1.2.1/venue.S.HTML
--rw-r--r--   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.2.1/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
--rw-r--r--   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     4089 2024-04-16 04:46:19.540294 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.2.1/venues/stages/factory_farm/__bin/factory_farm_1
--rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.2.1/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/book.s.HTML
--rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__init__.py
--rw-r--r--   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/--statuspy.py
--rwxr-xr-x   0        0        0   642927 2024-04-16 04:44:11.921458 factory_farm-1.2.1/venues/stages/factory_farm/_status/DB/records.json
--rw-r--r--   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.2.1/venues/stages/factory_farm/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/status_1.py
--rw-r--r--   0        0        0      367 2024-04-16 03:23:58.043895 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1065 2024-04-16 03:36:15.519687 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
--rw-r--r--   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
--rw-r--r--   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
--rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    64017 2024-04-16 04:44:04.233528 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.2.1/venues/stages/factory_farm/_status/status.proc.py
--rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/architecture.s.HTML
--rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.2.1/venues/stages/factory_farm/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.2.1/venues/stages/factory_farm/license.S.HTML
--rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.2.1/venues/stages/factory_farm/module.s.HTML
--rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     1604 2024-04-16 04:42:23.266436 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      537 2024-04-16 04:35:00.446216 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      976 2024-04-16 04:43:10.970009 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      570 2024-04-16 04:32:47.783248 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
--rwxr-xr-x   0        0        0      834 2024-04-16 04:42:59.962108 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     2004 2024-04-16 04:42:27.398399 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
--rw-r--r--   0        0        0     1970 2024-04-16 04:42:32.314355 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
--rw-r--r--   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
--rw-r--r--   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
--rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
--rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
--rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2379 2024-04-16 03:23:57.115905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
--rw-r--r--   0        0        0     3030 2024-04-16 03:21:03.897796 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
--rw-r--r--   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1232 2024-04-16 03:23:57.111905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rw-r--r--   0        0        0     2551 2024-04-16 04:30:02.548430 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rw-r--r--   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rw-r--r--   0        0        0      860 2024-04-16 03:35:16.680347 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rw-r--r--   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rw-r--r--   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     1678 2024-04-16 03:23:14.884368 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
--rw-r--r--   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
--rw-r--r--   0        0        0     3802 2024-04-16 04:29:57.212466 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
--rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
--rw-r--r--   0        0        0     1077 2024-04-16 03:35:13.940378 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py
--rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
--rwxr-xr-x   0        0        0     1213 2024-04-16 03:20:38.414072 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-16 03:23:57.111905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     6719 2024-04-16 03:40:15.480990 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__init__.py
--rw-r--r--   0        0        0     3217 2024-04-16 03:40:58.048510 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
--rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__.py
--rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
--rw-r--r--   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
--rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/processes.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/exceptions.py
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/one.py
--rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.2.1/venues/stages/factory_farm/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.2.1/venues/stages/factory_farm/variables/__init__.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 factory_farm-1.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.2.3/license.S.HTML
+-rwxr-xr-x   0        0        0     1176 2024-04-16 05:11:54.717964 factory_farm-1.2.3/pyproject.toml
+-rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.2.3/readme.md
+-rwxr-xr-x   0        0        0     2166 2024-04-16 05:05:42.042487 factory_farm-1.2.3/venue.S.HTML
+-rwxr-xr-x   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.2.3/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rwxr-xr-x   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4089 2024-04-16 04:46:19.540294 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.2.3/venues/stages/factory_farm/__bin/factory_farm_1
+-rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.2.3/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.2.3/venues/stages/factory_farm/_clique/__init__.py
+-rwxr-xr-x   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.2.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.2.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.2.3/venues/stages/factory_farm/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.2.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.2.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/--statuspy.py
+-rwxr-xr-x   0        0        0   648856 2024-04-16 05:18:35.553453 factory_farm-1.2.3/venues/stages/factory_farm/_status/DB/records.json
+-rwxr-xr-x   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.2.3/venues/stages/factory_farm/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/status_1.py
+-rwxr-xr-x   0        0        0      367 2024-04-16 03:23:58.043895 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1065 2024-04-16 03:36:15.519687 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/status_1.py
+-rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
+-rwxr-xr-x   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/7/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
+-rwxr-xr-x   0        0        0    64621 2024-04-16 05:18:27.845537 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.2.3/venues/stages/factory_farm/_status/status.proc.py
+-rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/architecture.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.2.3/venues/stages/factory_farm/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.2.3/venues/stages/factory_farm/license.S.HTML
+-rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.2.3/venues/stages/factory_farm/module.s.HTML
+-rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.2.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
+-rwxr-xr-x   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.2.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     1604 2024-04-16 04:42:23.266436 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      537 2024-04-16 04:35:00.446216 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      976 2024-04-16 04:43:10.970009 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      570 2024-04-16 04:32:47.783248 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      834 2024-04-16 04:42:59.962108 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2004 2024-04-16 04:42:27.398399 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
+-rwxr-xr-x   0        0        0     1970 2024-04-16 04:42:32.314355 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
+-rwxr-xr-x   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
+-rwxr-xr-x   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
+-rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
+-rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
+-rwxr-xr-x   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
+-rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
+-rwxr-xr-x   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2379 2024-04-16 03:23:57.115905 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
+-rwxr-xr-x   0        0        0     3030 2024-04-16 03:21:03.897796 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
+-rwxr-xr-x   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1232 2024-04-16 03:23:57.111905 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rwxr-xr-x   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2551 2024-04-16 04:30:02.548430 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rwxr-xr-x   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rwxr-xr-x   0        0        0      860 2024-04-16 03:35:16.680347 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     1678 2024-04-16 03:23:14.884368 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
+-rwxr-xr-x   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
+-rwxr-xr-x   0        0        0     3802 2024-04-16 04:29:57.212466 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
+-rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
+-rwxr-xr-x   0        0        0     1077 2024-04-16 03:35:13.940378 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py
+-rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
+-rwxr-xr-x   0        0        0     1213 2024-04-16 03:20:38.414072 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
+-rwxr-xr-x   0        0        0     1070 2024-04-16 03:23:57.111905 factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     6719 2024-04-16 03:40:15.480990 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/__init__.py
+-rwxr-xr-x   0        0        0     3217 2024-04-16 03:40:58.048510 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
+-rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__init__.py
+-rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
+-rwxr-xr-x   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
+-rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.2.3/venues/stages/factory_farm/procedures/processes.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__init__.py
+-rwxr-xr-x   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/thread/__init__.py
+-rwxr-xr-x   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.2.3/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.2.3/venues/stages/factory_farm/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
+-rwxr-xr-x   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
+-rwxr-xr-x   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.2.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.2.3/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/one.py
+-rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.2.3/venues/stages/factory_farm/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.2.3/venues/stages/factory_farm/variables/__init__.py
+-rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 factory_farm-1.2.3/PKG-INFO
```

### Comparing `factory_farm-1.2.1/pyproject.toml` & `factory_farm-1.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "factory_farm"
-version = "1.2.1"
+version = "1.2.3"
 description = "The automated cybentic herb harvest factory of plantary towns yet to be established."
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "factory_farm", from = "venues/stages" }
 ]
@@ -47,30 +47,27 @@
 	"improvements"
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-body-scan = "^1.0.6"
+body-scan = "^1.1.1"
 botanist = "^1.0.0"
 shares = "^3.1.9"
 click = "^8.1.7"
 coverage = "^7.4.4"
 flask = "^3.0.3"
-pdoc3 = "^0.10.0"
 pexpect = "^4.9.0"
 redis = "^5.0.3"
 requests = "^2.31.0"
-textual = "^0.56.4"
 tinydb = "^4.8.0"
 rich = "^13.7.1"
 sanic = "^23.12.1"
 pymongo = "^4.6.3"
-quart = "^0.19.5"
 
 
 [tool.poetry.scripts]
 factory_farm = 'factory_farm:clique'
 
 [tool.poetry.urls]
 GitLab = "https://gitlab.com/status600/climates/factory_farm"
```

### Comparing `factory_farm-1.2.1/readme.md` & `factory_farm-1.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venue.S.HTML` & `factory_farm-1.2.3/venue.S.HTML`

 * *Files 12% similar despite different names*

```diff
@@ -65,15 +65,23 @@
 
 		
 		#
 		#	statuses
 		#
 		python3 /factory_farm/venues/stages/factory_farm/_status/status.proc.py
 		
-
+		#
+		#	git push
+		#
+		#		if Circle CI is successful, then publish
+		#
+		
+		#
+		#	increase version
+		#
 		
 		#
 		#	poetry auth
 		#
 		rm -rf dist && poetry build --verbose && poetry publish --verbose;
```

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg` & `factory_farm-1.2.3/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary.S.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/itinerary.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/maybes.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/start.py` & `factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py` & `factory_farm-1.2.3/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html` & `factory_farm-1.2.3/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_book/advanced tutorial.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_book/book.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_book/relevant.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/DB/records.json` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/DB/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948979591836735%*

 * *Differences: {"'_default'": "{'195': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/9_aggregation_format_and_exit/status_1.py'), ('empty', False), "*

 * *               "('parsed', True), ('stats', OrderedDict([('passes', 1), ('alarms', 0)])), "*

 * *               "('checks', [OrderedDict([('check', 'aggregation format and exit'), ('passed', "*

 * *               "True), ('elapsed', [2.1796795659975032, 'seconds'])])])]), OrderedDict([('path', "*

 * *               "'_status/monitors/0_start/status_1.py' […]*

```diff
@@ -18019,14 +18019,534 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 13
                 },
                 "empty": 0
             }
         },
+        "195": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1796795659975032,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1459854999993695,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.640277623999282,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.112669290996564,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1122786729974905,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1863319620024413,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1082125539978733,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.128897804002918,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1347548859994276,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.119803776004119,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.164931086001161,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                2.126519240999187,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/8_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                7.150048206000065,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
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
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
+        "196": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.11688845900062,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1115185790040414,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/0_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.100802544999169,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4.1_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1250695679991622,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/4_bad_import/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1078877140025725,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/-1_start/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.6678941400023177,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/5__file__/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                1.1149763409994193,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/3_empty_glob/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1815260330040473,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/6_various/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.0968910949959536,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/2/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1828852980033844,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/1/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.1069682189991,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/7/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "tinyDB database can be utilized",
+                            "elapsed": [
+                                2.167933463002555,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/8_DB/status_1.py",
+                    "stats": {
+                        "alarms": 0,
+                        "passes": 1
+                    }
+                },
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                7.138780248998955,
+                                "seconds"
+                            ],
+                            "passed": true
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/10_time_limits/status_1.py",
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
+                    "passes": 13
+                },
+                "empty": 0
+            }
+        },
         "2": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
```

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/establish.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/establish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/6_various/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/7/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9951219512195122%*

 * *Differences: {"'_default'": "{'204': OrderedDict([('paths', [OrderedDict([('path', 'guarantee_1.py'), ('empty', "*

 * *               "False), ('parsed', True), ('stats', OrderedDict([('passes', 1), ('alarms', 0)])), "*

 * *               "('checks', [OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[2.515000232961029e-06, 'seconds'])])])])]), ('alarms', []), ('stats', "*

 * *               "OrderedDict([('alarms', 0), ('empty', 0), ('checks', OrderedDict([('passes', 1), "*

 * *               "('alarms', 0 […]*

```diff
@@ -3740,14 +3740,78 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "204": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.515000232961029e-06,
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
+        "205": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                2.701999619603157e-06,
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

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status/status.proc.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json` & `factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/status.proc.py` & `factory_farm-1.2.3/venues/stages/factory_farm/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/architecture.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/module.s.HTML` & `factory_farm-1.2.3/venues/stages/factory_farm/module.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/on.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/on.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/passes.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/simultaneously.py` & `factory_farm-1.2.3/venues/stages/factory_farm/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.1/PKG-INFO` & `factory_farm-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: factory_farm
-Version: 1.2.1
+Version: 1.2.3
 Summary: The automated cybentic herb harvest factory of plantary towns yet to be established.
 License: GPL-3.0-only
 Keywords: neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: body-scan (>=1.0.6,<2.0.0)
+Requires-Dist: body-scan (>=1.1.1,<2.0.0)
 Requires-Dist: botanist (>=1.0.0,<2.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: coverage (>=7.4.4,<8.0.0)
 Requires-Dist: flask (>=3.0.3,<4.0.0)
-Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
 Requires-Dist: pexpect (>=4.9.0,<5.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
-Requires-Dist: quart (>=0.19.5,<0.20.0)
 Requires-Dist: redis (>=5.0.3,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sanic (>=23.12.1,<24.0.0)
 Requires-Dist: shares (>=3.1.9,<4.0.0)
-Requires-Dist: textual (>=0.56.4,<0.57.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Project-URL: GitLab, https://gitlab.com/status600/climates/factory_farm
 Description-Content-Type: text/markdown
 
 
 
 ## certificate
```

