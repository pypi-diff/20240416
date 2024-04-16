# Comparing `tmp/redxclient-0.2.2.tar.gz` & `tmp/redxclient-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redxclient-0.2.2.tar", last modified: Sun Mar 31 16:47:28 2024, max compression
+gzip compressed data, was "redxclient-0.2.3.tar", last modified: Tue Apr 16 04:27:28 2024, max compression
```

## Comparing `redxclient-0.2.2.tar` & `redxclient-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      959 2024-03-31 16:47:10.512933 redxclient-0.2.2/README.md
--rw-r--r--   0        0        0     1156 2024-03-31 16:47:28.909900 redxclient-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4994 2024-03-31 16:47:10.512933 redxclient-0.2.2/src/redxclient/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 16:47:10.535933 redxclient-0.2.2/src/redxclient/schema/__init__.py
--rw-r--r--   0        0        0      855 2024-03-31 16:47:10.512933 redxclient-0.2.2/src/redxclient/schema/areas.py
--rw-r--r--   0        0        0     1033 2024-03-31 16:47:10.512933 redxclient-0.2.2/src/redxclient/schema/parcel.py
--rw-r--r--   0        0        0      368 2024-03-31 16:47:10.512933 redxclient-0.2.2/src/redxclient/schema/pickup.py
--rw-r--r--   0        0        0        0 2024-03-31 16:47:10.535933 redxclient-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1273 2024-03-31 16:47:10.512933 redxclient-0.2.2/tests/test_areas_api.py
--rw-r--r--   0        0        0     1631 2024-03-31 16:47:10.512933 redxclient-0.2.2/tests/test_parcels_api.py
--rw-r--r--   0        0        0     1187 2024-03-31 16:47:10.513933 redxclient-0.2.2/tests/test_stores_api.py
--rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 redxclient-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      959 2024-04-16 04:27:11.856043 redxclient-0.2.3/README.md
+-rw-r--r--   0        0        0     1156 2024-04-16 04:27:28.982021 redxclient-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4994 2024-04-16 04:27:11.857043 redxclient-0.2.3/src/redxclient/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 04:27:11.879043 redxclient-0.2.3/src/redxclient/schema/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-16 04:27:11.857043 redxclient-0.2.3/src/redxclient/schema/areas.py
+-rw-r--r--   0        0        0     1033 2024-04-16 04:27:11.857043 redxclient-0.2.3/src/redxclient/schema/parcel.py
+-rw-r--r--   0        0        0      368 2024-04-16 04:27:11.857043 redxclient-0.2.3/src/redxclient/schema/pickup.py
+-rw-r--r--   0        0        0        0 2024-04-16 04:27:11.879043 redxclient-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-16 04:27:11.857043 redxclient-0.2.3/tests/test_areas_api.py
+-rw-r--r--   0        0        0     1631 2024-04-16 04:27:11.857043 redxclient-0.2.3/tests/test_parcels_api.py
+-rw-r--r--   0        0        0     1187 2024-04-16 04:27:11.857043 redxclient-0.2.3/tests/test_stores_api.py
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 redxclient-0.2.3/PKG-INFO
```

### Comparing `redxclient-0.2.2/README.md` & `redxclient-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/pyproject.toml` & `redxclient-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "RedXClient"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Python Client for RedX Courier Service"
 authors = [
     { name = "Utsob Roy", email = "roy@co.design" },
 ]
 dependencies = [
     "pydantic>=2.6.4",
     "requests>=2.31.0",
```

### Comparing `redxclient-0.2.2/src/redxclient/__init__.py` & `redxclient-0.2.3/src/redxclient/__init__.py`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/src/redxclient/schema/areas.py` & `redxclient-0.2.3/src/redxclient/schema/areas.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from enum import IntEnum
 
 from pydantic import BaseModel, ValidationError, model_validator
 from typing_extensions import Any, Optional, Self
 
 
 class ZoneEnum(IntEnum):
-    DHAKA_CITY =  1
+    DHAKA_CITY = 1
     DHAKA_SUBURBS = 2
     OUTSIDE_DHAKA = 7
 
+
 class Area(BaseModel):
     id: int
     name: str
-    post_code: int
+    post_code: Optional[int] = None
     district_name: str
     division_name: str
     zone_id: ZoneEnum
 
 
 class AreaFilter(BaseModel):
     zone_id: Optional[ZoneEnum] = None
```

### Comparing `redxclient-0.2.2/src/redxclient/schema/parcel.py` & `redxclient-0.2.3/src/redxclient/schema/parcel.py`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/tests/test_areas_api.py` & `redxclient-0.2.3/tests/test_areas_api.py`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/tests/test_parcels_api.py` & `redxclient-0.2.3/tests/test_parcels_api.py`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/tests/test_stores_api.py` & `redxclient-0.2.3/tests/test_stores_api.py`

 * *Files identical despite different names*

### Comparing `redxclient-0.2.2/PKG-INFO` & `redxclient-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RedXClient
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python Client for RedX Courier Service
 Home-page: https://gitlab.com/codesigntheory/redxclient
 Author-Email: Utsob Roy <roy@co.design>
 License: MPL-2.0
 Project-URL: Homepage, https://gitlab.com/codesigntheory/redxclient
 Requires-Python: >=3.8
 Requires-Dist: pydantic>=2.6.4
```

