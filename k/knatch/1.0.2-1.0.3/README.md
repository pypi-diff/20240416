# Comparing `tmp/knatch-1.0.2.tar.gz` & `tmp/knatch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knatch-1.0.2.tar", max compression
+gzip compressed data, was "knatch-1.0.3.tar", max compression
```

## Comparing `knatch-1.0.2.tar` & `knatch-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2024-02-07 07:37:41.756429 knatch-1.0.2/LICENSE
--rw-r--r--   0        0        0      160 2024-02-07 07:37:41.756429 knatch-1.0.2/README.md
--rw-r--r--   0        0        0      421 2024-02-07 07:37:42.012429 knatch-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      107 2024-02-07 07:37:41.756429 knatch-1.0.2/src/knatch/__init__.py
--rw-r--r--   0        0        0     2640 2024-02-07 07:37:41.756429 knatch-1.0.2/src/knatch/quarto.py
--rw-r--r--   0        0        0      569 2024-02-07 07:37:41.756429 knatch-1.0.2/src/knatch/utils.py
--rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 knatch-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-16 08:21:57.539971 knatch-1.0.3/LICENSE
+-rw-r--r--   0        0        0      160 2024-04-16 08:21:57.539971 knatch-1.0.3/README.md
+-rw-r--r--   0        0        0      421 2024-04-16 08:21:57.791971 knatch-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/__init__.py
+-rw-r--r--   0        0        0     2640 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/quarto.py
+-rw-r--r--   0        0        0      569 2024-04-16 08:21:57.543971 knatch-1.0.3/src/knatch/utils.py
+-rw-r--r--   0        0        0      730 1970-01-01 00:00:00.000000 knatch-1.0.3/PKG-INFO
```

### Comparing `knatch-1.0.2/LICENSE` & `knatch-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `knatch-1.0.2/src/knatch/quarto.py` & `knatch-1.0.3/src/knatch/quarto.py`

 * *Files identical despite different names*

### Comparing `knatch-1.0.2/src/knatch/utils.py` & `knatch-1.0.3/src/knatch/utils.py`

 * *Files identical despite different names*

### Comparing `knatch-1.0.2/PKG-INFO` & `knatch-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knatch
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Author: Erik Vattekar
 Author-email: erik.vattekar@nav.no
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

