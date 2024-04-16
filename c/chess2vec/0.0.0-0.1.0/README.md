# Comparing `tmp/chess2vec-0.0.0.tar.gz` & `tmp/chess2vec-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.0.0.tar", max compression
+gzip compressed data, was "chess2vec-0.1.0.tar", max compression
```

## Comparing `chess2vec-0.0.0.tar` & `chess2vec-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,6 @@
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-04-15 20:17:56.616439 chess2vec-0.0.0/chess2vec/__init__.py
--rw-r--r--   0        0        0      285 2024-04-15 20:18:19.763426 chess2vec-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 chess2vec-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 20:17:56.619773 chess2vec-0.1.0/README.md
+-rw-r--r--   0        0        0     3497 2024-04-16 16:47:02.278818 chess2vec-0.1.0/chess2vec/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-16 16:21:07.852284 chess2vec-0.1.0/chess2vec/_utils/sparse.py
+-rw-r--r--   0        0        0      538 2024-04-16 16:46:49.087490 chess2vec-0.1.0/chess2vec/_utils/vector.py
+-rw-r--r--   0        0        0      339 2024-04-16 16:47:28.401366 chess2vec-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 chess2vec-0.1.0/PKG-INFO
```

