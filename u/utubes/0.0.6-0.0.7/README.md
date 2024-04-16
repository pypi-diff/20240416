# Comparing `tmp/utubes-0.0.6.tar.gz` & `tmp/utubes-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.6.tar", last modified: Tue Apr 16 14:09:51 2024, max compression
+gzip compressed data, was "utubes-0.0.7.tar", last modified: Tue Apr 16 15:15:14 2024, max compression
```

## Comparing `utubes-0.0.6.tar` & `utubes-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 14:09:46.000000 utubes-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 14:09:51.276024 utubes-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-16 14:09:46.000000 utubes-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.272024 utubes-0.0.6/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.272024 utubes-0.0.6/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 14:09:46.000000 utubes-0.0.6/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:09:51.276024 utubes-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 14:09:46.000000 utubes-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:09:51.276024 utubes-0.0.6/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 14:09:51.000000 utubes-0.0.6/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.382425 utubes-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 15:15:09.000000 utubes-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 15:15:14.382425 utubes-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-16 15:15:09.000000 utubes-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-16 15:15:09.000000 utubes-0.0.7/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:15:14.382425 utubes-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-16 15:15:09.000000 utubes-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:15:14.378425 utubes-0.0.7/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:15:14.000000 utubes-0.0.7/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.6/LICENSE` & `utubes-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.6/setup.py` & `utubes-0.0.7/setup.py`

 * *Files identical despite different names*

