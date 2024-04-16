# Comparing `tmp/skelescope-0.0.3.tar.gz` & `tmp/skelescope-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelescope-0.0.3.tar", max compression
+gzip compressed data, was "skelescope-0.0.4.tar", max compression
```

## Comparing `skelescope-0.0.3.tar` & `skelescope-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1069 2024-04-12 21:08:16.190566 skelescope-0.0.3/LICENSE
--rw-r--r--   0        0        0      402 2024-04-16 15:10:27.754367 skelescope-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2096 2024-04-12 21:08:16.195069 skelescope-0.0.3/README.md
--rw-r--r--   0        0        0     3878 2024-04-15 22:41:10.107646 skelescope-0.0.3/skelescope/__init__.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 skelescope-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-12 21:08:16.190566 skelescope-0.0.4/LICENSE
+-rw-r--r--   0        0        0      402 2024-04-16 17:27:10.779509 skelescope-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2096 2024-04-12 21:08:16.195069 skelescope-0.0.4/README.md
+-rw-r--r--   0        0        0     3878 2024-04-15 22:41:10.107646 skelescope-0.0.4/skelescope/__init__.py
+-rw-r--r--   0        0        0     3664 2024-04-16 17:24:31.857570 skelescope-0.0.4/skelescope/static/widget.css
+-rw-r--r--   0        0        0 32082300 2024-04-16 17:24:31.874459 skelescope-0.0.4/skelescope/static/widget.js
+-rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 skelescope-0.0.4/PKG-INFO
```

### Comparing `skelescope-0.0.3/LICENSE` & `skelescope-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `skelescope-0.0.3/README.md` & `skelescope-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `skelescope-0.0.3/skelescope/__init__.py` & `skelescope-0.0.4/skelescope/__init__.py`

 * *Files identical despite different names*

### Comparing `skelescope-0.0.3/PKG-INFO` & `skelescope-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelescope
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: MIT
 Author: Philipp Harth
 Author-email: harth@zib.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

