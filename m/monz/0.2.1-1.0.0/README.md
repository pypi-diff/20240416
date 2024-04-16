# Comparing `tmp/monz-0.2.1.tar.gz` & `tmp/monz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monz-0.2.1.tar", last modified: Fri Dec 30 16:56:57 2016, max compression
+gzip compressed data, was "monz-1.0.0.tar", last modified: Tue Apr 16 17:22:07 2024, max compression
```

## Comparing `monz-0.2.1.tar` & `monz-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,8 @@
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/bin/
--rwxr-xr-x   0 pawelad    (501) staff       (20)      390 2016-11-19 23:36:03.000000 monz-0.2.1/bin/monz
--rw-r--r--   0 pawelad    (501) staff       (20)     1082 2016-11-12 16:46:01.000000 monz-0.2.1/LICENSE
--rw-r--r--   0 pawelad    (501) staff       (20)      124 2016-11-19 23:26:47.000000 monz-0.2.1/MANIFEST.in
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/monz/
--rw-r--r--   0 pawelad    (501) staff       (20)       88 2016-12-30 16:56:19.000000 monz-0.2.1/monz/__init__.py
--rw-r--r--   0 pawelad    (501) staff       (20)     4501 2016-12-30 16:56:12.000000 monz-0.2.1/monz/command_line.py
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/monz/test/
--rw-r--r--   0 pawelad    (501) staff       (20)     2116 2016-12-30 16:56:12.000000 monz-0.2.1/monz/test/test_command_line.py
--rw-r--r--   0 pawelad    (501) staff       (20)      419 2016-11-19 23:33:48.000000 monz-0.2.1/monz/test/test_utils.py
--rw-r--r--   0 pawelad    (501) staff       (20)      460 2016-11-19 23:36:03.000000 monz-0.2.1/monz/utils.py
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/
--rw-r--r--   0 pawelad    (501) staff       (20)        1 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/dependency_links.txt
--rw-r--r--   0 pawelad    (501) staff       (20)     6360 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/PKG-INFO
--rw-r--r--   0 pawelad    (501) staff       (20)       82 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/requires.txt
--rw-r--r--   0 pawelad    (501) staff       (20)      363 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/SOURCES.txt
--rw-r--r--   0 pawelad    (501) staff       (20)        5 2016-12-30 16:56:57.000000 monz-0.2.1/monz.egg-info/top_level.txt
--rw-r--r--   0 pawelad    (501) staff       (20)     6360 2016-12-30 16:56:57.000000 monz-0.2.1/PKG-INFO
--rw-r--r--   0 pawelad    (501) staff       (20)     3974 2016-12-30 16:56:12.000000 monz-0.2.1/README.md
-drwxr-xr-x   0 pawelad    (501) staff       (20)        0 2016-12-30 16:56:57.000000 monz-0.2.1/requirements/
--rw-r--r--   0 pawelad    (501) staff       (20)       64 2016-12-30 16:56:12.000000 monz-0.2.1/requirements/common.txt
--rw-r--r--   0 pawelad    (501) staff       (20)      135 2016-12-28 16:59:09.000000 monz-0.2.1/requirements/dev.txt
--rw-r--r--   0 pawelad    (501) staff       (20)       27 2016-11-12 16:45:17.000000 monz-0.2.1/requirements.txt
--rw-r--r--   0 pawelad    (501) staff       (20)       59 2016-12-30 16:56:57.000000 monz-0.2.1/setup.cfg
--rw-r--r--   0 pawelad    (501) staff       (20)     2508 2016-12-30 16:56:34.000000 monz-0.2.1/setup.py
--rw-r--r--   0 pawelad    (501) staff       (20)      379 2016-12-28 17:00:51.000000 monz-0.2.1/tox.ini
+-rw-r--r--   0        0        0    16725 2024-04-16 17:22:07.000000 monz-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4463 2024-04-16 17:22:07.000000 monz-1.0.0/README.md
+-rw-r--r--   0        0        0     3528 2024-04-16 17:22:07.000000 monz-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      270 2024-04-16 17:22:07.000000 monz-1.0.0/src/monz/__init__.py
+-rw-r--r--   0        0        0      326 2024-04-16 17:22:07.000000 monz-1.0.0/src/monz/__main__.py
+-rw-r--r--   0        0        0     7000 2024-04-16 17:22:07.000000 monz-1.0.0/src/monz/command_line.py
+-rw-r--r--   0        0        0      209 2024-04-16 17:22:07.000000 monz-1.0.0/src/monz/utils.py
+-rw-r--r--   0        0        0     6675 1970-01-01 00:00:00.000000 monz-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

