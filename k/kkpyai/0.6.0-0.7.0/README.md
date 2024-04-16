# Comparing `tmp/kkpyai-0.6.0.tar.gz` & `tmp/kkpyai-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.6.0.tar", max compression
+gzip compressed data, was "kkpyai-0.7.0.tar", max compression
```

## Comparing `kkpyai-0.6.0.tar` & `kkpyai-0.7.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.6.0/LICENSE
--rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.6.0/README.md
--rw-r--r--   0        0        0     9455 2024-04-13 16:31:36.915313 kkpyai-0.6.0/kkpyai/kktorch.py
--rw-r--r--   0        0        0      439 2024-04-13 16:32:20.002620 kkpyai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 kkpyai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.7.0/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-10 13:52:34.317676 kkpyai-0.7.0/README.md
+-rw-r--r--   0        0        0    16457 2024-04-16 19:06:34.442440 kkpyai-0.7.0/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      486 2024-04-16 19:07:17.333019 kkpyai-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 kkpyai-0.7.0/PKG-INFO
```

### Comparing `kkpyai-0.6.0/LICENSE` & `kkpyai-0.7.0/LICENSE`

 * *Files identical despite different names*

