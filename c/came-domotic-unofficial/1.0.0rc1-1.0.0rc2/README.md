# Comparing `tmp/came_domotic_unofficial-1.0.0rc1.tar.gz` & `tmp/came_domotic_unofficial-1.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "came_domotic_unofficial-1.0.0rc1.tar", max compression
+gzip compressed data, was "came_domotic_unofficial-1.0.0rc2.tar", max compression
```

## Comparing `came_domotic_unofficial-1.0.0rc1.tar` & `came_domotic_unofficial-1.0.0rc2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-03-11 21:08:36.821597 came_domotic_unofficial-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0     9596 2024-03-11 21:08:36.821819 came_domotic_unofficial-1.0.0rc1/README.rst
--rw-r--r--   0        0        0     2334 2024-03-11 21:08:36.822119 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/__init__.py
--rw-r--r--   0        0        0    31686 2024-03-11 21:08:36.822256 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/came_etidomo_server.py
--rw-r--r--   0        0        0     1273 2024-03-11 21:08:36.822474 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/__init__.py
--rw-r--r--   0        0        0     5189 2024-03-11 21:08:36.822600 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/came_entity.py
--rw-r--r--   0        0        0     8448 2024-03-11 21:08:36.822736 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/digital_input.py
--rw-r--r--   0        0        0     2732 2024-03-11 21:08:36.822826 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/enums.py
--rw-r--r--   0        0        0     2002 2024-03-11 21:08:36.822901 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/exceptions.py
--rw-r--r--   0        0        0     3545 2024-03-11 21:08:36.822983 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/feature.py
--rw-r--r--   0        0        0     1499 2024-03-11 21:08:36.823059 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/helpers.py
--rw-r--r--   0        0        0     5842 2024-03-11 21:08:36.823169 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/light.py
--rw-r--r--   0        0        0     6371 2024-03-11 21:08:36.823284 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/opening.py
--rw-r--r--   0        0        0     6760 2024-03-11 21:08:36.823437 came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/scenario.py
--rw-r--r--   0        0        0     2830 2024-03-27 22:25:55.162638 came_domotic_unofficial-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0    10935 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 19:31:00.797445 came_domotic_unofficial-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0     9596 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/README.rst
+-rw-r--r--   0        0        0     1633 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/__init__.py
+-rw-r--r--   0        0        0     8122 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/auth.py
+-rw-r--r--   0        0        0     3729 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/came_domotic_api.py
+-rwxr-xr-x   0        0        0      758 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/concat_models.zsh
+-rw-r--r--   0        0        0     1650 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/errors.py
+-rw-r--r--   0        0        0     4354 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models.py
+-rw-r--r--   0        0        0     1333 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/came_entity.py
+-rw-r--r--   0        0        0     8532 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/digital_input.py
+-rw-r--r--   0        0        0     2768 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/enums.py
+-rw-r--r--   0        0        0     2002 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/exceptions.py
+-rw-r--r--   0        0        0     3589 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/feature.py
+-rw-r--r--   0        0        0     1587 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/helpers.py
+-rw-r--r--   0        0        0     5930 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/light.py
+-rw-r--r--   0        0        0     6451 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/opening.py
+-rw-r--r--   0        0        0     6912 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/scenario.py
+-rw-r--r--   0        0        0     2854 2024-04-16 19:31:00.801445 came_domotic_unofficial-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    10933 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc2/PKG-INFO
```

### Comparing `came_domotic_unofficial-1.0.0rc1/LICENSE` & `came_domotic_unofficial-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc1/README.rst` & `came_domotic_unofficial-1.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/__init__.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     CameDomoticServerNotFoundError,
     CameDomoticAuthError,
     CameDomoticRemoteServerError,
     CameDomoticRequestError,
     CameDomoticBadAckError,
 )
 from .enums import (
-    EntityType,
-    EntityStatus,
-    LightType,
-    OpeningType,
-    DigitalInputType,
-    ScenarioStatus,
-    ScenarioIcon,
+    EntityType_OLD,
+    EntityStatus_OLD,
+    LightType_OLD,
+    OpeningType_OLD,
+    DigitalInputType_OLD,
+    ScenarioStatus_OLD,
+    ScenarioIcon_OLD,
 )
-from .came_entity import CameEntity, CameEntitySet
-from .feature import Feature, FeatureSet
-from .light import Light
-from .opening import Opening
-from .scenario import Scenario
-from .digital_input import DigitalInput
+from .came_entity import CameEntity_OLD, CameEntitySet_OLD
+from .feature import Feature_OLD, FeatureSet_OLD
+from .light import Light_OLD
+from .opening import Opening_OLD
+from .scenario import Scenario_OLD
+from .digital_input import DigitalInput_OLD
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/came_entity.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/came_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,35 @@
 Raises:
     TypeError: if the entity ID is not an integer.
 """
 
 
 from typing import Optional
 from .enums import (
-    EntityStatus,
+    EntityStatus_OLD,
 )
 
 
-class CameEntity:
+class CameEntity_OLD:
     """Base class for all the CAME entities.
 
     :property id: the entity ID.
     :property name: the entity name (default "Unknown" if None or empty).
     :property status: the entity status (default EntityStatus.NOT_APPLICABLE).
     """
 
     _DEFAULT_NAME = "Unknown"
-    _DEFAULT_STATUS = EntityStatus.UNKNOWN
+    _DEFAULT_STATUS = EntityStatus_OLD.UNKNOWN
 
     def __init__(
         self,
         entity_id: int,
         name: Optional[str] = _DEFAULT_NAME,
         *,
-        status: EntityStatus = _DEFAULT_STATUS,
+        status: EntityStatus_OLD = _DEFAULT_STATUS,
     ):
         """Constructor for the CameEntity class.
 
         :param id: the entity ID
         :param name: the entity name ("Unknown" if None or empty)
         :param status: the entity status (can be None for some entities)
 
@@ -59,15 +59,15 @@
         self._id = entity_id
         self._name = (
             name
             if name and isinstance(name, str) and name != ""
             else self._DEFAULT_NAME
         )
         self._status = (
-            status if status and status in EntityStatus else self._DEFAULT_STATUS
+            status if status and status in EntityStatus_OLD else self._DEFAULT_STATUS
         )
 
     @property
     def id(self) -> int:
         """
         Returns the entity ID.
         """
@@ -77,28 +77,28 @@
     def name(self) -> str:
         """
         Returns the entity name.
         """
         return self._name
 
     @property
-    def status(self) -> EntityStatus:
+    def status(self) -> EntityStatus_OLD:
         """Returns the entity status."""
         return self._status
 
     @status.setter
-    def status(self, value: EntityStatus):
+    def status(self, value: EntityStatus_OLD):
         """Sets the entity status.
 
         :param value: the entity status (EntityStatus)
 
         :raises TypeError: if the value is not a valid EntityStatus.
         """
         # Validate the input.
-        if value not in EntityStatus:
+        if value not in EntityStatus_OLD:
             raise TypeError("The entity status must be a valid EntityStatus")
 
         self._status = value
 
     def __str__(self) -> str:
         return (
             f"{type(self).__name__} #{self.id}: {self.name} - Status: "
@@ -134,32 +134,32 @@
         Any other JSON property (like floor_ind, room_ind) is ignored.
 
         :param json_data: the JSON dictionary representing the light.
 
         :raises KeyError: if the JSON dictionary doesn't contain the "act_id".
         """
 
-        return CameEntity(
+        return CameEntity_OLD(
             json_data["act_id"],
             (
                 json_data["name"]
                 if "name" in json_data and isinstance(json_data["name"], str)
-                else CameEntity._DEFAULT_NAME
+                else CameEntity_OLD._DEFAULT_NAME
             ),
             status=(
-                EntityStatus(json_data["status"])
+                EntityStatus_OLD(json_data["status"])
                 if "status" in json_data
                 and json_data["status"]
-                in EntityStatus._value2member_map_  # pylint: disable=protected-access
-                else CameEntity._DEFAULT_STATUS
+                in EntityStatus_OLD._value2member_map_  # pylint: disable=protected-access
+                else CameEntity_OLD._DEFAULT_STATUS
             ),
         )
 
 
-class CameEntitySet(set):
+class CameEntitySet_OLD(set):
     """Represents a set of CAME entities.
 
     :param entities: the list of entities to add to the set (optional).
 
     :method add: adds a CameEntity object to the set, validating its type.
 
     :raises TypeError: if the item is not of type CameEntity.
@@ -169,10 +169,10 @@
         super().__init__()
 
         if entities is not None:
             for entity in entities:
                 self.add(entity)
 
     def add(self, item):
-        if not isinstance(item, CameEntity):
+        if not isinstance(item, CameEntity_OLD):
             raise TypeError("Item must be of type 'CameEntity'")
         super().add(item)
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/digital_input.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/digital_input.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 """
 This module contains the DigitalInput class, which represents a CAME digital input 
 (e.g. a physical button).
 """
 
 from datetime import datetime, UTC
 from typing import Optional
-from .came_entity import CameEntity
-from .enums import DigitalInputType, EntityStatus
+from .came_entity import CameEntity_OLD
+from .enums import DigitalInputType_OLD, EntityStatus_OLD
 
 
-class DigitalInput(CameEntity):
+class DigitalInput_OLD(CameEntity_OLD):
     """Represents a CAME digital input (e.g. a button).
 
     The DigitalIn class is a subclass of the CameEntity class, and it's used to
     represent a CAME digital input (e.g. a button).
 
     :param entity_id: the digital input ID.
     :param name: the digital input name.
@@ -35,27 +35,27 @@
     :param address: the digital input address (default: 0).
     :param ack_code: the digital input ack code (default: 1).
     :param radio_node_id: radio node ID (default: "00000000").
     :param rf_radio_link_quality: radio link quality (default: 0).
     :param utc_time: the digital input UTC time offset (default: 0).
     """
 
-    _DEFAULT_BUTTON_TYPE = DigitalInputType.BUTTON
+    _DEFAULT_BUTTON_TYPE = DigitalInputType_OLD.BUTTON
     _DEFAULT_ADDRESS = 0
     _DEFAULT_ACK_CODE = 1
     _DEFAULT_RADIO_NODE_ID = "00000000"
     _DEFAULT_RF_RADIO_LINK_QUALITY = 0
     _DEFAULT_UTC_TIME = 0
 
     def __init__(
         self,
         entity_id: int,
-        name: Optional[str] = CameEntity._DEFAULT_NAME,
+        name: Optional[str] = CameEntity_OLD._DEFAULT_NAME,
         *,
-        button_type: DigitalInputType = _DEFAULT_BUTTON_TYPE,
+        button_type: DigitalInputType_OLD = _DEFAULT_BUTTON_TYPE,
         address: int = _DEFAULT_ADDRESS,
         ack_code: int = _DEFAULT_ACK_CODE,
         radio_node_id: str = _DEFAULT_RADIO_NODE_ID,
         rf_radio_link_quality: int = _DEFAULT_RF_RADIO_LINK_QUALITY,
         utc_time: int = _DEFAULT_UTC_TIME,
     ):
         """Constructor for the DigitalInput class.
@@ -67,15 +67,15 @@
             address (int, optional): address of the device. Defaults to 0.
             ack_code (int, optional): ack code of the device. Defaults to 1.
             radio_node_id (str, optional): radio_node_id. Defaults to "00000000".
             rf_radio_link_quality (int, optional): rf radio link quality. Defaults to 0.
             utc_time (int, optional): UNIX epoch of the last trigger of the device. Defaults to 0.
         """
         # Validate the input
-        if button_type not in DigitalInputType:
+        if button_type not in DigitalInputType_OLD:
             raise TypeError("The digital input type must be a valid DigitalInType")
         if address is not None and not isinstance(address, int):
             raise TypeError("The digital input address must be an integer")
         if ack_code is not None and not isinstance(ack_code, int):
             raise TypeError("The digital input ack code must be an integer")
         if radio_node_id is not None and not isinstance(radio_node_id, str):
             raise TypeError("The radio node ID must be a string")
@@ -92,20 +92,20 @@
         self._radio_node_id = radio_node_id
         self._rf_radio_link_quality = rf_radio_link_quality
         self._utc_time = utc_time
 
         super().__init__(
             entity_id,
             name,
-            status=EntityStatus.NOT_APPLICABLE,
+            status=EntityStatus_OLD.NOT_APPLICABLE,
         )
 
     # Properties
     @property
-    def button_type(self) -> DigitalInputType:
+    def button_type(self) -> DigitalInputType_OLD:
         """Returns the digital input type."""
         return self._button_type
 
     @property
     def address(self) -> int:
         """Returns the digital input address."""
         return self._address
@@ -171,47 +171,47 @@
         Any other JSON property (like floor_ind, room_ind) is ignored.
 
         :param json_data: the JSON dictionary representing the digital input
 
         :raises KeyError: if the JSON dictionary doesn't contain the "act_id"
         """
 
-        return DigitalInput(
+        return DigitalInput_OLD(
             entity_id=json_data["act_id"],
             name=(
                 json_data["name"]
                 if "name" in json_data and isinstance(json_data["name"], str)
-                else CameEntity._DEFAULT_NAME
+                else CameEntity_OLD._DEFAULT_NAME
             ),
             button_type=(
-                DigitalInputType(json_data["type"])
-                if "type" in json_data and json_data["type"] in DigitalInputType
-                else DigitalInput._DEFAULT_BUTTON_TYPE
+                DigitalInputType_OLD(json_data["type"])
+                if "type" in json_data and json_data["type"] in DigitalInputType_OLD
+                else DigitalInput_OLD._DEFAULT_BUTTON_TYPE
             ),
             address=(
                 json_data["addr"]
                 if "addr" in json_data and isinstance(json_data["addr"], int)
-                else DigitalInput._DEFAULT_ADDRESS
+                else DigitalInput_OLD._DEFAULT_ADDRESS
             ),
             ack_code=(
                 json_data["ack"]
                 if "ack" in json_data and isinstance(json_data["ack"], int)
-                else DigitalInput._DEFAULT_ACK_CODE
+                else DigitalInput_OLD._DEFAULT_ACK_CODE
             ),
             radio_node_id=(
                 json_data["radio_node_id"]
                 if "radio_node_id" in json_data
                 and isinstance(json_data["radio_node_id"], str)
-                else DigitalInput._DEFAULT_RADIO_NODE_ID
+                else DigitalInput_OLD._DEFAULT_RADIO_NODE_ID
             ),
             rf_radio_link_quality=(
                 json_data["rf_radio_link_quality"]
                 if "rf_radio_link_quality" in json_data
                 and isinstance(json_data["rf_radio_link_quality"], int)
-                else DigitalInput._DEFAULT_RF_RADIO_LINK_QUALITY
+                else DigitalInput_OLD._DEFAULT_RF_RADIO_LINK_QUALITY
             ),
             utc_time=(
                 json_data["utc_time"]
                 if "utc_time" in json_data and isinstance(json_data["utc_time"], int)
-                else DigitalInput._DEFAULT_UTC_TIME
+                else DigitalInput_OLD._DEFAULT_UTC_TIME
             ),
         )
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/enums.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from enum import Enum
 
 
 class CameEnum(Enum):
     """Base class for all the CAME-related enums."""
 
 
-class EntityType(CameEnum):
+class EntityType_OLD(CameEnum):
     """Enum listing all the CAME entity types.
 
     The :name of each enum member maps to feature.name.upper(),
     where 'feature' is a Feature instance.
 
     The :value of each enum member is the command to send to the remote server
     if you want to retrieve the list of items related to that entity type.
@@ -44,68 +44,68 @@
     # TIMERS = "timers_list_req"
     # THERMOREGULATION = "thermo_list_req"
     # ANALOGIN = "analogin_list_req"
     # USERS = "sl_users_list_req"
     # MAPS = "map_descr_req"
 
 
-class EntityStatus(CameEnum):
+class EntityStatus_OLD(CameEnum):
     """Enum listing all the status of the CAME entities."""
 
     OFF_STOPPED = 0
     ON_OPEN_TRIGGERED = 1
     CLOSED = 2
     UNKNOWN = -1
     NOT_APPLICABLE = -99
 
 
-class LightType(CameEnum):
+class LightType_OLD(CameEnum):
     """Enum listing the light types."""
 
     ON_OFF = "STEP_STEP"
     DIMMABLE = "DIMMER"
 
 
-class OpeningType(CameEnum):
+class OpeningType_OLD(CameEnum):
     """Enum listing the opening types."""
 
     OPEN_CLOSE = 0
 
 
-class DigitalInputType(CameEnum):
+class DigitalInputType_OLD(CameEnum):
     """Enum listing the digital input types."""
 
     BUTTON = 1
 
 
-class ScenarioIcon(CameEnum):
+class ScenarioIcon_OLD(CameEnum):
     """Enum listing the scenario icons."""
 
     LIGHTS = 14
     OPENINGS_OPEN = 22
     OPENINGS_CLOSE = 23
     UNKNOWN = -1
 
 
-class ScenarioStatus(CameEnum):
+class ScenarioStatus_OLD(CameEnum):
     """Enum listing the scenario status."""
 
     NOT_APPLIED = 0
     ONGOING = 1
     APPLIED = 2
 
 
-class SeasonSetting(Enum):
+class SeasonSetting_OLD(Enum):
     """Enum listing the available seasons settings."""
 
     PLANT_OFF = "off"
     WINTER = "winter"
     SUMMER = "summer"
 
 
-class ThermoZoneStatus(Enum):
+class ThermoZoneStatus_OLD(Enum):
     """Enum listing the available thermostat zone status."""
 
     OFF = 0
     MANUAL = 1
     AUTO = 2
     JOLLY = 3
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/exceptions.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/exceptions.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/feature.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module contains the class representing a CAME feature."""
 
-from .came_entity import CameEntity, CameEntitySet
-from .enums import EntityStatus
+from .came_entity import CameEntity_OLD, CameEntitySet_OLD
+from .enums import EntityStatus_OLD
 
 
-class Feature(CameEntity):
+class Feature_OLD(CameEntity_OLD):
     """Represents a CAME server feature.
 
     The Feature class is a subclass of the CameEntity class, and it's used to
     represent a CAME server feature. The feature name is used as the unique
     identifier for the feature, and it's used to generate the entity ID.
 
     :property name: the feature name.
@@ -37,15 +37,15 @@
         # Validate the input.
         if name is None or not isinstance(name, str) or name == "":
             raise TypeError("The feature name must be a non-empty string")
 
         super().__init__(
             entity_id=hash(name),  # Use an arbitrary ID, based on the name
             name=name,
-            status=EntityStatus.NOT_APPLICABLE,
+            status=EntityStatus_OLD.NOT_APPLICABLE,
         )
 
     @property
     def name(self) -> str:
         """Returns the feature name."""
         return self._name
 
@@ -64,24 +64,24 @@
     #     return not self.__eq__(other)
 
     # # Override the hash function
     # def __hash__(self):
     #     return hash((type(self), self.name))
 
 
-class FeatureSet(CameEntitySet):
+class FeatureSet_OLD(CameEntitySet_OLD):
     """Represents a set of features managed by a CAME ETI/Domo server.
 
     :method add: adds a Feature object to the set, validating its type.
 
     :raises TypeError: if the item is not of type Feature.
     """
 
     def add(self, item):
-        if not isinstance(item, Feature):
+        if not isinstance(item, Feature_OLD):
             raise TypeError("Item must be of type 'Feature'")
         super().add(item)
 
     @staticmethod
     def from_json(features_list: dict):
         """Creates a Feature object from a JSON dictionary.
 
@@ -98,8 +98,8 @@
         if not isinstance(features_list, list):
             raise TypeError("Input should be a list of strings.")
 
         # Ensure all elements in the list are strings
         if not all(isinstance(item, str) for item in features_list):
             raise ValueError("All elements in the list should be strings.")
 
-        return FeatureSet([Feature(feature) for feature in features_list])
+        return FeatureSet_OLD([Feature_OLD(feature) for feature in features_list])
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/helpers.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 
 
 """
 CAME Domotic helpers (enums, mappers, etc.)
 """
 
 from typing import Type
-from .came_entity import CameEntity
-from .feature import Feature
-from .light import Light
-from .opening import Opening
-from .digital_input import DigitalInput
-from .scenario import Scenario
-from .enums import EntityType
+from .came_entity import CameEntity_OLD
+from .feature import Feature_OLD
+from .light import Light_OLD
+from .opening import Opening_OLD
+from .digital_input import DigitalInput_OLD
+from .scenario import Scenario_OLD
+from .enums import EntityType_OLD
 
 
 # region Mappers
 
-_EntityType2Class: dict[EntityType, Type[CameEntity]] = {
-    EntityType.FEATURES: Feature,
-    EntityType.LIGHTS: Light,
-    EntityType.OPENINGS: Opening,
-    EntityType.DIGITALIN: DigitalInput,
-    EntityType.SCENARIOS: Scenario,
+_EntityType2Class: dict[EntityType_OLD, Type[CameEntity_OLD]] = {
+    EntityType_OLD.FEATURES: Feature_OLD,
+    EntityType_OLD.LIGHTS: Light_OLD,
+    EntityType_OLD.OPENINGS: Opening_OLD,
+    EntityType_OLD.DIGITALIN: DigitalInput_OLD,
+    EntityType_OLD.SCENARIOS: Scenario_OLD,
     # EntityType.UPDATE:
     # EntityType.RELAYS:
     # EntityType.CAMERAS:
     # EntityType.TIMERS:
     # EntityType.THERMOREGULATION:
     # EntityType.ANALOGIN:
     # EntityType.USERS:
     # EntityType.MAPS:
 }
 
 _Class2SwitchCommand = {
-    Light: "light_switch_req",
-    Opening: "opening_move_req",
-    Scenario: "scenario_activation_req",
+    Light_OLD: "light_switch_req",
+    Opening_OLD: "opening_move_req",
+    Scenario_OLD: "scenario_activation_req",
 }
 
 # endregion
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/light.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/light.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,58 +12,58 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module contains the class representing a CAME light."""
 
 
 from typing import Optional
-from .came_entity import CameEntity
-from .enums import EntityStatus, LightType
+from .came_entity import CameEntity_OLD
+from .enums import EntityStatus_OLD, LightType_OLD
 
 
-class Light(CameEntity):
+class Light_OLD(CameEntity_OLD):
     """Represents a CAME light.
 
     The Light class is a subclass of the CameEntity class, and it's used to
     represent a CAME light.
 
     :property id: the light ID.
     :property name: the light name (default: "Unknown").
     :property status: the light status (ON or OFF, default: UNKNOWN).
     :property light_type: the light type (ON_OFF or DIMMABLE, default: ON_OFF).
     :property brightness: the light brightness (range: 0-100, default: 100).
 
     :method from_json: create a Light object from a JSON dictionary.
     """
 
-    _DEFAULT_STATUS = EntityStatus.UNKNOWN
-    _DEFAULT_LIGHT_TYPE = LightType.ON_OFF
+    _DEFAULT_STATUS = EntityStatus_OLD.UNKNOWN
+    _DEFAULT_LIGHT_TYPE = LightType_OLD.ON_OFF
     _DEFAULT_BRIGHTNESS = 100
 
     def __init__(
         self,
         entity_id: int,
-        name: Optional[str] = CameEntity._DEFAULT_NAME,
+        name: Optional[str] = CameEntity_OLD._DEFAULT_NAME,
         *,
-        status: EntityStatus = _DEFAULT_STATUS,
-        light_type: LightType = _DEFAULT_LIGHT_TYPE,
+        status: EntityStatus_OLD = _DEFAULT_STATUS,
+        light_type: LightType_OLD = _DEFAULT_LIGHT_TYPE,
         brightness: int = _DEFAULT_BRIGHTNESS,
     ):
         """
         Constructor for the Came Light class.
 
         :param entity_id: the light ID.
         :param name: the light name.
         :param status: the light status (default: OFF).
         :param light_type: the light type (default: ON_OFF).
         :param brightness: the light brightness (range: 0-100, default: 100).
         """
 
         # Validate the input
-        if light_type not in LightType:
+        if light_type not in LightType_OLD:
             raise TypeError("The light type must be a valid LightType")
         if brightness is not None and not isinstance(brightness, int):
             raise TypeError("The brightness value must be an integer")
 
         self._light_type = light_type
 
         # Set brightness, with range from 0 to 100
@@ -95,25 +95,25 @@
         :raises ValueError: if the brightness value is not in the range 0-100
         """
         if value is None or value < 0 or value > 100:
             raise ValueError("The brightness value must be between 0 and 100")
         self._brightness = value
 
     @property
-    def light_type(self) -> LightType:
+    def light_type(self) -> LightType_OLD:
         """Returns the light type (ON_OFF or DIMMABLE)."""
         return self._light_type
 
     def __str__(self) -> str:
         result = (
             f"{type(self).__name__} #{self.id}: {self.name} - "
             f"Type: ({self.light_type.name}) - Status: {self.status.name}"
         )
 
-        if self.light_type == LightType.DIMMABLE:
+        if self.light_type == LightType_OLD.DIMMABLE:
             result += f" - Brightness: {self.brightness}"
 
         return result
 
     def __repr__(self) -> str:
         return (
             f'{type(self).__name__}({self.id},"{self.name}",'
@@ -142,34 +142,34 @@
 
         :param json_data: the JSON dictionary representing the light.
 
         :raises KeyError: if the JSON dictionary doesn't contain the "act_id".
         :raises TypeError: if some of the values are not valid.
         """
 
-        return Light(
+        return Light_OLD(
             json_data["act_id"],
             (
                 json_data["name"]
                 if "name" in json_data and isinstance(json_data["name"], str)
-                else CameEntity._DEFAULT_NAME
+                else CameEntity_OLD._DEFAULT_NAME
             ),
             status=(
-                EntityStatus(json_data["status"])
+                EntityStatus_OLD(json_data["status"])
                 if "status" in json_data
                 and json_data["status"]
-                in EntityStatus._value2member_map_  # pylint: disable=protected-access
-                else Light._DEFAULT_STATUS
+                in EntityStatus_OLD._value2member_map_  # pylint: disable=protected-access
+                else Light_OLD._DEFAULT_STATUS
             ),
             light_type=(
-                LightType(json_data["type"])
+                LightType_OLD(json_data["type"])
                 if "type" in json_data
                 and json_data["type"]
-                in LightType._value2member_map_  # pylint: disable=protected-access
-                else Light._DEFAULT_LIGHT_TYPE
+                in LightType_OLD._value2member_map_  # pylint: disable=protected-access
+                else Light_OLD._DEFAULT_LIGHT_TYPE
             ),
             brightness=(
                 min(max(json_data["perc"], 0), 100)
                 if "perc" in json_data and isinstance(json_data["perc"], int)
-                else Light._DEFAULT_BRIGHTNESS
+                else Light_OLD._DEFAULT_BRIGHTNESS
             ),
         )
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/opening.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/opening.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """This module contains the class representing a CAME opening."""
 
 from typing import Optional
-from .came_entity import CameEntity
-from .enums import EntityStatus, OpeningType
+from .came_entity import CameEntity_OLD
+from .enums import EntityStatus_OLD, OpeningType_OLD
 
 
-class Opening(CameEntity):
+class Opening_OLD(CameEntity_OLD):
     """Represents a CAME opening.
 
     The Opening class is a subclass of the CameEntity class, and it's used to
     represent a CAME opening (e.g. a cover).
 
     :property id: the opening ID.
     :property name: the opening name.
@@ -31,25 +31,25 @@
     :property opening_type: the opening type (OPEN_CLOSE).
     :property close_entity_id: the closing entity ID.
     :property partial_openings: the list of partial openings.
 
     :method from_json: create an Opening object from a JSON dictionary.
     """
 
-    _DEFAULT_STATUS = EntityStatus.UNKNOWN
-    _DEFAULT_OPENING_TYPE = OpeningType.OPEN_CLOSE
+    _DEFAULT_STATUS = EntityStatus_OLD.UNKNOWN
+    _DEFAULT_OPENING_TYPE = OpeningType_OLD.OPEN_CLOSE
 
     def __init__(
         self,
         entity_id: int,
-        name: Optional[str] = CameEntity._DEFAULT_NAME,
+        name: Optional[str] = CameEntity_OLD._DEFAULT_NAME,
         *,
-        status: EntityStatus = _DEFAULT_STATUS,
+        status: EntityStatus_OLD = _DEFAULT_STATUS,
         close_entity_id: Optional[int] = None,
-        opening_type: OpeningType = _DEFAULT_OPENING_TYPE,
+        opening_type: OpeningType_OLD = _DEFAULT_OPENING_TYPE,
         partial_openings: Optional[list] = None,
     ):
         """
         Constructor for the Came Opening class.
 
         :param entity_id: the opening ID.
         :param close_entity_id: the closing ID (default: same as entity_id).
@@ -58,15 +58,15 @@
         :param opening_type: the opening type (default: OPEN_CLOSE).
         :param partial_openings: the list of partial openings (default: empty).
         """
 
         # Input validation
         if close_entity_id is not None and not isinstance(close_entity_id, int):
             raise TypeError("The closing entity ID must be an integer")
-        if opening_type not in OpeningType:
+        if opening_type not in OpeningType_OLD:
             raise TypeError("The opening type must be a valid OpeningType")
         if partial_openings is not None and not isinstance(partial_openings, list):
             raise TypeError("The partial openings must be a list")
 
         self._close_entity_id = close_entity_id if close_entity_id else entity_id
         self._opening_type = (
             opening_type if opening_type else self._DEFAULT_OPENING_TYPE
@@ -77,15 +77,15 @@
             entity_id,
             name,
             status=status,
         )
 
     # Properties
     @property
-    def opening_type(self) -> OpeningType:
+    def opening_type(self) -> OpeningType_OLD:
         """Returns the cover type."""
         return self._opening_type
 
     @property
     def close_entity_id(self) -> int:
         """Returns the closing entity ID."""
         return self._close_entity_id
@@ -137,40 +137,40 @@
         Any other JSON property (like floor_ind, room_ind) is ignored.
 
         :param json_data: the JSON dictionary representing the opening.
 
         :raises KeyError: if the JSON dictionary doesn't contain the "open_act_id".
         """
 
-        return Opening(
+        return Opening_OLD(
             entity_id=json_data["open_act_id"],
             close_entity_id=(
                 json_data["close_act_id"]
                 if "close_act_id" in json_data
                 and isinstance(json_data["close_act_id"], int)
                 else json_data["open_act_id"]
             ),
             name=(
                 json_data["name"]
                 if "name" in json_data and isinstance(json_data["name"], str)
-                else CameEntity._DEFAULT_NAME
+                else CameEntity_OLD._DEFAULT_NAME
             ),
             status=(
-                EntityStatus(json_data["status"])
+                EntityStatus_OLD(json_data["status"])
                 if "status" in json_data
                 and json_data["status"]
-                in EntityStatus._value2member_map_  # pylint: disable=protected-access
-                else Opening._DEFAULT_STATUS
+                in EntityStatus_OLD._value2member_map_  # pylint: disable=protected-access
+                else Opening_OLD._DEFAULT_STATUS
             ),
             opening_type=(
-                OpeningType(json_data["type"])
+                OpeningType_OLD(json_data["type"])
                 if "type" in json_data
                 and json_data["type"]
-                in OpeningType._value2member_map_  # pylint: disable=protected-access
-                else Opening._DEFAULT_OPENING_TYPE
+                in OpeningType_OLD._value2member_map_  # pylint: disable=protected-access
+                else Opening_OLD._DEFAULT_OPENING_TYPE
             ),
             partial_openings=(
                 json_data["partial"]
                 if "partial" in json_data and isinstance(json_data["partial"], list)
                 else None
             ),
         )
```

### Comparing `came_domotic_unofficial-1.0.0rc1/came_domotic_unofficial/models/scenario.py` & `came_domotic_unofficial-1.0.0rc2/came_domotic_unofficial/models_OLD/scenario.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 This module contains the class representing a CAME scenario.
 
 Raises:
     TypeError: If not assigning to the scenario_status property a valid ScenarioStatus.
 """
 
 from typing import Optional
-from .came_entity import CameEntity
-from .enums import EntityStatus, ScenarioStatus, ScenarioIcon
+from .came_entity import CameEntity_OLD
+from .enums import EntityStatus_OLD, ScenarioStatus_OLD, ScenarioIcon_OLD
 
 
-class Scenario(CameEntity):
+class Scenario_OLD(CameEntity_OLD):
     """Represents a CAME predefined scenario.
 
     The Scenario class is a subclass of the CameEntity class, and it's used to
     represent a CAME predefined scenario.
 
     :property id: the scenario ID
     :property name: the scenario name. Defaults to "Unknown" if None or empty.
@@ -36,26 +36,26 @@
     :property scenario_status: the scenario status (NOT_APPLIED, ONGOING, APPLIED). Defaults to NOT_APPLIED
     :property icon: the scenario icon type. Defaults to UNKNOWN.
     :property is_user_defined: the scenario is user defined. Defaults to False.
 
     :method from_json: create a Scenario object from a JSON dictionary.
     """
 
-    _DEFAULT_STATUS = EntityStatus.UNKNOWN
-    _DEFAULT_SCENARIO_STATUS = ScenarioStatus.NOT_APPLIED
-    _DEFAULT_ICON_ID = ScenarioIcon.UNKNOWN
+    _DEFAULT_STATUS = EntityStatus_OLD.UNKNOWN
+    _DEFAULT_SCENARIO_STATUS = ScenarioStatus_OLD.NOT_APPLIED
+    _DEFAULT_ICON_ID = ScenarioIcon_OLD.UNKNOWN
 
     def __init__(
         self,
         entity_id: int,
-        name: Optional[str] = CameEntity._DEFAULT_NAME,
+        name: Optional[str] = CameEntity_OLD._DEFAULT_NAME,
         *,
-        status: EntityStatus = _DEFAULT_STATUS,
-        scenario_status: ScenarioStatus = _DEFAULT_SCENARIO_STATUS,
-        icon: ScenarioIcon = _DEFAULT_ICON_ID,
+        status: EntityStatus_OLD = _DEFAULT_STATUS,
+        scenario_status: ScenarioStatus_OLD = _DEFAULT_SCENARIO_STATUS,
+        icon: ScenarioIcon_OLD = _DEFAULT_ICON_ID,
         is_user_defined: bool = False,
     ):
         """
         Constructor for the Came Scenario class.
 
         Args:
             entity_id (int): the scenario ID.
@@ -63,17 +63,17 @@
             status (EntityStatus, optional): the scenario status. Defaults to UNKNOWN.
             scenario_status (ScenarioStatus, optional): the scenario status. Defaults to NOT_APPLIED.
             icon (ScenarioIcon, optional): the scenario icon type. Defaults to UNKNOWN.
             is_user_defined (bool, optional): whether the scenario is user defined. Defaults to False.
         """
 
         # Validate the input
-        if scenario_status not in ScenarioStatus:
+        if scenario_status not in ScenarioStatus_OLD:
             raise TypeError("The scenario status must be a valid ScenarioStatus")
-        if icon not in ScenarioIcon:
+        if icon not in ScenarioIcon_OLD:
             raise TypeError("The scenario icon must be a valid ScenarioIcon")
         if is_user_defined is not None and not isinstance(is_user_defined, bool):
             raise TypeError("The is_user_defined value must be a boolean")
 
         self._scenario_status = scenario_status
         self._icon = icon
         self._is_user_defined = is_user_defined
@@ -82,35 +82,35 @@
             entity_id,
             name,
             status=status,
         )
 
     # Properties
     @property
-    def scenario_status(self) -> ScenarioStatus:
+    def scenario_status(self) -> ScenarioStatus_OLD:
         """Returns the scenario status (NOT_APPLIED, ONGOING, APPLIED)."""
         return self._scenario_status
 
     @scenario_status.setter
-    def scenario_status(self, value: ScenarioStatus):
+    def scenario_status(self, value: ScenarioStatus_OLD):
         """Sets the scenario status.
 
         Args:
             value (ScenarioStatus): the scenario status.
 
         Raises:
             TypeError: if the value is not a valid ScenarioStatus.
         """
-        if value not in ScenarioStatus:
+        if value not in ScenarioStatus_OLD:
             raise TypeError("The scenario status must be a valid ScenarioStatus")
 
         self._scenario_status = value
 
     @property
-    def icon(self) -> ScenarioIcon:
+    def icon(self) -> ScenarioIcon_OLD:
         """Returns the scenario icon type."""
         return self._icon
 
     @property
     def is_user_defined(self) -> bool:
         """Returns whether the scenario is user defined or not."""
         return self._is_user_defined
@@ -151,34 +151,36 @@
         Any other JSON property (like floor_ind, room_ind) is ignored.
 
         :param json_data: the JSON dictionary representing the scenario.
 
         :raises KeyError: if the JSON dictionary doesn't contain the "id".
         """
 
-        return Scenario(
+        return Scenario_OLD(
             entity_id=json_data["id"],
             name=(
-                json_data["name"] if "name" in json_data else CameEntity._DEFAULT_NAME
+                json_data["name"]
+                if "name" in json_data
+                else CameEntity_OLD._DEFAULT_NAME
             ),
             status=(
-                EntityStatus(json_data["status"])
-                if "status" in json_data and json_data["status"] in EntityStatus
-                else Scenario._DEFAULT_STATUS
+                EntityStatus_OLD(json_data["status"])
+                if "status" in json_data and json_data["status"] in EntityStatus_OLD
+                else Scenario_OLD._DEFAULT_STATUS
             ),
             scenario_status=(
-                ScenarioStatus(json_data["scenario_status"])
+                ScenarioStatus_OLD(json_data["scenario_status"])
                 if "scenario_status" in json_data
-                and json_data["scenario_status"] in ScenarioStatus
-                else Scenario._DEFAULT_SCENARIO_STATUS
+                and json_data["scenario_status"] in ScenarioStatus_OLD
+                else Scenario_OLD._DEFAULT_SCENARIO_STATUS
             ),
             icon=(
-                ScenarioIcon(json_data["icon_id"])
-                if "icon_id" in json_data and json_data["icon_id"] in ScenarioIcon
-                else Scenario._DEFAULT_ICON_ID
+                ScenarioIcon_OLD(json_data["icon_id"])
+                if "icon_id" in json_data and json_data["icon_id"] in ScenarioIcon_OLD
+                else Scenario_OLD._DEFAULT_ICON_ID
             ),
             is_user_defined=(
                 bool(json_data["user-defined"])
                 if "user-defined" in json_data
                 and isinstance(json_data["user-defined"], int)
                 else False
             ),
```

### Comparing `came_domotic_unofficial-1.0.0rc1/pyproject.toml` & `came_domotic_unofficial-1.0.0rc2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 [tool.poetry]
 name = "came_domotic_unofficial"
-version = "1.0.0rc1"
+version = "1.0.0rc2"
 description = "Python library to interact with a CAME ETI/Domo domotic server."
 license = "Apache-2.0"
 authors = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 maintainers = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 readme = "README.rst"
 
 homepage = "https://github.com/camedomotic-unofficial/came_domotic_unofficial"
@@ -47,31 +47,31 @@
 packages = [{ include = "came_domotic_unofficial" }]
 
 [tool.poetry.urls]
 "Bug tracker" = "https://github.com/camedomotic-unofficial/came_domotic_unofficial/issues"
 
 [tool.poetry.dependencies]
 python = '^3.12'
-requests = '^2.31.0'
+aiohttp = '^3.9.3'
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
 freezegun = '^1.4.0'
 hypothesis = '^6.98.17'
 pytest = '^8.0.2'
-pytest-cov = '^4.1.0'
+pytest-cov = '>=4.1,<6.0'
 pytest-timeout = '^2.3.1'
 
 [tool.poetry.group.code-quality]
 optional = true
 
 [tool.poetry.group.code-quality.dependencies]
-black = '^24.2.0'
+black = '^24.3.0'
 pylint = '^3.1.0'
 mypy = '^1.8.0'
 types-requests = '^2.31.0'
 
 [tool.poetry.group.docs]
 optional = true
 
@@ -81,14 +81,15 @@
 readthedocs-sphinx-search = "^0.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
+asyncio_mode = "auto"
 addopts = "--timeout=10"
 # addopts = "--timeout=10 --cov=came_domotic_unofficial --cov-report=term-missing --cov-report=html"
 
 [tool.coverage.run]
 omit = [
     "came_domotic_unofficial/_version.py", # Ignore: it is autogenerated by setuptools_scm
 ]
```

### Comparing `came_domotic_unofficial-1.0.0rc1/PKG-INFO` & `came_domotic_unofficial-1.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: came_domotic_unofficial
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: Python library to interact with a CAME ETI/Domo domotic server.
 Home-page: https://github.com/camedomotic-unofficial/came_domotic_unofficial
 License: Apache-2.0
 Keywords: CAME,ETI/Domo,domotic,home automation,home assistant,home-assistant
 Author: camedomotic-unofficial
 Author-email: camedomotic-unofficial@gmail.com
 Maintainer: camedomotic-unofficial
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Project-URL: Bug tracker, https://github.com/camedomotic-unofficial/came_domotic_unofficial/issues
 Project-URL: Documentation, https://came-domotic-unofficial.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/camedomotic-unofficial/came_domotic_unofficial.git
 Description-Content-Type: text/x-rst
 
 .. Copyright 2024 - GitHub user: fredericks1982
```

