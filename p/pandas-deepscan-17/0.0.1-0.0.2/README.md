# Comparing `tmp/pandas-deepscan-17-0.0.1.tar.gz` & `tmp/pandas-deepscan-17-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-deepscan-17-0.0.1.tar", last modified: Wed Apr 10 10:26:47 2024, max compression
+gzip compressed data, was "pandas-deepscan-17-0.0.2.tar", last modified: Tue Apr 16 13:21:25 2024, max compression
```

## Comparing `pandas-deepscan-17-0.0.1.tar` & `pandas-deepscan-17-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-10 10:26:47.011959 pandas-deepscan-17-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)      166 2024-04-10 10:26:47.011675 pandas-deepscan-17-0.0.1/PKG-INFO
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-10 10:26:47.011257 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      166 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      176 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-04-10 10:26:46.000000 pandas-deepscan-17-0.0.1/pandas_deepscan_17.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)       38 2024-04-10 10:26:47.012045 pandas-deepscan-17-0.0.1/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      205 2024-04-10 10:21:30.000000 pandas-deepscan-17-0.0.1/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-16 13:21:25.708278 pandas-deepscan-17-0.0.2/
+-rw-r--r--   0 user       (501) staff       (20)      166 2024-04-16 13:21:25.707957 pandas-deepscan-17-0.0.2/PKG-INFO
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-04-16 13:21:25.707499 pandas-deepscan-17-0.0.2/pandas_deepscan_17.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      166 2024-04-16 13:21:25.000000 pandas-deepscan-17-0.0.2/pandas_deepscan_17.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      176 2024-04-16 13:21:25.000000 pandas-deepscan-17-0.0.2/pandas_deepscan_17.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-16 13:21:25.000000 pandas-deepscan-17-0.0.2/pandas_deepscan_17.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-04-16 13:21:25.000000 pandas-deepscan-17-0.0.2/pandas_deepscan_17.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-04-16 13:21:25.708344 pandas-deepscan-17-0.0.2/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)     2705 2024-04-15 13:53:40.000000 pandas-deepscan-17-0.0.2/setup.py
```

