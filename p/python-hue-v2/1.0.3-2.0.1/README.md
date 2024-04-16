# Comparing `tmp/python_hue_v2-1.0.3.tar.gz` & `tmp/python_hue_v2-2.0.1.tar.gz`

## Comparing `python_hue_v2-1.0.3.tar` & `python_hue_v2-2.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.DS_Store
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/pytest.ini
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/hue-v2.iml
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/vcs.xml
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.vscode/settings.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/__init__.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/bridge.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/grouped_light.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/hue.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/light.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/mdns.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/resource_identifier_get.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/room.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/room/room_get.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/__init__.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/group.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/meta_data.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/scene.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/target.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/__init__.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_get.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_post.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_put.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/test_hue.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/tests/test_object_convert.py
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/LICENSE
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/README.md
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 python_hue_v2-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/pytest.ini
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/hue-v2.iml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/__init__.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/bridge.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/grouped_light.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/hue.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/light.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/mdns.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/room/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/room/resource_identifier_get.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/room/room.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/room/room_get.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/__init__.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/group.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/meta_data.py
+-rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/scene.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/target.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/action/__init__.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action_get.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action_post.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action_put.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/tests/test_hue.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/tests/test_hue_integration.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/tests/test_object_convert.py
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/LICENSE
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/README.md
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 python_hue_v2-2.0.1/PKG-INFO
```

### Comparing `python_hue_v2-1.0.3/.github/workflows/python-publish.yml` & `python_hue_v2-2.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/.idea/inspectionProfiles/Project_Default.xml` & `python_hue_v2-2.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/bridge.py` & `python_hue_v2-2.0.1/src/python_hue_v2/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,17 +146,17 @@
 
     def get_grouped_lights(self) -> List[dict]:
         return self._get(self._grouped_light_category)
 
     def get_grouped_light(self, grouped_light_id: str) -> dict:
         return self._get_by_id(self._grouped_light_category, grouped_light_id)
 
-    def set_grouped_light_service(self, grouped_light_id: str, property_name: str, property_value: dict) -> dict:
+    def set_grouped_light_service(self, grouped_light_id: str, properties: dict) -> dict:
         return self._put_by_id(self._grouped_light_category, grouped_light_id,
-                               properties={property_name: property_value})
+                               properties=properties)
 
     def get_devices(self):
         return self._get(self._device_category)
 
     def get_device(self, device_id: str):
         return self._get_by_id(self._device_category, device_id)
```

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/grouped_light.py` & `python_hue_v2-2.0.1/src/python_hue_v2/grouped_light.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,53 +15,68 @@
         return self._rtype
 
 
 class GroupedLight:
     """API to manage grouped light service, just one group
     Only supports HTTP PUT and GET method.
     """
+
     def __init__(self, bridge: Bridge, grouped_light_id: str):
         self.bridge = bridge
         self.grouped_light_id: str = grouped_light_id
 
     def _get(self):
         return self.bridge.get_grouped_light(self.grouped_light_id)
 
-    def _set(self, property_name: str, property_value: dict) -> dict:
+    def _set(self, properties: dict) -> dict:
         """_set is equal to HTTP PUT
 
         Arguments:
             property_name -- Property key like type, on, dimming, color_temperature, etc.
             property_value -- Value belong to key, it should be dict, refer to https://developers.meethue.com/develop/hue-api-v2/api-reference/#resource_grouped_light__id__put
 
         Returns:
             Response data, ResourceIdentifierPut, should be a dict for one id, not list
         """
-        return self.bridge.set_grouped_light_service(self.grouped_light_id, property_name, property_value)
+        return self.bridge.set_grouped_light_service(self.grouped_light_id, properties)
 
     @property
     def data_dict(self) -> dict:
         return self._get()
 
     @property
     def on(self) -> bool:
         return self._get()['on']['on']
 
     @on.setter
     def on(self, value: bool):
-        self._set('on', {'on': value})
+        self._set({'on': {'on': value}})
+
+    def set_state(self, on: bool, brightness: float = None, duration_ms: int = None):
+        """
+        Set the state of the grouped light
+        :param on: Boolean value to change the state of the grouped light
+        :param brightness: Group light brightness value
+        :param duration_ms: duration in dynamics
+        """
+        properties = {'on': {'on': on}}
+        if duration_ms:
+            properties['dynamics'] = {'duration': duration_ms}
+        if brightness:
+            properties['dimming'] = {'brightness': brightness}
+        self._set(properties)
 
     @property
     def type(self) -> str:
         return self._get()['type']
 
     @property
     def brightness(self) -> float:
         return self._get()['dimming']['brightness']
 
     @brightness.setter
     def brightness(self, value: float):
-        self._set('dimming', {'brightness': value})
+        self._set({'dimming': {'brightness': value}})
 
     @property
     def owner(self) -> Owner:
         return Owner(self.data_dict['owner'])
```

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/hue.py` & `python_hue_v2-2.0.1/src/python_hue_v2/hue.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/light.py` & `python_hue_v2-2.0.1/src/python_hue_v2/light.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/mdns.py` & `python_hue_v2-2.0.1/src/python_hue_v2/mdns.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/scene/scene.py` & `python_hue_v2-2.0.1/src/python_hue_v2/scene/scene.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action.py` & `python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_get.py` & `python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action_get.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/src/python_hue_v2/scene/action/action_post.py` & `python_hue_v2-2.0.1/src/python_hue_v2/scene/action/action_post.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/tests/test_hue.py` & `python_hue_v2-2.0.1/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/.gitignore` & `python_hue_v2-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/LICENSE` & `python_hue_v2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/README.md` & `python_hue_v2-2.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -108,20 +108,28 @@
 from python_hue_v2 import Hue
 
 hue = Hue('bridge-ip', 'app-key')
 grouped_lights = hue.grouped_lights
 
 for group in grouped_lights:
     print(group.type)
-    group.on = True
+    # group.on = True
+    group.set_state(True, 100, None) # Feature in 
+    group.set_state(on=True, brightness=100, duration_ms=1)
+    
 ```
 
 ## Low Level Control
 
-Also, you can use basic function in bridge class.
+> Low level function may be changed when update
+
+You can use some basic functions in this library. 
+
+For example, you can use `get_lights`,`set_light` or other low level control functions to implement
+some custom functions.
 
 ```python
 import time
 from python_hue_v2 import Hue
 
 # or hue = Hue('ip address','app-key')
 hue = Hue('host_name', 'hue app key')  # create Hue instance
@@ -133,10 +141,12 @@
 bridge.get_zones()
 ```
 
 ## Attention
 
 Some API may be de deprecated When major version updates.
 
+- Grouped light API will be changed after version `2.0.0`
+
 ## TODO
 
 - Zones Control Class
```

### Comparing `python_hue_v2-1.0.3/pyproject.toml` & `python_hue_v2-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_hue_v2-1.0.3/PKG-INFO` & `python_hue_v2-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: python-hue-v2
-Version: 1.0.3
+Version: 2.0.1
 Summary: A python library to control the Philips Hue lighting system.
 Project-URL: Documentation, https://github.com/FengChendian/python-hue-v2#readme
 Project-URL: Issues, https://github.com/FengChendian/python-hue-v2/issues
 Project-URL: Source, https://github.com/FengChendian/python-hue-v2
 Author-email: Yichen Zhao <njuzhaoyichen@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -131,20 +131,28 @@
 from python_hue_v2 import Hue
 
 hue = Hue('bridge-ip', 'app-key')
 grouped_lights = hue.grouped_lights
 
 for group in grouped_lights:
     print(group.type)
-    group.on = True
+    # group.on = True
+    group.set_state(True, 100, None) # Feature in 
+    group.set_state(on=True, brightness=100, duration_ms=1)
+    
 ```
 
 ## Low Level Control
 
-Also, you can use basic function in bridge class.
+> Low level function may be changed when update
+
+You can use some basic functions in this library. 
+
+For example, you can use `get_lights`,`set_light` or other low level control functions to implement
+some custom functions.
 
 ```python
 import time
 from python_hue_v2 import Hue
 
 # or hue = Hue('ip address','app-key')
 hue = Hue('host_name', 'hue app key')  # create Hue instance
@@ -156,10 +164,12 @@
 bridge.get_zones()
 ```
 
 ## Attention
 
 Some API may be de deprecated When major version updates.
 
+- Grouped light API will be changed after version `2.0.0`
+
 ## TODO
 
 - Zones Control Class
```

