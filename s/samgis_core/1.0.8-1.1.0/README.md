# Comparing `tmp/samgis_core-1.0.8.tar.gz` & `tmp/samgis_core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samgis_core-1.0.8.tar", max compression
+gzip compressed data, was "samgis_core-1.1.0.tar", max compression
```

## Comparing `samgis_core-1.0.8.tar` & `samgis_core-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.0.8/README.md
--rw-r--r--   0        0        0      632 2024-03-17 22:28:12.194301 samgis_core-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.0.8/samgis_core/__init__.py
--rw-r--r--   0        0        0       94 2024-03-17 11:54:20.222112 samgis_core-1.0.8/samgis_core/__version__.py
--rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.0.8/samgis_core/prediction_api/__init__.py
--rw-r--r--   0        0        0    11674 2024-02-14 23:20:42.768359 samgis_core-1.0.8/samgis_core/prediction_api/sam_onnx.py
--rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.0.8/samgis_core/utilities/__init__.py
--rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.0.8/samgis_core/utilities/constants.py
--rw-r--r--   0        0        0      615 2024-03-14 22:19:15.031902 samgis_core-1.0.8/samgis_core/utilities/fastapi_logger.py
--rw-r--r--   0        0        0     2749 2024-01-26 20:33:06.000000 samgis_core-1.0.8/samgis_core/utilities/serialize.py
--rw-r--r--   0        0        0      402 2024-02-06 08:51:42.454571 samgis_core-1.0.8/samgis_core/utilities/type_hints.py
--rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.0.8/samgis_core/utilities/utilities.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 samgis_core-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-01-27 16:18:49.002975 samgis_core-1.1.0/README.md
+-rw-r--r--   0        0        0      632 2024-04-15 21:58:32.482109 samgis_core-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      351 2024-01-31 18:31:46.678851 samgis_core-1.1.0/samgis_core/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-15 09:18:13.959941 samgis_core-1.1.0/samgis_core/__version__.py
+-rw-r--r--   0        0        0       57 2024-01-26 19:56:25.000000 samgis_core-1.1.0/samgis_core/prediction_api/__init__.py
+-rw-r--r--   0        0        0    15172 2024-04-16 13:28:00.947428 samgis_core-1.1.0/samgis_core/prediction_api/sam_onnx.py
+-rw-r--r--   0        0        0       32 2024-01-26 19:56:25.000000 samgis_core-1.1.0/samgis_core/utilities/__init__.py
+-rw-r--r--   0        0        0      157 2024-01-27 14:15:17.000000 samgis_core-1.1.0/samgis_core/utilities/constants.py
+-rw-r--r--   0        0        0      650 2024-04-15 21:25:49.690475 samgis_core-1.1.0/samgis_core/utilities/fastapi_logger.py
+-rw-r--r--   0        0        0     2749 2024-01-26 20:33:06.000000 samgis_core-1.1.0/samgis_core/utilities/serialize.py
+-rw-r--r--   0        0        0      659 2024-04-16 13:20:43.686978 samgis_core-1.1.0/samgis_core/utilities/type_hints.py
+-rw-r--r--   0        0        0     2434 2024-01-27 14:15:17.000000 samgis_core-1.1.0/samgis_core/utilities/utilities.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 samgis_core-1.1.0/PKG-INFO
```

### Comparing `samgis_core-1.0.8/pyproject.toml` & `samgis_core-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "samgis_core"
-version = "1.0.8"
+version = "1.1.0"
 description = "SamGIS CORE"
 authors = ["alessandro trinca tornidor <alessandro@trinca.tornidor.com>"]
 license = "MIT license"
 readme = "README.md"
 
 [metadata]
 name = "samgis_core"
```

### Comparing `samgis_core-1.0.8/samgis_core/utilities/fastapi_logger.py` & `samgis_core-1.1.0/samgis_core/utilities/fastapi_logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import loguru
 
 
-def setup_logging(debug: bool = False, formatter: str = "{time} - {level} - ({extra[request_id]}) {message} "
-                  ) -> loguru.logger:
+format_string = "{time} - {level} - {file} - {function} - ({extra[request_id]}) {message} "
+
+
+def setup_logging(debug: bool = False, formatter: str = format_string) -> loguru.logger:
     """
     Create a logging instance with log string formatter.
 
     Args:
         debug: logging debug argument
         formatter: log string formatter
```

### Comparing `samgis_core-1.0.8/samgis_core/utilities/serialize.py` & `samgis_core-1.1.0/samgis_core/utilities/serialize.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.0.8/samgis_core/utilities/utilities.py` & `samgis_core-1.1.0/samgis_core/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `samgis_core-1.0.8/PKG-INFO` & `samgis_core-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samgis_core
-Version: 1.0.8
+Version: 1.1.0
 Summary: SamGIS CORE
 License: MIT
 Author: alessandro trinca tornidor
 Author-email: alessandro@trinca.tornidor.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

