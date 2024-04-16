# Comparing `tmp/uav_collision_avoidance-0.4.0-py3-none-any.whl.zip` & `tmp/uav_collision_avoidance-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,23 @@
-Zip file size: 6255 bytes, number of entries: 9
+Zip file size: 24834 bytes, number of entries: 21
+-rw-r--r--  2.0 unx      107 b- defN 24-Apr-16 08:15 tests/test_sample.py
 -rw-r--r--  2.0 unx      121 b- defN 24-Mar-28 17:13 uav_collision_avoidance/__init__.py
--rw-r--r--  2.0 unx     2203 b- defN 24-Mar-28 17:35 uav_collision_avoidance/main.py
--rw-r--r--  2.0 unx       65 b- defN 24-Apr-11 19:11 uav_collision_avoidance/version.py
--rw-r--r--  2.0 unx     1075 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5710 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       24 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      845 b- defN 24-Apr-11 19:14 uav_collision_avoidance-0.4.0.dist-info/RECORD
-9 files, 10208 bytes uncompressed, 4759 bytes compressed:  53.4%
+-rw-r--r--  2.0 unx     2203 b- defN 24-Apr-15 19:36 uav_collision_avoidance/main.py
+-rw-r--r--  2.0 unx      191 b- defN 24-Apr-16 10:28 uav_collision_avoidance/version.py
+-rw-r--r--  2.0 unx     1662 b- defN 24-Mar-28 17:17 uav_collision_avoidance/src/aircraft/aircraft.py
+-rw-r--r--  2.0 unx     9540 b- defN 24-Apr-11 18:19 uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+-rw-r--r--  2.0 unx     4195 b- defN 24-Apr-05 07:31 uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+-rw-r--r--  2.0 unx     8671 b- defN 24-Apr-16 07:07 uav_collision_avoidance/src/simulation/simulation.py
+-rw-r--r--  2.0 unx     6057 b- defN 24-Apr-11 11:29 uav_collision_avoidance/src/simulation/simulation_adsb.py
+-rw-r--r--  2.0 unx     1979 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_fps.py
+-rw-r--r--  2.0 unx     7112 b- defN 24-Apr-11 19:12 uav_collision_avoidance/src/simulation/simulation_physics.py
+-rw-r--r--  2.0 unx     1041 b- defN 24-Mar-28 17:20 uav_collision_avoidance/src/simulation/simulation_render.py
+-rw-r--r--  2.0 unx      682 b- defN 24-Apr-06 09:52 uav_collision_avoidance/src/simulation/simulation_settings.py
+-rw-r--r--  2.0 unx     6110 b- defN 24-Apr-11 12:04 uav_collision_avoidance/src/simulation/simulation_state.py
+-rw-r--r--  2.0 unx    23164 b- defN 24-Apr-11 12:26 uav_collision_avoidance/src/simulation/simulation_widget.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6162 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2167 b- defN 24-Apr-16 10:29 uav_collision_avoidance-0.5.0.dist-info/RECORD
+21 files, 82456 bytes uncompressed, 21150 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,28 +1,64 @@
+Filename: tests/test_sample.py
+Comment: 
+
 Filename: uav_collision_avoidance/__init__.py
 Comment: 
 
 Filename: uav_collision_avoidance/main.py
 Comment: 
 
 Filename: uav_collision_avoidance/version.py
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/LICENSE
+Filename: uav_collision_avoidance/src/aircraft/aircraft.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/aircraft/aircraft_fcc.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/aircraft/aircraft_vehicle.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_adsb.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_fps.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_physics.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_render.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_settings.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_state.py
+Comment: 
+
+Filename: uav_collision_avoidance/src/simulation/simulation_widget.py
+Comment: 
+
+Filename: uav_collision_avoidance-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/METADATA
+Filename: uav_collision_avoidance-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/WHEEL
+Filename: uav_collision_avoidance-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/entry_points.txt
+Filename: uav_collision_avoidance-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/top_level.txt
+Filename: uav_collision_avoidance-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: uav_collision_avoidance-0.4.0.dist-info/RECORD
+Filename: uav_collision_avoidance-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uav_collision_avoidance/version.py

```diff
@@ -1,3 +1,9 @@
 """Contains the version of the package"""
 
-__version__ = "0.4.0"
+import toml
+
+def get_version():
+    pyproject = toml.load("pyproject.toml")
+    return pyproject['project']['version']
+
+__version__ = get_version()
```

## Comparing `uav_collision_avoidance-0.4.0.dist-info/LICENSE` & `uav_collision_avoidance-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uav_collision_avoidance-0.4.0.dist-info/METADATA` & `uav_collision_avoidance-0.5.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: uav-collision-avoidance
-Version: 0.4.0
+Version: 0.5.0
 Summary: UAV collision avoidance simulation
+Author-email: mldxo <miloszmaculewicz@gmail.com>
+Project-URL: Homepage, https://github.com/mldxo/uav-collision-avoidance
+Project-URL: Issues, https://github.com/mldxo/uav-collision-avoidance/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyside6
 
 # UAV Collision Avoidance
 
 Python project regarding implementation of UAV physics and collision detection/avoidance algorithms.
 - [Current version](https://github.com/mldxo/uav-collision-avoidance)
 - [Archived version](https://github.com/mldxo/uav-collision-avoidance-2)
 - [Pypi project](https://pypi.org/project/uav-collision-avoidance)
@@ -38,27 +44,29 @@
 There are three possible arguments at the moment:
 - realtime - runs GUI application with realtime simulation
 - prerender - runs physical simulation
 - tests - runs full tests with comparison of using and not using collision avoidance algorithm
 
 App defaults to realtime simulation.
 
-# Key shortcuts
+## Key shortcuts
 
 > [!NOTE]
 > Aircraft 0 is the first one, Aircraft 1 is the second one.
 
 There are several key shortcuts for realtime version of the app that allow full-scale testing.
 
 - Left mouse click - appends click location to the top of destination list of Aircraft 0
 - Right mouse click - adds click location to the end of destination list of Aircraft 0
 - Middle mouse click (scroll click) - teleports Aircraft 0 to the click location
 - Mouse wheel - zooms in/out the simulation render smoothly
 - Plus/minus keys (+/-) - zooms in/out the simulation render quickly
 - Arrow keys (↑ ↓ → ←) - moves the view
+- F1 key - toggles ADS-B Aircraft 0 info reporting
+- F2/F3 keys - speed up/down target speed of Aircraft 0
 - N key - toggles Aircraft 0/1 view following (default off)
 - M key - switches between Aircraft 0/1 view following (default 0)
 - O key - toggles Aircraft 0 targeting Aircraft 1's speed vector (default off)
 - P key - toggles Aircraft 1 targeting Aircraft 0's speed vector (default off)
 - T key - toggles collision avoidance maneuvering (default off)
 - WSAD keys - sets course for Aircraft 0 - 0, 180, 270, 90 degrees respectively
 - R - resets simulation to start state
```

