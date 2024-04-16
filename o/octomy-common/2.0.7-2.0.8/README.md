# Comparing `tmp/octomy-common-2.0.7.tar.gz` & `tmp/octomy-common-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-common-2.0.7.tar", last modified: Sun Apr 14 10:06:51 2024, max compression
+gzip compressed data, was "octomy-common-2.0.8.tar", last modified: Tue Apr 16 11:31:00 2024, max compression
```

## Comparing `octomy-common-2.0.7.tar` & `octomy-common-2.0.8.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.124287 octomy-common-2.0.7/
--rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.7/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.7/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.7/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.7/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-14 10:06:51.124287 octomy-common-2.0.7/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.7/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-14 10:06:02.000000 octomy-common-2.0.7/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/code_quality/
--rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.7/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.7/code_quality/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.7/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.7/code_quality/pylintrc
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/design/
--rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.7/design/logo-1024.png
--rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.7/design/logo-1024.svg
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.108287 octomy-common-2.0.7/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/access/
--rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.7/octomy/access/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/cad/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/cad/generators/
--rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.7/octomy/cad/generators/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.7/octomy/cad/generators/common.py
--rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.7/octomy/cad/generators/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.7/octomy/cad/generators/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.7/octomy/cad/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.7/octomy/cad/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.7/octomy/cad/parts.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/cad/types/
--rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.7/octomy/cad/types/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/config/
--rw-r--r--   0 leo       (1000) leo       (1000)    13353 2024-04-14 09:41:27.000000 octomy-common-2.0.7/octomy/config/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/db/
--rw-rw-r--   0 leo       (1000) leo       (1000)    17970 2024-04-14 10:03:37.000000 octomy-common-2.0.7/octomy/db/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.7/octomy/db/check.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/log/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.7/octomy/log/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.112287 octomy-common-2.0.7/octomy/storage/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.7/octomy/storage/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.7/octomy/storage/google_drive.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.116287 octomy-common-2.0.7/octomy/utils/
--rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.7/octomy/utils/Context.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.7/octomy/utils/Profiler.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.7/octomy/utils/Svg.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.7/octomy/utils/Watchdog.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.7/octomy/utils/WorkerPool.py
--rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.7/octomy/utils/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.7/octomy/utils/click.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.7/octomy/utils/credentials.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.7/octomy/utils/csv_to_db.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.7/octomy/utils/debug_view.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.7/octomy/utils/excavator.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.7/octomy/utils/expiry_cache.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.116287 octomy-common-2.0.7/octomy/version/
--rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.7/octomy/version/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.116287 octomy-common-2.0.7/octomy/web/
--rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.7/octomy/web/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.7/octomy/web/autoroute.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.116287 octomy-common-2.0.7/octomy/web/context/
--rw-r--r--   0 leo       (1000) leo       (1000)     2769 2024-04-14 09:54:39.000000 octomy-common-2.0.7/octomy/web/context/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.116287 octomy-common-2.0.7/octomy/web/search/
--rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.7/octomy/web/search/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/octomy_common.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-14 10:06:50.000000 octomy-common-2.0.7/octomy_common.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-14 10:06:51.000000 octomy-common-2.0.7/octomy_common.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-14 10:06:50.000000 octomy-common-2.0.7/octomy_common.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-14 10:06:50.000000 octomy-common-2.0.7/octomy_common.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-14 10:06:50.000000 octomy-common-2.0.7/octomy_common.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-14 10:06:50.000000 octomy-common-2.0.7/octomy_common.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.7/octomy_common.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.7/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.7/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.7/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.7/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-14 10:06:51.124287 octomy-common-2.0.7/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.7/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/tests/
--rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.7/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.7/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.120287 octomy-common-2.0.7/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.7/tests/integration/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.7/tests/integration/test_true.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.124287 octomy-common-2.0.7/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.7/tests/load/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.7/tests/load/test_true.py
--rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.7/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-14 10:06:51.124287 octomy-common-2.0.7/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.7/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1332 2024-04-14 10:04:39.000000 octomy-common-2.0.7/tests/unit/test_util.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.359543 octomy-common-2.0.8/
+-rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.8/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.8/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.8/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.8/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-16 11:31:00.359543 octomy-common-2.0.8/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.8/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-16 11:30:26.000000 octomy-common-2.0.8/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/code_quality/
+-rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.8/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.8/code_quality/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.8/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.8/code_quality/pylintrc
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/design/
+-rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.8/design/logo-1024.png
+-rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.8/design/logo-1024.svg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.343543 octomy-common-2.0.8/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/access/
+-rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.8/octomy/access/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/generators/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.8/octomy/cad/generators/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.8/octomy/cad/generators/common.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.8/octomy/cad/generators/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.8/octomy/cad/generators/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.8/octomy/cad/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.8/octomy/cad/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.8/octomy/cad/parts.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/cad/types/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.8/octomy/cad/types/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/config/
+-rw-r--r--   0 leo       (1000) leo       (1000)    13353 2024-04-14 09:41:27.000000 octomy-common-2.0.8/octomy/config/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/db/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    18290 2024-04-16 11:27:50.000000 octomy-common-2.0.8/octomy/db/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.8/octomy/db/check.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/log/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.8/octomy/log/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.347543 octomy-common-2.0.8/octomy/storage/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.8/octomy/storage/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.8/octomy/storage/google_drive.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/utils/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.8/octomy/utils/Context.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.8/octomy/utils/Profiler.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.8/octomy/utils/Svg.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.8/octomy/utils/Watchdog.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.8/octomy/utils/WorkerPool.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.8/octomy/utils/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.8/octomy/utils/click.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.8/octomy/utils/credentials.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.8/octomy/utils/csv_to_db.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.8/octomy/utils/debug_view.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.8/octomy/utils/excavator.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.8/octomy/utils/expiry_cache.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/version/
+-rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.8/octomy/version/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.8/octomy/web/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.8/octomy/web/autoroute.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/context/
+-rw-r--r--   0 leo       (1000) leo       (1000)     2769 2024-04-14 09:54:39.000000 octomy-common-2.0.8/octomy/web/context/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.351543 octomy-common-2.0.8/octomy/web/search/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.8/octomy/web/search/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/octomy_common.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-16 11:31:00.000000 octomy-common-2.0.8/octomy_common.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.8/octomy_common.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.8/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.8/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.8/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.8/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-16 11:31:00.359543 octomy-common-2.0.8/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.8/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/
+-rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/integration/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/integration/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.355543 octomy-common-2.0.8/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/load/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.8/tests/load/test_true.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.8/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-16 11:31:00.359543 octomy-common-2.0.8/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.8/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1332 2024-04-14 10:04:39.000000 octomy-common-2.0.8/tests/unit/test_util.py
```

### Comparing `octomy-common-2.0.7/.gitignore` & `octomy-common-2.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/.gitlab/ci.yaml` & `octomy-common-2.0.8/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/LICENSE` & `octomy-common-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/PKG-INFO` & `octomy-common-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.7
+Version: 2.0.8
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.7/README.md` & `octomy-common-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/code_quality/Makefile` & `octomy-common-2.0.8/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/code_quality/pylintrc` & `octomy-common-2.0.8/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/design/logo-1024.png` & `octomy-common-2.0.8/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/design/logo-1024.svg` & `octomy-common-2.0.8/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/access/__init__.py` & `octomy-common-2.0.8/octomy/access/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/generators/__init__.py` & `octomy-common-2.0.8/octomy/cad/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/generators/openscad.py` & `octomy-common-2.0.8/octomy/cad/generators/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/ntop.py` & `octomy-common-2.0.8/octomy/cad/ntop.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/openscad.py` & `octomy-common-2.0.8/octomy/cad/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/parts.py` & `octomy-common-2.0.8/octomy/cad/parts.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/cad/types/__init__.py` & `octomy-common-2.0.8/octomy/cad/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/config/__init__.py` & `octomy-common-2.0.8/octomy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/db/__init__.py` & `octomy-common-2.0.8/octomy/db/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,16 @@
 	def reset_queries(self):
 		"""Reset the internal cache of queries, forcing queries to be reloaded upon next invocation"""
 		self.queries = dict()
 
 	def preload_queries(self, do_debug = False):
 		"""Recursively load and register queries from .sql files in given path."""
 		self.reset_queries()
+		if do_debug:
+			logger.info("Scanning query dirs:")
 		for dir in self.query_dirs:
 			if not os.path.isdir(dir):
 				if do_debug:
 					logger.warning(f"Not a dir, skipping: '{dir}'")
 					logger.warning(f" * NOTE: CWD is '{os.getcwd()}'")
 				continue
 			if do_debug:
@@ -313,17 +315,22 @@
 				# some/path/file.sql --> some.path.file
 				if do_debug:
 					logger.info(f" |-Found candidate file: '{sql_file}'")
 				query_key = sql_file.relative_to(dir).with_suffix('').as_posix().replace('/', '.')
 				with open(sql_file, 'r', encoding='utf-8') as file:
 					query = file.read()
 					if do_debug:
-						logger.info(f" | |-Loading '{query_key}' from '{sql_file}' with '{query}'")
+						#logger.info(f" | |-Loading '{query_key}' from '{sql_file}' with '{query}'")
+						logger.info(f" | |-Loading '{query_key}' from '{sql_file}' with query size {len(query)} chars")
 					self.queries[query_key] = query
 
+		if do_debug:
+			logger.info("Scanning complete")
+
+
 	def register_query_dir(self, path, do_preload = False, do_debug = False):
 		"""Recursively load queries from .sql files in given path."""
 		real = os.path.realpath(path)
 		if do_debug:
 			logger.info(f"Adding query dir: '{path}' ({real})")
 		self.query_dirs.add(pathlib.Path(real))
 		if do_preload:
@@ -484,18 +491,20 @@
 	async def query_exists(self, query_key, params=dict(), prepare=True, do_debug=False):
 		if do_debug:
 			logger.info(f"query_exists params='{pprint.pformat(params)}' prepare={prepare}")
 		return await self.key_query(query_key = query_key, params = params, mode = "exists", prepare=prepare, do_debug=do_debug)
 
 
 #@lru_cache
-def get_database(config:dict, do_verify=True, do_online = True):
+def get_database(config:dict, do_verify=True, do_online = True, do_debug = True):
 	uri, err = db_uri_from_conf(config = config, do_verify = do_verify, do_online = do_online, do_redact = False)
 	if not uri:
 		logger.warning(f"db uri error: {err}")
 		return None, err
 	db = Database(db_uri = uri)
 	sql_dir = config.get("db-sql-dir")
 	if sql_dir:
-		db.register_query_dir(sql_dir)
+		if do_debug:
+			logger.info(f"Adding sql dir from config: {sql_dir}")
+		db.register_query_dir(sql_dir, do_debug = do_debug)
 	return db, None
```

### Comparing `octomy-common-2.0.7/octomy/db/check.py` & `octomy-common-2.0.8/octomy/db/check.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/log/__init__.py` & `octomy-common-2.0.8/octomy/log/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/storage/google_drive.py` & `octomy-common-2.0.8/octomy/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/Profiler.py` & `octomy-common-2.0.8/octomy/utils/Profiler.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/Svg.py` & `octomy-common-2.0.8/octomy/utils/Svg.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/Watchdog.py` & `octomy-common-2.0.8/octomy/utils/Watchdog.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/WorkerPool.py` & `octomy-common-2.0.8/octomy/utils/WorkerPool.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/__init__.py` & `octomy-common-2.0.8/octomy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/click.py` & `octomy-common-2.0.8/octomy/utils/click.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/credentials.py` & `octomy-common-2.0.8/octomy/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/csv_to_db.py` & `octomy-common-2.0.8/octomy/utils/csv_to_db.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/debug_view.py` & `octomy-common-2.0.8/octomy/utils/debug_view.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/excavator.py` & `octomy-common-2.0.8/octomy/utils/excavator.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/utils/expiry_cache.py` & `octomy-common-2.0.8/octomy/utils/expiry_cache.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/web/__init__.py` & `octomy-common-2.0.8/octomy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/web/autoroute.py` & `octomy-common-2.0.8/octomy/web/autoroute.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/web/context/__init__.py` & `octomy-common-2.0.8/octomy/web/context/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy/web/search/__init__.py` & `octomy-common-2.0.8/octomy/web/search/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/octomy_common.egg-info/PKG-INFO` & `octomy-common-2.0.8/octomy_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.7
+Version: 2.0.8
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
```

### Comparing `octomy-common-2.0.7/octomy_common.egg-info/SOURCES.txt` & `octomy-common-2.0.8/octomy_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/requirements/requirements.txt` & `octomy-common-2.0.8/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/requirements/test_requirements.txt` & `octomy-common-2.0.8/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/setup.py` & `octomy-common-2.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/tests/Makefile` & `octomy-common-2.0.8/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.7/tests/unit/test_util.py` & `octomy-common-2.0.8/tests/unit/test_util.py`

 * *Files identical despite different names*

