# Comparing `tmp/haskellian-asyn-0.3.2.tar.gz` & `tmp/haskellian_asyn-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-asyn-0.3.2.tar", last modified: Wed Apr 10 07:07:08 2024, max compression
+gzip compressed data, was "haskellian_asyn-0.3.3.tar", last modified: Tue Apr 16 06:32:28 2024, max compression
```

## Comparing `haskellian-asyn-0.3.2.tar` & `haskellian_asyn-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.675880 haskellian-asyn-0.3.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 07:07:08.675880 haskellian-asyn-0.3.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian-asyn-0.3.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      512 2024-04-10 07:07:06.000000 haskellian-asyn-0.3.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-10 07:07:08.675880 haskellian-asyn-0.3.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.665880 haskellian-asyn-0.3.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.665880 haskellian-asyn-0.3.2/src/haskellian/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.665880 haskellian-asyn-0.3.2/src/haskellian/asyn/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       76 2024-04-10 06:58:33.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.675880 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      127 2024-04-10 06:58:19.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      392 2024-04-10 07:06:56.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-10 07:01:42.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/ops.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      499 2024-04-08 18:47:33.000000 haskellian-asyn-0.3.2/src/haskellian/asyn/promises/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-10 07:07:08.675880 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      289 2024-04-10 07:07:08.000000 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      465 2024-04-10 07:07:08.000000 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-10 07:07:08.000000 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        6 2024-04-10 07:07:08.000000 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-10 07:07:08.000000 haskellian-asyn-0.3.2/src/haskellian_asyn.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       51 2024-04-02 06:01:45.000000 haskellian_asyn-0.3.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      536 2024-04-16 06:32:26.000000 haskellian_asyn-0.3.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.687826 haskellian_asyn-0.3.3/src/haskellian/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/src/haskellian/asyn/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-04-15 17:14:16.000000 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      423 2024-04-15 16:31:06.000000 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      479 2024-04-08 18:47:33.000000 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      807 2024-04-16 06:32:11.000000 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/ops.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      732 2024-04-15 16:34:59.000000 haskellian_asyn-0.3.3/src/haskellian/asyn/promises/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-16 06:32:28.697829 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      325 2024-04-16 06:32:28.000000 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-16 06:32:28.000000 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-16 06:32:28.000000 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       27 2024-04-16 06:32:28.000000 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-16 06:32:28.000000 haskellian_asyn-0.3.3/src/haskellian_asyn.egg-info/top_level.txt
```

