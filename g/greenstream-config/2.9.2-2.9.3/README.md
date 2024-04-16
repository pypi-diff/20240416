# Comparing `tmp/greenstream_config-2.9.2.tar.gz` & `tmp/greenstream_config-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greenstream_config-2.9.2.tar", last modified: Sun Feb 18 22:20:52 2024, max compression
+gzip compressed data, was "greenstream_config-2.9.3.tar", last modified: Mon Feb 19 00:02:41 2024, max compression
```

## Comparing `greenstream_config-2.9.2.tar` & `greenstream_config-2.9.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-18 22:20:52.283542 greenstream_config-2.9.2/
--rw-r--r--   0 runner    (1000) runner    (1001)      881 2024-02-18 22:20:52.283542 greenstream_config-2.9.2/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      187 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-18 22:20:52.283542 greenstream_config-2.9.2/greenstream_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)      376 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/greenstream_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     3192 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/greenstream_config/merge_cameras.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2504 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/greenstream_config/types.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2996 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/greenstream_config/urdf.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-18 22:20:52.283542 greenstream_config-2.9.2/greenstream_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)      881 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      396 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       18 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       19 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-02-18 22:20:52.000000 greenstream_config-2.9.2/greenstream_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      854 2024-02-18 22:20:52.283542 greenstream_config-2.9.2/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-02-18 22:20:29.000000 greenstream_config-2.9.2/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-19 00:02:41.880939 greenstream_config-2.9.3/
+-rw-r--r--   0 runner    (1000) runner    (1001)      881 2024-02-19 00:02:41.880939 greenstream_config-2.9.3/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      187 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-19 00:02:41.880939 greenstream_config-2.9.3/greenstream_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)      376 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/greenstream_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     3192 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/greenstream_config/merge_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2462 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/greenstream_config/types.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2996 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/greenstream_config/urdf.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-02-19 00:02:41.880939 greenstream_config-2.9.3/greenstream_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)      881 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      396 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       18 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       19 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-02-19 00:02:41.000000 greenstream_config-2.9.3/greenstream_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      854 2024-02-19 00:02:41.884939 greenstream_config-2.9.3/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-02-19 00:02:14.000000 greenstream_config-2.9.3/setup.py
```

### Comparing `greenstream_config-2.9.2/PKG-INFO` & `greenstream_config-2.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenstream_config
-Version: 2.9.2
+Version: 2.9.3
 Summary: A library for reading / writing Greenstream config files
 Home-page: https://github.com/Greenroom-Robotics/greenstream
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `greenstream_config-2.9.2/greenstream_config/merge_cameras.py` & `greenstream_config-2.9.3/greenstream_config/merge_cameras.py`

 * *Files identical despite different names*

### Comparing `greenstream_config-2.9.2/greenstream_config/types.py` & `greenstream_config-2.9.3/greenstream_config/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     sensor_height_mm: float
     fov: float
     # Published ros topic names
     camera_frame_topic: str
     camera_info_topic: str
     camera_info_ext_topic: str
     #Camera intrinsics and distortion parameters from callibration
-    distortion_parameters: Optional[List[float]] = [0.0, 0.0, 0.0, 0.0, 0.0]
+    distortion_parameters: Optional[List[float]] = None
     distortion_model: str = "plumb_bob"
     # The camera's position relative to the vessel base_link
     offsets: Optional[Offsets] = None
     type: str = "color"
     ros_throttle_time: float = 0.0000001
 
 
@@ -55,15 +55,15 @@
     sensor_height_mm: Optional[float]
     fov: Optional[float]
     # Published ros topic names
     camera_frame_topic: Optional[str]
     camera_info_topic: Optional[str]
     camera_info_ext_topic: Optional[str]
     #Camera intrinsics and distortion parameters from callibration
-    distortion_parameters: Optional[List[float]] = [0.0, 0.0, 0.0, 0.0, 0.0]
+    distortion_parameters: Optional[List[float]] = None
     distortion_model: str = "plumb_bob"
     # The camera's position relative to the vessel base_link
     offsets: Optional[Offsets] = None
     type: Optional[str] = "color"
     ros_throttle_time: Optional[float] = 0.0000001
```

### Comparing `greenstream_config-2.9.2/greenstream_config/urdf.py` & `greenstream_config-2.9.3/greenstream_config/urdf.py`

 * *Files identical despite different names*

### Comparing `greenstream_config-2.9.2/greenstream_config.egg-info/PKG-INFO` & `greenstream_config-2.9.3/greenstream_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greenstream_config
-Version: 2.9.2
+Version: 2.9.3
 Summary: A library for reading / writing Greenstream config files
 Home-page: https://github.com/Greenroom-Robotics/greenstream
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `greenstream_config-2.9.2/setup.cfg` & `greenstream_config-2.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = greenstream_config
-version = 2.9.2
+version = 2.9.3
 url = https://github.com/Greenroom-Robotics/greenstream
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

