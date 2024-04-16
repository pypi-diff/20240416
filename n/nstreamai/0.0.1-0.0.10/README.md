# Comparing `tmp/nstreamai-0.0.1.tar.gz` & `tmp/nstreamai-0.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nstreamai-0.0.1.tar", last modified: Sat Apr  6 20:05:26 2024, max compression
+gzip compressed data, was "nstreamai-0.0.10.tar", last modified: Tue Apr 16 17:54:23 2024, max compression
```

## Comparing `nstreamai-0.0.1.tar` & `nstreamai-0.0.10.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.644241 nstreamai-0.0.1/
--rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-06 19:47:11.000000 nstreamai-0.0.1/LICENSE
--rw-r--r--   0 shiv       (501) staff       (20)      550 2024-04-06 20:05:26.644011 nstreamai-0.0.1/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)       15 2024-04-06 19:47:11.000000 nstreamai-0.0.1/README.md
--rw-r--r--   0 shiv       (501) staff       (20)      608 2024-04-06 20:05:22.000000 nstreamai-0.0.1/pyproject.toml
--rw-r--r--   0 shiv       (501) staff       (20)       38 2024-04-06 20:05:26.644319 nstreamai-0.0.1/setup.cfg
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.642208 nstreamai-0.0.1/src/
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.643788 nstreamai-0.0.1/src/nstreamai.egg-info/
--rw-r--r--   0 shiv       (501) staff       (20)      550 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/PKG-INFO
--rw-r--r--   0 shiv       (501) staff       (20)      250 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/SOURCES.txt
--rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/dependency_links.txt
--rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-06 20:05:26.000000 nstreamai-0.0.1/src/nstreamai.egg-info/top_level.txt
-drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-06 20:05:26.643415 nstreamai-0.0.1/src/nstreamai_nstream_ai/
--rw-r--r--   0 shiv       (501) staff       (20)      257 2024-04-06 20:04:29.000000 nstreamai-0.0.1/src/nstreamai_nstream_ai/__init__.py
--rw-r--r--   0 shiv       (501) staff       (20)     3105 2024-04-06 20:03:26.000000 nstreamai-0.0.1/src/nstreamai_nstream_ai/main.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.045680 nstreamai-0.0.10/
+-rw-r--r--   0 shiv       (501) staff       (20)    35149 2024-04-16 12:23:16.000000 nstreamai-0.0.10/LICENSE
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-16 17:54:23.045478 nstreamai-0.0.10/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)    15429 2024-04-16 15:45:18.000000 nstreamai-0.0.10/README.md
+-rw-r--r--   0 shiv       (501) staff       (20)      229 2024-04-16 17:49:31.000000 nstreamai-0.0.10/pyproject.toml
+-rw-r--r--   0 shiv       (501) staff       (20)       74 2024-04-16 17:54:23.045918 nstreamai-0.0.10/setup.cfg
+-rw-r--r--   0 shiv       (501) staff       (20)     2063 2024-04-16 17:54:18.000000 nstreamai-0.0.10/setup.py
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.042963 nstreamai-0.0.10/src/
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.045159 nstreamai-0.0.10/src/nstreamai.egg-info/
+-rw-r--r--   0 shiv       (501) staff       (20)    16606 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/PKG-INFO
+-rw-r--r--   0 shiv       (501) staff       (20)      272 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/SOURCES.txt
+-rw-r--r--   0 shiv       (501) staff       (20)        1 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/dependency_links.txt
+-rw-r--r--   0 shiv       (501) staff       (20)      340 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/requires.txt
+-rw-r--r--   0 shiv       (501) staff       (20)       21 2024-04-16 17:54:23.000000 nstreamai-0.0.10/src/nstreamai.egg-info/top_level.txt
+drwxr-xr-x   0 shiv       (501) staff       (20)        0 2024-04-16 17:54:23.044979 nstreamai-0.0.10/src/nstreamai_nstream_ai/
+-rw-r--r--   0 shiv       (501) staff       (20)        0 2024-04-16 17:04:20.000000 nstreamai-0.0.10/src/nstreamai_nstream_ai/__init__.py
```

### Comparing `nstreamai-0.0.1/LICENSE` & `nstreamai-0.0.10/LICENSE`

 * *Files identical despite different names*

