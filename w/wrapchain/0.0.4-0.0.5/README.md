# Comparing `tmp/wrapchain-0.0.4.tar.gz` & `tmp/wrapchain-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapchain-0.0.4.tar", max compression
+gzip compressed data, was "wrapchain-0.0.5.tar", max compression
```

## Comparing `wrapchain-0.0.4.tar` & `wrapchain-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       14 2024-04-15 12:31:24.938306 wrapchain-0.0.4/README.md
--rw-r--r--   0        0        0      351 2024-04-15 14:14:14.612253 wrapchain-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       58 2024-04-15 12:54:02.130204 wrapchain-0.0.4/wrapchain/__init__.py
--rw-r--r--   0        0        0      472 2024-04-15 13:44:47.826139 wrapchain-0.0.4/wrapchain/main.py
--rw-r--r--   0        0        0     1730 2024-04-15 14:14:07.380039 wrapchain-0.0.4/wrapchain/wrapchain.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 wrapchain-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       14 2024-04-15 12:31:24.938306 wrapchain-0.0.5/README.md
+-rw-r--r--   0        0        0      370 2024-04-16 02:37:47.465318 wrapchain-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-04-15 12:54:02.130204 wrapchain-0.0.5/wrapchain/__init__.py
+-rw-r--r--   0        0        0      530 2024-04-16 02:38:03.215891 wrapchain-0.0.5/wrapchain/main.py
+-rw-r--r--   0        0        0     3008 2024-04-16 02:39:38.990464 wrapchain-0.0.5/wrapchain/wrapchain.py
+-rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 wrapchain-0.0.5/PKG-INFO
```

