# Comparing `tmp/octomy-batch-2.0.6.tar.gz` & `tmp/octomy-batch-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-2.0.6.tar", last modified: Sun Apr 14 10:11:05 2024, max compression
+gzip compressed data, was "octomy-batch-2.0.7.tar", last modified: Tue Apr 16 11:34:03 2024, max compression
```

## Comparing `octomy-batch-2.0.6.tar` & `octomy-batch-2.0.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.932023 octomy-batch-2.0.6/
--rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.6/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.6/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.6/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.6/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-14 10:11:05.932023 octomy-batch-2.0.6/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.6/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-14 10:10:44.000000 octomy-batch-2.0.6/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/bin/
--rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.6/bin/octomy-batch
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/code_quality/
--rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.6/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.6/code_quality/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.6/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.6/code_quality/pylintrc
--rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.6/config.json
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.920023 octomy-batch-2.0.6/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.924023 octomy-batch-2.0.6/octomy/batch/
--rw-r--r--   0 leo       (1000) leo       (1000)    20884 2024-04-13 21:48:00.000000 octomy-batch-2.0.6/octomy/batch/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.924023 octomy-batch-2.0.6/octomy/batch/filters/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.6/octomy/batch/filters/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.924023 octomy-batch-2.0.6/octomy/batch/filters/base/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.6/octomy/batch/filters/base/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.6/octomy/batch/filters/base/hello.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.924023 octomy-batch-2.0.6/octomy/batch/filters/utils/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.6/octomy/batch/filters/utils/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.6/octomy/batch/filters/utils/ping.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.6/octomy/batch/filters/utils/test.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.924023 octomy-batch-2.0.6/octomy/batch/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.6/octomy/batch/server/WebsiteIO.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.6/octomy/batch/server/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4487 2024-04-11 00:20:42.000000 octomy-batch-2.0.6/octomy/batch/types.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/octomy_batch.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-14 10:11:05.000000 octomy-batch-2.0.6/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.6/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-14 10:05:39.000000 octomy-batch-2.0.6/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-14 10:08:24.000000 octomy-batch-2.0.6/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.6/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.6/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-14 10:11:05.932023 octomy-batch-2.0.6/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7479 2024-04-11 00:17:44.000000 octomy-batch-2.0.6/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.6/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.6/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.6/tests/integration/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:35.000000 octomy-batch-2.0.6/tests/integration/test_integration.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.928023 octomy-batch-2.0.6/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.6/tests/load/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      118 2024-04-13 19:27:44.000000 octomy-batch-2.0.6/tests/load/test_load.py
--rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.6/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.932023 octomy-batch-2.0.6/tests/regressions/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.6/tests/regressions/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:26.000000 octomy-batch-2.0.6/tests/regressions/test_regressions.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:11:05.932023 octomy-batch-2.0.6/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.6/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1188 2024-04-13 21:48:19.000000 octomy-batch-2.0.6/tests/unit/test_batch_processor.py
--rw-r--r--   0 leo       (1000) leo       (1000)      178 2024-04-13 14:03:03.000000 octomy-batch-2.0.6/tests/unit/test_server.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2828 2024-04-13 14:24:05.000000 octomy-batch-2.0.6/tests/unit/test_unit.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/
+-rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.7/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.7/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.7/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.7/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.7/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-16 11:33:13.000000 octomy-batch-2.0.7/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/bin/
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.7/bin/octomy-batch
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/code_quality/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.7/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.7/code_quality/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.7/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.7/code_quality/pylintrc
+-rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.7/config.json
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.687605 octomy-batch-2.0.7/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.691605 octomy-batch-2.0.7/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    20878 2024-04-16 11:29:17.000000 octomy-batch-2.0.7/octomy/batch/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.691605 octomy-batch-2.0.7/octomy/batch/filters/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.7/octomy/batch/filters/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.691605 octomy-batch-2.0.7/octomy/batch/filters/base/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.7/octomy/batch/filters/base/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.7/octomy/batch/filters/base/hello.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.691605 octomy-batch-2.0.7/octomy/batch/filters/utils/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.7/octomy/batch/filters/utils/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.7/octomy/batch/filters/utils/ping.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.7/octomy/batch/filters/utils/test.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.7/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.7/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4487 2024-04-11 00:20:42.000000 octomy-batch-2.0.7/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/octomy_batch.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:34:03.000000 octomy-batch-2.0.7/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.7/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.695605 octomy-batch-2.0.7/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-16 11:30:48.000000 octomy-batch-2.0.7/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-16 11:33:47.000000 octomy-batch-2.0.7/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.7/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.7/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7479 2024-04-11 00:17:44.000000 octomy-batch-2.0.7/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.7/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.7/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.7/tests/integration/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:35.000000 octomy-batch-2.0.7/tests/integration/test_integration.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.7/tests/load/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      118 2024-04-13 19:27:44.000000 octomy-batch-2.0.7/tests/load/test_load.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.7/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/tests/regressions/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.7/tests/regressions/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:26.000000 octomy-batch-2.0.7/tests/regressions/test_regressions.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:34:03.699605 octomy-batch-2.0.7/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.7/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1188 2024-04-13 21:48:19.000000 octomy-batch-2.0.7/tests/unit/test_batch_processor.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      178 2024-04-13 14:03:03.000000 octomy-batch-2.0.7/tests/unit/test_server.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2828 2024-04-13 14:24:05.000000 octomy-batch-2.0.7/tests/unit/test_unit.py
```

### Comparing `octomy-batch-2.0.6/.gitlab/ci.yaml` & `octomy-batch-2.0.7/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/LICENSE` & `octomy-batch-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/PKG-INFO` & `octomy-batch-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.6
+Version: 2.0.7
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.6/README.md` & `octomy-batch-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/bin/octomy-batch` & `octomy-batch-2.0.7/bin/octomy-batch`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/code_quality/Makefile` & `octomy-batch-2.0.7/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/code_quality/pylintrc` & `octomy-batch-2.0.7/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/config.json` & `octomy-batch-2.0.7/config.json`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy/batch/__init__.py` & `octomy-batch-2.0.7/octomy/batch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 	def __del__(self):
 		if self.worker_id:
 			logger.info(f"Batch Processor {self.worker_id} deleted")
 			self.worker_id = None
 
 
 	async def create_tables(self):
-		await self.dbc.register_query_dir(self.package_dir, do_preload = True, do_debug = True)
+		self.dbc.register_query_dir(self.package_dir, do_preload = True, do_debug = True)
 		await self.dbc.query_none("overwatch.batch.create_batch_status_enum", prepare=False)
 		await self.dbc.query_none("overwatch.batch.create_batch_items", prepare=False)
 		await self.dbc.query_none("overwatch.batch.create_gcra_throttle", prepare=False)
 
 	async def verify(self):
 		modules = await self.list_modules()
 		# logger.info(f"modules: {pprint.pformat(modules)}")
```

### Comparing `octomy-batch-2.0.6/octomy/batch/filters/utils/ping.py` & `octomy-batch-2.0.7/octomy/batch/filters/utils/ping.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy/batch/filters/utils/test.py` & `octomy-batch-2.0.7/octomy/batch/filters/utils/test.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy/batch/server/WebsiteIO.py` & `octomy-batch-2.0.7/octomy/batch/server/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy/batch/server/__init__.py` & `octomy-batch-2.0.7/octomy/batch/server/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy/batch/types.py` & `octomy-batch-2.0.7/octomy/batch/types.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/octomy_batch.egg-info/PKG-INFO` & `octomy-batch-2.0.7/octomy_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.6
+Version: 2.0.7
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-batch-2.0.6/octomy_batch.egg-info/SOURCES.txt` & `octomy-batch-2.0.7/octomy_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/requirements/requirements.txt` & `octomy-batch-2.0.7/requirements/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via octomy-common
 idna==2.10
     # via
     #   email-validator
     #   requests
 markupsafe==2.1.5
     # via octomy-common
-octomy-common==2.0.7
+octomy-common==2.0.8
     # via -r requirements.in
 orderedmultidict==1.0.1
     # via furl
 psycopg[binary,pool]==3.1.10
     # via octomy-common
 psycopg-binary==3.1.10
     # via psycopg
```

### Comparing `octomy-batch-2.0.6/requirements/test_requirements.txt` & `octomy-batch-2.0.7/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/setup.py` & `octomy-batch-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/tests/Makefile` & `octomy-batch-2.0.7/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/tests/unit/test_batch_processor.py` & `octomy-batch-2.0.7/tests/unit/test_batch_processor.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.6/tests/unit/test_unit.py` & `octomy-batch-2.0.7/tests/unit/test_unit.py`

 * *Files identical despite different names*

