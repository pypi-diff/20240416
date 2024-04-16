# Comparing `tmp/api_pipe-1.0.61.tar.gz` & `tmp/api_pipe-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_pipe-1.0.61.tar", max compression
+gzip compressed data, was "api_pipe-1.0.7.tar", max compression
```

## Comparing `api_pipe-1.0.61.tar` & `api_pipe-1.0.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       11 2024-01-06 08:05:02.508433 api_pipe-1.0.61/README.md
--rw-r--r--   0        0        0      540 2024-04-16 01:40:23.412154 api_pipe-1.0.61/pyproject.toml
--rw-r--r--   0        0        0       44 2024-04-16 01:40:29.274929 api_pipe-1.0.61/src/api_pipe/__init__.py
--rw-r--r--   0        0        0    14994 2024-04-16 01:39:44.914685 api_pipe-1.0.61/src/api_pipe/api.py
--rw-r--r--   0        0        0      639 2024-02-04 09:34:12.409908 api_pipe-1.0.61/src/api_pipe/config.py
--rw-r--r--   0        0        0     1406 2024-02-11 06:37:54.364782 api_pipe-1.0.61/src/api_pipe/logger.py
--rw-r--r--   0        0        0     2791 2024-02-04 09:35:27.012476 api_pipe-1.0.61/src/api_pipe/manual_test_run.py
--rw-r--r--   0        0        0      721 2024-01-06 10:44:07.416343 api_pipe-1.0.61/src/api_pipe/url.py
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-1.0.61/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-06 08:05:02.508433 api_pipe-1.0.7/README.md
+-rw-r--r--   0        0        0      531 2024-02-02 08:03:13.996378 api_pipe-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-02-02 08:03:19.691939 api_pipe-1.0.7/src/api_pipe/__init__.py
+-rw-r--r--   0        0        0     8836 2024-02-02 08:02:57.207282 api_pipe-1.0.7/src/api_pipe/api.py
+-rw-r--r--   0        0        0      600 2024-01-14 07:11:54.785518 api_pipe-1.0.7/src/api_pipe/config.py
+-rw-r--r--   0        0        0      797 2024-01-06 10:12:12.494414 api_pipe-1.0.7/src/api_pipe/logger.py
+-rw-r--r--   0        0        0     1818 2024-02-02 06:48:33.176945 api_pipe-1.0.7/src/api_pipe/manual_test_run.py
+-rw-r--r--   0        0        0      721 2024-01-06 10:44:07.416343 api_pipe-1.0.7/src/api_pipe/url.py
+-rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 api_pipe-1.0.7/PKG-INFO
```

### Comparing `api_pipe-1.0.61/pyproject.toml` & `api_pipe-1.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "api-pipe"
-version = "1.0.61"
+version = "1.0.7"
 description = "API Pipe"
 authors = ["Rafael Roman Otero <rromanotero@gmail.com>"]
 readme = "README.md"
 packages = [{include = "api_pipe", from = "src"}]
 
 [tool.poetry.scripts]
 manual-test-run = "api_pipe.manual_test_run:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-httpx = ">=0.26.0,<1.0.0"
+httpx = "^0.26.0"
 rich = "^13.7.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 toml = "^0.10.2"
 rich = "^13.7.0"
```

### Comparing `api_pipe-1.0.61/src/api_pipe/config.py` & `api_pipe-1.0.7/src/api_pipe/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,17 @@
     Config
 
     This file is used to configure the module
 '''
 import logging
 
 #logger
-logger_level = logging.ERROR
+logger_level = logging.DEBUG
 logger_words_to_highlight = [
     "fetching",
-    "Keys",
-    "STEP",
-    "mapping",
     "filtering",
     "converting",
     "importing",
     "exporting",
     "validating",
     "deleting",
     "parsing",
```

### Comparing `api_pipe-1.0.61/src/api_pipe/url.py` & `api_pipe-1.0.7/src/api_pipe/url.py`

 * *Files identical despite different names*

