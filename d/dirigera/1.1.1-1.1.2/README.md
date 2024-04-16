# Comparing `tmp/dirigera-1.1.1.tar.gz` & `tmp/dirigera-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirigera-1.1.1.tar", last modified: Thu Apr 11 12:45:37 2024, max compression
+gzip compressed data, was "dirigera-1.1.2.tar", last modified: Tue Apr 16 06:56:45 2024, max compression
```

## Comparing `dirigera-1.1.1.tar` & `dirigera-1.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 12:45:33.000000 dirigera-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-11 12:45:37.453992 dirigera-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-11 12:45:33.000000 dirigera-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-11 12:45:33.000000 dirigera-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:45:37.453992 dirigera-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-11 12:45:33.000000 dirigera-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.445992 dirigera-1.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.449992 dirigera-1.1.1/src/dirigera/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.449992 dirigera-1.1.1/src/dirigera/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/base_ikea_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/devices/scene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/src/dirigera/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/abstract_smart_home_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-11 12:45:33.000000 dirigera-1.1.1/src/dirigera/hub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/src/dirigera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 12:45:37.000000 dirigera-1.1.1/src/dirigera.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:45:37.453992 dirigera-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_air_purifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_blinds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_environment_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_light.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_motion_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_open_close_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_outlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_scenes.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-11 12:45:33.000000 dirigera-1.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 06:56:38.000000 dirigera-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-16 06:56:45.672232 dirigera-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13314 2024-04-16 06:56:38.000000 dirigera-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-16 06:56:38.000000 dirigera-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:56:45.672232 dirigera-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 06:56:38.000000 dirigera-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.668232 dirigera-1.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.668232 dirigera-1.1.2/src/dirigera/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/base_ikea_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/devices/scene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/abstract_smart_home_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 06:56:38.000000 dirigera-1.1.2/src/dirigera/hub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/src/dirigera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15545 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 06:56:45.000000 dirigera-1.1.2/src/dirigera.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:56:45.672232 dirigera-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_air_purifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_blinds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_environment_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_motion_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_open_close_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_outlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 06:56:38.000000 dirigera-1.1.2/tests/test_utils.py
```

### Comparing `dirigera-1.1.1/LICENSE` & `dirigera-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/PKG-INFO` & `dirigera-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.1
+Version: 1.1.2
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.1/README.md` & `dirigera-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/pyproject.toml` & `dirigera-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dirigera"
-version = "1.1.1"
+version = "1.1.2"
 description = "An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub"
 readme = "README.md"
 authors = [{ name = "Leggin", email = "legginsun@gmail.com" }]
 license = { file = "LICENSE" }
 keywords = [
     "python",
     "iot",
```

### Comparing `dirigera-1.1.1/src/dirigera/devices/air_purifier.py` & `dirigera-1.1.2/src/dirigera/devices/air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/blinds.py` & `dirigera-1.1.2/src/dirigera/devices/blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/controller.py` & `dirigera-1.1.2/src/dirigera/devices/controller.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/device.py` & `dirigera-1.1.2/src/dirigera/devices/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     name: str
     color: str
     icon: str
 
 
 class Device(BaseIkeaModel):
     id: str
+    relation_id: Optional[str] = None
     type: str
     device_type: str
     created_at: datetime.datetime
     is_reachable: bool
     last_seen: datetime.datetime
     attributes: Attributes
     capabilities: Capabilities
```

### Comparing `dirigera-1.1.1/src/dirigera/devices/environment_sensor.py` & `dirigera-1.1.2/src/dirigera/devices/environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/light.py` & `dirigera-1.1.2/src/dirigera/devices/light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/motion_sensor.py` & `dirigera-1.1.2/src/dirigera/devices/motion_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/open_close_sensor.py` & `dirigera-1.1.2/src/dirigera/devices/open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/outlet.py` & `dirigera-1.1.2/src/dirigera/devices/outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/devices/scene.py` & `dirigera-1.1.2/src/dirigera/devices/scene.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/hub/abstract_smart_home_hub.py` & `dirigera-1.1.2/src/dirigera/hub/abstract_smart_home_hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/hub/auth.py` & `dirigera-1.1.2/src/dirigera/hub/auth.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera/hub/hub.py` & `dirigera-1.1.2/src/dirigera/hub/hub.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/src/dirigera.egg-info/PKG-INFO` & `dirigera-1.1.2/src/dirigera.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dirigera
-Version: 1.1.1
+Version: 1.1.2
 Summary: An unofficial Python client for controlling the IKEA Dirigera Smart Home Hub
 Author-email: Leggin <legginsun@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Leggin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dirigera-1.1.1/src/dirigera.egg-info/SOURCES.txt` & `dirigera-1.1.2/src/dirigera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_air_purifier.py` & `dirigera-1.1.2/tests/test_air_purifier.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_blinds.py` & `dirigera-1.1.2/tests/test_blinds.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_controller.py` & `dirigera-1.1.2/tests/test_motion_sensor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,115 +1,123 @@
-from typing import Any, Dict
+from typing import Dict
 import pytest
 from src.dirigera.hub.abstract_smart_home_hub import FakeDirigeraHub
-from src.dirigera.devices.controller import dict_to_controller
-from src.dirigera.devices.controller import Controller
+from src.dirigera.devices.motion_sensor import MotionSensor, dict_to_motion_sensor
 
 
 @pytest.fixture(name="fake_client")
 def fixture_fake_client() -> FakeDirigeraHub:
     return FakeDirigeraHub()
 
 
-@pytest.fixture(name="fake_controller")
-def fixture_controller(fake_client: FakeDirigeraHub) -> Controller:
-    return Controller(
-        dirigeraClient=fake_client,
-        **{
-            "id": "1237-343-2dfa",
-            "type": "controller",
-            "deviceType": "lightController",
-            "createdAt": "2023-01-07T20:07:19.000Z",
-            "isReachable": True,
-            "lastSeen": "2023-10-28T04:42:15.000Z",
-            "customIcon": "lighting_nightstand_light",
-            "attributes": {
-                "customName": "Remote",
-                "model": "TRADFRI STYRBAR",
-                "manufacturer": "IKEA of Sweden",
-                "firmwareVersion": "2.3.093",
-                "hardwareVersion": "2",
-                "isOn": False,
-                "batteryPercentage": 90,
-            },
-            "capabilities": {
-                "canSend": ["isOn", "lightLevel"],
-                "canReceive": [
-                    "customName",
-                ],
-            },
-            "room": {
-                "id": "23g2w34-d0b7-42b3-a5a1-324zaerfg3",
-                "name": "Bedroom",
-                "color": "ikea_yellow_no_24",
-                "icon": "rooms_bed",
-            },
-            "deviceSet": [],
-            "remoteLinks": ["3838120-12f0-256-9c63-bdf2dfg232"],
-        },
-    )
-
-
-def test_set_name(fake_controller: Controller, fake_client: FakeDirigeraHub) -> None:
-    new_name = "outofcontrol"
-    fake_controller.set_name(new_name)
-    action = fake_client.patch_actions.pop()
-    assert action["route"] == f"/devices/{fake_controller.id}"
-    assert action["data"] == [{"attributes": {"customName": new_name}}]
-    assert fake_controller.attributes.custom_name == new_name
-
-
-def test_dict_to_controller(fake_client: FakeDirigeraHub) -> None:
-    data: Dict[str, Any] = {
-        "id": "1237-343-2dfa",
-        "type": "controller",
-        "deviceType": "lightController",
-        "createdAt": "2023-01-07T20:07:19.000Z",
+@pytest.fixture(name="motion_sensor_dict")
+def fixture_motion_sensor_dict() -> Dict:
+    return {
+        "id": "62e95143-c8b6-4f28-b581-adfd622c0db7_1",
+        "type": "sensor",
+        "deviceType": "motionSensor",
+        "createdAt": "2023-12-14T18:28:57.000Z",
         "isReachable": True,
-        "lastSeen": "2023-10-28T04:42:15.000Z",
-        "customIcon": "lighting_nightstand_light",
+        "lastSeen": "2023-12-14T17:30:48.000Z",
         "attributes": {
-            "customName": "Remote",
-            "model": "TRADFRI STYRBAR",
+            "customName": "Bewegungssensor",
+            "firmwareVersion": "24.4.5",
+            "hardwareVersion": "1",
             "manufacturer": "IKEA of Sweden",
-            "firmwareVersion": "2.3.093",
-            "hardwareVersion": "2",
+            "model": "TRADFRI motion sensor",
+            "productCode": "E1745",
+            "serialNumber": "142D51FFFE229101",
+            "batteryPercentage": 100,
             "isOn": False,
-            "batteryPercentage": 90,
+            "lightLevel": 1,
+            "permittingJoin": False,
+            "otaPolicy": "autoUpdate",
+            "otaProgress": 0,
+            "otaScheduleEnd": "00:00",
+            "otaScheduleStart": "00:00",
+            "otaState": "readyToCheck",
+            "otaStatus": "upToDate",
+            "sensorConfig": {
+                "scheduleOn": False,
+                "onDuration": 120,
+                "schedule": {
+                    "onCondition": {"time": "sunset", "offset": -60},
+                    "offCondition": {"time": "sunrise", "offset": 60},
+                },
+            },
+            "circadianPresets": [],
         },
         "capabilities": {
             "canSend": ["isOn", "lightLevel"],
-            "canReceive": [
-                "customName",
-            ],
+            "canReceive": ["customName"],
         },
         "room": {
-            "id": "23g2w34-d0b7-42b3-a5a1-324zaerfg3",
-            "name": "Bedroom",
-            "color": "ikea_yellow_no_24",
-            "icon": "rooms_bed",
+            "id": "e1631a64-9ceb-4113-a6b3-1d866216503c",
+            "name": "Zimmer",
+            "color": "ikea_beige_1",
+            "icon": "rooms_arm_chair",
         },
         "deviceSet": [],
-        "remoteLinks": ["3838120-12f0-256-9c63-bdf2dfg232"],
+        "remoteLinks": [],
+        "isHidden": False,
     }
 
-    controller = dict_to_controller(data, fake_client)
-    assert controller.dirigera_client == fake_client
-    assert controller.id == data["id"]
-    assert controller.is_reachable == data["isReachable"]
-    assert controller.attributes.custom_name == data["attributes"]["customName"]
-    assert controller.attributes.is_on == data["attributes"]["isOn"]
+
+@pytest.fixture(name="fake_motion_sensor")
+def fixture_blind(
+    motion_sensor_dict: Dict, fake_client: FakeDirigeraHub
+) -> MotionSensor:
+    return MotionSensor(
+        dirigeraClient=fake_client,
+        **motion_sensor_dict,
+    )
+
+
+def test_set_motion_sensor_name(
+    fake_motion_sensor: MotionSensor, fake_client: FakeDirigeraHub
+) -> None:
+    new_name = "motion_sensor_name"
+    assert fake_motion_sensor.attributes.custom_name != new_name
+    fake_motion_sensor.set_name(new_name)
+    action = fake_client.patch_actions.pop()
+    assert action["route"] == f"/devices/{fake_motion_sensor.id}"
+    assert action["data"] == [{"attributes": {"customName": new_name}}]
+    assert fake_motion_sensor.attributes.custom_name == new_name
+
+
+def test_dict_to_blind(motion_sensor_dict: Dict, fake_client: FakeDirigeraHub) -> None:
+    motion_sensor = dict_to_motion_sensor(motion_sensor_dict, fake_client)
+    assert motion_sensor.dirigera_client == fake_client
+    assert motion_sensor.id == motion_sensor_dict["id"]
+    assert motion_sensor.is_reachable == motion_sensor_dict["isReachable"]
+    assert (
+        motion_sensor.attributes.custom_name
+        == motion_sensor_dict["attributes"]["customName"]
+    )
+    assert (
+        motion_sensor.attributes.battery_percentage
+        == motion_sensor_dict["attributes"]["batteryPercentage"]
+    )
+    assert motion_sensor.attributes.is_on == motion_sensor_dict["attributes"]["isOn"]
+    assert (
+        motion_sensor.attributes.light_level
+        == motion_sensor_dict["attributes"]["lightLevel"]
+    )
+    assert (
+        motion_sensor.capabilities.can_receive
+        == motion_sensor_dict["capabilities"]["canReceive"]
+    )
+    assert motion_sensor.room.id == motion_sensor_dict["room"]["id"]
+    assert motion_sensor.room.name == motion_sensor_dict["room"]["name"]
     assert (
-        controller.attributes.battery_percentage
-        == data["attributes"]["batteryPercentage"]
+        motion_sensor.attributes.firmware_version
+        == motion_sensor_dict["attributes"]["firmwareVersion"]
     )
-    assert controller.capabilities.can_receive == data["capabilities"]["canReceive"]
-    assert controller.room.id == data["room"]["id"]
-    assert controller.room.name == data["room"]["name"]
     assert (
-        controller.attributes.firmware_version == data["attributes"]["firmwareVersion"]
+        motion_sensor.attributes.hardware_version
+        == motion_sensor_dict["attributes"]["hardwareVersion"]
     )
+    assert motion_sensor.attributes.model == motion_sensor_dict["attributes"]["model"]
     assert (
-        controller.attributes.hardware_version == data["attributes"]["hardwareVersion"]
+        motion_sensor.attributes.manufacturer
+        == motion_sensor_dict["attributes"]["manufacturer"]
     )
-    assert controller.attributes.model == data["attributes"]["model"]
-    assert controller.attributes.manufacturer == data["attributes"]["manufacturer"]
```

### Comparing `dirigera-1.1.1/tests/test_environment_sensor.py` & `dirigera-1.1.2/tests/test_environment_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_light.py` & `dirigera-1.1.2/tests/test_light.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_open_close_sensor.py` & `dirigera-1.1.2/tests/test_open_close_sensor.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_outlet.py` & `dirigera-1.1.2/tests/test_outlet.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_scenes.py` & `dirigera-1.1.2/tests/test_scenes.py`

 * *Files identical despite different names*

### Comparing `dirigera-1.1.1/tests/test_utils.py` & `dirigera-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

