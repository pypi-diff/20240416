# Comparing `tmp/fulcra_api-0.1.8.tar.gz` & `tmp/fulcra_api-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fulcra_api-0.1.8.tar", max compression
+gzip compressed data, was "fulcra_api-0.1.9.tar", max compression
```

## Comparing `fulcra_api-0.1.8.tar` & `fulcra_api-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-10-11 06:33:14.862593 fulcra_api-0.1.8/LICENSE
--rw-r--r--   0        0        0      386 2023-10-11 06:34:37.036689 fulcra_api-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-10-11 06:33:14.863311 fulcra_api-0.1.8/fulcra_api/__init__.py
--rw-r--r--   0        0        0    25651 2023-11-22 20:19:57.476343 fulcra_api-0.1.8/fulcra_api/core.py
--rw-r--r--   0        0        0      638 2023-11-22 20:21:26.593921 fulcra_api-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 fulcra_api-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-11 06:33:14.862593 fulcra_api-0.1.9/LICENSE
+-rw-r--r--   0        0        0      386 2023-10-11 06:34:37.036689 fulcra_api-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-10-11 06:33:14.863311 fulcra_api-0.1.9/fulcra_api/__init__.py
+-rw-r--r--   0        0        0    25664 2023-12-07 15:06:03.064130 fulcra_api-0.1.9/fulcra_api/core.py
+-rw-r--r--   0        0        0      638 2023-12-07 15:06:20.709029 fulcra_api-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 fulcra_api-0.1.9/PKG-INFO
```

### Comparing `fulcra_api-0.1.8/LICENSE` & `fulcra_api-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fulcra_api-0.1.8/fulcra_api/core.py` & `fulcra_api-0.1.9/fulcra_api/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         qparams = urllib.parse.urlencode(
             {
                 "start_time": start_time,
                 "end_time": end_time,
                 "metrics": metrics,
                 "output": "arrow",
                 "samprate": sample_rate,
-                "replace_nulls": replace_nulls
+                "replace_nulls": int(replace_nulls == True)
             },
             doseq=True,
         )
         resp = self.fulcra_api(
             self.fulcra_cached_access_token, "/data/v0/time_series_grouped?" + qparams
         )
         return pd.read_feather(io.BytesIO(resp)).set_index("time")
```

### Comparing `fulcra_api-0.1.8/pyproject.toml` & `fulcra_api-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fulcra-api"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Brandon Creighton <brandon@fulcradynamics.com>"]
 readme = "README.md"
 packages = [{include = "fulcra_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fulcra_api-0.1.8/PKG-INFO` & `fulcra_api-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: fulcra-api
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Brandon Creighton
 Author-email: brandon@fulcradynamics.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>1.5,<3)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Fulcra Dynamics Python Client Library
 
 This is a Python library to simplify calling [Fulcra Dynamics](https://fulcradynamics.com/) APIs.
```

