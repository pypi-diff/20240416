# Comparing `tmp/body_scan-1.0.6.tar.gz` & `tmp/body_scan-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "body_scan-1.0.6.tar", last modified: Fri Feb  2 00:38:49 2024, max compression
+gzip compressed data, was "body_scan-1.1.0.tar", max compression
```

## Comparing `body_scan-1.0.6.tar` & `body_scan-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,64 @@
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.776957 body_scan-1.0.6/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     5171 2024-02-02 00:38:49.776957 body_scan-1.0.6/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     4809 2023-11-14 19:06:16.000000 body_scan-1.0.6/module.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1094 2024-02-02 00:38:45.000000 body_scan-1.0.6/pyproject.toml
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       38 2024-02-02 00:38:49.776957 body_scan-1.0.6/setup.cfg
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.771957 body_scan-1.0.6/structure/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.771957 body_scan-1.0.6/structure/decor/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.773957 body_scan-1.0.6/structure/decor/body_scan/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3393 2023-11-12 19:42:09.000000 body_scan-1.0.6/structure/decor/body_scan/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.773957 body_scan-1.0.6/structure/decor/body_scan/_license/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      361 2023-12-16 19:50:18.000000 body_scan-1.0.6/structure/decor/body_scan/_license/license.s.HTML
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/_license/list/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1102 2023-12-11 19:21:17.000000 body_scan-1.0.6/structure/decor/body_scan/_license/list/lentils license.s.HTML
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/aggregate/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      621 2023-10-28 18:33:44.000000 body_scan-1.0.6/structure/decor/body_scan/aggregate/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       50 2023-10-28 18:05:55.000000 body_scan-1.0.6/structure/decor/body_scan/body_scan.s.HTML
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/db/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      860 2023-10-29 16:40:03.000000 body_scan-1.0.6/structure/decor/body_scan/db/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/functions/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/functions/alarm_printer/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      544 2023-10-28 19:19:59.000000 body_scan-1.0.6/structure/decor/body_scan/functions/alarm_printer/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      410 2023-10-28 18:25:44.000000 body_scan-1.0.6/structure/decor/body_scan/functions/exceptions.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.774957 body_scan-1.0.6/structure/decor/body_scan/functions/start/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      274 2023-11-12 19:52:29.000000 body_scan-1.0.6/structure/decor/body_scan/functions/start/one.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      407 2023-11-12 19:51:53.000000 body_scan-1.0.6/structure/decor/body_scan/functions/start/sequentially.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      596 2023-11-12 19:51:43.000000 body_scan-1.0.6/structure/decor/body_scan/functions/start/simultaneously.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.772957 body_scan-1.0.6/structure/decor/body_scan/processes/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/collect/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      587 2023-10-13 22:41:31.000000 body_scan-1.0.6/structure/decor/body_scan/processes/collect/collect.s.HTML
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      248 2023-10-28 18:27:14.000000 body_scan-1.0.6/structure/decor/body_scan/processes/collect/path.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        0 2023-10-13 03:13:25.000000 body_scan-1.0.6/structure/decor/body_scan/processes/collect/start.proc.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.772957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/keg/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1441 2023-11-12 21:43:35.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/keg/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1760 2024-02-02 00:38:05.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/keg/check.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1022 2024-02-01 04:03:22.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/scan.process.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1294 2023-11-12 21:50:10.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/ask/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1014 2023-11-12 21:47:29.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/ask/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.775957 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/keg/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1248 2024-02-01 04:03:05.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/keg/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      372 2023-11-12 19:53:48.000000 body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/path.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-02 00:38:49.776957 body_scan-1.0.6/structure/decor/body_scan.egg-info/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     5171 2024-02-02 00:38:49.000000 body_scan-1.0.6/structure/decor/body_scan.egg-info/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1440 2024-02-02 00:38:49.000000 body_scan-1.0.6/structure/decor/body_scan.egg-info/SOURCES.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        1 2024-02-02 00:38:49.000000 body_scan-1.0.6/structure/decor/body_scan.egg-info/dependency_links.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       51 2024-02-02 00:38:49.000000 body_scan-1.0.6/structure/decor/body_scan.egg-info/requires.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       10 2024-02-02 00:38:49.000000 body_scan-1.0.6/structure/decor/body_scan.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1150 2023-11-11 05:25:29.106436 body_scan-1.1.0/business.s.HTML
+-rw-r--r--   0        0        0      701 2024-04-16 01:45:44.727736 body_scan-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5044 2024-04-16 01:29:59.399778 body_scan-1.1.0/readme.md
+-rw-r--r--   0        0        0     1988 2024-04-16 01:44:40.944345 body_scan-1.1.0/venue.S.HTML
+-rw-r--r--   0        0        0     3458 2024-04-16 01:40:55.874421 body_scan-1.1.0/venues/stages/body_scan/__init__.py
+-rw-r--r--   0        0        0     3103 2023-10-28 18:43:17.934907 body_scan-1.1.0/venues/stages/body_scan/_book/book.r.html
+-rw-r--r--   0        0        0      361 2023-12-16 19:50:18.396199 body_scan-1.1.0/venues/stages/body_scan/_license/license.s.HTML
+-rw-r--r--   0        0        0    37279 2023-12-01 20:51:04.310266 body_scan-1.1.0/venues/stages/body_scan/_license/list/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0     1102 2023-12-11 19:21:17.067116 body_scan-1.1.0/venues/stages/body_scan/_license/list/lentils license.s.HTML
+-rw-r--r--   0        0        0      621 2023-10-28 18:33:44.995680 body_scan-1.1.0/venues/stages/body_scan/aggregate/__init__.py
+-rw-r--r--   0        0        0      670 2024-02-01 04:01:56.878508 body_scan-1.1.0/venues/stages/body_scan/aggregate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1177 2023-10-28 18:33:51.656601 body_scan-1.1.0/venues/stages/body_scan/aggregate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      327 2023-10-28 18:27:14.438315 body_scan-1.1.0/venues/stages/body_scan/body_scan
+-rw-r--r--   0        0        0       50 2023-10-28 18:05:55.170498 body_scan-1.1.0/venues/stages/body_scan/body_scan.s.HTML
+-rw-r--r--   0        0        0      860 2023-10-29 16:40:03.244132 body_scan-1.1.0/venues/stages/body_scan/db/__init__.py
+-rw-r--r--   0        0        0     1007 2024-02-01 04:03:31.489395 body_scan-1.1.0/venues/stages/body_scan/db/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1707 2023-11-01 00:25:26.466620 body_scan-1.1.0/venues/stages/body_scan/db/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      823 2023-10-13 03:17:38.378900 body_scan-1.1.0/venues/stages/body_scan/functions/__pycache__/CHECK_STATUS_LOCATION.cpython-311.pyc
+-rw-r--r--   0        0        0     3031 2023-10-13 03:23:45.508960 body_scan-1.1.0/venues/stages/body_scan/functions/__pycache__/START_A_SCAN.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2024-02-01 04:03:08.499665 body_scan-1.1.0/venues/stages/body_scan/functions/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     1081 2023-10-28 18:25:47.125351 body_scan-1.1.0/venues/stages/body_scan/functions/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0      544 2023-10-28 19:19:59.472975 body_scan-1.1.0/venues/stages/body_scan/functions/alarm_printer/__init__.py
+-rw-r--r--   0        0        0      634 2024-02-01 04:01:56.881508 body_scan-1.1.0/venues/stages/body_scan/functions/alarm_printer/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1089 2023-10-28 19:20:56.076308 body_scan-1.1.0/venues/stages/body_scan/functions/alarm_printer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      410 2023-10-28 18:25:44.783379 body_scan-1.1.0/venues/stages/body_scan/functions/exceptions.py
+-rw-r--r--   0        0        0      654 2023-11-01 00:26:26.461936 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/before.cpython-311.pyc
+-rw-r--r--   0        0        0      469 2024-02-01 04:01:57.189504 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/one.cpython-310.pyc
+-rw-r--r--   0        0        0      682 2023-11-12 19:53:04.399358 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/one.cpython-311.pyc
+-rw-r--r--   0        0        0      582 2024-02-01 04:01:56.883508 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/sequentially.cpython-310.pyc
+-rw-r--r--   0        0        0      867 2023-11-12 19:52:01.128042 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/sequentially.cpython-311.pyc
+-rw-r--r--   0        0        0      880 2024-02-01 04:01:57.184504 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/simultaneously.cpython-310.pyc
+-rw-r--r--   0        0        0     1485 2023-11-12 19:52:01.133042 body_scan-1.1.0/venues/stages/body_scan/functions/start/__pycache__/simultaneously.cpython-311.pyc
+-rw-r--r--   0        0        0      274 2023-11-12 19:52:29.903731 body_scan-1.1.0/venues/stages/body_scan/functions/start/one.py
+-rw-r--r--   0        0        0      407 2023-11-12 19:51:53.009130 body_scan-1.1.0/venues/stages/body_scan/functions/start/sequentially.py
+-rw-r--r--   0        0        0      596 2023-11-12 19:51:43.389233 body_scan-1.1.0/venues/stages/body_scan/functions/start/simultaneously.py
+-rw-r--r--   0        0        0      587 2023-10-13 22:41:31.337422 body_scan-1.1.0/venues/stages/body_scan/processes/collect/collect.s.HTML
+-rw-r--r--   0        0        0      248 2023-10-28 18:27:14.482314 body_scan-1.1.0/venues/stages/body_scan/processes/collect/path.py
+-rw-r--r--   0        0        0        0 2023-10-13 03:13:25.295616 body_scan-1.1.0/venues/stages/body_scan/processes/collect/start.proc.py
+-rw-r--r--   0        0        0      895 2023-10-24 16:51:48.714898 body_scan-1.1.0/venues/stages/body_scan/processes/scan/__pycache__/PATH.cpython-311.pyc
+-rw-r--r--   0        0        0     2823 2023-11-12 19:47:54.502707 body_scan-1.1.0/venues/stages/body_scan/processes/scan/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      905 2023-11-12 19:52:01.133042 body_scan-1.1.0/venues/stages/body_scan/processes/scan/__pycache__/path.cpython-311.pyc
+-rw-r--r--   0        0        0     1441 2023-11-12 21:43:35.419356 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__init__.py
+-rw-r--r--   0        0        0     3530 2023-10-24 16:49:29.776382 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/SCAN.cpython-311.pyc
+-rw-r--r--   0        0        0     1893 2024-02-01 04:03:08.498665 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3349 2023-11-12 21:44:03.350051 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1799 2024-04-16 01:31:41.486649 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/check.cpython-310.pyc
+-rw-r--r--   0        0        0     3134 2024-02-02 00:38:19.125263 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/check.cpython-311.pyc
+-rw-r--r--   0        0        0     3122 2023-10-28 18:27:30.957119 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__pycache__/scan.cpython-311.pyc
+-rw-r--r--   0        0        0     1760 2024-02-02 00:38:05.690377 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/check.py
+-rw-r--r--   0        0        0     1022 2024-02-01 04:03:22.106505 body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/scan.process.py
+-rw-r--r--   0        0        0      167 2023-10-28 18:37:56.691704 body_scan-1.1.0/venues/stages/body_scan/processes/scan/scan.r.html
+-rw-r--r--   0        0        0     1294 2023-11-12 21:50:10.465040 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__init__.py
+-rw-r--r--   0        0        0     1352 2024-02-01 04:01:56.885508 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2152 2023-11-12 21:50:12.420018 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      598 2024-02-01 04:01:56.928507 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__pycache__/path.cpython-310.pyc
+-rw-r--r--   0        0        0      937 2023-11-12 19:55:13.235968 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__pycache__/path.cpython-311.pyc
+-rw-r--r--   0        0        0     1014 2023-11-12 21:47:29.231801 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/ask/__init__.py
+-rw-r--r--   0        0        0     1544 2024-02-01 04:01:57.011506 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/ask/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2339 2023-11-12 21:48:15.857292 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/ask/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1248 2024-02-01 04:03:05.683698 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/keg/__init__.py
+-rw-r--r--   0        0        0     1479 2024-02-01 04:03:08.277668 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/keg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2409 2024-02-02 00:36:57.090980 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/keg/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      372 2023-11-12 19:53:48.874878 body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/path.py
+-rw-r--r--   0        0        0     5844 1970-01-01 00:00:00.000000 body_scan-1.1.0/PKG-INFO
```

### Comparing `body_scan-1.0.6/PKG-INFO` & `body_scan-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: body_scan
-Version: 1.0.6
-Summary: Test Framework
-License: GPL 3.0
+Version: 1.1.0
+Summary: Health Checks
+License: GPL-3.0-only
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: botanist (>=1.0.0,<2.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: flask (>=3.0.3,<4.0.0)
+Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: textual (>=0.56.4,<0.57.0)
+Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/body_scan.git
-Description-Content-Type: text/plain
-Requires-Dist: botanist
-Requires-Dist: click
-Requires-Dist: flask
-Requires-Dist: pdoc3
-Requires-Dist: requests
-Requires-Dist: textual
-Requires-Dist: tinydb
+Description-Content-Type: text/markdown
 
 
 
+Bravo! You have received a Medical Diploma in "body_scan" from
+the Orbital Convergence University International Air and Water
+Embassy of the Tangerine Planet.
+
+You are now officially certified to include "body_scan" in your
+practice.
+
 <body>
 	<header>
 		<address>body scan</address>
 	</header>
 
 	<main>
 		<address>quick start</address>
```

### Comparing `body_scan-1.0.6/module.txt` & `body_scan-1.1.0/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 
 
+Bravo! You have received a Medical Diploma in "body_scan" from
+the Orbital Convergence University International Air and Water
+Embassy of the Tangerine Planet.
+
+You are now officially certified to include "body_scan" in your
+practice.
+
 <body>
 	<header>
 		<address>body scan</address>
 	</header>
 
 	<main>
 		<address>quick start</address>
```

### Comparing `body_scan-1.0.6/structure/decor/body_scan/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,31 @@
 from tinydb import TinyDB, Query
 
 '''
 	
 '''
 def start (
 	glob_string = "",
+	
+	paths = [],
+	
 	relative_path = False,
 	module_paths = [],
 	simultaneous = False,
 	print_alarms = True,
 	records = 1,
 	db_directory = False,
 	
 	before = False,
 	after = False
 ):
-	finds = glob.glob (glob_string, recursive = True)
+	if (len (paths) >= 1):
+		finds = paths
+	else:
+		finds = glob.glob (glob_string, recursive = True)
 		
 	relative_path = str (relative_path)	
 		
 	if (records >= 2):
 		print ()
 		print ("searching for glob_string:")
 		print ("	", glob_string)
```

### Comparing `body_scan-1.0.6/structure/decor/body_scan/_license/list/lentils license.s.HTML` & `body_scan-1.1.0/venues/stages/body_scan/_license/list/lentils license.s.HTML`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/aggregate/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/aggregate/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/db/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/db/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/functions/alarm_printer/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/functions/alarm_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/functions/start/simultaneously.py` & `body_scan-1.1.0/venues/stages/body_scan/functions/start/simultaneously.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/collect/collect.s.HTML` & `body_scan-1.1.0/venues/stages/body_scan/processes/collect/collect.s.HTML`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/keg/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/keg/check.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/keg/check.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/process/scan.process.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/process/scan.process.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/ask/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/ask/__init__.py`

 * *Files identical despite different names*

### Comparing `body_scan-1.0.6/structure/decor/body_scan/processes/scan/starter/keg/__init__.py` & `body_scan-1.1.0/venues/stages/body_scan/processes/scan/starter/keg/__init__.py`

 * *Files identical despite different names*

