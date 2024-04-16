# Comparing `tmp/overturemaps-0.2.0.tar.gz` & `tmp/overturemaps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overturemaps-0.2.0.tar", max compression
+gzip compressed data, was "overturemaps-0.3.0.tar", max compression
```

## Comparing `overturemaps-0.2.0.tar` & `overturemaps-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.2.0/LICENSE
--rw-r--r--   0        0        0     1541 2024-04-08 23:57:11.366560 overturemaps-0.2.0/README.md
--rw-r--r--   0        0        0     6632 2024-04-09 10:08:38.379252 overturemaps-0.2.0/overturemaps/cli.py
--rw-r--r--   0        0        0      480 2024-04-09 10:08:31.369219 overturemaps-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 overturemaps-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 10:31:26.935857 overturemaps-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2507 2024-04-11 15:34:22.013871 overturemaps-0.3.0/README.md
+-rw-r--r--   0        0        0       75 2024-04-11 16:40:32.681725 overturemaps-0.3.0/overturemaps/__init__.py
+-rw-r--r--   0        0        0     5086 2024-04-16 03:33:02.187599 overturemaps-0.3.0/overturemaps/cli.py
+-rw-r--r--   0        0        0     3246 2024-04-16 03:37:08.217413 overturemaps-0.3.0/overturemaps/core.py
+-rw-r--r--   0        0        0      480 2024-04-16 12:46:02.130484 overturemaps-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3108 1970-01-01 00:00:00.000000 overturemaps-0.3.0/PKG-INFO
```

### Comparing `overturemaps-0.2.0/LICENSE` & `overturemaps-0.3.0/LICENSE`

 * *Files identical despite different names*

