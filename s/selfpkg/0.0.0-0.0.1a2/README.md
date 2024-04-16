# Comparing `tmp/selfpkg-0.0.0.tar.gz` & `tmp/selfpkg-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfpkg-0.0.0.tar", last modified: Mon Apr 15 13:44:51 2024, max compression
+gzip compressed data, was "selfpkg-0.0.1a2.tar", last modified: Tue Apr 16 08:18:01 2024, max compression
```

## Comparing `selfpkg-0.0.0.tar` & `selfpkg-0.0.1a2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:44:51.323573 selfpkg-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 13:44:51.323573 selfpkg-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 13:44:47.000000 selfpkg-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 13:44:47.000000 selfpkg-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:44:51.323573 selfpkg-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:44:51.319573 selfpkg-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:44:51.319573 selfpkg-0.0.0/src/selfpkg/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 13:44:47.000000 selfpkg-0.0.0/src/selfpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 13:44:47.000000 selfpkg-0.0.0/src/selfpkg/greeting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:44:51.319573 selfpkg-0.0.0/src/selfpkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-15 13:44:51.000000 selfpkg-0.0.0/src/selfpkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-15 13:44:51.000000 selfpkg-0.0.0/src/selfpkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:44:51.000000 selfpkg-0.0.0/src/selfpkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 13:44:51.000000 selfpkg-0.0.0/src/selfpkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-16 08:17:50.000000 selfpkg-0.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-16 08:17:50.000000 selfpkg-0.0.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/src/selfpkg/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 08:17:50.000000 selfpkg-0.0.1a2/src/selfpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 08:17:50.000000 selfpkg-0.0.1a2/src/selfpkg/greeting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/src/selfpkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-16 08:18:01.000000 selfpkg-0.0.1a2/src/selfpkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 08:18:01.000000 selfpkg-0.0.1a2/src/selfpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:18:01.000000 selfpkg-0.0.1a2/src/selfpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 08:18:01.000000 selfpkg-0.0.1a2/src/selfpkg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:18:01.713527 selfpkg-0.0.1a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-16 08:17:50.000000 selfpkg-0.0.1a2/tests/test_greeting.py
```

