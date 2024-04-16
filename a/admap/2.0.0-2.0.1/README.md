# Comparing `tmp/admap-2.0.0.tar.gz` & `tmp/admap-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admap-2.0.0.tar", last modified: Mon Apr 15 09:37:29 2024, max compression
+gzip compressed data, was "admap-2.0.1.tar", last modified: Tue Apr 16 08:24:49 2024, max compression
```

## Comparing `admap-2.0.0.tar` & `admap-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:37:29.014929 admap-2.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2024-04-15 09:37:29.014929 admap-2.0.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-15 09:37:29.014929 admap-2.0.0/admap.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      210 2024-04-15 09:37:28.000000 admap-2.0.0/admap.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-15 09:37:28.000000 admap-2.0.0/admap.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 09:37:28.000000 admap-2.0.0/admap.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-15 09:37:28.000000 admap-2.0.0/admap.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-15 09:37:28.000000 admap-2.0.0/admap.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-15 09:37:29.014929 admap-2.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      558 2024-04-15 09:31:32.000000 admap-2.0.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:24:49.827813 admap-2.0.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2024-04-16 08:24:49.827813 admap-2.0.1/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 08:24:49.827813 admap-2.0.1/admap.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 08:24:49.000000 admap-2.0.1/admap.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 08:24:49.827813 admap-2.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1202 2024-04-16 08:22:38.000000 admap-2.0.1/setup.py
```

