# Comparing `tmp/webthing_client-0.2.7.tar.gz` & `tmp/webthing_client-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webthing_client-0.2.7.tar", max compression
+gzip compressed data, was "webthing_client-0.2.8.tar", max compression
```

## Comparing `webthing_client-0.2.7.tar` & `webthing_client-0.2.8.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.7/LICENSE
--rw-r--r--   0        0        0      629 2024-04-02 11:11:27.210775 webthing_client-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.7/webthing_client/__init__.py
--rw-r--r--   0        0        0    24696 2024-04-02 09:28:40.558278 webthing_client-0.2.7/webthing_client/client.py
--rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.7/webthing_client/input/action/event_input.py
--rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.7/webthing_client/input/action/event_type_input.py
--rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.7/webthing_client/input/action/from_to_user_input.py
--rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.7/webthing_client/input/action/iri_user_input.py
--rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.7/webthing_client/input/action/resolution_input.py
--rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.7/webthing_client/input/from_to_input.py
--rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.7/webthing_client/input/iri_input.py
--rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.7/webthing_client/input/property_observations_input.py
--rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.7/webthing_client/model/action/action.py
--rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.7/webthing_client/model/action/base.py
--rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.7/webthing_client/model/action/operation/operation.py
--rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.7/webthing_client/model/action/request.py
--rw-r--r--   0        0        0     2303 2024-04-02 09:37:23.149678 webthing_client-0.2.7/webthing_client/model/action/resolution.py
--rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.7/webthing_client/model/event/event.py
--rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.7/webthing_client/model/event/event_type.py
--rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.7/webthing_client/model/event/feedback.py
--rw-r--r--   0        0        0     2792 2024-03-07 14:05:26.244036 webthing_client-0.2.7/webthing_client/model/event/feedback_schema.py
--rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.7/webthing_client/model/event/observation.py
--rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.7/webthing_client/model/event/stimulus.py
--rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.7/webthing_client/model/ontology.py
--rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.7/webthing_client/model/property/observable_property.py
--rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.7/webthing_client/model/system/sensor.py
--rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.7/webthing_client/model/system/system.py
--rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.7/webthing_client/model/user/user.py
--rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.7/webthing_client/model/webthing_observation.py
--rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.7/webthing_client/standard_api/__init__.py
--rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.7/webthing_client/standard_api/api_handler.py
--rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.7/webthing_client/standard_api/api_marshalling.py
--rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.7/webthing_client/stomp.py
--rw-r--r--   0        0        0     1552 2024-03-05 12:21:27.646974 webthing_client-0.2.7/webthing_client/utils.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1649 2023-02-06 09:57:29.936975 webthing_client-0.2.8/LICENSE
+-rw-r--r--   0        0        0      629 2024-04-16 07:02:16.402645 webthing_client-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-09-01 06:19:20.858836 webthing_client-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2023-09-01 06:19:20.859837 webthing_client-0.2.8/webthing_client/__init__.py
+-rw-r--r--   0        0        0    32194 2024-04-16 06:52:52.447000 webthing_client-0.2.8/webthing_client/client.py
+-rw-r--r--   0        0        0     1110 2024-02-25 09:18:17.801821 webthing_client-0.2.8/webthing_client/input/action/event_input.py
+-rw-r--r--   0        0        0      559 2024-02-25 09:18:25.339336 webthing_client-0.2.8/webthing_client/input/action/event_type_input.py
+-rw-r--r--   0        0        0      552 2024-02-28 12:31:21.667211 webthing_client-0.2.8/webthing_client/input/action/from_to_user_input.py
+-rw-r--r--   0        0        0      335 2024-02-25 09:18:47.773047 webthing_client-0.2.8/webthing_client/input/action/iri_user_input.py
+-rw-r--r--   0        0        0      958 2024-02-25 09:50:00.172735 webthing_client-0.2.8/webthing_client/input/action/resolution_input.py
+-rw-r--r--   0        0        0      501 2024-02-28 12:31:21.674209 webthing_client-0.2.8/webthing_client/input/from_to_input.py
+-rw-r--r--   0        0        0      284 2024-02-25 09:17:40.428692 webthing_client-0.2.8/webthing_client/input/iri_input.py
+-rw-r--r--   0        0        0      573 2024-02-29 08:15:42.300381 webthing_client-0.2.8/webthing_client/input/property_observations_input.py
+-rw-r--r--   0        0        0     1262 2024-04-11 11:55:16.307929 webthing_client-0.2.8/webthing_client/input/replay/replay_input.py
+-rw-r--r--   0        0        0     1497 2024-03-07 08:08:34.615412 webthing_client-0.2.8/webthing_client/model/action/action.py
+-rw-r--r--   0        0        0      483 2024-02-25 08:39:10.164817 webthing_client-0.2.8/webthing_client/model/action/base.py
+-rw-r--r--   0        0        0     5769 2024-03-07 08:10:40.389847 webthing_client-0.2.8/webthing_client/model/action/operation/operation.py
+-rw-r--r--   0        0        0     1354 2024-03-07 08:09:59.699008 webthing_client-0.2.8/webthing_client/model/action/request.py
+-rw-r--r--   0        0        0     2303 2024-04-02 09:37:23.149678 webthing_client-0.2.8/webthing_client/model/action/resolution.py
+-rw-r--r--   0        0        0     2576 2024-03-08 10:35:26.561490 webthing_client-0.2.8/webthing_client/model/event/event.py
+-rw-r--r--   0        0        0     2167 2024-03-07 08:11:29.041992 webthing_client-0.2.8/webthing_client/model/event/event_type.py
+-rw-r--r--   0        0        0     1078 2024-02-25 09:10:43.844340 webthing_client-0.2.8/webthing_client/model/event/feedback.py
+-rw-r--r--   0        0        0     2792 2024-03-07 14:05:26.244036 webthing_client-0.2.8/webthing_client/model/event/feedback_schema.py
+-rw-r--r--   0        0        0      845 2024-02-28 12:31:21.667211 webthing_client-0.2.8/webthing_client/model/event/observation.py
+-rw-r--r--   0        0        0     1276 2024-02-23 16:53:39.147090 webthing_client-0.2.8/webthing_client/model/event/stimulus.py
+-rw-r--r--   0        0        0      125 2024-03-07 08:09:17.428059 webthing_client-0.2.8/webthing_client/model/ontology.py
+-rw-r--r--   0        0        0      591 2024-02-29 09:01:40.135207 webthing_client-0.2.8/webthing_client/model/property/observable_property.py
+-rw-r--r--   0        0        0     3781 2024-04-16 06:59:05.967785 webthing_client-0.2.8/webthing_client/model/replay/replay.py
+-rw-r--r--   0        0        0      871 2024-02-25 08:42:01.491567 webthing_client-0.2.8/webthing_client/model/system/sensor.py
+-rw-r--r--   0        0        0      890 2024-02-25 08:41:34.495865 webthing_client-0.2.8/webthing_client/model/system/system.py
+-rw-r--r--   0        0        0     1635 2024-03-07 08:12:27.305511 webthing_client-0.2.8/webthing_client/model/user/user.py
+-rw-r--r--   0        0        0      900 2024-02-28 12:31:21.670210 webthing_client-0.2.8/webthing_client/model/webthing_observation.py
+-rw-r--r--   0        0        0        0 2021-11-19 14:10:06.477733 webthing_client-0.2.8/webthing_client/standard_api/__init__.py
+-rw-r--r--   0        0        0     9996 2023-06-07 11:34:51.827080 webthing_client-0.2.8/webthing_client/standard_api/api_handler.py
+-rw-r--r--   0        0        0     1651 2021-11-29 12:35:22.731824 webthing_client-0.2.8/webthing_client/standard_api/api_marshalling.py
+-rw-r--r--   0        0        0     6354 2024-03-20 12:02:38.241459 webthing_client-0.2.8/webthing_client/stomp.py
+-rw-r--r--   0        0        0     1897 2024-04-11 10:57:32.328600 webthing_client-0.2.8/webthing_client/utils.py
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 webthing_client-0.2.8/PKG-INFO
```

### Comparing `webthing_client-0.2.7/LICENSE` & `webthing_client-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/pyproject.toml` & `webthing_client-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webthing-client"
-version = "0.2.7"
+version = "0.2.8"
 description = "Client for the Dynamic Dashboard Webthings"
 authors = ["Emile Deman"]
 maintainers = [
     "Emile Deman <emile.deman@ugent.be>",
 	"Stef Pletinck <s@stefpletinck.be>"
 ]
 readme = "README.md"
```

### Comparing `webthing_client-0.2.7/webthing_client/client.py` & `webthing_client-0.2.8/webthing_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from datetime import datetime
 import json
 from typing import *
+from rdflib import Graph
 import requests
 
 from .standard_api.api_handler import ApiRequester
 
 from .input.iri_input import IRIInput
 from .input.from_to_input import FromToInput
 from .input.property_observations_input import PropertyObservationsInput
 from .input.action.from_to_user_input import FromToUserInput
 from .input.action.event_input import CreateEventInput, UpdateEventInput
 from .input.action.event_type_input import UpdateEventTypeInput
 from .input.action.iri_user_input import IRIUserInput
 from .input.action.resolution_input import ResolutionInput
+from .input.replay.replay_input import ReplayInput
 from .model.webthing_observation import WebthingObservation
 from .model.event.event import Event
 from .model.event.stimulus import Stimulus
 from .model.event.feedback import Feedback
 from .model.event.feedback_schema import FeedbackSchema
 from .model.event.event_type import EventType
 from .model.action.action import Action
 from .model.action.request import Request
 from .model.action.operation.operation import Operation, CreateEventOperation, UpdateEventOperation, DeleteEventOperation, UpdateEventTypeOperation
 from .model.action.resolution import Resolution, VerdictResultType
 from .model.user.user import User
+from .model.property.observable_property import ObservableProperty
+from .model.system.sensor import Sensor
+from .model.system.system import System
+from .model.replay.replay import Replay
 
 from .stomp import StompWebsocket
-from .utils import encode_uri_component
+from .utils import encode_uri_component, jsonld_object_to_graph
 
 
 class WebthingClient:
     """Client for interacting with a Webthing."""
 
     def __init__(self, webthing_fqdn: str, user_iri: Optional[str]=None, secure: bool=True, websocket: bool=True):
         """
@@ -107,14 +113,93 @@
         """Subscribe to realtime Resolutions.
 
         Args:
             callback (Callable[[Resolution], None]): Callback for new Resolutions.
         """
         self._ws.subscribe('/resolutions', lambda json_str: callback(Resolution.from_json_object(json.loads(json_str))))
 
+    def get_property(self, property_iri: str) -> ObservableProperty:
+        """Get ObservableProperty with IRI.
+
+        Args:
+            property_iri (str): IRI of property.
+
+        Returns:
+            ObservableProperty: ObservableProperty
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('get_property',
+            IRIInput.to_json_object(property_iri))
+        return ObservableProperty.from_json_object(json_object)
+    
+    def get_property_graph(self, property_iri: str) -> Graph:
+        """Get ObservableProperty with IRI.
+
+        Args:
+            property_iri (str): IRI of property.
+
+        Returns:
+            Graph: ObservableProperty as Graph
+        """
+        jsonld: Dict[str, Any] = self._api_requester.call('get_property',
+            IRIInput.to_json_object(property_iri))
+        return jsonld_object_to_graph(jsonld)
+    
+    def get_properties(self) -> List[ObservableProperty]:
+        """Get all ObservableProperties.
+
+        Returns:
+            List[ObservableProperty]: ObservableProperties
+        """
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_properties', {})
+        return [ObservableProperty.from_json_object(property_object) for property_object in json_array]
+    
+    def get_sensor(self, sensor_iri: str) -> Sensor:
+        """Get Sensor with IRI.
+
+        Args:
+            sensor_iri (str): IRI of sensor.
+
+        Returns:
+            ObservableSensor: Sensor
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('get_sensor',
+            IRIInput.to_json_object(sensor_iri))
+        return Sensor.from_json_object(json_object)
+    
+    def get_sensors(self) -> List[Sensor]:
+        """Get all Sensors.
+
+        Returns:
+            List[ObservableSensor]: Sensors
+        """
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_sensors', {})
+        return [Sensor.from_json_object(sensor_object) for sensor_object in json_array]
+    
+    def get_system(self, system_iri: str) -> System:
+        """Get System with IRI.
+
+        Args:
+            system_iri (str): IRI of system.
+
+        Returns:
+            ObservableSystem: System
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('get_system',
+            IRIInput.to_json_object(system_iri))
+        return System.from_json_object(json_object)
+    
+    def get_systems(self) -> List[System]:
+        """Get all Systems.
+
+        Returns:
+            List[ObservableSystem]: Systems
+        """
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_systems', {})
+        return [System.from_json_object(system_object) for system_object in json_array]
+
     def get_event(self, event_iri: str) -> Event:
         """Get event with IRI.
 
         Args:
             event_iri (str): IRI of event.
 
         Returns:
@@ -133,14 +218,40 @@
         Returns:
             Event: Event.
         """
         json_object: Dict[str, Any] = self._api_requester.call('get_event_user_view',
             IRIUserInput.to_json_object(user_iri, event_iri))
         return Event.from_json_object(json_object)
     
+    def get_event_graph(self, event_iri: str) -> Graph:
+        """Get event with IRI.
+
+        Args:
+            event_iri (str): IRI of event.
+
+        Returns:
+            Graph: Event as Graph.
+        """
+        jsonld: Dict[str, Any] = self._api_requester.call('get_event_jsonld',
+            IRIInput.to_json_object(event_iri))
+        return jsonld_object_to_graph(jsonld)
+    
+    def get_event_user_view_graph(self, event_iri: str) -> Graph:
+        """Get event with IRI as provided user.
+
+        Args:
+            event_iri (str): IRI of event.
+
+        Returns:
+            Graph: Event as Graph.
+        """
+        jsonld: Dict[str, Any] = self._api_requester.call('get_event_user_view_jsonld',
+            IRIInput.to_json_object(event_iri))
+        return jsonld_object_to_graph(jsonld)
+    
     def get_event_self_view(self, event_iri: str) -> Event:
         """Get event with view as user set in client.
 
         Args:
             event_iri (str): The IRI
         Returns:
             Event: Event.
@@ -153,15 +264,15 @@
         Args:
             from_ (Optional[datetime], optional): From time. Defaults to None.
             to (Optional[datetime], optional): To time. Defaults to None.
 
         Returns:
             List[Event]: Events in range.
         """
-        json_array: Dict[str, Any] = self._api_requester.call('get_events',
+        json_array: List[Dict[str, Any]] = self._api_requester.call('get_events',
             FromToInput.to_json_object(from_, to))
         return [Event.from_json_object(event_object) for event_object in json_array]
     
     def get_events_user_view(self, user_iri: str, from_: Optional[datetime]=None, to: Optional[datetime]=None) -> List[Event]:
         """Get all events as user in optional range.
 
         Args:
@@ -477,14 +588,23 @@
             if request.iri == accapted_request_iri:
                 operation = request.operation
                 verdicts[request.iri] = VerdictResultType.ACCEPTED
             else:
                 verdicts[request.iri] = VerdictResultType.REJECTED
         return self.create_resolution(verdicts, operation)
     
+    def get_users(self) -> List[User]:
+        """Get all the users.
+
+        Returns:
+            List[User]: Users
+        """
+        json_array = List[Dict[str, Any]] = self._api_requester.call('get_user', {})
+        return [User.from_json_object(user_object) for user_object in json_array]
+    
     def get_user(self, user_iri: str) -> User:
         """Get the User associated with the IRI.
 
         Args:
             user_iri (str): User IRI
 
         Returns:
@@ -584,7 +704,75 @@
                                                     data=graph.encode('utf-8'))
         return response.text
 
     def reload(self) -> None:
         """Reload the webthing.
         """
         requests.Response = requests.get(self._webthing_url + "/admin/reload")
+
+
+class WebthingReplayClient:
+    """Class for replay endpoints on webthing."""
+
+    def __init__(self, webthing_fqdn: str, secure: bool=True):
+        """Client for replay endpoints.
+
+        Args:
+            webthing_fqdn (str): The fully quallified domain name e.g. 'webthing.example.com'.
+            secure (bool, optional):  If the Webthing uses TLS (https). Defaults to True.
+        """
+        self._webthing_fqdn: str = webthing_fqdn.strip('/')
+        self._secure: bool = secure
+
+        if self._secure:
+            self._webthing_url = f"https://{self._webthing_fqdn}"
+        else:
+            self._webthing_url = f"http://{self._webthing_fqdn}"
+
+        self._api_requester = ApiRequester(self._webthing_url)
+
+    def set_replay(self, from_historical: datetime,
+                         to_historical: datetime,
+                         from_replay: Optional[datetime] = None,
+                         speed_multiplier: Optional[float] = None,
+                         loop: Optional[bool] = None,
+                         scale_timestamps: Optional[bool] = None,
+                         seconds_interval: Optional[int] = None,
+                         replay_semantic_submissions_user_iris: Optional[List[str]] = None) -> Replay:
+        """Set the paramaters for replay.
+
+        Args:
+            from_historical (datetime): The historical window from.
+            to_historical (datetime): The historical window to.
+            from_replay (datetime): The current replay window from. Defaults to now.
+            speed_multiplier (Optional[float], optional): The approximate multiplier to speed up or slow down. Defaults to 1.
+            loop (Optional[bool], optional): Indicating if the replay is finished it should restart. Defaults to False.
+            scale_timestamps (Optional[bool], optional): If the transformed historical timestamps should be scaled depending on speed, if true will change the difference between timestamps,
+                if false will just move timestamps in time by the difference between historical and replay windows. Defaults to True.
+            seconds_interval (Optional[int], optional): The polling interval to use. Defaults to 5 seconds.
+            replay_semantic_submissions_user_iris (Optional[List[str]], optional): The IRI's of the users whose semantic submissions (requests,actions,resolutions) we must replay. Defaults to no users.
+
+        Returns:
+            Replay: The replay status.
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('replay/set',
+            ReplayInput.to_json_object(from_historical, to_historical, from_replay, speed_multiplier,
+                                       loop, scale_timestamps, seconds_interval, replay_semantic_submissions_user_iris))
+        return Replay.from_json_object(json_object)
+
+    def start_replay(self) -> Replay:
+        """Start the replay form set parameters.
+
+        Returns:
+            Replay: The replay status.
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('replay/start', {})
+        return Replay.from_json_object(json_object)
+    
+    def stop_replay(self) -> Replay:
+        """Stop the replay.
+
+        Returns:
+            Replay: The replay status.
+        """
+        json_object: Dict[str, Any] = self._api_requester.call('replay/stop', {})
+        return Replay.from_json_object(json_object)
```

### Comparing `webthing_client-0.2.7/webthing_client/input/action/event_input.py` & `webthing_client-0.2.8/webthing_client/input/action/event_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/input/action/event_type_input.py` & `webthing_client-0.2.8/webthing_client/input/action/event_type_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/input/action/from_to_user_input.py` & `webthing_client-0.2.8/webthing_client/input/action/from_to_user_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/input/action/resolution_input.py` & `webthing_client-0.2.8/webthing_client/input/action/resolution_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/input/property_observations_input.py` & `webthing_client-0.2.8/webthing_client/input/property_observations_input.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/action/action.py` & `webthing_client-0.2.8/webthing_client/model/action/action.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/action/operation/operation.py` & `webthing_client-0.2.8/webthing_client/model/action/operation/operation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/action/request.py` & `webthing_client-0.2.8/webthing_client/model/action/request.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/action/resolution.py` & `webthing_client-0.2.8/webthing_client/model/action/resolution.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/event.py` & `webthing_client-0.2.8/webthing_client/model/event/event.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/event_type.py` & `webthing_client-0.2.8/webthing_client/model/event/event_type.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/feedback.py` & `webthing_client-0.2.8/webthing_client/model/event/feedback.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/feedback_schema.py` & `webthing_client-0.2.8/webthing_client/model/event/feedback_schema.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/observation.py` & `webthing_client-0.2.8/webthing_client/model/event/observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/event/stimulus.py` & `webthing_client-0.2.8/webthing_client/model/event/stimulus.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/property/observable_property.py` & `webthing_client-0.2.8/webthing_client/model/property/observable_property.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/system/sensor.py` & `webthing_client-0.2.8/webthing_client/model/system/sensor.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/system/system.py` & `webthing_client-0.2.8/webthing_client/model/system/system.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/user/user.py` & `webthing_client-0.2.8/webthing_client/model/user/user.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/model/webthing_observation.py` & `webthing_client-0.2.8/webthing_client/model/webthing_observation.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/standard_api/api_handler.py` & `webthing_client-0.2.8/webthing_client/standard_api/api_handler.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/standard_api/api_marshalling.py` & `webthing_client-0.2.8/webthing_client/standard_api/api_marshalling.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/stomp.py` & `webthing_client-0.2.8/webthing_client/stomp.py`

 * *Files identical despite different names*

### Comparing `webthing_client-0.2.7/webthing_client/utils.py` & `webthing_client-0.2.8/webthing_client/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime, timezone
+import json
 from urllib.parse import quote
 from typing import *
 from dateutil import parser
+from rdflib import Graph
 
 
 def parse_iso_time_format(iso: Optional[str]) -> datetime:
     """Parse valid in ISO 8601 format strings into timezone aware datetime objects.
 
     Args:
         iso (str): Timestamp string in ISO 8601 format.
@@ -48,7 +50,16 @@
     Returns:
         datetime: Datetime.
     """
     return datetime.now(timezone.utc)
 
 def encode_uri_component(uri_component: Optional[str]):
     return quote(uri_component, safe="!~*'()") if uri_component is not None else None
+
+def jsonld_object_to_graph(jsonld_object: dict, graph: Graph=None) -> Graph:
+    """
+    Convert a json-ld object to Graph.
+    """
+    if graph is None:
+        graph = Graph()
+    # Is there a better way than to serialize and load?
+    return graph.parse(format='json-ld', data=json.dumps(jsonld_object))
```

### Comparing `webthing_client-0.2.7/PKG-INFO` & `webthing_client-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webthing-client
-Version: 0.2.7
+Version: 0.2.8
 Summary: Client for the Dynamic Dashboard Webthings
 Home-page: https://github.com/predict-idlab/webthing-client-python
 Author: Emile Deman
 Maintainer: Emile Deman
 Maintainer-email: emile.deman@ugent.be
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

