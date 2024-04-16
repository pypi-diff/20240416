# Comparing `tmp/wiwb-2024.4.0.tar.gz` & `tmp/wiwb-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wiwb-2024.4.0.tar", last modified: Tue Apr 16 11:40:49 2024, max compression
+gzip compressed data, was "dist\wiwb-2024.4.1.tar", last modified: Tue Apr 16 13:13:49 2024, max compression
```

## Comparing `wiwb-2024.4.0.tar` & `wiwb-2024.4.1.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.195314 wiwb-2024.4.0/
--rw-rw-rw-   0        0        0     1094 2024-04-02 10:40:28.000000 wiwb-2024.4.0/LICENSE
--rw-rw-rw-   0        0        0     5044 2024-04-16 11:40:51.372312 wiwb-2024.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4487 2024-04-02 10:40:28.000000 wiwb-2024.4.0/README.md
--rw-rw-rw-   0        0        0      873 2024-04-16 11:15:02.000000 wiwb-2024.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 11:40:51.381306 wiwb-2024.4.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2024-04-02 10:40:28.000000 wiwb-2024.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.191317 wiwb-2024.4.0/tests/
--rw-rw-rw-   0        0        0      202 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_api.py
--rw-rw-rw-   0        0        0      133 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_data_sources.py
--rw-rw-rw-   0        0        0     2595 2024-04-16 11:19:57.000000 wiwb-2024.4.0/tests/test_grids.py
--rw-rw-rw-   0        0        0      552 2024-04-16 11:19:57.000000 wiwb-2024.4.0/tests/test_sample_nc.py
--rw-rw-rw-   0        0        0      149 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_variable_codes.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.195314 wiwb-2024.4.0/wiwb/
--rw-rw-rw-   0        0        0      676 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/__init__.py
--rw-rw-rw-   0        0        0     1138 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/api.py
--rw-rw-rw-   0        0        0     3617 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/auth.py
--rw-rw-rw-   0        0        0     1456 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/constants.py
--rw-rw-rw-   0        0        0      226 2024-04-02 10:40:29.000000 wiwb-2024.4.0/wiwb/converters.py
--rw-rw-rw-   0        0        0     6354 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/sample.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.197313 wiwb-2024.4.0/wiwb.egg-info/
--rw-rw-rw-   0        0        0     5044 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-16 13:13:51.086977 wiwb-2024.4.1/
+-rw-rw-rw-   0        0        0     1094 2024-04-02 10:40:28.000000 wiwb-2024.4.1/LICENSE
+-rw-rw-rw-   0        0        0     5044 2024-04-16 13:13:51.336955 wiwb-2024.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4487 2024-04-02 10:40:28.000000 wiwb-2024.4.1/README.md
+-rw-rw-rw-   0        0        0      883 2024-04-16 13:10:39.000000 wiwb-2024.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:13:51.346945 wiwb-2024.4.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-02 10:40:28.000000 wiwb-2024.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:13:51.084981 wiwb-2024.4.1/tests/
+-rw-rw-rw-   0        0        0      202 2024-04-02 10:40:28.000000 wiwb-2024.4.1/tests/test_api.py
+-rw-rw-rw-   0        0        0      133 2024-04-02 10:40:28.000000 wiwb-2024.4.1/tests/test_data_sources.py
+-rw-rw-rw-   0        0        0     2595 2024-04-16 11:19:57.000000 wiwb-2024.4.1/tests/test_grids.py
+-rw-rw-rw-   0        0        0      552 2024-04-16 11:19:57.000000 wiwb-2024.4.1/tests/test_sample_nc.py
+-rw-rw-rw-   0        0        0      149 2024-04-02 10:40:28.000000 wiwb-2024.4.1/tests/test_variable_codes.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:13:51.086977 wiwb-2024.4.1/wiwb/
+-rw-rw-rw-   0        0        0      676 2024-04-16 13:12:31.000000 wiwb-2024.4.1/wiwb/__init__.py
+-rw-rw-rw-   0        0        0     1138 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:13:51.090971 wiwb-2024.4.1/wiwb/api_calls/
+-rw-rw-rw-   0        0        0      274 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api_calls/__init__.py
+-rw-rw-rw-   0        0        0      350 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api_calls/base.py
+-rw-rw-rw-   0        0        0      964 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api_calls/get_data_sources.py
+-rw-rw-rw-   0        0        0    15312 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api_calls/get_grids.py
+-rw-rw-rw-   0        0        0      959 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/api_calls/get_variables.py
+-rw-rw-rw-   0        0        0     3617 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/auth.py
+-rw-rw-rw-   0        0        0     1456 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/constants.py
+-rw-rw-rw-   0        0        0      226 2024-04-02 10:40:29.000000 wiwb-2024.4.1/wiwb/converters.py
+-rw-rw-rw-   0        0        0     6354 2024-04-16 11:19:57.000000 wiwb-2024.4.1/wiwb/sample.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:13:51.088973 wiwb-2024.4.1/wiwb.egg-info/
+-rw-rw-rw-   0        0        0     5044 2024-04-16 13:13:50.000000 wiwb-2024.4.1/wiwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2024-04-16 13:13:51.000000 wiwb-2024.4.1/wiwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:13:50.000000 wiwb-2024.4.1/wiwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-16 13:13:50.000000 wiwb-2024.4.1/wiwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 13:13:50.000000 wiwb-2024.4.1/wiwb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 11:40:50.000000 wiwb-2024.4.1/wiwb.egg-info/zip-safe
```

### Comparing `wiwb-2024.4.0/LICENSE` & `wiwb-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/PKG-INFO` & `wiwb-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiwb
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Python API to work with WIWB
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.kramer@hdsr.nl>
 License: MIT
 Project-URL: Source, https://github.com/d2hydro/wiwb
 Requires-Python: <=3.12,>3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wiwb-2024.4.0/README.md` & `wiwb-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/pyproject.toml` & `wiwb-2024.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 [tool.setuptools]
 zip-safe = true
 
 [tool.setuptools.dynamic]
 version = { attr = "wiwb.__version__" }
 
 [tool.setuptools.packages.find]
-include = ["wiwb"]
+include = ["wiwb", "wiwb.*"]
 
 [project.urls]
 Source = "https://github.com/d2hydro/wiwb"
```

### Comparing `wiwb-2024.4.0/tests/test_grids.py` & `wiwb-2024.4.1/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/tests/test_sample_nc.py` & `wiwb-2024.4.1/tests/test_sample_nc.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/wiwb/__init__.py` & `wiwb-2024.4.1/wiwb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2024.4.0"
+__version__ = "2024.4.1"
 from wiwb.api import Api
 from wiwb.auth import Auth
 import warnings
 
 __all__ = ["Auth", "Api"]
 
 warnings.filterwarnings(
```

### Comparing `wiwb-2024.4.0/wiwb/api.py` & `wiwb-2024.4.1/wiwb/api.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/wiwb/auth.py` & `wiwb-2024.4.1/wiwb/auth.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/wiwb/constants.py` & `wiwb-2024.4.1/wiwb/constants.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/wiwb/sample.py` & `wiwb-2024.4.1/wiwb/sample.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.4.0/wiwb.egg-info/PKG-INFO` & `wiwb-2024.4.1/wiwb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiwb
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Python API to work with WIWB
 Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.kramer@hdsr.nl>
 License: MIT
 Project-URL: Source, https://github.com/d2hydro/wiwb
 Requires-Python: <=3.12,>3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

