# Comparing `tmp/pyworxcloud-4.1.8.tar.gz` & `tmp/pyworxcloud-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyworxcloud-4.1.8.tar", max compression
+gzip compressed data, was "pyworxcloud-4.1.9.tar", max compression
```

## Comparing `pyworxcloud-4.1.8.tar` & `pyworxcloud-4.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    35149 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/LICENSE
--rw-r--r--   0        0        0      929 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/README.md
--rw-r--r--   0        0        0      609 2024-03-27 10:03:16.915406 pyworxcloud-4.1.8/pyproject.toml
--rw-r--r--   0        0        0    38511 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/__init__.py
--rw-r--r--   0        0        0     4722 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/api.py
--rw-r--r--   0        0        0     1129 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/clouds.py
--rw-r--r--   0        0        0      928 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/const.py
--rw-r--r--   0        0        0      205 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/day_map.py
--rw-r--r--   0        0        0     3648 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/events.py
--rw-r--r--   0        0        0     2220 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/exceptions.py
--rw-r--r--   0        0        0      205 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/helpers/__init__.py
--rw-r--r--   0        0        0      638 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/helpers/logger.py
--rw-r--r--   0        0        0     2795 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/helpers/time_format.py
--rw-r--r--   0        0        0      839 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/__init__.py
--rw-r--r--   0        0        0     3457 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/battery.py
--rw-r--r--   0        0        0     2092 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/blades.py
--rw-r--r--   0        0        0     2052 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/capability.py
--rw-r--r--   0        0        0     3624 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/devices.py
--rw-r--r--   0        0        0      619 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/firmware.py
--rw-r--r--   0        0        0      282 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/landroid_class.py
--rw-r--r--   0        0        0      307 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/lawn.py
--rw-r--r--   0        0        0      428 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/location.py
--rw-r--r--   0        0        0     9428 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/mqtt.py
--rw-r--r--   0        0        0      412 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/orientation.py
--rw-r--r--   0        0        0     1349 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/product.py
--rw-r--r--   0        0        0     1110 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/rainsensor.py
--rw-r--r--   0        0        0     3189 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/requests.py
--rw-r--r--   0        0        0     6232 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/schedules.py
--rw-r--r--   0        0        0     2892 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/state.py
--rw-r--r--   0        0        0      658 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/statistics.py
--rw-r--r--   0        0        0      727 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/warranty.py
--rw-r--r--   0        0        0     2523 2024-03-27 10:03:03.855478 pyworxcloud-4.1.8/pyworxcloud/utils/zone.py
--rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 pyworxcloud-4.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/LICENSE
+-rw-r--r--   0        0        0      929 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/README.md
+-rw-r--r--   0        0        0      608 2024-04-08 09:08:21.010042 pyworxcloud-4.1.9/pyproject.toml
+-rw-r--r--   0        0        0    38763 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/__init__.py
+-rw-r--r--   0        0        0     4722 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/api.py
+-rw-r--r--   0        0        0     1129 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/clouds.py
+-rw-r--r--   0        0        0      928 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/const.py
+-rw-r--r--   0        0        0      205 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/day_map.py
+-rw-r--r--   0        0        0     3648 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/events.py
+-rw-r--r--   0        0        0     2220 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/exceptions.py
+-rw-r--r--   0        0        0      205 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/helpers/__init__.py
+-rw-r--r--   0        0        0      638 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/helpers/logger.py
+-rw-r--r--   0        0        0     2795 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/helpers/time_format.py
+-rw-r--r--   0        0        0      839 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/__init__.py
+-rw-r--r--   0        0        0     3457 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/battery.py
+-rw-r--r--   0        0        0     2092 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/blades.py
+-rw-r--r--   0        0        0     2052 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/capability.py
+-rw-r--r--   0        0        0     3624 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/devices.py
+-rw-r--r--   0        0        0      619 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/firmware.py
+-rw-r--r--   0        0        0      282 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/landroid_class.py
+-rw-r--r--   0        0        0      307 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/lawn.py
+-rw-r--r--   0        0        0      428 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/location.py
+-rw-r--r--   0        0        0     9428 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/mqtt.py
+-rw-r--r--   0        0        0      412 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/orientation.py
+-rw-r--r--   0        0        0     1349 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/product.py
+-rw-r--r--   0        0        0     1110 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/rainsensor.py
+-rw-r--r--   0        0        0     3189 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/requests.py
+-rw-r--r--   0        0        0     6232 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/schedules.py
+-rw-r--r--   0        0        0     2892 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/state.py
+-rw-r--r--   0        0        0      658 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/statistics.py
+-rw-r--r--   0        0        0      727 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/warranty.py
+-rw-r--r--   0        0        0     2523 2024-04-08 09:08:11.238069 pyworxcloud-4.1.9/pyworxcloud/utils/zone.py
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 pyworxcloud-4.1.9/PKG-INFO
```

### Comparing `pyworxcloud-4.1.8/LICENSE` & `pyworxcloud-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/README.md` & `pyworxcloud-4.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyproject.toml` & `pyworxcloud-4.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pyworxcloud"
-version = "v4.1.8"
+version = "v4.1.9"
 description = "Landroid cloud (Positec) API library"
 authors = ["Malene Trab <malene@trab.dk>"]
 documentation = "https://github.com/mtrab/pyworxcloud"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
@@ -16,10 +16,10 @@
 readme = "README.md"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mtrab/pyworxcloud/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-urllib3 = "^1.26.10"
+urllib3 = "^1.26.5"
 requests = "^2.28.0"
 paho-mqtt = "^1.6.1"
```

### Comparing `pyworxcloud-4.1.8/pyworxcloud/__init__.py` & `pyworxcloud-4.1.9/pyworxcloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """pyWorxCloud definition."""
 
 # pylint: disable=undefined-loop-variable
 # pylint: disable=line-too-long
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
+from asyncio import sleep
 import json
 import logging
 import sys
 import threading
 from datetime import datetime, timedelta
 from typing import Any
 
@@ -488,16 +489,18 @@
             if "dt" in data["cfg"]:
                 dt_split = data["cfg"]["dt"].split("/")
                 date = (
                     f"{dt_split[2]}-{dt_split[1]}-{dt_split[0]}"
                     + " "
                     + data["cfg"]["tm"]
                 )
-            else:
+            elif "tm" in data["dat"]:
                 date = datetime.fromisoformat(data["dat"]["tm"])
+            else:
+                date = datetime.now()
 
             device.updated = date
             device.rainsensor.delay = int(data["cfg"]["rd"])
 
             # Fetch wheel torque
             if "tq" in data["cfg"]:
                 device.capabilities.add(DeviceCapability.TORQUE)
@@ -856,25 +859,30 @@
         else:
             raise OfflineError("The device is currently offline, no action was sent.")
 
     def set_partymode(self, serial_number: str, state: bool) -> None:
         """Turn on or off the partymode.
 
         Args:
-            enable (bool): True is enabling partymode, Fasle is disabling partymode.
+            enable (bool): True is enabling partymode, False is disabling partymode.
 
         Raises:
             NoPartymodeError: Raised if the device does not support partymode.
             OfflineError: Raised if the device is offline.
         """
         mower = self.get_mower(serial_number)
 
         if mower["online"]:
             device = DeviceHandler(self._api, mower)
             if device.capabilities.check(DeviceCapability.PARTY_MODE):
+                if state:
+                    self.safehome(serial_number)
+                    self.home(serial_number)
+                    sleep(1)
+
                 if mower["protocol"] == 0:
                     self.mqtt.publish(
                         serial_number if mower["protocol"] == 0 else mower["uuid"],
                         mower["mqtt_topics"]["command_in"],
                         (
                             {"sc": {"m": 2, "distm": 0}}
                             if state
```

### Comparing `pyworxcloud-4.1.8/pyworxcloud/api.py` & `pyworxcloud-4.1.9/pyworxcloud/api.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/clouds.py` & `pyworxcloud-4.1.9/pyworxcloud/clouds.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/const.py` & `pyworxcloud-4.1.9/pyworxcloud/const.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/events.py` & `pyworxcloud-4.1.9/pyworxcloud/events.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/exceptions.py` & `pyworxcloud-4.1.9/pyworxcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/helpers/logger.py` & `pyworxcloud-4.1.9/pyworxcloud/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/helpers/time_format.py` & `pyworxcloud-4.1.9/pyworxcloud/helpers/time_format.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/__init__.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/battery.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/battery.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/blades.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/blades.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/capability.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/capability.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/devices.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/devices.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/firmware.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/firmware.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/mqtt.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/mqtt.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/product.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/product.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/rainsensor.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/rainsensor.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/requests.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/requests.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/schedules.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/schedules.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/state.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/state.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/statistics.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/warranty.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/warranty.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/pyworxcloud/utils/zone.py` & `pyworxcloud-4.1.9/pyworxcloud/utils/zone.py`

 * *Files identical despite different names*

### Comparing `pyworxcloud-4.1.8/PKG-INFO` & `pyworxcloud-4.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyworxcloud
-Version: 4.1.8
+Version: 4.1.9
 Summary: Landroid cloud (Positec) API library
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.10,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/mtrab/pyworxcloud/issues
 Project-URL: Documentation, https://github.com/mtrab/pyworxcloud
 Description-Content-Type: text/markdown
 
 <a href="https://www.buymeacoffee.com/mtrab" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
 
 # pyWorxCloud
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: pyworxcloud Version: 4.1.8 Summary: Landroid cloud
+Metadata-Version: 2.1 Name: pyworxcloud Version: 4.1.9 Summary: Landroid cloud
 (Positec) API library License: MIT Author: Malene Trab Author-email:
 malene@trab.dk Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved
 :: MIT License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Dist: paho-mqtt
 (>=1.6.1,<2.0.0) Requires-Dist: requests (>=2.28.0,<3.0.0) Requires-Dist:
-urllib3 (>=1.26.10,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
+urllib3 (>=1.26.5,<2.0.0) Project-URL: Bug Tracker, https://github.com/mtrab/
 pyworxcloud/issues Project-URL: Documentation, https://github.com/mtrab/
 pyworxcloud Description-Content-Type: text/markdown _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]#
 pyWorxCloud This is a PyPI module for communicating with Worx Cloud mowers,
 primarily developed for use with [Home Assistant](https://home-assistant.io),
 but I try to keep it as widely usable as possible.
 
 The module are compatible with cloud enabled devices from [these vendors]
```

