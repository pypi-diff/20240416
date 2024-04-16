# Comparing `tmp/pslines-0.1.0.tar.gz` & `tmp/pslines-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pslines-0.1.0.tar", max compression
+gzip compressed data, was "pslines-0.1.1.tar", max compression
```

## Comparing `pslines-0.1.0.tar` & `pslines-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      769 2024-03-27 12:21:24.634516 pslines-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-10-17 12:51:25.779811 pslines-0.1.0/pslines/__init__.py
--rw-r--r--   0        0        0    15633 2024-03-27 12:25:19.125811 pslines-0.1.0/pslines/pslines.py
--rw-r--r--   0        0        0      397 2024-04-16 09:29:01.193124 pslines-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 pslines-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      698 2024-04-16 09:40:12.512819 pslines-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-10-17 12:51:25.779811 pslines-0.1.1/pslines/__init__.py
+-rw-r--r--   0        0        0    15633 2024-03-27 12:25:19.125811 pslines-0.1.1/pslines/pslines.py
+-rw-r--r--   0        0        0      322 2024-04-16 09:48:42.688622 pslines-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 pslines-0.1.1/PKG-INFO
```

### Comparing `pslines-0.1.0/pslines/pslines.py` & `pslines-0.1.1/pslines/pslines.py`

 * *Files identical despite different names*

