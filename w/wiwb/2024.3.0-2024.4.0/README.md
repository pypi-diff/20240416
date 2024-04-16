# Comparing `tmp/wiwb-2024.3.0.tar.gz` & `tmp/wiwb-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiwb-2024.3.0.tar", last modified: Thu Mar  7 09:26:11 2024, max compression
+gzip compressed data, was "dist\wiwb-2024.4.0.tar", last modified: Tue Apr 16 11:40:49 2024, max compression
```

## Comparing `wiwb-2024.3.0.tar` & `wiwb-2024.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-07 09:26:11.323411 wiwb-2024.3.0/
--rw-rw-rw-   0        0        0     1094 2023-11-12 21:50:35.000000 wiwb-2024.3.0/LICENSE
--rw-rw-rw-   0        0        0     5044 2024-03-07 09:26:11.322414 wiwb-2024.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     4487 2024-03-07 09:17:20.000000 wiwb-2024.3.0/README.md
--rw-rw-rw-   0        0        0      828 2024-02-27 15:43:54.000000 wiwb-2024.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-07 09:26:11.323411 wiwb-2024.3.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-09 11:35:36.000000 wiwb-2024.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-07 09:26:11.284471 wiwb-2024.3.0/tests/
--rw-rw-rw-   0        0        0      202 2024-02-14 20:45:40.000000 wiwb-2024.3.0/tests/test_api.py
--rw-rw-rw-   0        0        0      133 2024-02-14 20:45:40.000000 wiwb-2024.3.0/tests/test_data_sources.py
--rw-rw-rw-   0        0        0     2595 2024-03-04 07:57:47.000000 wiwb-2024.3.0/tests/test_grids.py
--rw-rw-rw-   0        0        0      552 2024-02-29 15:48:26.000000 wiwb-2024.3.0/tests/test_sample_nc.py
--rw-rw-rw-   0        0        0      149 2024-02-14 20:45:40.000000 wiwb-2024.3.0/tests/test_variable_codes.py
-drwxrwxrwx   0        0        0        0 2024-03-07 09:26:11.291576 wiwb-2024.3.0/wiwb/
--rw-rw-rw-   0        0        0      676 2024-03-07 09:17:36.000000 wiwb-2024.3.0/wiwb/__init__.py
--rw-rw-rw-   0        0        0     1110 2024-02-28 20:48:34.000000 wiwb-2024.3.0/wiwb/api.py
--rw-rw-rw-   0        0        0     3617 2024-02-29 16:43:33.000000 wiwb-2024.3.0/wiwb/auth.py
--rw-rw-rw-   0        0        0     1456 2024-02-29 20:02:32.000000 wiwb-2024.3.0/wiwb/constants.py
--rw-rw-rw-   0        0        0      226 2023-11-12 22:03:16.000000 wiwb-2024.3.0/wiwb/converters.py
--rw-rw-rw-   0        0        0     6354 2024-03-07 09:24:44.000000 wiwb-2024.3.0/wiwb/sample.py
-drwxrwxrwx   0        0        0        0 2024-03-07 09:26:11.321413 wiwb-2024.3.0/wiwb.egg-info/
--rw-rw-rw-   0        0        0     5044 2024-03-07 09:26:10.000000 wiwb-2024.3.0/wiwb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2024-03-07 09:26:10.000000 wiwb-2024.3.0/wiwb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-07 09:26:10.000000 wiwb-2024.3.0/wiwb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-03-07 09:26:10.000000 wiwb-2024.3.0/wiwb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-07 09:26:10.000000 wiwb-2024.3.0/wiwb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-13 10:07:10.000000 wiwb-2024.3.0/wiwb.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.195314 wiwb-2024.4.0/
+-rw-rw-rw-   0        0        0     1094 2024-04-02 10:40:28.000000 wiwb-2024.4.0/LICENSE
+-rw-rw-rw-   0        0        0     5044 2024-04-16 11:40:51.372312 wiwb-2024.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4487 2024-04-02 10:40:28.000000 wiwb-2024.4.0/README.md
+-rw-rw-rw-   0        0        0      873 2024-04-16 11:15:02.000000 wiwb-2024.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:40:51.381306 wiwb-2024.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-02 10:40:28.000000 wiwb-2024.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.191317 wiwb-2024.4.0/tests/
+-rw-rw-rw-   0        0        0      202 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_api.py
+-rw-rw-rw-   0        0        0      133 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_data_sources.py
+-rw-rw-rw-   0        0        0     2595 2024-04-16 11:19:57.000000 wiwb-2024.4.0/tests/test_grids.py
+-rw-rw-rw-   0        0        0      552 2024-04-16 11:19:57.000000 wiwb-2024.4.0/tests/test_sample_nc.py
+-rw-rw-rw-   0        0        0      149 2024-04-02 10:40:28.000000 wiwb-2024.4.0/tests/test_variable_codes.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.195314 wiwb-2024.4.0/wiwb/
+-rw-rw-rw-   0        0        0      676 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/__init__.py
+-rw-rw-rw-   0        0        0     1138 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/api.py
+-rw-rw-rw-   0        0        0     3617 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/auth.py
+-rw-rw-rw-   0        0        0     1456 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/constants.py
+-rw-rw-rw-   0        0        0      226 2024-04-02 10:40:29.000000 wiwb-2024.4.0/wiwb/converters.py
+-rw-rw-rw-   0        0        0     6354 2024-04-16 11:19:57.000000 wiwb-2024.4.0/wiwb/sample.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:40:51.197313 wiwb-2024.4.0/wiwb.egg-info/
+-rw-rw-rw-   0        0        0     5044 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-16 11:40:50.000000 wiwb-2024.4.0/wiwb.egg-info/zip-safe
```

### Comparing `wiwb-2024.3.0/LICENSE` & `wiwb-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/PKG-INFO` & `wiwb-2024.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wiwb
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Python API to work with WIWB
-Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.Kramer@hdsr.nl>
+Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.kramer@hdsr.nl>
 License: MIT
 Project-URL: Source, https://github.com/d2hydro/wiwb
 Requires-Python: <=3.12,>3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: pyjwt
```

### Comparing `wiwb-2024.3.0/README.md` & `wiwb-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/pyproject.toml` & `wiwb-2024.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-[build-system]
-requires = ["setuptools>=61"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "wiwb"
-description = "Python API to work with WIWB"
-readme = "README.md"
-authors = [
-    { name = "Daniel Tollenaar", email = "daniel@d2hydro.nl" },
-	{ name = "Renier Kramer", email = "renier.Kramer@hdsr.nl" }
-]
-license = { text = "MIT" }
-
-requires-python = ">3.7,<=3.12"
-dependencies = [
-    "geopandas",
-    "pyjwt",
-    "xarray",
-    "rasterio",
-    "requests",
-    "netcdf4"
-]
-dynamic = ["version"]
-
-[project.optional-dependencies]
-tests = ["pytest"]
-
-[tool.flake8]
-max-line-length = 120
-max-complexity = 10
-
-[tool.setuptools]
-zip-safe = true
-
-[tool.setuptools.dynamic]
-version = { attr = "wiwb.__version__" }
-
-[tool.setuptools.packages.find]
-include = ["wiwb"]
-
-[project.urls]
-Source = "https://github.com/d2hydro/wiwb"
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "wiwb"
+description = "Python API to work with WIWB"
+readme = "README.md"
+authors = [
+    { name = "Daniel Tollenaar", email = "daniel@d2hydro.nl" },
+	{ name = "Renier Kramer", email = "renier.kramer@hdsr.nl" }
+]
+license = { text = "MIT" }
+
+requires-python = ">3.7,<=3.12"
+dependencies = [
+    "geopandas",
+    "pyjwt",
+    "xarray",
+    "rasterio",
+    "requests",
+    "netcdf4"
+]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+tests = ["pytest"]
+
+[tool.flake8]
+max-line-length = 120
+max-complexity = 10
+
+[tool.setuptools]
+zip-safe = true
+
+[tool.setuptools.dynamic]
+version = { attr = "wiwb.__version__" }
+
+[tool.setuptools.packages.find]
+include = ["wiwb"]
+
+[project.urls]
+Source = "https://github.com/d2hydro/wiwb"
+
```

### Comparing `wiwb-2024.3.0/tests/test_grids.py` & `wiwb-2024.4.0/tests/test_grids.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/tests/test_sample_nc.py` & `wiwb-2024.4.0/tests/test_sample_nc.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/wiwb/api.py` & `wiwb-2024.4.0/wiwb/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from wiwb.auth import Auth
 from dataclasses import dataclass
 from typing import Union
-from wiwb import api_calls
+from wiwb.api_calls.get_data_sources import GetDataSources
+from wiwb.api_calls.get_variables import GetVariables
+from wiwb.api_calls.get_grids import GetGrids
 from wiwb.constants import API_URL
 
 
 @dataclass
 class Api:
     """Python API for WIWB service."""
 
@@ -17,23 +19,17 @@
             self.auth = Auth()
         if self.base_url is None:
             raise ValueError(
                 f"Provide a valid base_url. Current value is {self.base_url}"
             )
 
     def get_data_sources(self, **kwargs):
-        api_call = api_calls.GetDataSources(
-            base_url=self.base_url, auth=self.auth, **kwargs
-        )
+        api_call = GetDataSources(base_url=self.base_url, auth=self.auth, **kwargs)
         return api_call.run()
 
     def get_variables(self, **kwargs):
-        api_call = api_calls.GetVariables(
-            base_url=self.base_url, auth=self.auth, **kwargs
-        )
+        api_call = GetVariables(base_url=self.base_url, auth=self.auth, **kwargs)
         return api_call.run()
 
     def get_grids(self, **kwargs):
-        get_grids = api_calls.GetVariables(
-            base_url=self.base_url, auth=self.auth, **kwargs
-        )
+        get_grids = GetGrids(base_url=self.base_url, auth=self.auth, **kwargs)
         return get_grids
```

### Comparing `wiwb-2024.3.0/wiwb/auth.py` & `wiwb-2024.4.0/wiwb/auth.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/wiwb/constants.py` & `wiwb-2024.4.0/wiwb/constants.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/wiwb/sample.py` & `wiwb-2024.4.0/wiwb/sample.py`

 * *Files identical despite different names*

### Comparing `wiwb-2024.3.0/wiwb.egg-info/PKG-INFO` & `wiwb-2024.4.0/wiwb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: wiwb
-Version: 2024.3.0
+Version: 2024.4.0
 Summary: Python API to work with WIWB
-Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.Kramer@hdsr.nl>
+Author-email: Daniel Tollenaar <daniel@d2hydro.nl>, Renier Kramer <renier.kramer@hdsr.nl>
 License: MIT
 Project-URL: Source, https://github.com/d2hydro/wiwb
 Requires-Python: <=3.12,>3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: geopandas
 Requires-Dist: pyjwt
```

