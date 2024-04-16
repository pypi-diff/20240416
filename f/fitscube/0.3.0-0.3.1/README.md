# Comparing `tmp/fitscube-0.3.0.tar.gz` & `tmp/fitscube-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitscube-0.3.0.tar", max compression
+gzip compressed data, was "fitscube-0.3.1.tar", max compression
```

## Comparing `fitscube-0.3.0.tar` & `fitscube-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2022-11-30 13:17:10.782000 fitscube-0.3.0/LICENSE
--rw-r--r--   0        0        0     3481 2023-07-31 08:59:54.128122 fitscube-0.3.0/README.md
--rw-r--r--   0        0        0      124 2023-07-31 08:59:54.128719 fitscube-0.3.0/fitscube/__init__.py
--rw-r--r--   0        0        0    12083 2023-07-31 08:59:54.129447 fitscube-0.3.0/fitscube/fitscube.py
--rw-r--r--   0        0        0     4106 2023-07-31 08:59:54.130057 fitscube-0.3.0/fitscube/stokescube.py
--rw-r--r--   0        0        0      443 2023-07-31 09:00:02.613665 fitscube-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 fitscube-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-11-30 13:17:10.782000 fitscube-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3481 2023-07-31 08:59:54.128122 fitscube-0.3.1/README.md
+-rw-r--r--   0        0        0      124 2023-07-31 08:59:54.128719 fitscube-0.3.1/fitscube/__init__.py
+-rw-r--r--   0        0        0    12083 2023-07-31 08:59:54.129447 fitscube-0.3.1/fitscube/fitscube.py
+-rw-r--r--   0        0        0     4106 2023-07-31 08:59:54.130057 fitscube-0.3.1/fitscube/stokescube.py
+-rw-r--r--   0        0        0      442 2024-04-16 08:45:33.557289 fitscube-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4139 1970-01-01 00:00:00.000000 fitscube-0.3.1/PKG-INFO
```

### Comparing `fitscube-0.3.0/LICENSE` & `fitscube-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fitscube-0.3.0/README.md` & `fitscube-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fitscube-0.3.0/fitscube/fitscube.py` & `fitscube-0.3.1/fitscube/fitscube.py`

 * *Files identical despite different names*

### Comparing `fitscube-0.3.0/fitscube/stokescube.py` & `fitscube-0.3.1/fitscube/stokescube.py`

 * *Files identical despite different names*

### Comparing `fitscube-0.3.0/PKG-INFO` & `fitscube-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fitscube
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Thomson, Alec (S&A, Kensington)
 Author-email: AlecThomson@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astropy (>=5.0,<6.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: astropy (>=5)
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # FITSCUBE
 
 From the [wsclean](https://wsclean.readthedocs.io/) docs:
```

