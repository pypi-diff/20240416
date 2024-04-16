# Comparing `tmp/admap-2.0.1.tar.gz` & `tmp/admap-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admap-2.0.1.tar", last modified: Tue Apr 16 08:24:49 2024, max compression
+gzip compressed data, from Unix
```

## Comparing `admap-2.0.1.tar` & `admap-2.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:24:49.827813 admap-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2024-04-16 08:24:49.827813 admap-2.0.1/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:24:49.827813 admap-2.0.1/admap.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 08:24:49.827813 admap-2.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2024-04-16 08:22:38.000000 admap-2.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 09:57:10.000000 admap-2.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-04-16 09:53:17.000000 admap-2.0.2/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 09:53:28.000000 admap-2.0.2/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 09:53:28.000000 admap-2.0.2/admap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      582 2024-04-16 09:57:06.000000 admap-2.0.2/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 09:53:28.000000 admap-2.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2024-04-16 09:57:10.000000 admap-2.0.2/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

