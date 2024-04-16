# Comparing `tmp/tactigon_gear-5.0.4.tar.gz` & `tmp/tactigon_gear-5.0.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tactigon_gear-5.0.4.tar", last modified: Wed Mar 27 15:44:03 2024, max compression
+gzip compressed data, was "tactigon_gear-5.0.4.post1.tar", last modified: Tue Apr 16 08:44:30 2024, max compression
```

## Comparing `tactigon_gear-5.0.4.tar` & `tactigon_gear-5.0.4.post1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.200375 tactigon_gear-5.0.4/
--rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_gear-5.0.4/LICENSE
--rw-rw-rw-   0        0        0      383 2024-03-27 15:43:10.000000 tactigon_gear-5.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3613 2024-03-27 15:44:03.199355 tactigon_gear-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2856 2024-03-07 11:04:20.000000 tactigon_gear-5.0.4/README.md
--rw-rw-rw-   0        0        0       92 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 15:44:03.202229 tactigon_gear-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2690 2024-03-27 15:42:57.000000 tactigon_gear-5.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.035154 tactigon_gear-5.0.4/tactigon_gear/
--rw-rw-rw-   0        0        0     2477 2024-03-27 15:43:36.000000 tactigon_gear-5.0.4/tactigon_gear/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.066143 tactigon_gear-5.0.4/tactigon_gear/client/
--rw-rw-rw-   0        0        0     8712 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/client/Data_Collection.py
--rw-rw-rw-   0        0        0     5871 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/client/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/client/models.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.152587 tactigon_gear-5.0.4/tactigon_gear/client/utilities/
--rw-rw-rw-   0        0        0     2527 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/client/utilities/Client_Account_Managment.py
--rw-rw-rw-   0        0        0     6841 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/client/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.155564 tactigon_gear-5.0.4/tactigon_gear/hal/
--rw-rw-rw-   0        0        0       41 2024-03-15 10:16:54.000000 tactigon_gear-5.0.4/tactigon_gear/hal/__init__.py
--rw-rw-rw-   0        0        0    10179 2024-03-27 15:38:34.000000 tactigon_gear-5.0.4/tactigon_gear/hal/ble.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.164110 tactigon_gear-5.0.4/tactigon_gear/middleware/
--rw-rw-rw-   0        0        0   443371 2024-03-27 15:43:47.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Audio.c
--rw-rw-rw-   0        0        0   499540 2024-03-27 15:43:47.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Gesture.c
--rw-rw-rw-   0        0        0   430462 2024-03-27 15:43:47.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Recorder.c
--rw-rw-rw-   0        0        0      243 2024-03-15 15:12:23.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.197344 tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/
--rw-rw-rw-   0        0        0   518832 2024-03-27 15:43:47.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/Data_Preprocessor.c
--rw-rw-rw-   0        0        0   701641 2024-03-27 15:43:48.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c
--rw-rw-rw-   0        0        0      212 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/__init__.py
--rw-rw-rw-   0        0        0     4755 2024-03-15 09:33:23.000000 tactigon_gear-5.0.4/tactigon_gear/models.py
-drwxrwxrwx   0        0        0        0 2024-03-27 15:44:03.198358 tactigon_gear-5.0.4/tactigon_gear.egg-info/
--rw-rw-rw-   0        0        0     3613 2024-03-27 15:44:02.000000 tactigon_gear-5.0.4/tactigon_gear.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1132 2024-03-27 15:44:03.000000 tactigon_gear-5.0.4/tactigon_gear.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 15:44:02.000000 tactigon_gear-5.0.4/tactigon_gear.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2024-03-27 15:44:02.000000 tactigon_gear-5.0.4/tactigon_gear.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-27 15:44:02.000000 tactigon_gear-5.0.4/tactigon_gear.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.930371 tactigon_gear-5.0.4.post1/
+-rw-rw-rw-   0        0        0        0 2023-08-28 15:35:20.000000 tactigon_gear-5.0.4.post1/LICENSE
+-rw-rw-rw-   0        0        0      383 2024-03-27 15:43:10.000000 tactigon_gear-5.0.4.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3619 2024-04-16 08:44:30.929367 tactigon_gear-5.0.4.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     2856 2024-03-07 11:04:20.000000 tactigon_gear-5.0.4.post1/README.md
+-rw-rw-rw-   0        0        0       92 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 08:44:30.941373 tactigon_gear-5.0.4.post1/setup.cfg
+-rw-rw-rw-   0        0        0     2690 2024-03-27 15:42:57.000000 tactigon_gear-5.0.4.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.725233 tactigon_gear-5.0.4.post1/tactigon_gear/
+-rw-rw-rw-   0        0        0     2427 2024-04-16 08:37:01.000000 tactigon_gear-5.0.4.post1/tactigon_gear/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.820232 tactigon_gear-5.0.4.post1/tactigon_gear/client/
+-rw-rw-rw-   0        0        0     8673 2024-04-16 08:42:53.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/Data_Collection.py
+-rw-rw-rw-   0        0        0     5871 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/models.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.827234 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/
+-rw-rw-rw-   0        0        0     2527 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/Client_Account_Managment.py
+-rw-rw-rw-   0        0        0     6841 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.832233 tactigon_gear-5.0.4.post1/tactigon_gear/hal/
+-rw-rw-rw-   0        0        0       41 2024-03-15 10:16:54.000000 tactigon_gear-5.0.4.post1/tactigon_gear/hal/__init__.py
+-rw-rw-rw-   0        0        0    10310 2024-04-16 08:42:10.000000 tactigon_gear-5.0.4.post1/tactigon_gear/hal/ble.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.877808 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/
+-rw-rw-rw-   0        0        0   443371 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Audio.c
+-rw-rw-rw-   0        0        0   499540 2024-04-16 08:44:11.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Gesture.c
+-rw-rw-rw-   0        0        0   430462 2024-04-16 08:44:11.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Recorder.c
+-rw-rw-rw-   0        0        0      243 2024-03-27 15:44:22.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.911375 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/
+-rw-rw-rw-   0        0        0   518832 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Data_Preprocessor.c
+-rw-rw-rw-   0        0        0   701641 2024-04-16 08:44:12.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c
+-rw-rw-rw-   0        0        0      212 2024-01-03 16:51:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/__init__.py
+-rw-rw-rw-   0        0        0     4755 2024-03-15 09:33:23.000000 tactigon_gear-5.0.4.post1/tactigon_gear/models.py
+drwxrwxrwx   0        0        0        0 2024-04-16 08:44:30.925370 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/
+-rw-rw-rw-   0        0        0     3619 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1132 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-16 08:44:30.000000 tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/top_level.txt
```

### Comparing `tactigon_gear-5.0.4/PKG-INFO` & `tactigon_gear-5.0.4.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_gear
-Version: 5.0.4
+Version: 5.0.4.post1
 Summary: Tactigon Gear to connect to Tactigon Skin wereable platform
 Home-page: https://www.thetactigon.com
 Maintainer: Next Industries s.r.l.
 Maintainer-email: info@thetactigon.com
 License: MIT
 Keywords: tactigon,wereable,gestures controller,human interface
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tactigon_gear-5.0.4/README.md` & `tactigon_gear-5.0.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/setup.py` & `tactigon_gear-5.0.4.post1/setup.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/__init__.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-__version__ = "5.0.4"
+__version__ = "5.0.4.post1"
 __all__ = ["TSkin", "TSkinConfig", "GestureConfig", "TSkinState", "Hand", "Touch", "Angle", "Gyro", "Acceleration", "Gesture", "OneFingerGesture", "TwoFingerGesture"]
 
 import logging
 from typing import Optional
 from multiprocessing import Pipe
-from multiprocessing.connection import _ConnectionBase
 
 from .hal import Ble
 from .middleware import Tactigon_Gesture
 from .models import Gesture, Touch, OneFingerGesture, TwoFingerGesture, Angle, Acceleration, Gyro, TSkinState, TSkinConfig, Hand, GestureConfig
 
 class TSkin(Ble):
     _tgesture: Optional[Tactigon_Gesture] = None
```

### Comparing `tactigon_gear-5.0.4/tactigon_gear/client/Data_Collection.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/client/Data_Collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #     sys.path.insert(0, path.join(CLIENT_PY_PATH, "utilities"))
 #     sys.path.insert(0, path.join(CLIENT_PY_PATH, "hal"))
 #     sys.path.insert(0, path.join(CLIENT_PY_PATH, "middleware"))
 #     sys.path.insert(0, path.join(CLIENT_PY_PATH, "data_managment/utilities"))
 
 
 from .utilities import create_dir, load_info, update_dataframe, get_index, update_info
-from ..hal import BLE
+from ..hal import Ble
 from ..middleware import Tactigon_Recorder
 from ..models import Hand
 
 from .models import UserData, DataCollectionConfig, HAL
 
 def collect(user_data: UserData, hal: HAL, data_collection_config: DataCollectionConfig):
     """
@@ -79,23 +79,22 @@
 
 
     # pipes
     rx_sensor_pipe, tx_sensor_pipe = multiprocessing.Pipe(duplex=False)
     rx_angle_pipe, tx_angle_pipe = multiprocessing.Pipe(duplex=False)
 
 
-    pro_in = BLE(
-        b_name,
+    pro_in = Ble(
         b_add,
-        b_hand,
-        logging.getLogger(),
-        sensor_pipe=tx_sensor_pipe,
-        angle_pipe=tx_angle_pipe
+        b_hand
     )
 
+    pro_in._sensor_tx = tx_sensor_pipe
+    pro_in._angle_tx = tx_angle_pipe
+
     print("Waiting for Tactigon connection...")
     pro_in.start()
 
     while not pro_in.connected:
         pass
 
     # loop through one gesture at a time to collect data
```

### Comparing `tactigon_gear-5.0.4/tactigon_gear/client/__init__.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/client/__init__.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/client/models.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/client/models.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/client/utilities/Client_Account_Managment.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/Client_Account_Managment.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/client/utilities/__init__.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/client/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/hal/ble.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/hal/ble.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     hand: Hand
     debug: bool
 
     _stop_event: Event
     client: Optional[BleakClient]
     selector: TBleSelector
     _sensor_tx: Optional[_ConnectionBase] = None
+    _angle_tx: Optional[_ConnectionBase] = None
     _audio_tx: Optional[_ConnectionBase] = None
     _update: Lock
     _update_touch: Lock
     _update_selector: Lock
 
     _angle: Optional[Angle] = None
     _acceleration: Optional[Acceleration] = None
@@ -176,14 +177,17 @@
             logging.debug("Acceleration: %f,%f,%f",accX, accY, accZ)
             logging.debug("Gyro: %f,%f,%f",gyroX, gyroY, gyroZ)
             logging.debug("Battery: %f", battery/1000)
 
         if self._sensor_tx:
             self._sensor_tx.send([accX, accY, accZ, gyroX, gyroY, gyroZ])
 
+        if self._angle_tx:
+            self._angle_tx.send([roll, pitch, yaw])
+
     def handle_touchpad(self, char, data: bytearray):
         self._update_touch.acquire()
         one_finger = OneFingerGesture(int.from_bytes(data[0:1], "big"))
         two_finger = TwoFingerGesture(int.from_bytes(data[1:2], "big"))
         if one_finger is not OneFingerGesture.NONE or two_finger is not TwoFingerGesture.NONE:
             self._touch = Touch(
                 one_finger,
@@ -275,8 +279,8 @@
     def connect(self):
         self.start()
 
     def disconnect(self):
         self.join()
 
     def terminate(self):
-        self.join(0)
+        self.join()
```

### Comparing `tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Audio.c` & `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Audio.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Gesture.c` & `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Gesture.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/middleware/Tactigon_Recorder.c` & `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/Tactigon_Recorder.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/Data_Preprocessor.c` & `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Data_Preprocessor.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c` & `tactigon_gear-5.0.4.post1/tactigon_gear/middleware/utilities/Tactigon_RT_Computing.c`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear/models.py` & `tactigon_gear-5.0.4.post1/tactigon_gear/models.py`

 * *Files identical despite different names*

### Comparing `tactigon_gear-5.0.4/tactigon_gear.egg-info/PKG-INFO` & `tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tactigon_gear
-Version: 5.0.4
+Version: 5.0.4.post1
 Summary: Tactigon Gear to connect to Tactigon Skin wereable platform
 Home-page: https://www.thetactigon.com
 Maintainer: Next Industries s.r.l.
 Maintainer-email: info@thetactigon.com
 License: MIT
 Keywords: tactigon,wereable,gestures controller,human interface
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tactigon_gear-5.0.4/tactigon_gear.egg-info/SOURCES.txt` & `tactigon_gear-5.0.4.post1/tactigon_gear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

