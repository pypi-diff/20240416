# Comparing `tmp/factory_farm-1.2.0.tar.gz` & `tmp/factory_farm-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factory_farm-1.2.0.tar", max compression
+gzip compressed data, was "factory_farm-1.2.1.tar", max compression
```

## Comparing `factory_farm-1.2.0.tar` & `factory_farm-1.2.1.tar`

### file list

```diff
@@ -1,710 +1,710 @@
--rw-r--r--   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.2.0/license.S.HTML
--rw-r--r--   0        0        0     1232 2024-04-16 03:42:14.879645 factory_farm-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.2.0/readme.md
--rw-r--r--   0        0        0     2064 2024-04-16 03:42:28.111496 factory_farm-1.2.0/venue.S.HTML
--rw-r--r--   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.2.0/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
--rw-r--r--   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
--rwxr-xr-x   0        0        0     3866 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/maybes.s.HTML
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/script.py
--rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/start.py
--rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
--rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
--rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
--rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
--rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.2.0/venues/stages/factory_farm/__bin/factory_farm_1
--rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/__init__.py
--rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.2.0/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
--rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
--rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/book.s.HTML
--rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_book/relevant.s.HTML
--rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__init__.py
--rw-r--r--   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__init__.py
--rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/--statuspy.py
--rwxr-xr-x   0        0        0   623712 2024-04-16 03:41:36.588076 factory_farm-1.2.0/venues/stages/factory_farm/_status/DB/records.json
--rw-r--r--   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
--rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
--rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
--rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.2.0/venues/stages/factory_farm/_status/establish.py
--rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
--rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
--rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
--rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
--rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
--rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
--rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/status_1.py
--rw-r--r--   0        0        0      367 2024-04-16 03:23:58.043895 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0     1065 2024-04-16 03:36:15.519687 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py
--rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
--rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
--rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
--rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/status_1.py
--rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
--rw-r--r--   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
--rw-r--r--   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rw-r--r--   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
--rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
--rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
--rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
--rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
--rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
--rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
--rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
--rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
--rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
--rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
--rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
--rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/status_1.py
--rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
--rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
--rwxr-xr-x   0        0        0    63715 2024-04-16 03:41:28.864163 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
--rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
--rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
--rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
--rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
--rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.2.0/venues/stages/factory_farm/_status/status.proc.py
--rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status/status.s.HTML
--rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
--rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
--rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
--rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
--rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
--rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/status.proc.py
--rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/architecture.s.HTML
--rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.2.0/venues/stages/factory_farm/emojis.S.HTML
--rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.2.0/venues/stages/factory_farm/license.S.HTML
--rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.2.0/venues/stages/factory_farm/module.s.HTML
--rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
--rw-r--r--   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
--rw-r--r--   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
--rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/on.py
--rwxr-xr-x   0        0        0     1146 2024-04-16 02:40:51.696992 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
--rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      562 2024-04-16 02:39:38.309829 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      890 2024-04-16 02:41:24.580618 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      588 2024-04-16 02:39:33.821881 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
--rwxr-xr-x   0        0        0      877 2024-04-16 02:41:20.608663 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
--rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
--rwxr-xr-x   0        0        0     2005 2024-04-14 05:33:00.731251 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
--rwxr-xr-x   0        0        0     1956 2024-04-14 05:33:07.555211 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
--rw-r--r--   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
--rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
--rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
--rw-r--r--   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
--rw-r--r--   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
--rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
--rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
--rw-r--r--   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
--rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
--rw-r--r--   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0     2379 2024-04-16 03:23:57.115905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
--rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
--rw-r--r--   0        0        0     3030 2024-04-16 03:21:03.897796 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
--rw-r--r--   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
--rw-r--r--   0        0        0     1232 2024-04-16 03:23:57.111905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
--rw-r--r--   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
--rw-r--r--   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
--rw-r--r--   0        0        0     2561 2024-04-16 03:40:58.876501 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
--rw-r--r--   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
--rw-r--r--   0        0        0      860 2024-04-16 03:35:16.680347 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
--rw-r--r--   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
--rw-r--r--   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
--rwxr-xr-x   0        0        0     1678 2024-04-16 03:23:14.884368 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
--rw-r--r--   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
--rw-r--r--   0        0        0     3638 2024-04-16 03:41:47.775951 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
--rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
--rw-r--r--   0        0        0     1077 2024-04-16 03:35:13.940378 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py
--rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
--rwxr-xr-x   0        0        0     1213 2024-04-16 03:20:38.414072 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
--rw-r--r--   0        0        0     1070 2024-04-16 03:23:57.111905 factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     6719 2024-04-16 03:40:15.480990 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__init__.py
--rw-r--r--   0        0        0     3217 2024-04-16 03:40:58.048510 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
--rw-r--r--   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
--rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
--rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
--rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__.py
--rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
--rw-r--r--   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
--rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.2.0/venues/stages/factory_farm/procedures/processes.S.HTML
--rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
--rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
--rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__init__.py
--rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__init__.py
--rw-r--r--   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/exceptions.py
--rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/proc/__init__.py
--rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__init__.py
--rw-r--r--   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
--rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/passes.py
--rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
--rw-r--r--   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
--rw-r--r--   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
--rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
--rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
--rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
--rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
--rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
--rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
--rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
--rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
--rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/one.py
--rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/sequentially.py
--rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/simultaneously.py
--rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.2.0/venues/stages/factory_farm/topics/topics.S.HTML
--rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.2.0/venues/stages/factory_farm/variables/__init__.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 factory_farm-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      211 2024-04-16 02:07:59.993436 factory_farm-1.2.1/license.S.HTML
+-rw-r--r--   0        0        0     1232 2024-04-16 04:43:42.649723 factory_farm-1.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0     4123 2024-04-16 02:56:11.134508 factory_farm-1.2.1/readme.md
+-rw-r--r--   0        0        0     2064 2024-04-16 03:42:28.111496 factory_farm-1.2.1/venue.S.HTML
+-rw-r--r--   0        0        0   838272 2024-04-16 02:03:26.700967 factory_farm-1.2.1/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg
+-rw-r--r--   0        0        0      845 2024-04-15 23:43:38.033889 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML
+-rwxr-xr-x   0        0        0     4089 2024-04-16 04:46:19.540294 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0      650 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/maybes.s.HTML
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/script.py
+-rwxr-xr-x   0        0        0     1255 2024-01-22 23:00:47.026745 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/start.py
+-rwxr-xr-x   0        0        0      189 2023-12-17 00:23:56.149451 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v1/script.py
+-rwxr-xr-x   0        0        0      186 2023-11-01 19:11:23.429061 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v1/start.py
+-rwxr-xr-x   0        0        0      190 2023-12-17 00:38:53.626201 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/script.py
+-rwxr-xr-x   0        0        0     1141 2023-12-17 00:37:48.514945 factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py
+-rwxr-xr-x   0        0        0        0 2024-04-11 23:18:49.717845 factory_farm-1.2.1/venues/stages/factory_farm/__bin/factory_farm_1
+-rwxr-xr-x   0        0        0       83 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/__init__.py
+-rwxr-xr-x   0        0        0    37279 2023-12-01 20:51:04.310266 factory_farm-1.2.1/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html
+-rwxr-xr-x   0        0        0     1262 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/advanced tutorial.s.HTML
+-rwxr-xr-x   0        0        0     1816 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/book.s.HTML
+-rwxr-xr-x   0        0        0      552 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_book/relevant.s.HTML
+-rwxr-xr-x   0        0        0     2134 2024-04-16 02:23:09.401422 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__init__.py
+-rw-r--r--   0        0        0     2583 2024-04-16 02:30:29.460199 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4457 2024-01-23 03:33:39.774986 factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      294 2023-12-01 19:53:30.939388 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__init__.py
+-rwxr-xr-x   0        0        0      691 2024-02-01 03:47:07.815153 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1097 2023-12-01 19:54:39.623410 factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      496 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/--statuspy.py
+-rwxr-xr-x   0        0        0   642927 2024-04-16 04:44:11.921458 factory_farm-1.2.1/venues/stages/factory_farm/_status/DB/records.json
+-rw-r--r--   0        0        0     1173 2024-04-16 02:44:57.438195 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1589 2024-01-31 18:59:07.248364 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1116 2024-01-31 18:59:07.246364 factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1476 2024-04-16 02:44:53.078244 factory_farm-1.2.1/venues/stages/factory_farm/_status/establish.py
+-rwxr-xr-x   0        0        0      319 2024-04-13 23:09:38.416143 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       83 2023-11-16 16:37:37.841366 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      730 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py
+-rwxr-xr-x   0        0        0      316 2024-04-13 23:09:36.100167 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/__pycache__/monitor_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      101 2023-11-16 16:51:33.600010 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/chassis/modules/monitor_1.py
+-rwxr-xr-x   0        0        0      803 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/status_1.py
+-rwxr-xr-x   0        0        0      742 2023-09-27 00:02:37.766379 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      739 2023-09-26 23:58:31.261901 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      904 2023-09-26 23:55:59.156456 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc
+-rwxr-xr-x   0        0        0      560 2024-04-13 23:09:44.192080 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:44.772074 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      282 2023-10-28 18:23:15.708149 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/path_1_health.py
+-rwxr-xr-x   0        0        0      265 2023-10-28 18:23:15.722148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/path_2_health.py
+-rwxr-xr-x   0        0        0     1171 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/status_1.py
+-rw-r--r--   0        0        0      367 2024-04-16 03:23:58.043895 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0       96 2024-04-16 03:13:55.298349 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0     1065 2024-04-16 03:36:15.519687 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py
+-rwxr-xr-x   0        0        0      321 2023-10-28 18:23:15.735148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/1_health.py
+-rwxr-xr-x   0        0        0        2 2023-09-30 01:11:18.281117 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/2_health.py
+-rwxr-xr-x   0        0        0      623 2024-04-13 23:09:43.004093 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      157 2024-04-13 23:09:42.440099 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0       50 2023-09-30 00:56:59.786100 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/MODULE_1.py
+-rwxr-xr-x   0        0        0      287 2024-02-01 05:17:56.997590 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      391 2023-10-13 03:07:22.071513 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/modules/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1224 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/status_1.py
+-rwxr-xr-x   0        0        0      804 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py
+-rw-r--r--   0        0        0      289 2024-04-16 00:28:17.871373 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/1_health.py
+-rw-r--r--   0        0        0      517 2024-04-16 00:32:46.948536 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rw-r--r--   0        0        0      962 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py
+-rwxr-xr-x   0        0        0       35 2023-10-04 21:28:49.944107 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/1_health.py
+-rwxr-xr-x   0        0        0      206 2024-04-13 23:09:37.280155 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      959 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py
+-rwxr-xr-x   0        0        0      518 2023-12-11 19:46:37.800583 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py
+-rwxr-xr-x   0        0        0      155 2023-12-11 19:46:41.768550 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      377 2024-02-01 05:17:53.631613 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2023-12-11 19:46:44.334529 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0      774 2024-04-13 23:09:39.544130 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py
+-rwxr-xr-x   0        0        0      311 2023-10-28 18:23:15.757148 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/1_health.py
+-rwxr-xr-x   0        0        0       31 2023-10-13 04:03:32.440343 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/2_health.py
+-rwxr-xr-x   0        0        0        0 2023-10-13 04:03:42.970230 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/3_health.py
+-rwxr-xr-x   0        0        0      150 2023-10-13 03:39:00.591139 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/MODULE_1.py
+-rwxr-xr-x   0        0        0      547 2023-10-13 03:39:26.199864 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1032 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      179 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/2_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      165 2024-04-13 23:09:41.284112 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/3_health.cpython-310.pyc
+-rwxr-xr-x   0        0        0      910 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/status_1.py
+-rwxr-xr-x   0        0        0      462 2024-04-13 23:09:45.904062 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      160 2023-10-28 18:15:12.609882 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0      819 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/status_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-13 23:09:47.092049 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/stasis/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0       73 2023-10-28 19:16:57.530118 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/stasis/guarantee_1.py
+-rwxr-xr-x   0        0        0     1506 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py
+-rwxr-xr-x   0        0        0    64017 2024-04-16 04:44:04.233528 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      448 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      210 2024-04-13 23:09:30.844224 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/__pycache__/guarantee_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      119 2024-04-12 02:59:08.849320 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_1.py
+-rwxr-xr-x   0        0        0      124 2024-04-12 02:56:39.979062 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_2.py
+-rwxr-xr-x   0        0        0        7 2024-04-12 02:58:13.233973 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/guarantees/guarantee_3.py
+-rwxr-xr-x   0        0        0     1059 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py
+-rwxr-xr-x   0        0        0      949 2024-04-16 02:23:09.529420 factory_farm-1.2.1/venues/stages/factory_farm/_status/status.proc.py
+-rwxr-xr-x   0        0        0      276 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status/status.s.HTML
+-rwxr-xr-x   0        0        0     1518 2024-04-16 02:23:09.525420 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@1/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@2/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@3/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@4/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/1/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/2/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/3/5/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/1/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/2/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/3/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/4/guarantee_5.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_1.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_2.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_3.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_4.py
+-rwxr-xr-x   0        0        0       75 2023-11-01 00:24:46.272077 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/100@5/4/5/guarantee_5.py
+-rwxr-xr-x   0        0        0      406 2023-11-01 00:43:27.270306 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/after.py
+-rwxr-xr-x   0        0        0      358 2023-11-01 00:42:38.216865 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/stasis/before.py
+-rwxr-xr-x   0        0        0   542989 2023-12-11 20:11:58.306027 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json
+-rwxr-xr-x   0        0        0      919 2023-12-11 19:59:28.106227 factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/status.proc.py
+-rwxr-xr-x   0        0        0     1804 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/architecture.s.HTML
+-rwxr-xr-x   0        0        0       80 2024-04-03 21:49:21.484948 factory_farm-1.2.1/venues/stages/factory_farm/emojis.S.HTML
+-rwxr-xr-x   0        0        0      286 2024-04-16 02:11:08.570681 factory_farm-1.2.1/venues/stages/factory_farm/license.S.HTML
+-rwxr-xr-x   0        0        0     3133 2024-04-16 02:23:09.401422 factory_farm-1.2.1/venues/stages/factory_farm/module.s.HTML
+-rwxr-xr-x   0        0        0      864 2024-04-16 02:23:09.437421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py
+-rw-r--r--   0        0        0      976 2024-04-16 02:30:58.947854 factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      494 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/dynamic_port.cpython-310.pyc
+-rw-r--r--   0        0        0     1896 2024-04-16 02:44:58.274185 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      357 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/dynamic_port.py
+-rwxr-xr-x   0        0        0     2151 2024-04-16 02:44:36.946428 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/on.py
+-rwxr-xr-x   0        0        0     1604 2024-04-16 04:42:23.266436 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py
+-rwxr-xr-x   0        0        0      660 2024-04-14 03:23:08.431579 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      537 2024-04-16 04:35:00.446216 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      976 2024-04-16 04:43:10.970009 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      570 2024-04-16 04:32:47.783248 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py
+-rwxr-xr-x   0        0        0      834 2024-04-16 04:42:59.962108 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py
+-rwxr-xr-x   0        0        0     2957 2024-04-14 02:57:09.298904 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py
+-rwxr-xr-x   0        0        0     2004 2024-04-16 04:42:27.398399 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py
+-rw-r--r--   0        0        0     1970 2024-04-16 04:42:32.314355 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      779 2024-04-16 02:23:09.469421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py
+-rw-r--r--   0        0        0     1336 2024-04-15 21:13:32.676638 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      542 2024-04-14 03:40:33.432138 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc
+-rwxr-xr-x   0        0        0      321 2024-04-14 03:40:28.788170 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/format_rel_path.py
+-rwxr-xr-x   0        0        0      132 2024-04-14 00:31:50.138470 factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules_pip.UTF8
+-rw-r--r--   0        0        0     1491 2024-04-16 02:30:29.480199 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      626 2024-04-15 21:44:04.889606 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc
+-rw-r--r--   0        0        0       77 2024-04-16 00:57:52.151598 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/implicit_procedure.S.HTML
+-rwxr-xr-x   0        0        0     1462 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      359 2024-04-15 21:41:08.268047 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/paths.py
+-rwxr-xr-x   0        0        0      554 2024-04-14 01:25:11.648020 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py
+-rw-r--r--   0        0        0     1147 2024-04-15 21:44:21.713379 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      356 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/implicit_procedure.process.py
+-rwxr-xr-x   0        0        0      783 2024-04-16 00:52:47.863029 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py
+-rw-r--r--   0        0        0     1223 2024-04-16 00:52:52.470976 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-15 21:41:10.048022 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0      918 2024-04-16 02:30:30.324189 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0     2379 2024-04-16 03:23:57.115905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc
+-rwxr-xr-x   0        0        0      520 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py
+-rw-r--r--   0        0        0     3030 2024-04-16 03:21:03.897796 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py
+-rw-r--r--   0        0        0     1734 2024-04-16 02:30:30.372188 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc
+-rw-r--r--   0        0        0     1282 2024-04-15 20:31:31.342880 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc
+-rw-r--r--   0        0        0     1232 2024-04-16 03:23:57.111905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2024-04-15 23:17:17.483301 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/format_path.cpython-310.pyc
+-rw-r--r--   0        0        0      687 2024-04-15 22:21:10.822989 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc
+-rw-r--r--   0        0        0     2551 2024-04-16 04:30:02.548430 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc
+-rw-r--r--   0        0        0      630 2024-04-15 20:31:31.342880 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc
+-rw-r--r--   0        0        0      860 2024-04-16 03:35:16.680347 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc
+-rw-r--r--   0        0        0      933 2024-04-15 23:20:20.086332 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc
+-rw-r--r--   0        0        0     2952 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py
+-rwxr-xr-x   0        0        0     1678 2024-04-16 03:23:14.884368 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py
+-rw-r--r--   0        0        0      182 2024-04-15 23:17:12.503322 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/format_path.py
+-rw-r--r--   0        0        0     3802 2024-04-16 04:29:57.212466 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py
+-rwxr-xr-x   0        0        0      384 2024-04-15 20:28:52.255899 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/send_done.py
+-rw-r--r--   0        0        0     1077 2024-04-16 03:35:13.940378 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py
+-rwxr-xr-x   0        0        0     1220 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py
+-rwxr-xr-x   0        0        0     1213 2024-04-16 03:20:38.414072 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py
+-rw-r--r--   0        0        0     1070 2024-04-16 03:23:57.111905 factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     6719 2024-04-16 03:40:15.480990 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__init__.py
+-rw-r--r--   0        0        0     3217 2024-04-16 03:40:58.048510 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1214 2024-04-16 02:30:29.516198 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc
+-rw-r--r--   0        0        0      935 2024-04-16 02:30:29.552198 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0      877 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py
+-rwxr-xr-x   0        0        0      639 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py
+-rwxr-xr-x   0        0        0     1541 2024-04-15 20:59:54.302740 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__.py
+-rwxr-xr-x   0        0        0     1401 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py
+-rw-r--r--   0        0        0     2587 2024-04-15 20:59:57.206699 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1452 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py
+-rwxr-xr-x   0        0        0      177 2024-04-16 02:23:09.437421 factory_farm-1.2.1/venues/stages/factory_farm/procedures/processes.S.HTML
+-rwxr-xr-x   0        0        0      823 2023-10-13 03:17:38.378900 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rwxr-xr-x   0        0        0     3031 2023-10-13 03:23:45.508960 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc
+-rwxr-xr-x   0        0        0      672 2024-03-18 22:02:15.470350 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1061 2024-01-23 03:36:15.581237 factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1416 2024-04-12 03:08:18.350769 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__init__.py
+-rwxr-xr-x   0        0        0     1053 2024-04-12 03:08:20.674773 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2023-10-28 18:33:51.656601 factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      713 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__init__.py
+-rw-r--r--   0        0        0      688 2024-04-16 02:30:30.372188 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1069 2024-01-23 03:33:39.781986 factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      410 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/exceptions.py
+-rwxr-xr-x   0        0        0     1055 2024-04-15 19:06:08.332868 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-04-15 19:19:22.749400 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/proc/__init__.py
+-rwxr-xr-x   0        0        0     1159 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__init__.py
+-rw-r--r--   0        0        0      865 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      727 2024-04-11 23:00:04.881636 factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc
+-rwxr-xr-x   0        0        0      740 2024-04-11 22:59:33.037957 factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/passes.py
+-rwxr-xr-x   0        0        0     2261 2024-04-13 23:24:59.671341 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1884 2024-04-16 02:23:09.509420 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py
+-rw-r--r--   0        0        0     1857 2024-04-16 02:30:29.496199 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1386 2024-04-15 19:15:45.902514 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc
+-rw-r--r--   0        0        0     1503 2024-04-16 02:30:29.500198 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1471 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py
+-rwxr-xr-x   0        0        0       75 2024-04-13 23:45:41.546277 factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/process_on.S.HTML
+-rwxr-xr-x   0        0        0     1447 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py
+-rw-r--r--   0        0        0     1479 2024-04-16 02:30:30.376188 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      274 2024-04-12 02:01:33.840957 factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/unlimited_capacity/__init__.py
+-rwxr-xr-x   0        0        0      654 2023-11-01 00:26:26.461936 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc
+-rwxr-xr-x   0        0        0      454 2024-04-11 23:27:25.296367 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-310.pyc
+-rwxr-xr-x   0        0        0      666 2024-01-23 03:33:39.864985 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc
+-rwxr-xr-x   0        0        0      567 2024-04-11 23:26:30.968944 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc
+-rwxr-xr-x   0        0        0      851 2024-01-23 03:33:39.781986 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-13 17:40:31.649267 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-01-23 03:33:39.859985 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc
+-rwxr-xr-x   0        0        0      278 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/one.py
+-rwxr-xr-x   0        0        0      411 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/sequentially.py
+-rwxr-xr-x   0        0        0      542 2024-04-16 02:23:09.513420 factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/simultaneously.py
+-rwxr-xr-x   0        0        0       76 2024-04-11 22:22:22.425917 factory_farm-1.2.1/venues/stages/factory_farm/topics/topics.S.HTML
+-rwxr-xr-x   0        0        0        3 2024-04-14 01:59:42.225292 factory_farm-1.2.1/venues/stages/factory_farm/variables/__init__.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 factory_farm-1.2.1/PKG-INFO
```

### Comparing `factory_farm-1.2.0/pyproject.toml` & `factory_farm-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 
 
 
 [tool.poetry]
 name = "factory_farm"
-version = "1.2.0"
+version = "1.2.1"
 description = "The automated cybentic herb harvest factory of plantary towns yet to be established."
 authors = []
 readme = "readme.md"
 
 packages = [
     { include = "factory_farm", from = "venues/stages" }
 ]
```

### Comparing `factory_farm-1.2.0/readme.md` & `factory_farm-1.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venue.S.HTML` & `factory_farm-1.2.1/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg` & `factory_farm-1.2.1/venues/stages/factory_farm/BrightAgrotech--vertical-farm-916337_1920.jpg`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary - breaking.S.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/itinerary.S.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/itinerary.S.HTML`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,33 @@
 
 
 <pre>
 
 
 	<h1>agenda</h1>
 
+		<h2>urgent ranked</h2>
+			
+			[ ] if health scan doesn't send 
+				/done_with scan
+				
+					ask status?
+					
+					
+				[ ] there could have been an error
+					sending /done_with_scan
+					to the aggregator
+
+
+
 		<h2>ranked</h2>
 			
+	
+			
+			
 			[ ] before and after were lost
 			
 			[ ] health_scan dependency lock
 			
 			[ ] timeout in status_1.py
 			
 				timeout = 2
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/maybes.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/maybes.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout/start.py` & `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py` & `factory_farm-1.2.1/venues/stages/factory_farm/___itinerary/processes/errout_v2/start.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html` & `factory_farm-1.2.1/venues/stages/factory_farm/__license/options/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_book/advanced tutorial.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/_book/advanced tutorial.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_book/book.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/_book/book.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_book/relevant.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/_book/relevant.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_clique/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_clique/group/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/DB/records.json` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/DB/records.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561855670103092%*

 * *Differences: {"'_default'": "{'178': OrderedDict([('paths', [OrderedDict([('path', "*

 * *               "'_status/monitors/9_aggregation_format_and_exit/status_1.py'), ('empty', False), "*

 * *               "('parsed', True), ('stats', OrderedDict([('passes', 0), ('alarms', 1)])), "*

 * *               "('checks', [OrderedDict([('check', 'aggregation format and exit'), ('passed', "*

 * *               'False), (\'exception\', "OSError(98, \'Address already in use\')"), (\'exception '*

 * *               "trace', ['Traceback (most recent call  […]*

```diff
@@ -16621,14 +16621,120 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 13
                 },
                 "empty": 0
             }
         },
+        "178": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "179": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1706177859960007,
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
         "18": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
@@ -16829,14 +16935,502 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 10
                 },
                 "empty": 1
             }
         },
+        "180": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1493114230033825,
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
+        "181": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "182": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.134198164996633,
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
+        "183": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1195742870040704,
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
+        "184": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1250356860036845,
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
+        "185": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1160876319991075,
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
+        "186": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.142589229006262,
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
+        "187": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "188": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
+        "189": {
+            "alarms": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py"
+                }
+            ],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "exception": "OSError(98, 'Address already in use')",
+                            "exception trace": [
+                                "Traceback (most recent call last):",
+                                "  File \"/factory_farm/venues/stages_pip/body_scan/processes/scan/process/keg/check.py\", line 68, in start",
+                                "    checks [ check ] ()",
+                                "  File \"<string>\", line 16, in check_1",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/__init__.py\", line 118, in start",
+                                "    intro_harbor.start ()",
+                                "  File \"/factory_farm/venues/stages/factory_farm/procedures/intro/keg/__init__.py\", line 61, in start",
+                                "    self.httpd = HTTPServer ((self.host, self.port), RequestHandler)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 452, in __init__",
+                                "    self.server_bind()",
+                                "  File \"/usr/lib/python3.10/http/server.py\", line 137, in server_bind",
+                                "    socketserver.TCPServer.server_bind(self)",
+                                "  File \"/usr/lib/python3.10/socketserver.py\", line 466, in server_bind",
+                                "    self.socket.bind(self.server_address)",
+                                "OSError: [Errno 98] Address already in use"
+                            ],
+                            "passed": false
+                        }
+                    ],
+                    "empty": false,
+                    "parsed": true,
+                    "path": "_status/monitors/9_aggregation_format_and_exit/status_1.py",
+                    "stats": {
+                        "alarms": 1,
+                        "passes": 0
+                    }
+                }
+            ],
+            "stats": {
+                "alarms": 0,
+                "checks": {
+                    "alarms": 1,
+                    "passes": 0
+                },
+                "empty": 0
+            }
+        },
         "19": {
             "alarms": [],
             "paths": [
                 {
                     "empty": true,
                     "parsed": true,
                     "path": "_status/status_py.py"
@@ -17037,14 +17631,402 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 10
                 },
                 "empty": 1
             }
         },
+        "190": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.12739474800037,
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
+        "191": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.612783078002394,
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
+        "192": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.1157778829947347,
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
+        "193": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.133193873996788,
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
+        "194": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "aggregation format and exit",
+                            "elapsed": [
+                                2.0925768059969414,
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
+                                2.155547287002264,
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
+                                2.089465711003868,
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
+                                2.1557761630028835,
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
+                                2.1307354559976375,
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
+                                2.1354579410035512,
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
+                                1.1036140880023595,
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
+                                2.178881101994193,
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
+                                2.114288528006,
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
+                                2.1273263119946932,
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
+                                2.1023703640021267,
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
+                                2.164955877000466,
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
+                                7.123469168996962,
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

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/establish.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/__pycache__/status_py.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/establish.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/establish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/-1_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/0_start/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/0_start/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/CHECK_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_1_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/UT_2_HEALTH.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/stasis/__pycache__/path_1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/1/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/1/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/10_time_limits/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/2/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/2/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/3_empty_glob/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4.1_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/4_bad_import/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/1_health.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/5__file__/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/MODULES/__pycache__/MODULE_1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/stasis/__pycache__/1_health.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/6_various/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/6_various/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/7/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/7/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/8_DB/variable/status_db/records.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975369458128078%*

 * *Differences: {"'_default'": "{'203': OrderedDict([('paths', [OrderedDict([('path', 'guarantee_1.py'), ('empty', "*

 * *               "False), ('parsed', True), ('stats', OrderedDict([('passes', 1), ('alarms', 0)])), "*

 * *               "('checks', [OrderedDict([('check', 'check 1'), ('passed', True), ('elapsed', "*

 * *               "[3.278997610323131e-06, 'seconds'])])])])]), ('alarms', []), ('stats', "*

 * *               "OrderedDict([('alarms', 0), ('empty', 0), ('checks', OrderedDict([('passes', 1), "*

 * *               "('alarms', 0 […]*

```diff
@@ -3708,14 +3708,46 @@
                 "checks": {
                     "alarms": 0,
                     "passes": 1
                 },
                 "empty": 0
             }
         },
+        "203": {
+            "alarms": [],
+            "paths": [
+                {
+                    "checks": [
+                        {
+                            "check": "check 1",
+                            "elapsed": [
+                                3.278997610323131e-06,
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

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/monitors/9_aggregation_format_and_exit/status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status/status.proc.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/advanced_status_1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json` & `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/monitors/1/variable/status_db/records.json`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/_status_advanced/status.proc.py` & `factory_farm-1.2.1/venues/stages/factory_farm/_status_advanced/status.proc.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/architecture.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/architecture.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/module.s.HTML` & `factory_farm-1.2.1/venues/stages/factory_farm/module.s.HTML`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/data_nodes/tiny/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/on.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/health_scan.proc.py`

 * *Files 27% similar despite different names*

```diff
@@ -15,48 +15,60 @@
 from __import_from_path import import_from_path
 
 from __coms.done_with_scan import done_with_scan
 from __mixes.format_rel_path import format_rel_path
 
 import os
 import time
+from pprint import pprint
 
-#import rich
 
 import sys
 for path in sys.path:
 	print ("health scan, sys path:", path)
 
-'''
-rich.print_json (data = {
-	"health scan, sys paths": sys.path
-})
-'''
-
+import traceback
+import io
+def find_trace (exception : Exception) -> str:
+	try:
+		file = io.StringIO ()
+		traceback.print_exception (exception, file = file)
+		
+		return file.getvalue ().rstrip ().split ("\n")
+	except Exception:
+		pass;
+		
+	return 'An exception occurred while calculating trace.'
 
 def main ():
-	status_path = os.environ.get ("factory_farm___status_path")
-	status_relative_path = os.environ.get ("factory_farm___status_relative_path")
-
-	host = os.environ.get ("factory_farm___harbor_host")
-	port = int (os.environ.get ("factory_farm___harbor_port"))
-
-	proceeds = import_from_path (status_path)
-
-	'''
-	rich.print_json (data = {
-		"pid": os.getpid (),
-		"proceeds": proceeds,
-		"harbor": {
-			"host": host,
-			"port": port
+	#raise Exception ("An exception occurred")
+	try:
+		status_path = os.environ.get ("factory_farm___status_path")
+		status_relative_path = os.environ.get ("factory_farm___status_relative_path")
+
+		host = os.environ.get ("factory_farm___harbor_host")
+		port = int (os.environ.get ("factory_farm___harbor_port"))
+
+		proceeds = import_from_path (status_path)
+
+		pprint ({
+			"pid": os.getpid (),
+			"proceeds": proceeds,
+			"harbor": {
+				"host": host,
+				"port": port
+			}
+		})
+	except Exception as E:
+		proceeds = {
+			"parsed": False,
+			"alarm": "An exception occurred while running the scan.",
+			"exception": repr (E),
+			"exception trace": find_trace (E)
 		}
-	})
-	'''
-
 
 	done_with_scan (
 		host = host,
 		port = port,
 		
 		proceeds = {
 			"path": format_rel_path (status_path, status_relative_path),
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/__pycache__/send_patch.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 02:41:20 2024 UTC, .py size: 877 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
-00000000: 6f0d 0d0a 0000 0000 50e5 1d66 6d03 0000  o.......P..fm...
+00000000: 6f0d 0d0a 0000 0000 d301 1e66 4203 0000  o..........fB...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
+00000020: 0002 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a02 6403 6404 8400 5a03 6402 5300 2905  Z.d.d...Z.d.S.).
-00000050: 7a5a 0a09 6672 6f6d 202e 7365 6e64 5f70  zZ..from .send_p
-00000060: 6174 6368 2069 6d70 6f72 7420 7365 6e64  atch import send
-00000070: 5f70 6174 6368 0a09 7365 6e64 5f70 6174  _patch..send_pat
-00000080: 6368 2028 2230 2e30 2e30 2e30 222c 2070  ch ("0.0.0.0", p
-00000090: 6f72 742c 2022 2f64 6f6e 655f 7769 7468  ort, "/done_with
-000000a0: 5f73 6361 6e22 2c20 7b7d 290a e900 0000  _scan", {}).....
-000000b0: 004e 6304 0000 0000 0000 0000 0000 0009  .Nc.............
-000000c0: 0000 0009 0000 0043 0000 0073 a800 0000  .......C...s....
-000000d0: 7400 a001 7c03 a101 7d04 7402 a002 7402  t...|...}.t...t.
-000000e0: 6a03 7402 6a04 a102 8f36 7d05 7c05 a005  j.t.j....6}.|...
-000000f0: 7c00 7c01 6602 a101 0100 6401 7c02 9b00  |.|.f.....d.|...
-00000100: 6402 7c00 9b00 6403 7406 7c04 8301 9b00  d.|...d.t.|.....
-00000110: 6404 7c04 9b00 9d08 7d06 7c05 a007 7c06  d.|.....}.|...|.
-00000120: a008 a100 a101 0100 6405 7d07 0900 7c05  ........d.}...|.
-00000130: a009 6407 a101 7d08 7c08 7337 6e05 7c07  ..d...}.|.s7n.|.
-00000140: 7c08 3700 7d07 712f 5700 6400 0400 0400  |.7.}.q/W.d.....
-00000150: 8303 0100 6e08 3100 7346 7701 0100 0100  ....n.1.sFw.....
-00000160: 0100 5900 0100 740a 6408 7c07 a00b a100  ..Y...t.d.|.....
-00000170: 8302 0100 6400 5300 2909 4e7a 0650 4154  ....d.S.).Nz.PAT
-00000180: 4348 207a 1120 4854 5450 2f31 2e31 0d0a  CH z. HTTP/1.1..
-00000190: 486f 7374 3a20 7a32 0d0a 436f 6e74 656e  Host: z2..Conten
-000001a0: 742d 5479 7065 3a20 6170 706c 6963 6174  t-Type: applicat
-000001b0: 696f 6e2f 6a73 6f6e 0d0a 436f 6e74 656e  ion/json..Conten
-000001c0: 742d 4c65 6e67 7468 3a20 7a04 0d0a 0d0a  t-Length: z.....
-000001d0: f300 0000 0054 6900 0400 007a 0972 6573  .....Ti....z.res
-000001e0: 706f 6e73 653a 290c da04 6a73 6f6e da05  ponse:)...json..
-000001f0: 6475 6d70 73da 0673 6f63 6b65 74da 0741  dumps..socket..A
-00000200: 465f 494e 4554 da0b 534f 434b 5f53 5452  F_INET..SOCK_STR
-00000210: 4541 4dda 0763 6f6e 6e65 6374 da03 6c65  EAM..connect..le
-00000220: 6eda 0773 656e 6461 6c6c da06 656e 636f  n..sendall..enco
-00000230: 6465 da04 7265 6376 da05 7072 696e 74da  de..recv..print.
-00000240: 0664 6563 6f64 6529 09da 0468 6f73 74da  .decode)...host.
-00000250: 0470 6f72 74da 0470 6174 68da 096a 736f  .port..path..jso
-00000260: 6e5f 6461 7461 da08 6a73 6f6e 5f73 7472  n_data..json_str
-00000270: da01 73da 0772 6571 7565 7374 da08 7265  ..s..request..re
-00000280: 7370 6f6e 7365 da04 6461 7461 a900 7218  sponse..data..r.
-00000290: 0000 00fa 642f 6661 6374 6f72 795f 6661  ....d/factory_fa
-000002a0: 726d 2f76 656e 7565 732f 7374 6167 6573  rm/venues/stages
-000002b0: 2f66 6163 746f 7279 5f66 6172 6d2f 7072  /factory_farm/pr
-000002c0: 6f63 6564 7572 6573 2f68 6561 6c74 685f  ocedures/health_
-000002d0: 7363 616e 2f70 726f 6365 7373 2f6d 6f64  scan/process/mod
-000002e0: 756c 6573 2f5f 5f63 6f6d 732f 7365 6e64  ules/__coms/send
-000002f0: 5f70 6174 6368 2e70 79da 0a73 656e 645f  _patch.py..send_
-00000300: 7061 7463 6809 0000 0073 1e00 0000 0a02  patch....s......
-00000310: 1203 0e02 2003 0e01 0403 0201 0a01 0401  .... ...........
-00000320: 0201 0801 02fc 0203 1cf3 1211 721a 0000  ............r...
-00000330: 0029 04da 075f 5f64 6f63 5f5f 7205 0000  .)...__doc__r...
-00000340: 0072 0300 0000 721a 0000 0072 1800 0000  .r....r....r....
-00000350: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
-00000360: 083c 6d6f 6475 6c65 3e01 0000 0073 0800  .<module>....s..
-00000370: 0000 0401 0805 0801 0c01                 ..........
+00000040: 5a02 6401 6402 6c03 5a03 6403 6404 8400  Z.d.d.l.Z.d.d...
+00000050: 5a04 6402 5300 2905 7a5a 0a09 6672 6f6d  Z.d.S.).zZ..from
+00000060: 202e 7365 6e64 5f70 6174 6368 2069 6d70   .send_patch imp
+00000070: 6f72 7420 7365 6e64 5f70 6174 6368 0a09  ort send_patch..
+00000080: 7365 6e64 5f70 6174 6368 2028 2230 2e30  send_patch ("0.0
+00000090: 2e30 2e30 222c 2070 6f72 742c 2022 2f64  .0.0", port, "/d
+000000a0: 6f6e 655f 7769 7468 5f73 6361 6e22 2c20  one_with_scan", 
+000000b0: 7b7d 290a e900 0000 004e 6304 0000 0000  {})......Nc.....
+000000c0: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
+000000d0: 0000 0073 c400 0000 7400 8300 0100 7400  ...s....t.....t.
+000000e0: 6401 7401 a002 a100 7c03 8303 0100 7400  d.t.....|.....t.
+000000f0: 8300 0100 7403 a004 7c03 a101 7d04 7405  ....t...|...}.t.
+00000100: a005 7405 6a06 7405 6a07 a102 8f36 7d05  ..t.j.t.j....6}.
+00000110: 7c05 a008 7c00 7c01 6602 a101 0100 6402  |...|.|.f.....d.
+00000120: 7c02 9b00 6403 7c00 9b00 6404 7409 7c04  |...d.|...d.t.|.
+00000130: 8301 9b00 6405 7c04 9b00 9d08 7d06 7c05  ....d.|.....}.|.
+00000140: a00a 7c06 a00b a100 a101 0100 6406 7d07  ..|.........d.}.
+00000150: 0900 7c05 a00c 6408 a101 7d08 7c08 7345  ..|...d...}.|.sE
+00000160: 6e05 7c07 7c08 3700 7d07 713d 5700 6400  n.|.|.7.}.q=W.d.
+00000170: 0400 0400 8303 0100 6e08 3100 7354 7701  ........n.1.sTw.
+00000180: 0100 0100 0100 5900 0100 7400 6409 7c07  ......Y...t.d.|.
+00000190: a00d a100 8302 0100 6400 5300 290a 4e7a  ........d.S.).Nz
+000001a0: 1773 656e 6469 6e67 202f 646f 6e65 5f77  .sending /done_w
+000001b0: 6974 685f 7363 616e 7a06 5041 5443 4820  ith_scanz.PATCH 
+000001c0: 7a11 2048 5454 502f 312e 310d 0a48 6f73  z. HTTP/1.1..Hos
+000001d0: 743a 207a 320d 0a43 6f6e 7465 6e74 2d54  t: z2..Content-T
+000001e0: 7970 653a 2061 7070 6c69 6361 7469 6f6e  ype: application
+000001f0: 2f6a 736f 6e0d 0a43 6f6e 7465 6e74 2d4c  /json..Content-L
+00000200: 656e 6774 683a 207a 040d 0a0d 0af3 0000  ength: z........
+00000210: 0000 5469 0004 0000 7a09 7265 7370 6f6e  ..Ti....z.respon
+00000220: 7365 3a29 0eda 0570 7269 6e74 da02 6f73  se:)...print..os
+00000230: da06 6765 7470 6964 da04 6a73 6f6e da05  ..getpid..json..
+00000240: 6475 6d70 73da 0673 6f63 6b65 74da 0741  dumps..socket..A
+00000250: 465f 494e 4554 da0b 534f 434b 5f53 5452  F_INET..SOCK_STR
+00000260: 4541 4dda 0763 6f6e 6e65 6374 da03 6c65  EAM..connect..le
+00000270: 6eda 0773 656e 6461 6c6c da06 656e 636f  n..sendall..enco
+00000280: 6465 da04 7265 6376 da06 6465 636f 6465  de..recv..decode
+00000290: 2909 da04 686f 7374 da04 706f 7274 da04  )...host..port..
+000002a0: 7061 7468 da09 6a73 6f6e 5f64 6174 61da  path..json_data.
+000002b0: 086a 736f 6e5f 7374 72da 0173 da07 7265  .json_str..s..re
+000002c0: 7175 6573 74da 0872 6573 706f 6e73 65da  quest..response.
+000002d0: 0464 6174 61a9 0072 1a00 0000 fa64 2f66  .data..r.....d/f
+000002e0: 6163 746f 7279 5f66 6172 6d2f 7665 6e75  actory_farm/venu
+000002f0: 6573 2f73 7461 6765 732f 6661 6374 6f72  es/stages/factor
+00000300: 795f 6661 726d 2f70 726f 6365 6475 7265  y_farm/procedure
+00000310: 732f 6865 616c 7468 5f73 6361 6e2f 7072  s/health_scan/pr
+00000320: 6f63 6573 732f 6d6f 6475 6c65 732f 5f5f  ocess/modules/__
+00000330: 636f 6d73 2f73 656e 645f 7061 7463 682e  coms/send_patch.
+00000340: 7079 da0a 7365 6e64 5f70 6174 6368 0b00  py..send_patch..
+00000350: 0000 7324 0000 0006 0110 0106 010a 0312  ..s$............
+00000360: 030e 0120 030e 0104 0302 010a 0104 0102  ... ............
+00000370: 0108 0102 fc02 031c f412 1072 1c00 0000  ...........r....
+00000380: 2905 da07 5f5f 646f 635f 5f72 0800 0000  )...__doc__r....
+00000390: 7206 0000 0072 0400 0000 721c 0000 0072  r....r....r....r
+000003a0: 1a00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+000003b0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000003c0: 0073 0a00 0000 0401 0805 0801 0801 0c02  .s..............
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/done_with_scan.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 
 
 '''
 	from __coms.done_with_scan import done_with_scan
 	done_with_scan ()
 '''
 
-import requests
-
+from .send_patch import send_patch
 
 def done_with_scan (
 	host = "0.0.0.0",
 	URL_path = "/done_with_scan",
 	port = "",
 	
 	path = "",
 	proceeds = {}
 ):
-	from .send_patch import send_patch
 	send_patch ("0.0.0.0", port, "/done_with_scan", proceeds)
 
 	"""
 	URL = f"http://{ host }:{ port }{ URL_path }"
 	print (f'''
 	
 	done with scan:
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__coms/send_patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 '''
 	from .send_patch import send_patch
 	send_patch ("0.0.0.0", port, "/done_with_scan", {})
 '''
 
 import socket
 import json
+import os
+
 def send_patch (host, port, path, json_data):
-    # Convert JSON data to a string
-    json_str = json.dumps(json_data)
+	print ()
+	print ("sending /done_with_scan", os.getpid(), json_data)
+	print ()
+
+	# Convert JSON data to a string
+	json_str = json.dumps(json_data)
+
+	# Create a TCP/IP socket
+	with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+		s.connect ((host, port))
+		
+		# Send the HTTP request
+		request = f"PATCH {path} HTTP/1.1\r\nHost: {host}\r\nContent-Type: application/json\r\nContent-Length: {len(json_str)}\r\n\r\n{json_str}"
+		s.sendall (request.encode())
 
-    # Create a TCP/IP socket
-    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-        # Connect to the server
-        s.connect((host, port))
-        
-        # Send the HTTP request
-        request = f"PATCH {path} HTTP/1.1\r\nHost: {host}\r\nContent-Type: application/json\r\nContent-Length: {len(json_str)}\r\n\r\n{json_str}"
-        s.sendall(request.encode())
-
-        # Receive the response
-        response = b""
-        while True:
-            data = s.recv(1024)
-            if not data:
-                break
-            response += data
+		# Receive the response
+		response = b""
+		while True:
+			data = s.recv (1024)
+			if not data:
+				break
+			response += data
 
-    # Print the response
-    print ("response:", response.decode())
+	# Print the response
+	print ("response:", response.decode())
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__exec_from_path/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from pathlib import Path
 import sys
 import time
 from time import sleep
 from time import perf_counter
 import traceback
 
-
 def find_trace (exception : Exception) -> str:
 	try:
 		file = io.StringIO ()
 		traceback.print_exception (exception, file = file)
 		
 		return file.getvalue ().rstrip ().split ("\n")
 	except Exception:
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__import_from_path/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Apr 14 05:33:00 2024 UTC, .py size: 2005 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8c6a 1b66 d507 0000  o........j.f....
+00000000: 6f0d 0d0a 0000 0000 b301 1e66 d407 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6403 6c05 5a05 6401  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c06 5a06 6401 6404 6c07 6d08 5a08  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6403 6c09 5a09 6401 6403 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6401 6405 6c0a 6d0b 5a0b 0100 6401  Z.d.d.l.m.Z...d.
@@ -28,96 +28,97 @@
 000001b0: 7768 696c 6520 6361 6c63 756c 6174 696e  while calculatin
 000001c0: 6720 7472 6163 652e 2908 da02 696f da08  g trace.)...io..
 000001d0: 5374 7269 6e67 494f da09 7472 6163 6562  StringIO..traceb
 000001e0: 6163 6bda 0f70 7269 6e74 5f65 7863 6570  ack..print_excep
 000001f0: 7469 6f6e da08 6765 7476 616c 7565 da06  tion..getvalue..
 00000200: 7273 7472 6970 da05 7370 6c69 74da 0945  rstrip..split..E
 00000210: 7863 6570 7469 6f6e 2902 7206 0000 0072  xception).r....r
-00000220: 0800 0000 a900 7212 0000 00fa 602f 766f  ......r.....`/vo
-00000230: 6c74 732f 7665 6e75 6573 2f73 7461 6765  lts/venues/stage
-00000240: 732f 766f 6c74 732f 7072 6f63 6564 7572  s/volts/procedur
-00000250: 6573 2f68 6561 6c74 685f 7363 616e 2f70  es/health_scan/p
-00000260: 726f 6365 7373 2f6d 6f64 756c 6573 2f5f  rocess/modules/_
-00000270: 5f69 6d70 6f72 745f 6672 6f6d 5f70 6174  _import_from_pat
-00000280: 682f 5f5f 696e 6974 5f5f 2e70 79da 0a66  h/__init__.py..f
-00000290: 696e 645f 7472 6163 6513 0000 0073 1000  ind_trace....s..
-000002a0: 0000 0201 0801 0e01 1402 0c01 0201 0402  ................
-000002b0: 02fd 7214 0000 0063 0100 0000 0000 0000  ..r....c........
-000002c0: 0000 0000 0e00 0000 0b00 0000 4300 0000  ............C...
-000002d0: 7364 0100 0064 017d 017a 9067 007d 0264  sd...d.}.z.g.}.d
-000002e0: 0264 0264 039c 027d 0364 047d 0474 006a  .d.d...}.d.}.t.j
-000002f0: 01a0 027c 047c 00a1 027d 0574 006a 01a0  ...|.|...}.t.j..
-00000300: 037c 05a1 017d 067c 056a 04a0 057c 06a1  .|...}.|.j...|..
-00000310: 017d 0774 0664 057c 0783 0201 0074 0664  .}.t.d.|.....t.d
-00000320: 0674 077c 0664 0783 0283 0201 0074 077c  .t.|.d.......t.|
-00000330: 0664 0783 0272 8d7c 066a 087d 087c 0844  .d...r.|.j.}.|.D
-00000340: 005d 4e7d 097a 2474 0983 007d 0a7c 087c  .]N}.z$t...}.|.|
-00000350: 0919 0083 0001 0074 0983 007d 0b7c 0b7c  .......t...}.|.|
-00000360: 0a18 007d 0c7c 02a0 0a7c 0964 087c 0c64  ...}.|...|.d.|.d
-00000370: 0967 0264 0a9c 03a1 0101 007c 0364 0b05  .g.d.......|.d..
-00000380: 0019 0064 0c37 0003 003c 0057 0071 3604  ...d.7...<.W.q6.
-00000390: 0074 0b79 8401 007d 0d01 007a 1c7c 02a0  .t.y...}...z.|..
-000003a0: 0a7c 0964 0d74 0c7c 0d83 0174 0d7c 0d83  .|.d.t.|...t.|..
-000003b0: 0164 0e9c 04a1 0101 007c 0364 0f05 0019  .d.......|.d....
-000003c0: 0064 0c37 0003 003c 0057 0059 0064 007d  .d.7...<.W.Y.d.}
-000003d0: 0d7e 0d71 3664 007d 0d7e 0d77 0177 0064  .~.q6d.}.~.w.w.d
-000003e0: 0d64 087c 037c 0264 109c 0457 0053 0064  .d.|.|.d...W.S.d
-000003f0: 0864 0864 119c 0257 0053 0004 0074 0b79  .d.d...W.S...t.y
-00000400: a601 007d 0d01 007a 087c 0d7d 0157 0059  ...}...z.|.}.W.Y
-00000410: 0064 007d 0d7e 0d6e 0564 007d 0d7e 0d77  .d.}.~.n.d.}.~.w
-00000420: 0177 0064 0d64 1274 0c7c 0183 0174 0d7c  .w.d.d.t.|...t.|
-00000430: 0183 0164 139c 0453 0029 144e da00 7201  ...d...S.).N..r.
-00000440: 0000 0029 02da 0670 6173 7365 73da 0661  ...)...passes..a
-00000450: 6c61 726d 73da 085f 5f6d 6169 6e5f 5fda  larms..__main__.
-00000460: 0870 726f 6365 6564 737a 1063 6865 636b  .proceedsz.check
-00000470: 7320 696e 206d 6f64 756c 65da 0663 6865  s in module..che
-00000480: 636b 7354 da07 7365 636f 6e64 7329 03da  cksT..seconds)..
-00000490: 0563 6865 636b da06 7061 7373 6564 da07  .check..passed..
-000004a0: 656c 6170 7365 6472 1600 0000 e901 0000  elapsedr........
-000004b0: 0046 2904 721c 0000 0072 1d00 0000 7206  .F).r....r....r.
-000004c0: 0000 00fa 0f65 7863 6570 7469 6f6e 2074  .....exception t
-000004d0: 7261 6365 7217 0000 0029 04da 0565 6d70  racer....)...emp
-000004e0: 7479 da06 7061 7273 6564 da05 7374 6174  ty..parsed..stat
-000004f0: 7372 1a00 0000 2902 7221 0000 0072 2200  sr....).r!...r".
-00000500: 0000 7a2f 416e 2065 7863 6570 7469 6f6e  ..z/An exception
-00000510: 206f 6363 7572 7265 6420 7768 696c 6520   occurred while 
-00000520: 696d 706f 7274 696e 6720 7468 6520 7061  importing the pa
-00000530: 7468 2e29 0472 2200 0000 da05 616c 6172  th.).r".....alar
-00000540: 6d72 0600 0000 7220 0000 0029 0eda 0969  mr....r ...)...i
-00000550: 6d70 6f72 746c 6962 da04 7574 696c da17  mportlib..util..
-00000560: 7370 6563 5f66 726f 6d5f 6669 6c65 5f6c  spec_from_file_l
-00000570: 6f63 6174 696f 6eda 106d 6f64 756c 655f  ocation..module_
-00000580: 6672 6f6d 5f73 7065 63da 066c 6f61 6465  from_spec..loade
-00000590: 72da 0b65 7865 635f 6d6f 6475 6c65 da05  r..exec_module..
-000005a0: 7072 696e 74da 0768 6173 6174 7472 721a  print..hasattrr.
-000005b0: 0000 0072 0500 0000 da06 6170 7065 6e64  ...r......append
-000005c0: 7211 0000 00da 0472 6570 7272 1400 0000  r......reprr....
-000005d0: 290e da0b 6d6f 6475 6c65 5f70 6174 68da  )...module_path.
-000005e0: 0e70 6174 685f 6578 6365 7074 696f 6eda  .path_exception.
-000005f0: 0866 696e 6469 6e67 7372 2300 0000 da0b  .findingsr#.....
-00000600: 6d6f 6475 6c65 5f6e 616d 65da 0473 7065  module_name..spe
-00000610: 63da 0a74 6865 5f6d 6f64 756c 6572 1900  c..the_moduler..
-00000620: 0000 721a 0000 0072 1c00 0000 da0a 7469  ..r....r......ti
-00000630: 6d65 5f73 7461 7274 da08 7469 6d65 5f65  me_start..time_e
-00000640: 6e64 da0c 7469 6d65 5f65 6c61 7073 6564  nd..time_elapsed
-00000650: da01 4572 1200 0000 7212 0000 0072 1300  ..Er....r....r..
-00000660: 0000 da10 696d 706f 7274 5f66 726f 6d5f  ....import_from_
-00000670: 7061 7468 1e00 0000 736a 0000 0004 0102  path....sj......
-00000680: 0204 0102 0202 0106 fe04 050e 020c 010c  ................
-00000690: 010a 0210 010a 0106 0108 0202 0106 010a  ................
-000006a0: 0206 0208 0104 0202 0102 0106 0108 fd14  ................
-000006b0: 060e 0204 0102 0102 0106 0106 0108 fc1c  ................
-000006c0: 0708 8002 f802 0b02 0102 0202 0108 fb02  ................
-000006d0: 0a02 0108 fe0e 0510 0108 8002 ff02 0402  ................
-000006e0: 0106 0106 0106 fc72 3900 0000 2912 da07  .......r9...)...
-000006f0: 5f5f 646f 635f 5fda 0966 7261 6374 696f  __doc__..fractio
-00000700: 6e73 7202 0000 00da 0e69 6d70 6f72 746c  nsr......importl
-00000710: 6962 2e75 7469 6c72 2500 0000 720a 0000  ib.utilr%...r...
-00000720: 00da 046a 736f 6eda 0770 6174 686c 6962  ...json..pathlib
-00000730: 7203 0000 00da 0373 7973 da04 7469 6d65  r......sys..time
-00000740: 7204 0000 0072 0500 0000 720c 0000 0072  r....r....r....r
-00000750: 1100 0000 da03 7374 7272 1400 0000 7239  ......strr....r9
-00000760: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00000770: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000780: 3e01 0000 0073 1a00 0000 0401 0c05 0801  >....s..........
-00000790: 0801 0801 0c01 0801 0801 0c01 0c01 0801  ................
-000007a0: 1203 0c0b                                ....
+00000220: 0800 0000 a900 7212 0000 00fa 6e2f 6661  ......r.....n/fa
+00000230: 6374 6f72 795f 6661 726d 2f76 656e 7565  ctory_farm/venue
+00000240: 732f 7374 6167 6573 2f66 6163 746f 7279  s/stages/factory
+00000250: 5f66 6172 6d2f 7072 6f63 6564 7572 6573  _farm/procedures
+00000260: 2f68 6561 6c74 685f 7363 616e 2f70 726f  /health_scan/pro
+00000270: 6365 7373 2f6d 6f64 756c 6573 2f5f 5f69  cess/modules/__i
+00000280: 6d70 6f72 745f 6672 6f6d 5f70 6174 682f  mport_from_path/
+00000290: 5f5f 696e 6974 5f5f 2e70 79da 0a66 696e  __init__.py..fin
+000002a0: 645f 7472 6163 6512 0000 0073 1000 0000  d_trace....s....
+000002b0: 0201 0801 0e01 1402 0c01 0201 0402 02fd  ................
+000002c0: 7214 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000002d0: 0000 0e00 0000 0b00 0000 4300 0000 7364  ..........C...sd
+000002e0: 0100 0064 017d 017a 9067 007d 0264 0264  ...d.}.z.g.}.d.d
+000002f0: 0264 039c 027d 0364 047d 0474 006a 01a0  .d...}.d.}.t.j..
+00000300: 027c 047c 00a1 027d 0574 006a 01a0 037c  .|.|...}.t.j...|
+00000310: 05a1 017d 067c 056a 04a0 057c 06a1 017d  ...}.|.j...|...}
+00000320: 0774 0664 057c 0783 0201 0074 0664 0674  .t.d.|.....t.d.t
+00000330: 077c 0664 0783 0283 0201 0074 077c 0664  .|.d.......t.|.d
+00000340: 0783 0272 8d7c 066a 087d 087c 0844 005d  ...r.|.j.}.|.D.]
+00000350: 4e7d 097a 2474 0983 007d 0a7c 087c 0919  N}.z$t...}.|.|..
+00000360: 0083 0001 0074 0983 007d 0b7c 0b7c 0a18  .....t...}.|.|..
+00000370: 007d 0c7c 02a0 0a7c 0964 087c 0c64 0967  .}.|...|.d.|.d.g
+00000380: 0264 0a9c 03a1 0101 007c 0364 0b05 0019  .d.......|.d....
+00000390: 0064 0c37 0003 003c 0057 0071 3604 0074  .d.7...<.W.q6..t
+000003a0: 0b79 8401 007d 0d01 007a 1c7c 02a0 0a7c  .y...}...z.|...|
+000003b0: 0964 0d74 0c7c 0d83 0174 0d7c 0d83 0164  .d.t.|...t.|...d
+000003c0: 0e9c 04a1 0101 007c 0364 0f05 0019 0064  .......|.d.....d
+000003d0: 0c37 0003 003c 0057 0059 0064 007d 0d7e  .7...<.W.Y.d.}.~
+000003e0: 0d71 3664 007d 0d7e 0d77 0177 0064 0d64  .q6d.}.~.w.w.d.d
+000003f0: 087c 037c 0264 109c 0457 0053 0064 0864  .|.|.d...W.S.d.d
+00000400: 0864 119c 0257 0053 0004 0074 0b79 a601  .d...W.S...t.y..
+00000410: 007d 0d01 007a 087c 0d7d 0157 0059 0064  .}...z.|.}.W.Y.d
+00000420: 007d 0d7e 0d6e 0564 007d 0d7e 0d77 0177  .}.~.n.d.}.~.w.w
+00000430: 0064 0d64 1274 0c7c 0183 0174 0d7c 0183  .d.d.t.|...t.|..
+00000440: 0164 139c 0453 0029 144e da00 7201 0000  .d...S.).N..r...
+00000450: 0029 02da 0670 6173 7365 73da 0661 6c61  .)...passes..ala
+00000460: 726d 73da 085f 5f6d 6169 6e5f 5fda 0870  rms..__main__..p
+00000470: 726f 6365 6564 737a 1063 6865 636b 7320  roceedsz.checks 
+00000480: 696e 206d 6f64 756c 65da 0663 6865 636b  in module..check
+00000490: 7354 da07 7365 636f 6e64 7329 03da 0563  sT..seconds)...c
+000004a0: 6865 636b da06 7061 7373 6564 da07 656c  heck..passed..el
+000004b0: 6170 7365 6472 1600 0000 e901 0000 0046  apsedr.........F
+000004c0: 2904 721c 0000 0072 1d00 0000 7206 0000  ).r....r....r...
+000004d0: 00fa 0f65 7863 6570 7469 6f6e 2074 7261  ...exception tra
+000004e0: 6365 7217 0000 0029 04da 0565 6d70 7479  cer....)...empty
+000004f0: da06 7061 7273 6564 da05 7374 6174 7372  ..parsed..statsr
+00000500: 1a00 0000 2902 7221 0000 0072 2200 0000  ....).r!...r"...
+00000510: 7a2f 416e 2065 7863 6570 7469 6f6e 206f  z/An exception o
+00000520: 6363 7572 7265 6420 7768 696c 6520 696d  ccurred while im
+00000530: 706f 7274 696e 6720 7468 6520 7061 7468  porting the path
+00000540: 2e29 0472 2200 0000 da05 616c 6172 6d72  .).r".....alarmr
+00000550: 0600 0000 7220 0000 0029 0eda 0969 6d70  ....r ...)...imp
+00000560: 6f72 746c 6962 da04 7574 696c da17 7370  ortlib..util..sp
+00000570: 6563 5f66 726f 6d5f 6669 6c65 5f6c 6f63  ec_from_file_loc
+00000580: 6174 696f 6eda 106d 6f64 756c 655f 6672  ation..module_fr
+00000590: 6f6d 5f73 7065 63da 066c 6f61 6465 72da  om_spec..loader.
+000005a0: 0b65 7865 635f 6d6f 6475 6c65 da05 7072  .exec_module..pr
+000005b0: 696e 74da 0768 6173 6174 7472 721a 0000  int..hasattrr...
+000005c0: 0072 0500 0000 da06 6170 7065 6e64 7211  .r......appendr.
+000005d0: 0000 00da 0472 6570 7272 1400 0000 290e  .....reprr....).
+000005e0: da0b 6d6f 6475 6c65 5f70 6174 68da 0e70  ..module_path..p
+000005f0: 6174 685f 6578 6365 7074 696f 6eda 0866  ath_exception..f
+00000600: 696e 6469 6e67 7372 2300 0000 da0b 6d6f  indingsr#.....mo
+00000610: 6475 6c65 5f6e 616d 65da 0473 7065 63da  dule_name..spec.
+00000620: 0a74 6865 5f6d 6f64 756c 6572 1900 0000  .the_moduler....
+00000630: 721a 0000 0072 1c00 0000 da0a 7469 6d65  r....r......time
+00000640: 5f73 7461 7274 da08 7469 6d65 5f65 6e64  _start..time_end
+00000650: da0c 7469 6d65 5f65 6c61 7073 6564 da01  ..time_elapsed..
+00000660: 4572 1200 0000 7212 0000 0072 1300 0000  Er....r....r....
+00000670: da10 696d 706f 7274 5f66 726f 6d5f 7061  ..import_from_pa
+00000680: 7468 1d00 0000 736a 0000 0004 0102 0204  th....sj........
+00000690: 0102 0202 0106 fe04 050e 020c 010c 010a  ................
+000006a0: 0210 010a 0106 0108 0202 0106 010a 0206  ................
+000006b0: 0208 0104 0202 0102 0106 0108 fd14 060e  ................
+000006c0: 0204 0102 0102 0106 0106 0108 fc1c 0708  ................
+000006d0: 8002 f802 0b02 0102 0202 0108 fb02 0a02  ................
+000006e0: 0108 fe0e 0510 0108 8002 ff02 0402 0106  ................
+000006f0: 0106 0106 fc72 3900 0000 2912 da07 5f5f  .....r9...)...__
+00000700: 646f 635f 5fda 0966 7261 6374 696f 6e73  doc__..fractions
+00000710: 7202 0000 00da 0e69 6d70 6f72 746c 6962  r......importlib
+00000720: 2e75 7469 6c72 2500 0000 720a 0000 00da  .utilr%...r.....
+00000730: 046a 736f 6eda 0770 6174 686c 6962 7203  .json..pathlibr.
+00000740: 0000 00da 0373 7973 da04 7469 6d65 7204  .....sys..timer.
+00000750: 0000 0072 0500 0000 720c 0000 0072 1100  ...r....r....r..
+00000760: 0000 da03 7374 7272 1400 0000 7239 0000  ....strr....r9..
+00000770: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000780: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000790: 0000 0073 1a00 0000 0401 0c05 0801 0801  ...s............
+000007a0: 0801 0c01 0801 0801 0c01 0c01 0801 1202  ................
+000007b0: 0c0b                                     ..
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/health_scan/process/modules/__mixes/__pycache__/format_rel_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/__pycache__/paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/on.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/__pycache__/paths_patch.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/keg/spaces/paths_patch.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/aggregate_stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_path.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/done_with_scan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/is_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/print_is_done_status_repetively.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 16 03:40:54 2024 UTC, .py size: 3638 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,160 @@
-00000000: 6f0d 0d0a 0000 0000 46f3 1d66 360e 0000  o.......F..f6...
+00000000: 6f0d 0d0a 0000 0000 c5fe 1d66 da0e 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
+00000020: 0002 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6401 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c08 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c09 6d09 5a09 0100 6405 6408 6c0a  d.l.m.Z...d.d.l.
-00000080: 6d0a 5a0a 0100 6409 640a 8400 5a0b 640b  m.Z...d.d...Z.d.
-00000090: 640c 8400 5a0c 640d 640e 8400 5a0d 6402  d...Z.d.d...Z.d.
-000000a0: 5300 290f 7a23 0a09 7468 655f 7363 616e  S.).z#..the_scan
-000000b0: 205b 2270 726f 6365 7373 225d 2e69 735f   ["process"].is_
-000000c0: 616c 6976 6520 2829 0ae9 0000 0000 4e29  alive ()......N)
-000000d0: 01da 1c69 6d70 6c69 6369 745f 7072 6f63  ...implicit_proc
-000000e0: 6564 7572 655f 7661 7269 6162 6c65 7329  edure_variables)
-000000f0: 01da 0f69 6d70 6c69 6369 745f 7468 7265  ...implicit_thre
-00000100: 6164 e901 0000 0029 01da 0973 656e 645f  ad.....)...send_
-00000110: 646f 6e65 2901 da0f 6167 6772 6567 6174  done)...aggregat
-00000120: 655f 7374 6174 7329 01da 0c73 746f 705f  e_stats)...stop_
-00000130: 7072 6f63 6573 7363 0000 0000 0000 0000  processc........
-00000140: 0000 0000 0700 0000 0b00 0000 4300 0000  ............C...
-00000150: 7382 0100 0074 0064 0119 007d 0074 0064  s....t.d...}.t.d
-00000160: 0219 0064 0319 007d 0169 007d 0267 007d  ...d...}.i.}.g.}
-00000170: 037c 0044 005d 997d 0464 047d 0509 007a  .|.D.].}.d.}...z
-00000180: 287c 007c 0419 0064 0519 0064 0519 00a0  (|.|...d...d....
-00000190: 01a1 0064 066b 0272 3c74 02a0 02a1 0074  ...d.k.r<t.....t
-000001a0: 037c 007c 0419 0064 0719 0064 0819 0083  .|.|...d...d....
-000001b0: 0118 0074 037c 0183 016b 0572 3c74 047c  ...t.|...k.r<t.|
-000001c0: 0464 0964 0a69 0164 0b8d 0201 0057 006e  .d.d.i.d.....W.n
-000001d0: 1904 0074 0579 5601 007d 0601 007a 0d74  ...t.yV..}...z.t
-000001e0: 0664 0c74 07a0 08a1 0083 0201 0057 0059  .d.t.........W.Y
-000001f0: 0064 007d 067e 066e 0564 007d 067e 0677  .d.}.~.n.d.}.~.w
-00000200: 0177 007a 1a7c 007c 0419 0064 0519 0064  .w.z.|.|...d...d
-00000210: 0519 00a0 01a1 0064 0d6b 0272 7064 0e7d  .......d.k.rpd.}
-00000220: 0564 0e74 0064 0119 007c 0419 0064 0f19  .d.t.d...|...d..
-00000230: 0064 053c 0057 006e 2a04 0074 0579 8a01  .d.<.W.n*..t.y..
-00000240: 007d 0601 007a 0d74 0664 1074 07a0 08a1  .}...z.t.d.t....
-00000250: 0083 0201 0057 0059 0064 007d 067e 066e  .....W.Y.d.}.~.n
-00000260: 1664 007d 067e 0677 0104 0074 0579 9b01  .d.}.~.w...t.y..
-00000270: 007d 0601 007a 0657 0059 0064 007d 067e  .}...z.W.Y.d.}.~
-00000280: 066e 0564 007d 067e 0677 0177 007c 007c  .n.d.}.~.w.w.|.|
-00000290: 0419 0064 0f19 0064 1119 007c 0564 129c  ...d...d...|.d..
-000002a0: 027c 027c 043c 0071 1009 007c 0244 005d  .|.|.<.q...|.D.]
-000002b0: 0f7d 047c 027c 0419 0064 0519 0064 0e6b  .}.|.|...d...d.k
-000002c0: 0372 bc7c 03a0 097c 04a1 0101 0071 ad7c  .r.|...|.....q.|
-000002d0: 027c 0367 0253 0029 134e da11 696e 7465  .|.g.S.).N..inte
-000002e0: 726e 616c 5f73 7461 7475 7365 73da 0f69  rnal_statuses..i
-000002f0: 6e74 726f 5f76 6172 6961 626c 6573 da0a  ntro_variables..
-00000300: 7469 6d65 5f6c 696d 6974 da07 7065 6e64  time_limit..pend
-00000310: 696e 67da 0770 726f 6365 7373 54da 0574  ing..processT..t
-00000320: 696d 6573 da07 7374 6172 7465 64da 0561  imes..started..a
-00000330: 6c61 726d 7a13 7469 6d65 206c 696d 6974  larmz.time limit
-00000340: 2065 7863 6565 6465 6429 01da 0673 7461   exceeded)...sta
-00000350: 7475 737a 1b74 696d 6520 6c69 6d69 7420  tusz.time limit 
-00000360: 6368 6563 6b20 6578 6365 7074 696f 6e3a  check exception:
-00000370: 46da 0464 6f6e 6572 1000 0000 7a1a 7061  F..doner....z.pa
-00000380: 7273 6520 616e 6420 6368 6563 6b20 6578  rse and check ex
-00000390: 6365 7074 696f 6e3a da04 7363 616e 2902  ception:..scan).
-000003a0: 7212 0000 0072 0c00 0000 290a 7202 0000  r....r....).r...
-000003b0: 00da 0869 735f 616c 6976 65da 0474 696d  ...is_alive..tim
-000003c0: 65da 0566 6c6f 6174 7207 0000 00da 0945  e..floatr......E
-000003d0: 7863 6570 7469 6f6e da05 7072 696e 74da  xception..print.
-000003e0: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
-000003f0: 6174 5f65 7863 da06 6170 7065 6e64 2907  at_exc..append).
-00000400: 7208 0000 0072 0a00 0000 da08 7374 6174  r....r......stat
-00000410: 7573 6573 da0a 756e 6669 6e69 7368 6564  uses..unfinished
-00000420: da0b 7374 6174 7573 5f70 6174 68da 0e70  ..status_path..p
-00000430: 726f 6365 7373 5f73 7461 7475 73da 0145  rocess_status..E
-00000440: a900 7220 0000 00fa 772f 6661 6374 6f72  ..r ....w/factor
-00000450: 795f 6661 726d 2f76 656e 7565 732f 7374  y_farm/venues/st
-00000460: 6167 6573 2f66 6163 746f 7279 5f66 6172  ages/factory_far
-00000470: 6d2f 7072 6f63 6564 7572 6573 2f69 6d70  m/procedures/imp
-00000480: 6c69 6369 745f 7072 6f63 6564 7572 652f  licit_procedure/
-00000490: 7072 6f63 6573 732f 6d6f 7665 732f 7072  process/moves/pr
-000004a0: 696e 745f 6973 5f64 6f6e 655f 7374 6174  int_is_done_stat
-000004b0: 7573 5f72 6570 6574 6976 656c 792e 7079  us_repetively.py
-000004c0: da24 7061 7273 655f 616e 645f 6368 6563  .$parse_and_chec
-000004d0: 6b5f 6973 5f61 6c69 7665 5f6f 665f 7374  k_is_alive_of_st
-000004e0: 6174 7573 6573 1200 0000 7356 0000 0008  atuses....sV....
-000004f0: 010c 0104 0204 0108 0104 0102 0302 0318  ................
-00000500: 0124 0102 0102 0104 0202 ff06 fe04 800e  .$..............
-00000510: 060e 010c 0108 8002 fe02 0418 0204 0714  ................
-00000520: 0104 800e 020e 010c 0108 800e 060c 0108  ................
-00000530: 8002 ff0e 0502 010c fe02 0508 0510 010a  ................
-00000540: 0102 8008 0272 2200 0000 6301 0000 0000  .....r"...c.....
-00000550: 0000 0000 0000 0003 0000 0005 0000 0043  ...............C
-00000560: 0000 0073 6400 0000 7400 7c00 8301 6401  ...sd...t.|...d.
-00000570: 6b05 7208 6400 5300 0900 7401 6402 1900  k.r.d.S...t.d...
-00000580: 7d01 7c01 4400 5d0f 7d02 7c01 7c02 1900  }.|.D.].}.|.|...
-00000590: 6403 1900 6404 1900 6405 6b03 721e 0100  d...d...d.k.r...
-000005a0: 6400 5300 710f 0900 7402 7401 6406 1900  d.S.q...t.t.d...
-000005b0: 6407 1900 7401 6406 1900 6408 1900 7403  d...t.d...d...t.
-000005c0: 8300 6409 8d03 0100 6400 5300 290a 4e72  ..d.....d.S.).Nr
-000005d0: 0400 0000 7208 0000 0072 1000 0000 720c  ....r....r....r.
-000005e0: 0000 0072 1100 0000 da0c 696e 7472 6f5f  ...r......intro_
-000005f0: 6861 7262 6f72 da04 686f 7374 da04 706f  harbor..host..po
-00000600: 7274 2903 7224 0000 0072 2500 0000 da08  rt).r$...r%.....
-00000610: 7072 6f63 6565 6473 2904 da03 6c65 6e72  proceeds)...lenr
-00000620: 0200 0000 7205 0000 0072 0600 0000 2903  ....r....r....).
-00000630: 721c 0000 00da 1574 6865 5f69 6e74 6572  r......the_inter
-00000640: 6e61 6c5f 7374 6174 7573 6573 da0f 696e  nal_statuses..in
-00000650: 7465 726e 616c 5f73 7461 7475 7372 2000  ternal_statusr .
-00000660: 0000 7220 0000 0072 2100 0000 da15 7365  ..r ...r!.....se
-00000670: 6e64 5f64 6f6e 655f 6966 5f66 696e 6973  nd_done_if_finis
-00000680: 6865 6455 0000 0073 1c00 0000 0c01 0401  hedU...s........
-00000690: 0202 0803 0801 140d 0601 02ff 0204 0203  ................
-000006a0: 0a01 0a01 0402 0afc 722a 0000 0063 0000  ........r*...c..
-000006b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000006c0: 0000 0300 0000 7330 0000 0074 0064 0119  ......s0...t.d..
-000006d0: 0089 0009 0064 0687 0066 0164 0264 0384  .....d...f.d.d..
-000006e0: 097d 0074 017c 0064 048d 017d 017c 0164  .}.t.|.d...}.|.d
-000006f0: 0519 0083 0001 0064 0053 0029 074e da07  .......d.S.).N..
-00000700: 6465 7461 696c 7363 0100 0000 0000 0000  detailsc........
-00000710: 0000 0000 0300 0000 0300 0000 1300 0000  ................
-00000720: 736c 0000 007c 00a0 00a1 0073 3409 0074  sl...|.....s4..t
-00000730: 0164 0119 0064 026b 0372 0c71 0074 0283  .d...d.k.r.q.t..
-00000740: 005c 027d 017d 0288 0064 036b 0572 1d74  .\.}.}...d.k.r.t
-00000750: 036a 0464 047c 0169 0164 058d 0101 0074  .j.d.|.i.d.....t
-00000760: 036a 0464 067c 0269 0164 058d 0101 0074  .j.d.|.i.d.....t
-00000770: 057c 0283 0101 0074 06a0 0764 07a1 0101  .|.....t...d....
-00000780: 007c 00a0 00a1 0072 0464 0053 0064 0053  .|.....r.d.S.d.S
-00000790: 0029 084e da17 696e 7465 726e 616c 5f73  .).N..internal_s
-000007a0: 7461 7475 7365 735f 6275 696c 74da 0379  tatuses_built..y
-000007b0: 6573 e903 0000 007a 1269 6e74 6572 6e61  es.....z.interna
-000007c0: 6c5f 7374 6174 7573 6573 3a29 01da 0464  l_statuses:)...d
-000007d0: 6174 617a 0c77 6169 7469 6e67 2066 6f72  ataz.waiting for
-000007e0: 3a72 0400 0000 2908 da06 6973 5f73 6574  :r....)...is_set
-000007f0: 7202 0000 0072 2200 0000 da04 7269 6368  r....r".....rich
-00000800: da0a 7072 696e 745f 6a73 6f6e 722a 0000  ..print_jsonr*..
-00000810: 0072 1400 0000 da05 736c 6565 7029 03da  .r......sleep)..
-00000820: 0a73 746f 705f 6576 656e 7472 0800 0000  .stop_eventr....
-00000830: 721c 0000 00a9 0172 2b00 0000 7220 0000  r......r+...r ..
-00000840: 0072 2100 0000 da04 7461 736b 7c00 0000  .r!.....task|...
-00000850: 7322 0000 0008 0302 010c 0302 010a 0208  s"..............
-00000860: 0204 0104 0202 ff06 ff04 0604 0202 ff06  ................
-00000870: ff08 060a 0210 e87a 2d70 7269 6e74 5f69  .......z-print_i
-00000880: 735f 646f 6e65 5f73 7461 7475 735f 7265  s_done_status_re
-00000890: 7065 7469 7665 6c79 2e3c 6c6f 6361 6c73  petively.<locals
-000008a0: 3e2e 7461 736b 2901 7236 0000 00da 026f  >.task).r6.....o
-000008b0: 6e29 014e 2902 7202 0000 0072 0300 0000  n).N).r....r....
-000008c0: 2902 7236 0000 00da 0874 6865 5f74 6173  ).r6.....the_tas
-000008d0: 6b72 2000 0000 7235 0000 0072 2100 0000  kr ...r5...r!...
-000008e0: da1f 7072 696e 745f 6973 5f64 6f6e 655f  ..print_is_done_
-000008f0: 7374 6174 7573 5f72 6570 6574 6976 656c  status_repetivel
-00000900: 7979 0000 0073 0e00 0000 0801 0203 0eff  yy...s..........
-00000910: 0220 0201 06ff 0e03 7239 0000 0029 0eda  . ......r9...)..
-00000920: 075f 5f64 6f63 5f5f 7214 0000 0072 1800  .__doc__r....r..
-00000930: 0000 7231 0000 00da 3c66 6163 746f 7279  ..r1....<factory
-00000940: 5f66 6172 6d2e 7072 6f63 6564 7572 6573  _farm.procedures
-00000950: 2e69 6d70 6c69 6369 745f 7072 6f63 6564  .implicit_proced
-00000960: 7572 652e 7072 6f63 6573 732e 7661 7269  ure.process.vari
-00000970: 6162 6c65 7372 0200 0000 da23 6661 6374  ablesr.....#fact
-00000980: 6f72 795f 6661 726d 2e74 6f70 6963 732e  ory_farm.topics.
-00000990: 696d 706c 6963 6974 2e74 6872 6561 6472  implicit.threadr
-000009a0: 0300 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-000009b0: 0000 0072 2200 0000 722a 0000 0072 3900  ...r"...r*...r9.
-000009c0: 0000 7220 0000 0072 2000 0000 7220 0000  ..r ...r ...r ..
-000009d0: 0072 2100 0000 da08 3c6d 6f64 756c 653e  .r!.....<module>
-000009e0: 0100 0000 7318 0000 0004 0208 0408 0108  ....s...........
-000009f0: 020c 010c 010c 020c 010c 0108 0208 430c  ..............C.
-00000a00: 24                                       $
+00000080: 6d0a 5a0a 0100 6401 6409 6c0b 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000090: 0100 640a 640b 8400 5a0c 640c 640d 8400  ..d.d...Z.d.d...
+000000a0: 5a0d 640e 640f 8400 5a0e 6402 5300 2910  Z.d.d...Z.d.S.).
+000000b0: 7a23 0a09 7468 655f 7363 616e 205b 2270  z#..the_scan ["p
+000000c0: 726f 6365 7373 225d 2e69 735f 616c 6976  rocess"].is_aliv
+000000d0: 6520 2829 0ae9 0000 0000 4e29 01da 1c69  e ()......N)...i
+000000e0: 6d70 6c69 6369 745f 7072 6f63 6564 7572  mplicit_procedur
+000000f0: 655f 7661 7269 6162 6c65 7329 01da 0f69  e_variables)...i
+00000100: 6d70 6c69 6369 745f 7468 7265 6164 e901  mplicit_thread..
+00000110: 0000 0029 01da 0973 656e 645f 646f 6e65  ...)...send_done
+00000120: 2901 da0f 6167 6772 6567 6174 655f 7374  )...aggregate_st
+00000130: 6174 7329 01da 0c73 746f 705f 7072 6f63  ats)...stop_proc
+00000140: 6573 7329 01da 0670 7072 696e 7463 0000  ess)...pprintc..
+00000150: 0000 0000 0000 0000 0000 0700 0000 0b00  ................
+00000160: 0000 4300 0000 7392 0100 0074 0064 0119  ..C...s....t.d..
+00000170: 007d 0074 0064 0219 0064 0319 007d 0169  .}.t.d...d...}.i
+00000180: 007d 0267 007d 037c 0044 005d 9a7d 0464  .}.g.}.|.D.].}.d
+00000190: 047d 0509 007a 287c 007c 0419 0064 0519  .}...z(|.|...d..
+000001a0: 0064 0519 00a0 01a1 0064 066b 0272 3c74  .d.......d.k.r<t
+000001b0: 02a0 02a1 0074 037c 007c 0419 0064 0719  .....t.|.|...d..
+000001c0: 0064 0819 0083 0118 0074 037c 0183 016b  .d.......t.|...k
+000001d0: 0572 3c74 047c 0464 0964 0a69 0164 0b8d  .r<t.|.d.d.i.d..
+000001e0: 0201 0057 006e 1904 0074 0579 5601 007d  ...W.n...t.yV..}
+000001f0: 0601 007a 0d74 0664 0c74 07a0 08a1 0083  ...z.t.d.t......
+00000200: 0201 0057 0059 0064 007d 067e 066e 0564  ...W.Y.d.}.~.n.d
+00000210: 007d 067e 0677 0177 0009 007a 1a7c 007c  .}.~.w.w...z.|.|
+00000220: 0419 0064 0519 0064 0519 00a0 01a1 0064  ...d...d.......d
+00000230: 0d6b 0272 7164 0e7d 0564 0e74 0064 0119  .k.rqd.}.d.t.d..
+00000240: 007c 0419 0064 0f19 0064 053c 0057 006e  .|...d...d.<.W.n
+00000250: 2a04 0074 0579 8b01 007d 0601 007a 0d74  *..t.y...}...z.t
+00000260: 0664 1074 07a0 08a1 0083 0201 0057 0059  .d.t.........W.Y
+00000270: 0064 007d 067e 066e 1664 007d 067e 0677  .d.}.~.n.d.}.~.w
+00000280: 0104 0074 0579 9c01 007d 0601 007a 0657  ...t.y...}...z.W
+00000290: 0059 0064 007d 067e 066e 0564 007d 067e  .Y.d.}.~.n.d.}.~
+000002a0: 0677 0177 007c 007c 0419 0064 0f19 0064  .w.w.|.|...d...d
+000002b0: 1119 007c 0564 129c 027c 027c 043c 0071  ...|.d...|.|.<.q
+000002c0: 1009 007c 0244 005d 167d 047c 027c 0419  ...|.D.].}.|.|..
+000002d0: 0064 0519 0064 0e6b 0372 c47c 03a0 097c  .d...d.k.r.|...|
+000002e0: 0474 0064 0119 007c 0419 0064 139c 02a1  .t.d...|...d....
+000002f0: 0101 0071 ae7c 027c 0367 0253 0029 144e  ...q.|.|.g.S.).N
+00000300: da11 696e 7465 726e 616c 5f73 7461 7475  ..internal_statu
+00000310: 7365 73da 0f69 6e74 726f 5f76 6172 6961  ses..intro_varia
+00000320: 626c 6573 da0a 7469 6d65 5f6c 696d 6974  bles..time_limit
+00000330: da07 7065 6e64 696e 67da 0770 726f 6365  ..pending..proce
+00000340: 7373 54da 0574 696d 6573 da07 7374 6172  ssT..times..star
+00000350: 7465 64da 0561 6c61 726d 7a13 7469 6d65  ted..alarmz.time
+00000360: 206c 696d 6974 2065 7863 6565 6465 6429   limit exceeded)
+00000370: 01da 0673 7461 7475 737a 1b74 696d 6520  ...statusz.time 
+00000380: 6c69 6d69 7420 6368 6563 6b20 6578 6365  limit check exce
+00000390: 7074 696f 6e3a 46da 0464 6f6e 6572 1100  ption:F..doner..
+000003a0: 0000 7a1a 7061 7273 6520 616e 6420 6368  ..z.parse and ch
+000003b0: 6563 6b20 6578 6365 7074 696f 6e3a da04  eck exception:..
+000003c0: 7363 616e 2902 7213 0000 0072 0d00 0000  scan).r....r....
+000003d0: 2902 da04 7061 7468 da09 696e 7465 726e  )...path..intern
+000003e0: 616c 7329 0a72 0200 0000 da08 6973 5f61  als).r......is_a
+000003f0: 6c69 7665 da04 7469 6d65 da05 666c 6f61  live..time..floa
+00000400: 7472 0700 0000 da09 4578 6365 7074 696f  tr......Exceptio
+00000410: 6eda 0570 7269 6e74 da09 7472 6163 6562  n..print..traceb
+00000420: 6163 6bda 0a66 6f72 6d61 745f 6578 63da  ack..format_exc.
+00000430: 0661 7070 656e 6429 0772 0900 0000 720b  .append).r....r.
+00000440: 0000 00da 0873 7461 7475 7365 73da 0a75  .....statuses..u
+00000450: 6e66 696e 6973 6865 64da 0b73 7461 7475  nfinished..statu
+00000460: 735f 7061 7468 da0e 7072 6f63 6573 735f  s_path..process_
+00000470: 7374 6174 7573 da01 45a9 0072 2300 0000  status..E..r#...
+00000480: fa77 2f66 6163 746f 7279 5f66 6172 6d2f  .w/factory_farm/
+00000490: 7665 6e75 6573 2f73 7461 6765 732f 6661  venues/stages/fa
+000004a0: 6374 6f72 795f 6661 726d 2f70 726f 6365  ctory_farm/proce
+000004b0: 6475 7265 732f 696d 706c 6963 6974 5f70  dures/implicit_p
+000004c0: 726f 6365 6475 7265 2f70 726f 6365 7373  rocedure/process
+000004d0: 2f6d 6f76 6573 2f70 7269 6e74 5f69 735f  /moves/print_is_
+000004e0: 646f 6e65 5f73 7461 7475 735f 7265 7065  done_status_repe
+000004f0: 7469 7665 6c79 2e70 79da 2470 6172 7365  tively.py.$parse
+00000500: 5f61 6e64 5f63 6865 636b 5f69 735f 616c  _and_check_is_al
+00000510: 6976 655f 6f66 5f73 7461 7475 7365 7314  ive_of_statuses.
+00000520: 0000 0073 5e00 0000 0801 0c01 0402 0401  ...s^...........
+00000530: 0801 0401 0203 0203 1801 2401 0201 0201  ..........$.....
+00000540: 0402 02ff 06fe 0480 0e06 0e01 0c01 0880  ................
+00000550: 02fe 0205 0203 1802 0407 1401 0480 0e02  ................
+00000560: 0e01 0c01 0880 0e03 0c01 0880 02ff 0e05  ................
+00000570: 0201 0cfe 0205 0805 1001 0401 0201 0a01  ................
+00000580: 08fe 0280 0805 7225 0000 0063 0100 0000  ......r%...c....
+00000590: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+000005a0: 4300 0000 7364 0000 0074 007c 0083 0164  C...sd...t.|...d
+000005b0: 016b 0572 0864 0053 0009 0074 0164 0219  .k.r.d.S...t.d..
+000005c0: 007d 017c 0144 005d 0f7d 027c 017c 0219  .}.|.D.].}.|.|..
+000005d0: 0064 0319 0064 0419 0064 056b 0372 1e01  .d...d...d.k.r..
+000005e0: 0064 0053 0071 0f09 0074 0274 0164 0619  .d.S.q...t.t.d..
+000005f0: 0064 0719 0074 0164 0619 0064 0819 0074  .d...t.d...d...t
+00000600: 0383 0064 098d 0301 0064 0053 0029 0a4e  ...d.....d.S.).N
+00000610: 7204 0000 0072 0900 0000 7211 0000 0072  r....r....r....r
+00000620: 0d00 0000 7212 0000 00da 0c69 6e74 726f  ....r......intro
+00000630: 5f68 6172 626f 72da 0468 6f73 74da 0470  _harbor..host..p
+00000640: 6f72 7429 0372 2700 0000 7228 0000 00da  ort).r'...r(....
+00000650: 0870 726f 6365 6564 7329 04da 036c 656e  .proceeds)...len
+00000660: 7202 0000 0072 0500 0000 7206 0000 0029  r....r....r....)
+00000670: 0372 1f00 0000 da15 7468 655f 696e 7465  .r......the_inte
+00000680: 726e 616c 5f73 7461 7475 7365 73da 0f69  rnal_statuses..i
+00000690: 6e74 6572 6e61 6c5f 7374 6174 7573 7223  nternal_statusr#
+000006a0: 0000 0072 2300 0000 7224 0000 00da 1573  ...r#...r$.....s
+000006b0: 656e 645f 646f 6e65 5f69 665f 6669 6e69  end_done_if_fini
+000006c0: 7368 6564 5b00 0000 731c 0000 000c 0104  shed[...s.......
+000006d0: 0102 0208 0308 0114 0d06 0102 ff02 0402  ................
+000006e0: 030a 010a 0104 020a fc72 2d00 0000 6300  .........r-...c.
+000006f0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00000700: 0000 0043 0000 0073 2c00 0000 7400 6401  ...C...s,...t.d.
+00000710: 1900 7d00 0900 6406 6402 6403 8401 7d01  ..}...d.d.d...}.
+00000720: 7401 7c01 6404 8d01 7d02 7c02 6405 1900  t.|.d...}.|.d...
+00000730: 8300 0100 6400 5300 2907 4eda 0764 6574  ....d.S.).N..det
+00000740: 6169 6c73 6301 0000 0000 0000 0000 0000  ailsc...........
+00000750: 0003 0000 0003 0000 0053 0000 0073 5200  .........S...sR.
+00000760: 0000 7c00 a000 a100 7327 0900 7401 6401  ..|.....s'..t.d.
+00000770: 1900 6402 6b03 720c 7100 7402 8300 5c02  ..d.k.r.q.t...\.
+00000780: 7d01 7d02 0900 7403 6403 7c02 6901 8301  }.}...t.d.|.i...
+00000790: 0100 7404 7c02 8301 0100 7405 a006 6404  ..t.|.....t...d.
+000007a0: a101 0100 7c00 a000 a100 7204 6400 5300  ....|.....r.d.S.
+000007b0: 6400 5300 2905 4eda 1769 6e74 6572 6e61  d.S.).N..interna
+000007c0: 6c5f 7374 6174 7573 6573 5f62 7569 6c74  l_statuses_built
+000007d0: da03 7965 737a 0c77 6169 7469 6e67 2066  ..yesz.waiting f
+000007e0: 6f72 3a72 0400 0000 2907 da06 6973 5f73  or:r....)...is_s
+000007f0: 6574 7202 0000 0072 2500 0000 7208 0000  etr....r%...r...
+00000800: 0072 2d00 0000 7217 0000 00da 0573 6c65  .r-...r......sle
+00000810: 6570 2903 da0a 7374 6f70 5f65 7665 6e74  ep)...stop_event
+00000820: 7209 0000 0072 1f00 0000 7223 0000 0072  r....r....r#...r
+00000830: 2300 0000 7224 0000 00da 0474 6173 6b82  #...r$.....task.
+00000840: 0000 0073 1800 0000 0803 0201 0c03 0201  ...s............
+00000850: 0a02 0202 0207 0401 06ff 0804 0a02 10ea  ................
+00000860: 7a2d 7072 696e 745f 6973 5f64 6f6e 655f  z-print_is_done_
+00000870: 7374 6174 7573 5f72 6570 6574 6976 656c  status_repetivel
+00000880: 792e 3c6c 6f63 616c 733e 2e74 6173 6b29  y.<locals>.task)
+00000890: 0172 3400 0000 da02 6f6e 2901 4e29 0272  .r4.....on).N).r
+000008a0: 0200 0000 7203 0000 0029 0372 2e00 0000  ....r....).r....
+000008b0: 7234 0000 00da 0874 6865 5f74 6173 6b72  r4.....the_taskr
+000008c0: 2300 0000 7223 0000 0072 2400 0000 da1f  #...r#...r$.....
+000008d0: 7072 696e 745f 6973 5f64 6f6e 655f 7374  print_is_done_st
+000008e0: 6174 7573 5f72 6570 6574 6976 656c 797f  atus_repetively.
+000008f0: 0000 0073 0e00 0000 0801 0203 0aff 021e  ...s............
+00000900: 0201 06ff 0e03 7237 0000 0029 0fda 075f  ......r7...)..._
+00000910: 5f64 6f63 5f5f 7217 0000 0072 1b00 0000  _doc__r....r....
+00000920: da04 7269 6368 da3c 6661 6374 6f72 795f  ..rich.<factory_
+00000930: 6661 726d 2e70 726f 6365 6475 7265 732e  farm.procedures.
+00000940: 696d 706c 6963 6974 5f70 726f 6365 6475  implicit_procedu
+00000950: 7265 2e70 726f 6365 7373 2e76 6172 6961  re.process.varia
+00000960: 626c 6573 7202 0000 00da 2366 6163 746f  blesr.....#facto
+00000970: 7279 5f66 6172 6d2e 746f 7069 6373 2e69  ry_farm.topics.i
+00000980: 6d70 6c69 6369 742e 7468 7265 6164 7203  mplicit.threadr.
+00000990: 0000 0072 0500 0000 7206 0000 0072 0700  ...r....r....r..
+000009a0: 0000 7208 0000 0072 2500 0000 722d 0000  ..r....r%...r-..
+000009b0: 0072 3700 0000 7223 0000 0072 2300 0000  .r7...r#...r#...
+000009c0: 7223 0000 0072 2400 0000 da08 3c6d 6f64  r#...r$.....<mod
+000009d0: 756c 653e 0100 0000 731a 0000 0004 0208  ule>....s.......
+000009e0: 0408 0108 020c 010c 010c 020c 010c 010c  ................
+000009f0: 0208 0208 470c 24                        ....G.$
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/send_done.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/stop_process.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/__pycache__/venture_finish.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/done_with_scan.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/print_is_done_status_repetively.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from factory_farm.procedures.implicit_procedure.process.variables import implicit_procedure_variables
 from factory_farm.topics.implicit.thread import implicit_thread
 
 from .send_done import send_done
 from .aggregate_stats import aggregate_stats
 from .stop_process import stop_process
 
+from pprint import pprint
+
 def parse_and_check_is_alive_of_statuses ():
 	internal_statuses = implicit_procedure_variables ["internal_statuses"]
 	time_limit = implicit_procedure_variables ["intro_variables"] ["time_limit"]
 
 	statuses = {}
 	unfinished = []
 	for status_path in internal_statuses:
@@ -37,14 +39,18 @@
 							"alarm": "time limit exceeded"
 						}
 					)
 		except Exception as E:
 			print ("time limit check exception:", traceback.format_exc ())
 			pass;
 		
+		
+		'''
+			check if process is_alive is false
+		'''
 		try:
 			#print ("checking process status:", internal_statuses [ status_path ])		
 			if (internal_statuses [ status_path ] ["process"] ["process"].is_alive () == False):				
 				#
 				#	
 				#
 				#	check if the scan is done, if not the process exitted 
@@ -54,17 +60,14 @@
 				implicit_procedure_variables ["internal_statuses"] [ status_path ] ["status"] ["process"] = "done"
 
 		except Exception as E:
 			print ("parse and check exception:", traceback.format_exc ())
 			pass;
 
 		
-				
-			
-		
 		except Exception as E:
 			pass;
 			
 
 		statuses [ status_path ] = {
 			"scan": internal_statuses [ status_path ] ["status"] ["scan"],
 			"process": process_status
@@ -73,15 +76,18 @@
 	'''
 		loop through again,
 		because exceptions might
 		have occurred.
 	'''
 	for status_path in statuses:
 		if (statuses [ status_path ] ["process"] != "done"):
-			unfinished.append (status_path)
+			unfinished.append ({
+				"path": status_path,
+				"internals": implicit_procedure_variables ["internal_statuses"] [ status_path ]
+			})
 		
 	return [ statuses, unfinished ]
 		
 
 def send_done_if_finished (unfinished):
 	if (len (unfinished) >= 1):
 		return;
@@ -129,26 +135,24 @@
 				check if internal_statuses_built
 			'''
 			if (implicit_procedure_variables ["internal_statuses_built"] != "yes"):
 				continue;
 		
 			[ internal_statuses, unfinished ] = parse_and_check_is_alive_of_statuses ()
 			
-			if (details >= 3):
-				rich.print_json (
-					data = {
-						"internal_statuses:": internal_statuses
-					}
-				)
-			
-			rich.print_json (
-				data = {
-					"waiting for:": unfinished
-				}
-			)
+			'''
+			if (details >= 2):
+				pprint ({
+						"internal_statuses:": implicit_procedure_variables ["internal_statuses"]
+				})
+			'''
+			
+			pprint ({
+				"waiting for:": unfinished
+			})
 			
 			send_done_if_finished (unfinished)
 			
 			time.sleep (1)
```

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/stop_process.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/moves/venture_finish.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/implicit_procedure/process/variables/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/__pycache__/send_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/on.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/coms/implicit_procedure/send_paths.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__init__v1.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/procedures/intro/keg/quart__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/START_A_SCAN.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/aggregate/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/alarm_parser/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/implicit/thread/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/__pycache__/passes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/printout/passes.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/printout/passes.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/background.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/__pycache__/implicit.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/process_on/p_expect/implicit.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/queues/queue_capacity_limiter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/before.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/one.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/sequentially.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/__pycache__/simultaneously.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/venues/stages/factory_farm/topics/start--/simultaneously.py` & `factory_farm-1.2.1/venues/stages/factory_farm/topics/start--/simultaneously.py`

 * *Files identical despite different names*

### Comparing `factory_farm-1.2.0/PKG-INFO` & `factory_farm-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: factory_farm
-Version: 1.2.0
+Version: 1.2.1
 Summary: The automated cybentic herb harvest factory of plantary towns yet to be established.
 License: GPL-3.0-only
 Keywords: neurons,nervous system,bioelectric,homeostasis,reliability,consistency,integrity,guarantees,vows,oaths,assurances,insurances,ensurances,speed,calmness,education,augmentation,enhancement,improvements
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

