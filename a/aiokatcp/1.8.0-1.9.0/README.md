# Comparing `tmp/aiokatcp-1.8.0.tar.gz` & `tmp/aiokatcp-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/bmerry/work/sdp/git/aiokatcp/dist/.tmp-f0phl4st/aiokatcp-1.8.0.tar", last modified: Tue Sep 19 15:08:26 2023, max compression
+gzip compressed data, was "aiokatcp-1.9.0.tar", last modified: Tue Apr  9 08:06:10 2024, max compression
```

## Comparing `aiokatcp-1.8.0.tar` & `aiokatcp-1.9.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       53 2022-04-14 06:11:41.000000 aiokatcp-1.8.0/.flake8
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/.github/
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/.github/workflows/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1474 2023-09-19 11:18:20.000000 aiokatcp-1.8.0/.github/workflows/test.yml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       91 2021-07-26 11:03:08.000000 aiokatcp-1.8.0/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1245 2023-09-18 14:41:01.000000 aiokatcp-1.8.0/.pre-commit-config.yaml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      156 2023-09-19 11:19:05.000000 aiokatcp-1.8.0/.readthedocs.yml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1486 2022-04-14 06:11:41.000000 aiokatcp-1.8.0/LICENSE.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1144 2022-04-14 06:11:41.000000 aiokatcp-1.8.0/README.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      480 2022-04-19 12:05:31.000000 aiokatcp-1.8.0/TODO
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/doc/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2017-09-27 07:56:58.000000 aiokatcp-1.8.0/doc/.gitignore
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      670 2018-01-11 09:16:27.000000 aiokatcp-1.8.0/doc/Makefile
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/doc/_static/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2018-01-11 09:16:27.000000 aiokatcp-1.8.0/doc/_static/.keep
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1205 2022-12-08 13:25:04.000000 aiokatcp-1.8.0/doc/aiokatcp.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      346 2022-12-08 13:25:04.000000 aiokatcp-1.8.0/doc/aiokatcp.tools.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     5943 2023-09-19 15:07:36.000000 aiokatcp-1.8.0/doc/changelog.rst
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/doc/client/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2371 2018-01-11 09:16:27.000000 aiokatcp-1.8.0/doc/client/reconnect.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1658 2019-06-03 08:19:32.000000 aiokatcp-1.8.0/doc/client/sensor_watcher.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4288 2019-06-03 08:19:32.000000 aiokatcp-1.8.0/doc/client/tutorial.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      152 2019-06-03 08:19:32.000000 aiokatcp-1.8.0/doc/client.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2118 2023-09-19 15:07:36.000000 aiokatcp-1.8.0/doc/conf.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      499 2018-01-11 09:16:27.000000 aiokatcp-1.8.0/doc/index.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      741 2019-11-11 08:33:27.000000 aiokatcp-1.8.0/doc/intro.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3196 2019-06-03 08:19:32.000000 aiokatcp-1.8.0/doc/migration.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       61 2022-12-06 15:10:53.000000 aiokatcp-1.8.0/doc/modules.rst
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/doc/server/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1892 2022-07-18 10:37:55.000000 aiokatcp-1.8.0/doc/server/logging.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1647 2022-04-19 12:04:15.000000 aiokatcp-1.8.0/doc/server/service_tasks.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14674 2022-11-15 06:01:07.000000 aiokatcp-1.8.0/doc/server/tutorial.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      149 2022-04-19 12:04:15.000000 aiokatcp-1.8.0/doc/server.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1654 2017-11-06 19:05:40.000000 aiokatcp-1.8.0/doc/unicode.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      122 2018-01-11 09:16:27.000000 aiokatcp-1.8.0/doc/user.rst
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2023-09-19 15:07:36.000000 aiokatcp-1.8.0/doc-requirements.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/examples/
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     2161 2022-11-15 08:24:36.000000 aiokatcp-1.8.0/examples/example_client.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     5130 2022-11-15 08:24:36.000000 aiokatcp-1.8.0/examples/example_server.py
--rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     3551 2022-10-24 06:29:45.000000 aiokatcp-1.8.0/examples/mirror_sensors.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      173 2022-04-13 12:58:23.000000 aiokatcp-1.8.0/mypy.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      155 2023-09-18 14:41:01.000000 aiokatcp-1.8.0/pyproject.toml
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      129 2022-04-19 07:10:17.000000 aiokatcp-1.8.0/pytest.ini
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      124 2022-11-13 09:09:04.000000 aiokatcp-1.8.0/requirements.in
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1797 2023-09-18 14:41:01.000000 aiokatcp-1.8.0/requirements.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1143 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/setup.cfg
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1592 2022-04-14 06:11:41.000000 aiokatcp-1.8.0/setup.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2366 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4461 2023-09-18 11:28:33.000000 aiokatcp-1.8.0/src/aiokatcp/adjtimex.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39972 2023-09-18 14:08:25.000000 aiokatcp-1.8.0/src/aiokatcp/client.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    12958 2023-09-18 14:08:25.000000 aiokatcp-1.8.0/src/aiokatcp/connection.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    21066 2023-09-19 11:18:20.000000 aiokatcp-1.8.0/src/aiokatcp/core.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2021-07-26 11:03:08.000000 aiokatcp-1.8.0/src/aiokatcp/py.typed
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    35521 2023-09-18 14:09:21.000000 aiokatcp-1.8.0/src/aiokatcp/sensor.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    42097 2023-09-19 11:18:20.000000 aiokatcp-1.8.0/src/aiokatcp/server.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3766 2023-09-18 11:28:33.000000 aiokatcp-1.8.0/src/aiokatcp/time_sync.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp/tools/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp/tools/__init__.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4105 2022-11-15 08:24:36.000000 aiokatcp-1.8.0/src/aiokatcp/tools/katcpcmd.py
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/
--rw-r--r--   0 bmerry    (1000) bmerry    (1000)     1932 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/PKG-INFO
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1356 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/SOURCES.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/dependency_links.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/entry_points.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-04-13 14:35:48.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/not-zip-safe
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      136 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/requires.txt
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        9 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/src/aiokatcp.egg-info/top_level.txt
-drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2023-09-19 15:08:26.000000 aiokatcp-1.8.0/tests/
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    34873 2023-09-18 14:00:48.000000 aiokatcp-1.8.0/tests/test_client.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8972 2022-10-24 06:29:45.000000 aiokatcp-1.8.0/tests/test_connection.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14597 2022-11-16 09:51:48.000000 aiokatcp-1.8.0/tests/test_core.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    18492 2023-09-18 13:15:44.000000 aiokatcp-1.8.0/tests/test_sensor.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39408 2022-10-24 06:29:45.000000 aiokatcp-1.8.0/tests/test_server.py
--rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4586 2023-09-18 11:28:33.000000 aiokatcp-1.8.0/tests/test_time_sync.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      107 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/.flake8
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.538837 aiokatcp-1.9.0/.github/
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.542837 aiokatcp-1.9.0/.github/workflows/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1093 2024-04-09 07:59:31.000000 aiokatcp-1.9.0/.github/workflows/test.yml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       91 2021-07-26 11:03:08.000000 aiokatcp-1.9.0/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1245 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/.pre-commit-config.yaml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      156 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/.readthedocs.yml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1486 2022-04-14 06:11:41.000000 aiokatcp-1.9.0/LICENSE.txt
+-rw-r--r--   0 bmerry    (1000) bmerry    (1000)     2288 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1144 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/README.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      480 2024-03-28 09:38:21.000000 aiokatcp-1.9.0/TODO
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.542837 aiokatcp-1.9.0/doc/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        7 2017-09-27 07:56:58.000000 aiokatcp-1.9.0/doc/.gitignore
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      670 2018-01-11 09:16:27.000000 aiokatcp-1.9.0/doc/Makefile
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.542837 aiokatcp-1.9.0/doc/_static/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2018-01-11 09:16:27.000000 aiokatcp-1.9.0/doc/_static/.keep
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1205 2022-12-08 13:25:04.000000 aiokatcp-1.9.0/doc/aiokatcp.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      346 2022-12-08 13:25:04.000000 aiokatcp-1.9.0/doc/aiokatcp.tools.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     6295 2024-04-09 08:05:39.000000 aiokatcp-1.9.0/doc/changelog.rst
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.546837 aiokatcp-1.9.0/doc/client/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2371 2018-01-11 09:16:27.000000 aiokatcp-1.9.0/doc/client/reconnect.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1658 2019-06-03 08:19:32.000000 aiokatcp-1.9.0/doc/client/sensor_watcher.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4288 2019-06-03 08:19:32.000000 aiokatcp-1.9.0/doc/client/tutorial.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      152 2019-06-03 08:19:32.000000 aiokatcp-1.9.0/doc/client.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2118 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/doc/conf.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      499 2018-01-11 09:16:27.000000 aiokatcp-1.9.0/doc/index.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      741 2019-11-11 08:33:27.000000 aiokatcp-1.9.0/doc/intro.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3196 2019-06-03 08:19:32.000000 aiokatcp-1.9.0/doc/migration.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       61 2022-12-06 15:10:53.000000 aiokatcp-1.9.0/doc/modules.rst
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.546837 aiokatcp-1.9.0/doc/server/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1892 2022-07-18 10:37:55.000000 aiokatcp-1.9.0/doc/server/logging.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1647 2022-04-19 12:04:15.000000 aiokatcp-1.9.0/doc/server/service_tasks.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14674 2022-11-15 06:01:07.000000 aiokatcp-1.9.0/doc/server/tutorial.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      149 2022-04-19 12:04:15.000000 aiokatcp-1.9.0/doc/server.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1654 2017-11-06 19:05:40.000000 aiokatcp-1.9.0/doc/unicode.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      122 2018-01-11 09:16:27.000000 aiokatcp-1.9.0/doc/user.rst
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/doc-requirements.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.546837 aiokatcp-1.9.0/examples/
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     2161 2022-11-15 08:24:36.000000 aiokatcp-1.9.0/examples/example_client.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     5130 2022-11-15 08:24:36.000000 aiokatcp-1.9.0/examples/example_server.py
+-rwxrwxr-x   0 bmerry    (1000) bmerry    (1000)     3551 2022-10-24 06:29:45.000000 aiokatcp-1.9.0/examples/mirror_sensors.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      173 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/mypy.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      155 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/pyproject.toml
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      129 2022-04-19 07:10:17.000000 aiokatcp-1.9.0/pytest.ini
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      124 2022-11-13 09:09:04.000000 aiokatcp-1.9.0/requirements.in
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1550 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/requirements.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1143 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/setup.cfg
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1592 2022-04-14 06:11:41.000000 aiokatcp-1.9.0/setup.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.538837 aiokatcp-1.9.0/src/
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.546837 aiokatcp-1.9.0/src/aiokatcp/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     2366 2024-04-09 08:06:10.554837 aiokatcp-1.9.0/src/aiokatcp/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4461 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/src/aiokatcp/adjtimex.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    43779 2024-04-08 12:37:17.000000 aiokatcp-1.9.0/src/aiokatcp/client.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    13475 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/src/aiokatcp/connection.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    22427 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/src/aiokatcp/core.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        0 2021-07-26 11:03:08.000000 aiokatcp-1.9.0/src/aiokatcp/py.typed
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    35472 2024-04-08 12:37:17.000000 aiokatcp-1.9.0/src/aiokatcp/sensor.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    41939 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/src/aiokatcp/server.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     3766 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/src/aiokatcp/time_sync.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/src/aiokatcp/tools/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       59 2024-04-09 08:06:10.554837 aiokatcp-1.9.0/src/aiokatcp/tools/__init__.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4105 2022-11-15 08:24:36.000000 aiokatcp-1.9.0/src/aiokatcp/tools/katcpcmd.py
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/src/aiokatcp.egg-info/
+-rw-r--r--   0 bmerry    (1000) bmerry    (1000)     2288 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/PKG-INFO
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     1356 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/SOURCES.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/dependency_links.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)       58 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/entry_points.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        1 2022-04-13 14:35:48.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/not-zip-safe
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)      136 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/requires.txt
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)        9 2024-04-09 08:06:10.000000 aiokatcp-1.9.0/src/aiokatcp.egg-info/top_level.txt
+drwxrwxr-x   0 bmerry    (1000) bmerry    (1000)        0 2024-04-09 08:06:10.550837 aiokatcp-1.9.0/tests/
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    38699 2024-04-08 12:37:17.000000 aiokatcp-1.9.0/tests/test_client.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     8972 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/tests/test_connection.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    14609 2024-03-19 13:40:54.000000 aiokatcp-1.9.0/tests/test_core.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    18492 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/tests/test_sensor.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)    39410 2024-04-05 13:20:00.000000 aiokatcp-1.9.0/tests/test_server.py
+-rw-rw-r--   0 bmerry    (1000) bmerry    (1000)     4586 2024-03-15 06:03:07.000000 aiokatcp-1.9.0/tests/test_time_sync.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiokatcp-1.8.0/.pre-commit-config.yaml` & `aiokatcp-1.9.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.4.1'
+    rev: 'v1.9.0'
     hooks:
       - id: mypy
         # Passing filenames to mypy can do odd things. See
         # https://github.com/pre-commit/mirrors-mypy/issues/33.
         # mypy.ini determines the set of files that will actually be checked.
         pass_filenames: false
         # The pre-commit hook passes some options, but we set options in mypy.ini.
```

### Comparing `aiokatcp-1.8.0/LICENSE.txt` & `aiokatcp-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/PKG-INFO` & `aiokatcp-1.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: aiokatcp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Asynchronous I/O implementation of the katcp protocol
 Home-page: https://github.com/ska-sa/aiokatcp
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: BSD
 Keywords: asyncio,katcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: async-timeout
+Requires-Dist: decorator>=4.1
+Requires-Dist: typing-extensions
 Provides-Extra: test
+Requires-Dist: async-solipsism; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: doc
-License-File: LICENSE.txt
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 
 aiokatcp
 ========
 
 .. image:: https://github.com/ska-sa/aiokatcp/actions/workflows/test.yml/badge.svg
    :target: https://github.com/ska-sa/aiokatcp/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/github/ska-sa/aiokatcp/badge.svg
    :target: https://coveralls.io/github/ska-sa/aiokatcp
 .. image:: https://readthedocs.org/projects/aiokatcp/badge/?version=latest
    :target: http://aiokatcp.readthedocs.io/en/latest/
 
 aiokatcp is an implementation of the `katcp`_ protocol based around the Python
-asyncio system module. It requires Python 3.7 or later. It is loosely inspired
+asyncio system module. It requires Python 3.8 or later. It is loosely inspired
 by the `Python 2 bindings`_, but has a much narrower scope.
 
 .. _katcp: https://katcp-python.readthedocs.io/en/latest/_downloads/361189acb383a294be20d6c10c257cb4/NRF-KAT7-6.0-IFCE-002-Rev5-1.pdf
 
 .. _Python 2 bindings: https://github.com/ska-sa/katcp-python
 
 The current implementation provides both client and server APIs. It only
```

### Comparing `aiokatcp-1.8.0/README.rst` & `aiokatcp-1.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
    :target: https://github.com/ska-sa/aiokatcp/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/github/ska-sa/aiokatcp/badge.svg
    :target: https://coveralls.io/github/ska-sa/aiokatcp
 .. image:: https://readthedocs.org/projects/aiokatcp/badge/?version=latest
    :target: http://aiokatcp.readthedocs.io/en/latest/
 
 aiokatcp is an implementation of the `katcp`_ protocol based around the Python
-asyncio system module. It requires Python 3.7 or later. It is loosely inspired
+asyncio system module. It requires Python 3.8 or later. It is loosely inspired
 by the `Python 2 bindings`_, but has a much narrower scope.
 
 .. _katcp: https://katcp-python.readthedocs.io/en/latest/_downloads/361189acb383a294be20d6c10c257cb4/NRF-KAT7-6.0-IFCE-002-Rev5-1.pdf
 
 .. _Python 2 bindings: https://github.com/ska-sa/katcp-python
 
 The current implementation provides both client and server APIs. It only
```

### Comparing `aiokatcp-1.8.0/doc/Makefile` & `aiokatcp-1.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/aiokatcp.rst` & `aiokatcp-1.9.0/doc/aiokatcp.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/changelog.rst` & `aiokatcp-1.9.0/doc/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+.. rubric:: Version 1.9.0
+
+- Drop support for end-of-life Python 3.7.
+- Significantly speed up argument decoding for request handlers. Note that any
+  code that calls :func:`.register_type` will need to be updated.
+- Add :meth:`.Client.sensor_reading` and :meth:`.Client.sensor_value` helper
+  methods.
+- Update dependency versions in Github Actions.
+
 .. rubric:: Version 1.8.0
 
 - Make :class:`.Reading` a dataclass.
 - Fix server shutdown on Python 3.12.
 - Update versions of dependencies used in CI.
 - Remove wheel from ``build-system.requires``.
 - Make the unit tests pass on Python 3.11.5.
```

### Comparing `aiokatcp-1.8.0/doc/client/reconnect.rst` & `aiokatcp-1.9.0/doc/client/reconnect.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/client/sensor_watcher.rst` & `aiokatcp-1.9.0/doc/client/sensor_watcher.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/client/tutorial.rst` & `aiokatcp-1.9.0/doc/client/tutorial.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/conf.py` & `aiokatcp-1.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/intro.rst` & `aiokatcp-1.9.0/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/migration.rst` & `aiokatcp-1.9.0/doc/migration.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/server/logging.rst` & `aiokatcp-1.9.0/doc/server/logging.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/server/service_tasks.rst` & `aiokatcp-1.9.0/doc/server/service_tasks.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/server/tutorial.rst` & `aiokatcp-1.9.0/doc/server/tutorial.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/doc/unicode.rst` & `aiokatcp-1.9.0/doc/unicode.rst`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/examples/example_client.py` & `aiokatcp-1.9.0/examples/example_client.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/examples/example_server.py` & `aiokatcp-1.9.0/examples/example_server.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/examples/mirror_sensors.py` & `aiokatcp-1.9.0/examples/mirror_sensors.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/requirements.txt` & `aiokatcp-1.9.0/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile requirements.in
 #
 async-solipsism==0.5
     # via -r requirements.in
 async-timeout==4.0.3
@@ -22,28 +22,22 @@
     # via -r requirements.in
 decorator==5.1.1
     # via -r requirements.in
 distlib==0.3.7
     # via virtualenv
 docopt==0.6.2
     # via coveralls
-exceptiongroup==1.1.3
+exceptiongroup==1.2.0
     # via pytest
 filelock==3.12.2
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==6.7.0
-    # via
-    #   pluggy
-    #   pre-commit
-    #   pytest
-    #   virtualenv
 iniconfig==2.0.0
     # via pytest
 nodeenv==1.8.0
     # via pre-commit
 packaging==23.1
     # via pytest
 platformdirs==3.10.0
@@ -69,22 +63,15 @@
 requests==2.31.0
     # via coveralls
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
 typing-extensions==4.7.1
-    # via
-    #   -r requirements.in
-    #   async-timeout
-    #   importlib-metadata
-    #   platformdirs
-    #   pytest-asyncio
-urllib3==2.0.4
+    # via -r requirements.in
+urllib3==2.0.7
     # via requests
 virtualenv==20.24.5
     # via pre-commit
-zipp==3.15.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `aiokatcp-1.8.0/setup.cfg` & `aiokatcp-1.9.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 package_dir = 
 	= src
 packages = find:
 install_requires = 
 	async-timeout
 	decorator>=4.1
 	typing-extensions
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False  # For py.typed
 
 [options.extras_require]
 test = 
 	async-solipsism
 	pytest
 	pytest-asyncio
```

### Comparing `aiokatcp-1.8.0/setup.py` & `aiokatcp-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/src/aiokatcp/__init__.py` & `aiokatcp-1.9.0/src/aiokatcp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
 # Automatically added by katversion
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 
 from .client import (  # noqa: F401
     AbstractSensorWatcher,
     Client,
     ProtocolError,
     SensorWatcher,
     SyncState,
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/adjtimex.py` & `aiokatcp-1.9.0/src/aiokatcp/adjtimex.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/src/aiokatcp/client.py` & `aiokatcp-1.9.0/src/aiokatcp/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017, 2019, 2022 National Research Foundation (SARAO)
+# Copyright 2017, 2019, 2022, 2024 National Research Foundation (SARAO)
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 # list of conditions and the following disclaimer.
 #
@@ -45,38 +45,41 @@
     Iterable,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
+    TypeVar,
     Union,
     cast,
+    overload,
 )
 
 from typing_extensions import Protocol
 
 from . import connection, core, sensor
 from .connection import FailReply, InvalidReply
 
 logger = logging.getLogger(__name__)
+_T = TypeVar("_T")
 
 
 class _Handler(Protocol):
     _aiokatcp_orig_handler: Callable[..., None]
 
 
 class _InformHandler(_Handler):
     def __call__(self, _client: "Client", _msg: core.Message) -> None:
-        ...
+        ...  # pragma: nocover
 
 
 class _InformCallback(_Handler):
     def __call__(self, _msg: core.Message) -> None:
-        ...
+        ...  # pragma: nocover
 
 
 class _PendingRequest:
     def __init__(self, name: str, mid: Optional[int], loop: asyncio.AbstractEventLoop) -> None:
         self.name = name
         self.mid = mid
         self.informs: List[core.Message] = []
@@ -217,15 +220,15 @@
             else:
                 if msg.mtype == core.Message.Type.REPLY:
                     if not req.reply.done():
                         req.reply.set_result(msg)
                 elif msg.mtype == core.Message.Type.INFORM:
                     req.informs.append(msg)
                 else:
-                    self.logger.warning("Unknown message type %s", msg.mtype)  # pragma: no cover
+                    self.logger.warning("Unknown message type %s", msg.mtype)  # pragma: nocover
         elif msg.mtype == core.Message.Type.INFORM:
             self.handle_inform(msg)
         else:
             self.logger.info(
                 "Received unexpected %s (%s) from server without message ID",
                 msg.mtype.name,
                 msg.name,
@@ -611,14 +614,96 @@
         if type_ == core.Message.OK:
             return reply_msg.arguments[1:], informs
         elif type_ == core.Message.FAIL:
             raise FailReply(error.decode("utf-8", errors="replace"))
         else:
             raise InvalidReply(error.decode("utf-8", errors="replace"))
 
+    @overload
+    async def sensor_reading(self, sensor_name: str, sensor_type: None = None) -> sensor.Reading:
+        ...  # pragma: nocover
+
+    @overload
+    async def sensor_reading(self, sensor_name: str, sensor_type: Type[_T]) -> sensor.Reading[_T]:
+        ...  # pragma: nocover
+
+    async def sensor_reading(
+        self, sensor_name: str, sensor_type: Optional[type] = None
+    ) -> sensor.Reading:
+        """Request the reading of a single sensor from the server.
+
+        This is a wrapper around a ``?sensor-value`` request that decodes the
+        result. If you know the type of the sensor, it can be passed as a
+        parameter; if it is not specified, ``?sensor-list`` is used to
+        determine it. Note that this introduces a race condition (but an
+        unlikely one) where the sensor could be replaced by one of a different
+        type between the two requests.
+
+        If `sensor_type` is not given and the sensor has a discrete type, the
+        returned reading will contain a byte string rather than an enum.
+        Similarly, string sensors are returned as byte strings, but
+        `sensor_type` can be passed as `str` to override this.
+
+        This is not a high-performance interface. If you need to sample a
+        large number of sensors, better performance can be obtained with
+        hand-coded implementations, such as by pipelining multiple requests.
+
+        Raises
+        ------
+        FailReply
+            If any of the requests fails e.g., because the sensor does not exist.
+        InvalidReply
+            If any of the requests is invalid. This generally indicates a bug, either
+            in this function or in the server.
+        """
+        if sensor_type is None:
+            list_resp, value_resp = await asyncio.gather(
+                asyncio.create_task(self.request("sensor-list", sensor_name)),
+                asyncio.create_task(self.request("sensor-value", sensor_name)),
+            )
+            type_name = core.decode(str, list_resp[1][0].arguments[3])
+            if type_name == "discrete":
+                sensor_type = bytes
+            else:
+                sensor_type = SensorWatcher.SENSOR_TYPES[type_name]
+        else:
+            value_resp = await self.request("sensor-value", sensor_name)
+        value_informs = value_resp[1]
+        if len(value_informs) != 1:
+            raise FailReply(f"Server returned {len(value_informs)} sensors, but only 1 expected")
+        value_inform = value_informs[0]
+        timestamp = float(core.decode(core.Timestamp, value_inform.arguments[0]))
+        status = core.decode(sensor.Sensor.Status, value_inform.arguments[3])
+        value = core.decode(sensor_type, value_inform.arguments[4])
+        return sensor.Reading(value=value, status=status, timestamp=timestamp)
+
+    @overload
+    async def sensor_value(self, sensor_name: str, sensor_type: None = None) -> Any:
+        ...  # pragma: nocover
+
+    @overload
+    async def sensor_value(self, sensor_name: str, sensor_type: Type[_T]) -> _T:
+        ...  # pragma: nocover
+
+    async def sensor_value(self, sensor_name: str, sensor_type: Optional[type] = None) -> Any:
+        """Request the value of a single sensor from the server.
+
+        See :meth:`sensor_reading` for more information. This is a thin
+        wrapper that just returns the value from the reading.
+
+        Raises
+        ------
+        ValueError
+            if the sensor status indicates that the value is invalid.
+        """
+        reading = await self.sensor_reading(sensor_name, sensor_type)
+        if not reading.status.valid_value():
+            raise ValueError(f"Reading for {sensor_name} has status {reading.status}")
+        return reading.value
+
     def add_sensor_watcher(self, watcher: "AbstractSensorWatcher") -> None:
         if self._sensor_monitor is None:
             self._sensor_monitor = _SensorMonitor(self)
         self._sensor_monitor.add_watcher(watcher)
 
     def remove_sensor_watcher(self, watcher: "AbstractSensorWatcher") -> None:
         if self._sensor_monitor is not None:
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/connection.py` & `aiokatcp-1.9.0/src/aiokatcp/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017, 2022 National Research Foundation (SARAO)
+# Copyright 2017, 2022, 2024 National Research Foundation (SARAO)
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 # list of conditions and the following disclaimer.
 #
@@ -28,15 +28,15 @@
 import asyncio
 import functools
 import inspect
 import ipaddress
 import logging
 import re
 import time
-from typing import Callable, Iterable, Optional, TypeVar
+from typing import Any, Callable, Iterable, Optional, TypeVar
 
 import decorator
 from typing_extensions import Protocol
 
 from . import core
 
 logger = logging.getLogger(__name__)
@@ -258,14 +258,22 @@
     This isn't as useless as it sounds: given a function with a
     ``__signature__`` attribute, it generates a wrapper that really
     does have that signature.
     """
     return func(*args, **kwargs)
 
 
+def _parameter_decoder(parameter: inspect.Parameter) -> Callable[[bytes], Any]:
+    """Get the decoder for a formal parameter."""
+    if parameter.annotation is inspect.Signature.empty:
+        return core.get_decoder(bytes)
+    else:
+        return core.get_decoder(parameter.annotation)
+
+
 def wrap_handler(name: str, handler: Callable, fixed: int) -> Callable:
     """Convert a handler that takes a sequence of typed arguments into one
     that takes a message.
 
     The message is unpacked to the types given by the signature. If it could
     not be unpacked, the wrapper raises :exc:`FailReply`.
 
@@ -291,32 +299,35 @@
         ):
             pos.append(parameter)
         if parameter.name == "_msg":
             raise ValueError("Parameter cannot be named _msg")
     if len(pos) < fixed:
         raise TypeError(f"Handler must accept at least {fixed} positional argument(s)")
 
+    pos_decoders = [_parameter_decoder(arg) for arg in pos[fixed:]]
+    if var_pos is not None:
+        var_pos_decoder = _parameter_decoder(var_pos)
+    else:
+        var_pos_decoder = None
+
     def transform_args(args) -> list:
         assert len(args) == fixed + 1
         msg = args[-1]
         args = list(args[:-1])
-        for argument in msg.arguments:
-            if len(args) >= len(pos):
-                if var_pos is None:
+        # This relies on zip stopping at the end of the shorter sequence
+        try:
+            for argument, decoder in zip(msg.arguments, pos_decoders):
+                args.append(decoder(argument))
+            if len(msg.arguments) > len(pos_decoders):
+                if var_pos_decoder is None:
                     raise FailReply(f"too many arguments for {name}")
-                else:
-                    hint = var_pos.annotation
-            else:
-                hint = pos[len(args)].annotation
-            if hint is inspect.Signature.empty:
-                hint = bytes
-            try:
-                args.append(core.decode(hint, argument))
-            except ValueError as error:
-                raise FailReply(str(error)) from error
+                for argument in msg.arguments[len(pos_decoders) :]:
+                    args.append(var_pos_decoder(argument))
+        except ValueError as error:
+            raise FailReply(str(error)) from error
         # Validate the arguments against sig. We could catch TypeError when
         # we invoke the function, but then we would also catch TypeErrors
         # raised from inside the implementation.
         try:
             sig.bind(*args)
         except TypeError as error:
             raise FailReply(str(error)) from error  # e.g. too few arguments
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/core.py` & `aiokatcp-1.9.0/src/aiokatcp/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017, 2022 National Research Foundation (SARAO)
+# Copyright 2017, 2022, 2024 National Research Foundation (SARAO)
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 # list of conditions and the following disclaimer.
 #
@@ -22,25 +22,40 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import enum
+import functools
 import io
 import ipaddress
 import logging
 import numbers
 import re
 import sys
-from typing import Any, Callable, Dict, Generic, List, Match, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generic,
+    List,
+    Match,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 _T = TypeVar("_T")
-_T_contra = TypeVar("_T_contra", contravariant=True)
 _E = TypeVar("_E", bound=enum.Enum)
+_F = TypeVar("_F", bound=numbers.Real)
+_I = TypeVar("_I", bound=numbers.Integral)
+_S = TypeVar("_S", bound=str)
 _IPAddress = Union[ipaddress.IPv4Address, ipaddress.IPv6Address]
 if sys.version_info >= (3, 10):
     # Union[A, B] and A | B have different classes, even though they behave similarly
     _UnionTypes = (type(Union[int, float]), type(int | float))
 else:
     _UnionTypes = (type(Union[int, float]),)
 
@@ -187,171 +202,155 @@
     """Discrete `device-status` readings."""
 
     OK = 1
     DEGRADED = 2
     FAIL = 3
 
 
-class TypeInfo(Generic[_T_contra]):
+class TypeInfo(Generic[_T]):
     """Type database entry. Refer to :func:`register_type` for details."""
 
     def __init__(
         self,
-        type_: Type[_T_contra],
+        type_: Type[_T],
         name: str,
-        encode: Callable[[_T_contra], bytes],
-        decode: Callable[[Type[_T_contra], bytes], _T_contra],
-        default: Callable[[Type[_T_contra]], _T_contra],
+        encode: Callable[[_T], bytes],
+        get_decoder: Callable[[Type[_T]], Callable[[bytes], _T]],
+        default: Callable[[Type[_T]], _T],
     ) -> None:
         self.type_ = type_
         self.name = name
         self.encode = encode
-        self.decode = decode
+        self.get_decoder = get_decoder
         self.default = default
 
+    # Just for backwards compatibility
+    def decode(self, cls: Type[_T], value: bytes) -> _T:
+        return self.get_decoder(cls)(value)
+
 
 _types: List[TypeInfo] = []
-_types_cache: Dict[type, TypeInfo] = {}  # Cache for get_type
 
 
 def register_type(
     type_: Type[_T],
     name: str,
     encode: Callable[[_T], bytes],
-    decode: Callable[[Type[_T], bytes], _T],
+    get_decoder: Callable[[Type[_T]], Callable[[bytes], _T]],
     default: Optional[Callable[[Type[_T]], _T]] = None,
 ) -> None:
     """Register a type for encoding and decoding in messages.
 
     The registration is also used for subclasses of `type_` if no more
     specific registration has been made. This is particularly used for the
     registration for :class:`enum.Enum`, which is used for all enum types.
 
     Parameters
     ----------
     type_
         Python class.
     encode
         Function to encode values of this type to bytes
-    decode
-        Function to decode values of this type from bytes. It is given the
-        actual derived class as the first argument.
+    get_decoder
+        Function to that takes the actual derived class and returns a decoder
+        that converts instances of :class:`bytes` to that class.
     default
         Function to generate a default value of this type (used by the sensor
         framework). It is given the actual derived class as the first argument.
     """
-    global _types_cache
     if default is None:
         default = _default_generic
     for info in _types:
         if info.type_ == type_:
             raise ValueError(f"{type_} is already registered")
-    _types_cache = {}
-    _types.append(TypeInfo(type_, name, encode, decode, default))
+    get_type.cache_clear()  # type: ignore
+    _get_decoder.cache_clear()  # type: ignore
+    _types.append(TypeInfo(type_, name, encode, get_decoder, default))
 
 
 def get_type(type_: Type[_T]) -> TypeInfo[_T]:
     """Retrieve the type information previously registered with :func:`register_type`.
 
     It returns the last type info registered that is a superclass of `type_` (according
     to ``issubclass``.
 
     Raises
     ------
     TypeError
         if none of the registrations match `type_`
     """
-    try:
-        return _types_cache[type_]
-    except KeyError:
-        for info in reversed(_types):
-            if issubclass(type_, info.type_):
-                _types_cache[type_] = info
-                return info
+    for info in reversed(_types):
+        if issubclass(type_, info.type_):
+            return info
     raise TypeError(f"{type_} is not registered")
 
 
-def _decode_bool(cls: type, raw: bytes) -> bool:
-    if raw == b"1":
-        return cls(True)
-    elif raw == b"0":
-        return cls(False)
-    else:
-        raise ValueError(f"boolean must be 0 or 1, not {raw!r}")
+def _get_decoder_bool(cls: type) -> Callable[[bytes], bool]:
+    def decode(raw: bytes) -> bool:
+        if raw == b"1":
+            return cls(True)
+        elif raw == b"0":
+            return cls(False)
+        else:
+            raise ValueError(f"boolean must be 0 or 1, not {raw!r}")
+
+    return decode
 
 
 def _encode_enum(value: enum.Enum) -> bytes:
     if hasattr(value, "katcp_value"):
         return getattr(value, "katcp_value")
     else:
         return value.name.encode("ascii").lower().replace(b"_", b"-")
 
 
-def _decode_enum(cls: Type[_E], raw: bytes) -> _E:
-    # ignore to work around https://github.com/python/mypy/issues/12553
-    if hasattr(next(iter(cls)), "katcp_value"):  # type: ignore
-        for member in cls:
-            if getattr(member, "katcp_value") == raw:
-                return member
-    else:
-        name = raw.upper().replace(b"-", b"_").decode("ascii")
+def _get_decoder_enum(cls: Type[_E]) -> Callable[[bytes], _E]:
+    lookup = {_encode_enum(member): member for member in cls}
+
+    def decode(raw: bytes) -> _E:
         try:
-            value = cls[name]
-            if raw == _encode_enum(value):
-                return cls[name]
+            return lookup[raw]
         except KeyError:
-            pass
-    raise ValueError(f"{raw!r} is not a valid value for {cls.__name__}")
+            raise ValueError(f"{raw!r} is not a valid value for {cls.__name__}") from None
+
+    return decode
 
 
 def _default_generic(cls: Type[_T]) -> _T:
     return cls()
 
 
 def _default_enum(cls: Type[_E]) -> _E:
-    # ignore to work around https://github.com/python/mypy/issues/12553
-    return next(iter(cls))  # type: ignore
+    return next(iter(cls))
 
 
-# mypy doesn't allow an abstract class to be passed to Type[], hence the
-# suppressions.
-register_type(
-    numbers.Real,  # type: ignore
-    "float",
-    lambda value: repr(float(value)).encode("ascii"),
-    lambda cls, raw: cls(float(raw.decode("ascii"))),  # type: ignore
-)
-register_type(
-    numbers.Integral,  # type: ignore
-    "integer",
-    lambda value: str(int(value)).encode("ascii"),
-    lambda cls, raw: cls(int(raw.decode("ascii"))),  # type: ignore
-)
-register_type(bool, "boolean", lambda value: b"1" if value else b"0", _decode_bool)
-register_type(bytes, "string", lambda value: value, lambda cls, raw: cls(raw))
-register_type(
-    str,
-    "string",
-    lambda value: value.encode("utf-8"),
-    lambda cls, raw: cls(raw, encoding="utf-8"),
-)
-register_type(
-    Address,
-    "address",
-    lambda value: bytes(value),
-    lambda cls, raw: cls.parse(raw),
-    lambda cls: cls(ipaddress.IPv4Address("0.0.0.0")),
-)
-register_type(
-    Timestamp,
-    "timestamp",
-    lambda value: repr(value).encode("ascii"),
-    lambda cls, raw: cls(raw.decode("ascii")),
-)
-register_type(enum.Enum, "discrete", _encode_enum, _decode_enum, _default_enum)
+def _get_decoder_float(cls: Type[_F]) -> Callable[[bytes], _F]:
+    if cls is float:
+        return cls
+    else:
+        # numbers.Real doesn't actually guarantee any way to construct it
+        # from a float; we just assume that any concrete class is likely to
+        # support this.
+        return lambda raw: cls(float(raw))  # type: ignore[call-arg]
+
+
+def _get_decoder_int(cls: Type[_T]) -> Callable[[bytes], _T]:
+    if cls is int:
+        return cls
+    else:
+        # As above, this isn't guaranteed to exist by the type system.
+        return lambda raw: cls(int(raw))  # type: ignore[call-arg]
+
+
+def _get_decoder_str(cls: Type[_S]) -> Callable[[bytes], _S]:
+    if cls is str:
+        # mypy doesn't resolve _S to str in this branch
+        return bytes.decode  # type: ignore[return-value]
+    else:
+        return lambda raw: cls(raw, encoding="utf-8")
 
 
 def encode(value: Any) -> bytes:
     """Encode a value to raw bytes for katcp.
 
     Parameters
     ----------
@@ -376,14 +375,60 @@
     Returns ``None`` if `cls` is not a specific :class:`typing.Union` type.
     """
     if not isinstance(cls, _UnionTypes):
         return None
     return cls.__args__  # type: ignore
 
 
+def get_decoder(cls: Type[_T]) -> Callable[[bytes], _T]:
+    """Get a decoder function.
+
+    See :func:`decode` for more details. This function is useful for
+    efficiency: the decoder for a class can be looked up once then used many
+    times.
+    """
+    union_args = _union_args(cls)
+    # Allows arguments like 'foo: Optional[str] = None' to exist, where None
+    # indicates that the argument was not passed at all. More generally, this
+    # allows Union[A, B, None] to behave like Union[A, B].
+    if union_args is not None:
+        union_args = tuple(arg for arg in union_args if arg is not type(None))  # noqa: E721
+        if len(union_args) == 1:  # Flatten Optional[T] to T
+            cls = union_args[0]
+            union_args = None
+    if union_args is not None:
+        sub_decoders = tuple(get_decoder(type_) for type_ in union_args)
+
+        def decoder(value: bytes) -> Any:
+            values: List[Any] = []
+            for sub_decoder in sub_decoders:
+                try:
+                    values.append(sub_decoder(value))
+                except ValueError:
+                    pass
+            if len(values) == 1:
+                return values[0]
+            elif not values:
+                raise ValueError(f"None of the types in {cls} could decode {value!r}")
+            else:
+                raise ValueError(f"{value!r} is ambiguous for {cls}")
+
+        return decoder
+    else:
+        return get_type(cls).get_decoder(cls)
+
+
+if not TYPE_CHECKING:
+    # This is hidden from type checking because otherwise mypy keeps
+    # complaining that Type is not Hashable.
+    get_type = functools.lru_cache(get_type)
+    get_decoder = functools.lru_cache(get_decoder)
+    _get_decoder = get_decoder  # Used in register_type to work around a shadowing issue
+
+
 def decode(cls: Any, value: bytes) -> Any:
     """Decode value in katcp message to a type.
 
     If a union type is provided, the value must decode successfully (i.e.,
     without raising :exc:`ValueError`) for exactly one of the types in the
     union, otherwise a :exc:`ValueError` is raised.
 
@@ -402,40 +447,15 @@
         if `cls` is not a registered type or union of registered
         types.
 
     See also
     --------
     :func:`register_type`
     """
-    union_args = _union_args(cls)
-    # Allows arguments like 'foo: Optional[str] = None' to exist, where None
-    # indicates that the argument was not passed at all. More generally, this
-    # allows Union[A, B, None] to behave like Union[A, B].
-    if union_args is not None:
-        union_args = tuple(arg for arg in union_args if arg is not type(None))  # noqa: E721
-        if len(union_args) == 1:  # Flatten Optional[T] to T
-            cls = union_args[0]
-            union_args = None
-    if union_args is not None:
-        values: List[Any] = []
-        for type_ in union_args:
-            if type_ is None:
-                pass
-            try:
-                values.append(decode(type_, value))
-            except ValueError:
-                pass
-        if len(values) == 1:
-            return values[0]
-        elif not values:
-            raise ValueError("None of the types in {} could decode {!r}".format(cls, value))
-        else:
-            raise ValueError(f"{value!r} is ambiguous for {cls}")
-    else:
-        return get_type(cls).decode(cls, value)
+    return get_decoder(cls)(value)
 
 
 class KatcpSyntaxError(ValueError):
     """Raised by parsers when encountering a syntax error."""
 
     def __init__(self, message: str, raw: Optional[bytes] = None) -> None:
         super().__init__(message)
@@ -635,7 +655,45 @@
     # __hash__ = None
 
     def reply_ok(self) -> bool:
         """Return True if this is a reply and its first argument is 'ok'."""
         return (
             self.mtype == self.Type.REPLY and bool(self.arguments) and self.arguments[0] == self.OK
         )
+
+
+# mypy doesn't allow an abstract class to be passed to Type[], hence the
+# suppressions.
+register_type(
+    numbers.Real,  # type: ignore
+    "float",
+    lambda value: repr(float(value)).encode("ascii"),
+    _get_decoder_float,
+)
+register_type(
+    numbers.Integral,  # type: ignore
+    "integer",
+    lambda value: str(int(value)).encode("ascii"),
+    _get_decoder_int,
+)
+register_type(bool, "boolean", lambda value: b"1" if value else b"0", _get_decoder_bool)
+register_type(bytes, "string", lambda value: value, lambda cls: cls)
+register_type(
+    str,
+    "string",
+    lambda value: value.encode("utf-8"),
+    _get_decoder_str,
+)
+register_type(
+    Address,
+    "address",
+    lambda value: bytes(value),
+    lambda cls: cls.parse,
+    lambda cls: cls(ipaddress.IPv4Address("0.0.0.0")),
+)
+register_type(
+    Timestamp,
+    "timestamp",
+    lambda value: repr(value).encode("ascii"),
+    lambda cls: cls,
+)
+register_type(enum.Enum, "discrete", _encode_enum, _get_decoder_enum, _default_enum)
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/sensor.py` & `aiokatcp-1.9.0/src/aiokatcp/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
         if self.sensor is not None:
             self.sensor.detach(self._receive_update)
             self.sensor = None
         self._observer = None
 
     @abc.abstractmethod
     def _parameters(self) -> tuple:
-        pass  # pragma: no cover
+        pass  # pragma: nocover
 
     def parameters(self) -> tuple:
         """Return the parameters with which the sensor was created."""
         if self.is_auto:
             return (SensorSampler.Strategy.AUTO,)
         else:
             return self._parameters()
@@ -454,17 +454,15 @@
                 if sensor.stype not in (int, float):
                     raise TypeError(
                         "differential strategies only valid for integer and float sensors"
                     )
                 types = list(types)
                 types[0] = sensor.stype
             if len(types) != len(args):
-                raise ValueError(
-                    "expected {} strategy arguments, found {}".format(len(types), len(args))
-                )
+                raise ValueError(f"expected {len(types)} strategy arguments, found {len(args)}")
             decoded_args = tuple(core.decode(type_, arg) for type_, arg in zip(types, args))
             is_auto = False
 
         if out_cls is None:
             return None
         else:
             return out_cls(sensor, observer, loop, *decoded_args, is_auto=is_auto)
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/server.py` & `aiokatcp-1.9.0/src/aiokatcp/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -473,19 +473,15 @@
         remove = False
         try:
             task.result()  # Evaluated just for side effects
             remove = True
         except asyncio.CancelledError:
             remove = True
         except BaseException as exc:
-            try:
-                name = f"task {task.get_name()!r}"  # type: ignore
-            except AttributeError:
-                # Python 3.7 does not have task names
-                name = "a task"
+            name = f"task {task.get_name()!r}"
             logger.warning("Halting the server because %s raised %s", name, exc, exc_info=True)
             self.halt()
         if remove:
             # No exception to report during shutdown, so clean it up
             try:
                 self._service_tasks.remove(task)
             except ValueError:  # Can happen during shutdown
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp/time_sync.py` & `aiokatcp-1.9.0/src/aiokatcp/time_sync.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/src/aiokatcp/tools/katcpcmd.py` & `aiokatcp-1.9.0/src/aiokatcp/tools/katcpcmd.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/src/aiokatcp.egg-info/PKG-INFO` & `aiokatcp-1.9.0/src/aiokatcp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 Metadata-Version: 2.1
 Name: aiokatcp
-Version: 1.8.0
+Version: 1.9.0
 Summary: Asynchronous I/O implementation of the katcp protocol
 Home-page: https://github.com/ska-sa/aiokatcp
 Author: Bruce Merry
 Author-email: bmerry@sarao.ac.za
 License: BSD
 Keywords: asyncio,katcp
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: AsyncIO
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: async-timeout
+Requires-Dist: decorator>=4.1
+Requires-Dist: typing-extensions
 Provides-Extra: test
+Requires-Dist: async-solipsism; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Requires-Dist: pytest-mock; extra == "test"
 Provides-Extra: doc
-License-File: LICENSE.txt
+Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: sphinx-rtd-theme; extra == "doc"
 
 aiokatcp
 ========
 
 .. image:: https://github.com/ska-sa/aiokatcp/actions/workflows/test.yml/badge.svg
    :target: https://github.com/ska-sa/aiokatcp/actions/workflows/test.yml
 .. image:: https://coveralls.io/repos/github/ska-sa/aiokatcp/badge.svg
    :target: https://coveralls.io/github/ska-sa/aiokatcp
 .. image:: https://readthedocs.org/projects/aiokatcp/badge/?version=latest
    :target: http://aiokatcp.readthedocs.io/en/latest/
 
 aiokatcp is an implementation of the `katcp`_ protocol based around the Python
-asyncio system module. It requires Python 3.7 or later. It is loosely inspired
+asyncio system module. It requires Python 3.8 or later. It is loosely inspired
 by the `Python 2 bindings`_, but has a much narrower scope.
 
 .. _katcp: https://katcp-python.readthedocs.io/en/latest/_downloads/361189acb383a294be20d6c10c257cb4/NRF-KAT7-6.0-IFCE-002-Rev5-1.pdf
 
 .. _Python 2 bindings: https://github.com/ska-sa/katcp-python
 
 The current implementation provides both client and server APIs. It only
```

### Comparing `aiokatcp-1.8.0/src/aiokatcp.egg-info/SOURCES.txt` & `aiokatcp-1.9.0/src/aiokatcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/tests/test_client.py` & `aiokatcp-1.9.0/tests/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2017, 2019-2020, 2022 National Research Foundation (SARAO)
+# Copyright 2017, 2019-2020, 2022, 2024 National Research Foundation (SARAO)
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 # list of conditions and the following disclaimer.
 #
@@ -37,14 +37,15 @@
 
 import async_solipsism
 import pytest
 
 from aiokatcp import (
     AbstractSensorWatcher,
     Client,
+    DeviceStatus,
     FailReply,
     InvalidReply,
     Message,
     ProtocolError,
     Reading,
     Sensor,
     SensorWatcher,
@@ -231,14 +232,90 @@
         [
             Message.inform("help", b"help", b"Show help", mid=1),
             Message.inform("help", b"halt", b"Halt", mid=1),
         ],
     )
 
 
+async def test_sensor_reading_explicit_type(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_reading("device-status", DeviceStatus))
+    assert await channel.reader.readline() == b"?sensor-value[1] device-status\n"
+    channel.writer.write(b"#sensor-value[1] 1234567890.1 1 device-status nominal ok\n")
+    channel.writer.write(b"!sensor-value[1] ok 1\n")
+    result = await future
+    assert result == Reading(1234567890.1, Sensor.Status.NOMINAL, DeviceStatus.OK)
+
+
+async def test_sensor_reading_int(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_reading("foo"))
+    assert await channel.reader.readline() == b"?sensor-list[1] foo\n"
+    channel.writer.write(b"#sensor-list[1] foo description\\_stuff unit integer\n")
+    channel.writer.write(b"!sensor-list[1] ok 1\n")
+    assert await channel.reader.readline() == b"?sensor-value[2] foo\n"
+    channel.writer.write(b"#sensor-value[2] 1234567890.1 1 device-status warn 7\n")
+    channel.writer.write(b"!sensor-value[2] ok 1\n")
+    result = await future
+    assert result == Reading(1234567890.1, Sensor.Status.WARN, 7)
+
+
+async def test_sensor_reading_discrete(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_reading("foo"))
+    assert await channel.reader.readline() == b"?sensor-list[1] foo\n"
+    channel.writer.write(b"#sensor-list[1] foo description\\_stuff unit discrete hello world\n")
+    channel.writer.write(b"!sensor-list[1] ok 1\n")
+    assert await channel.reader.readline() == b"?sensor-value[2] foo\n"
+    channel.writer.write(b"#sensor-value[2] 1234567890.1 1 device-status warn hello\n")
+    channel.writer.write(b"!sensor-value[2] ok 1\n")
+    result = await future
+    assert result == Reading(1234567890.1, Sensor.Status.WARN, b"hello")
+
+
+async def test_sensor_reading_missing(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_reading("foo", str))
+    assert await channel.reader.readline() == b"?sensor-value[1] foo\n"
+    channel.writer.write(b"!sensor-value[1] fail Unknown\\_sensor\\_'foo'\n")
+    with pytest.raises(FailReply):
+        await future
+
+
+async def test_sensor_reading_wrong_count(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_reading("/foo/", str))
+    assert await channel.reader.readline() == b"?sensor-value[1] /foo/\n"
+    channel.writer.write(b"#sensor-value[1] 1234567890.1 1 foo1 nominal ok\n")
+    channel.writer.write(b"#sensor-value[1] 1234567890.2 1 foo2 nominal ok\n")
+    channel.writer.write(b"!sensor-value[1] ok 2\n")
+    with pytest.raises(FailReply, match="Server returned 2 sensors, but only 1 expected"):
+        await future
+
+
+async def test_sensor_value_ok(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_value("foo", int))
+    assert await channel.reader.readline() == b"?sensor-value[1] foo\n"
+    channel.writer.write(b"#sensor-value[1] 1234567890.1 1 device-status warn 7\n")
+    channel.writer.write(b"!sensor-value[1] ok 1\n")
+    result = await future
+    assert result == 7
+
+
+async def test_sensor_value_invalid_status(channel, event_loop) -> None:
+    await channel.wait_connected()
+    future = event_loop.create_task(channel.client.sensor_value("foo", int))
+    assert await channel.reader.readline() == b"?sensor-value[1] foo\n"
+    channel.writer.write(b"#sensor-value[1] 1234567890.1 1 device-status unknown 7\n")
+    channel.writer.write(b"!sensor-value[1] ok 1\n")
+    with pytest.raises(ValueError):
+        await future
+
+
 async def test_inform(channel, caplog) -> None:
     client = cast(DummyClient, channel.client)
     await channel.wait_connected()
     with caplog.at_level(logging.INFO, "aiokatcp.client"):
         # Put in bad ones before the good one, so that as soon as we've
         # received the good one from the queue we can finish the test.
         channel.writer.write(b"#exception\n#foo bad notinteger\n#foo \xc3\xa9 123\n")
```

### Comparing `aiokatcp-1.8.0/tests/test_connection.py` & `aiokatcp-1.9.0/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/tests/test_core.py` & `aiokatcp-1.9.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,19 +182,23 @@
     @pytest.mark.parametrize("type_, value", BAD_VALUES)
     def test_bad_raw(self, type_, value) -> None:
         with pytest.raises(ValueError):
             decode(type_, value)
 
     def test_register_type(self, mocker) -> None:
         mocker.patch("aiokatcp.core._types", [])
+
+        def get_decoder(cls):
+            return lambda value: cls(json.loads(value.decode("utf-8")))
+
         register_type(
             dict,
             "string",
             lambda value: json.dumps(value, sort_keys=True).encode("utf-8"),
-            lambda cls, value: cls(json.loads(value.decode("utf-8"))),
+            get_decoder,
         )
         value = {"h": 1, "i": [2]}
         raw = b'{"h": 1, "i": [2]}'
         assert encode(value) == raw
         assert decode(dict, raw) == value
         with pytest.raises(ValueError):
             decode(dict, b'"string"')
@@ -202,15 +206,15 @@
             decode(dict, b"{missing_quotes: 1}")
         # Try re-registering for an already registered type
         with pytest.raises(ValueError):
             register_type(
                 dict,
                 "string",
                 lambda value: json.dumps(value, sort_keys=True).encode("utf-8"),
-                lambda cls, value: cls(json.loads(value.decode("utf-8"))),
+                get_decoder,
             )
 
     @pytest.mark.parametrize(
         "type_, default",
         [
             (int, 0),
             (float, 0.0),
```

### Comparing `aiokatcp-1.8.0/tests/test_sensor.py` & `aiokatcp-1.9.0/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `aiokatcp-1.8.0/tests/test_server.py` & `aiokatcp-1.9.0/tests/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,15 +487,15 @@
     writer.write(b"?bytes-arg raw\n")
     assert await reader.readline() == b"!bytes-arg ok raw\n"
 
 
 async def test_bad_arg_type(reader: asyncio.StreamReader, writer: asyncio.StreamWriter) -> None:
     writer.write(b"?double bad\n")
     line = await reader.readline()
-    assert line == rb"!double fail could\_not\_convert\_string\_to\_float:\_'bad'" + b"\n"
+    assert line == rb"!double fail could\_not\_convert\_string\_to\_float:\_b'bad'" + b"\n"
 
 
 async def test_concurrent(
     server: DummyServer, reader: asyncio.StreamReader, writer: asyncio.StreamWriter
 ) -> None:
     writer.write(b"?wait[1]\n?echo[2] test\n")
     assert await reader.readline() == b"!echo[2] ok test\n"
@@ -677,15 +677,15 @@
 
 
 async def test_sensor_sampling_bad_parameter(
     reader: asyncio.StreamReader, writer: asyncio.StreamWriter
 ) -> None:
     writer.write(b"?sensor-sampling float-sensor period foo\n")
     line = await reader.readline()
-    assert line == rb"!sensor-sampling fail could\_not\_convert\_string\_to\_float:\_'foo'" + b"\n"
+    assert line == rb"!sensor-sampling fail could\_not\_convert\_string\_to\_float:\_b'foo'" + b"\n"
 
 
 async def test_sensor_sampling_auto(
     mock_time,
     server: DummyServer,
     reader: asyncio.StreamReader,
     writer: asyncio.StreamWriter,
```

### Comparing `aiokatcp-1.8.0/tests/test_time_sync.py` & `aiokatcp-1.9.0/tests/test_time_sync.py`

 * *Files identical despite different names*

