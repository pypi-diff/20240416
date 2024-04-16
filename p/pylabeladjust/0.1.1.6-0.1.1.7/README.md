# Comparing `tmp/pylabeladjust-0.1.1.6.tar.gz` & `tmp/pylabeladjust-0.1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.1.6.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.1.7.tar", max compression
```

## Comparing `pylabeladjust-0.1.1.6.tar` & `pylabeladjust-0.1.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.6/LICENSE
--rw-r--r--   0        0        0     4067 2024-04-15 20:18:51.282089 pylabeladjust-0.1.1.6/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.6/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.6/pylabeladjust/core.py
--rw-r--r--   0        0        0      435 2024-04-15 20:18:57.986359 pylabeladjust-0.1.1.6/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.7/LICENSE
+-rw-r--r--   0        0        0     4067 2024-04-15 20:18:51.282089 pylabeladjust-0.1.1.7/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.7/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.7/pylabeladjust/core.py
+-rw-r--r--   0        0        0      434 2024-04-15 20:30:58.912202 pylabeladjust-0.1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.7/PKG-INFO
```

### Comparing `pylabeladjust-0.1.1.6/LICENSE` & `pylabeladjust-0.1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.6/README.md` & `pylabeladjust-0.1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.6/pylabeladjust/core.py` & `pylabeladjust-0.1.1.7/pylabeladjust/core.py`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.6/PKG-INFO` & `pylabeladjust-0.1.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: pylabeladjust
-Version: 0.1.1.6
+Version: 0.1.1.7
 Summary: `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python.
 License: MIT
 Author: MNoichl
 Author-email: noichlmax@hotmail.co.uk
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pyqtree (>=1.0.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

