# Comparing `tmp/sinnia_shared-0.2.1.tar.gz` & `tmp/sinnia_shared-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinnia_shared-0.2.1.tar", last modified: Tue May 24 01:25:46 2022, max compression
+gzip compressed data, was "sinnia_shared-0.3.0.tar", max compression
```

## Comparing `sinnia_shared-0.2.1.tar` & `sinnia_shared-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,8 @@
-drwxr-xr-x   0 sonia      (501) staff       (20)        0 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/
--rw-r--r--   0 sonia      (501) staff       (20)      792 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/PKG-INFO
--rw-r--r--   0 sonia      (501) staff       (20)      550 2022-05-24 00:06:17.000000 sinnia_shared-0.2.1/README.md
--rw-r--r--   0 sonia      (501) staff       (20)       38 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/setup.cfg
--rw-r--r--   0 sonia      (501) staff       (20)      557 2022-05-24 00:06:44.000000 sinnia_shared-0.2.1/setup.py
-drwxr-xr-x   0 sonia      (501) staff       (20)        0 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/shared/
--rw-r--r--   0 sonia      (501) staff       (20)        0 2020-06-24 17:14:39.000000 sinnia_shared-0.2.1/shared/__init__.py
--rw-r--r--   0 sonia      (501) staff       (20)     7746 2022-02-05 01:29:09.000000 sinnia_shared-0.2.1/shared/amqp.py
--rw-r--r--   0 sonia      (501) staff       (20)     2975 2020-06-24 17:14:41.000000 sinnia_shared-0.2.1/shared/timezones.py
--rw-r--r--   0 sonia      (501) staff       (20)     5978 2020-06-24 17:14:41.000000 sinnia_shared-0.2.1/shared/utils.py
-drwxr-xr-x   0 sonia      (501) staff       (20)        0 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/
--rw-r--r--   0 sonia      (501) staff       (20)      792 2022-05-24 01:25:45.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/PKG-INFO
--rw-r--r--   0 sonia      (501) staff       (20)      308 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/SOURCES.txt
--rw-r--r--   0 sonia      (501) staff       (20)        1 2022-05-24 01:25:45.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/dependency_links.txt
--rw-r--r--   0 sonia      (501) staff       (20)        1 2019-11-06 00:45:40.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/not-zip-safe
--rw-r--r--   0 sonia      (501) staff       (20)       15 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/requires.txt
--rw-r--r--   0 sonia      (501) staff       (20)        7 2022-05-24 01:25:46.000000 sinnia_shared-0.2.1/sinnia_shared.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1200 2024-04-16 01:36:15.640196 sinnia_shared-0.3.0/README.md
+-rw-r--r--   0        0        0      360 2024-04-16 00:39:49.423317 sinnia_shared-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:19:29.862856 sinnia_shared-0.3.0/sinnia_shared/__init__.py
+-rw-r--r--   0        0        0     7746 2023-07-14 23:19:29.862856 sinnia_shared-0.3.0/sinnia_shared/amqp.py
+-rw-r--r--   0        0        0     4599 2024-04-16 01:36:15.640196 sinnia_shared-0.3.0/sinnia_shared/string_utils.py
+-rw-r--r--   0        0        0     2975 2023-07-14 23:19:29.862856 sinnia_shared-0.3.0/sinnia_shared/timezones.py
+-rw-r--r--   0        0        0    10059 2024-04-16 01:36:15.640196 sinnia_shared-0.3.0/sinnia_shared/utils.py
+-rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 sinnia_shared-0.3.0/PKG-INFO
```

### Comparing `sinnia_shared-0.2.1/shared/amqp.py` & `sinnia_shared-0.3.0/sinnia_shared/amqp.py`

 * *Files identical despite different names*

### Comparing `sinnia_shared-0.2.1/shared/timezones.py` & `sinnia_shared-0.3.0/sinnia_shared/timezones.py`

 * *Files identical despite different names*

