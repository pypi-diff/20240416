# Comparing `tmp/lookout_config-1.2.0.tar.gz` & `tmp/lookout_config-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lookout_config-1.2.0.tar", last modified: Mon Apr 15 07:15:03 2024, max compression
+gzip compressed data, was "lookout_config-1.2.1.tar", last modified: Mon Apr 15 09:21:29 2024, max compression
```

## Comparing `lookout_config-1.2.0.tar` & `lookout_config-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:03.617627 lookout_config-1.2.0/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 07:15:03.617627 lookout_config-1.2.0/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-15 07:13:44.000000 lookout_config-1.2.0/README.md
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:03.617627 lookout_config-1.2.0/lookout_config/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     6530 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/generate_cameras.py
--rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/generate_schemas.py
--rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/generate_urdf.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:03.617627 lookout_config-1.2.0/lookout_config/schemas/
--rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/schemas/lookout.schema.json
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:03.617627 lookout_config-1.2.0/lookout_config/test/
--rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-15 07:13:44.000000 lookout_config-1.2.0/lookout_config/test/lookout_config_test.py
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 07:15:03.617627 lookout_config-1.2.0/lookout_config.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 07:15:03.000000 lookout_config-1.2.0/lookout_config.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-15 07:15:03.000000 lookout_config-1.2.0/lookout_config.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 07:15:03.000000 lookout_config-1.2.0/lookout_config.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-15 07:15:03.000000 lookout_config-1.2.0/lookout_config.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-15 07:15:03.000000 lookout_config-1.2.0/lookout_config.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 07:14:47.000000 lookout_config-1.2.0/lookout_config.egg-info/zip-safe
--rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-15 07:15:03.617627 lookout_config-1.2.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 07:13:44.000000 lookout_config-1.2.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:29.554790 lookout_config-1.2.1/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 09:21:29.554790 lookout_config-1.2.1/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      625 2024-04-15 09:20:10.000000 lookout_config-1.2.1/README.md
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:29.554790 lookout_config-1.2.1/lookout_config/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2438 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     6530 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/generate_cameras.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)      436 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/generate_schemas.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2762 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/generate_urdf.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:29.554790 lookout_config-1.2.1/lookout_config/schemas/
+-rw-rw-r--   0 runner    (1000) runner    (1001)     2769 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/schemas/lookout.schema.json
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:29.554790 lookout_config-1.2.1/lookout_config/test/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       73 2024-04-15 09:20:10.000000 lookout_config-1.2.1/lookout_config/test/lookout_config_test.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2024-04-15 09:21:29.554790 lookout_config-1.2.1/lookout_config.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1001)     1437 2024-04-15 09:21:29.000000 lookout_config-1.2.1/lookout_config.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      465 2024-04-15 09:21:29.000000 lookout_config-1.2.1/lookout_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 09:21:29.000000 lookout_config-1.2.1/lookout_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       72 2024-04-15 09:21:29.000000 lookout_config-1.2.1/lookout_config.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2024-04-15 09:21:29.000000 lookout_config-1.2.1/lookout_config.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2024-04-15 09:21:13.000000 lookout_config-1.2.1/lookout_config.egg-info/zip-safe
+-rw-rw-r--   0 runner    (1000) runner    (1001)      914 2024-04-15 09:21:29.554790 lookout_config-1.2.1/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2024-04-15 09:20:10.000000 lookout_config-1.2.1/setup.py
```

### Comparing `lookout_config-1.2.0/PKG-INFO` & `lookout_config-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.2.0/README.md` & `lookout_config-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lookout_config-1.2.0/lookout_config/__init__.py` & `lookout_config-1.2.1/lookout_config/__init__.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.2.0/lookout_config/generate_cameras.py` & `lookout_config-1.2.1/lookout_config/generate_cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             camera_frame_topic="perception/frames/bow_color",
             camera_info_topic="sensors/cameras/bow_color/camera_info",
             camera_info_ext_topic="sensors/cameras/bow_color/camera_info_ext",
             k_intrinsic=k_intrinsic,
             # distortion_parameters=distortion_parameters,
             offsets=Offsets(
                 roll=radians(2.0),
-                pitch=radians(5.85),
+                pitch=radians(-3.0),
                 yaw=0.0,
                 forward=3.190,
                 left=0.015,
                 up=-0.205,
             ),
         ),
         Camera(
```

### Comparing `lookout_config-1.2.0/lookout_config/generate_urdf.py` & `lookout_config-1.2.1/lookout_config/generate_urdf.py`

 * *Files identical despite different names*

### Comparing `lookout_config-1.2.0/lookout_config/schemas/lookout.schema.json` & `lookout_config-1.2.1/lookout_config/schemas/lookout.schema.json`

 * *Files identical despite different names*

### Comparing `lookout_config-1.2.0/lookout_config.egg-info/PKG-INFO` & `lookout_config-1.2.1/lookout_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lookout_config
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for reading / writing Lookout config files
 Home-page: https://github.com/Greenroom-Robotics/lookout
 Author: Greenroom Robotics
 Author-email: team@greenroomrobotics.com
 Maintainer: David Revay
 Maintainer-email: david.revay@greenroomrobotics.com
 License: Copyright (C) 2023, Greenroom Robotics
```

### Comparing `lookout_config-1.2.0/setup.cfg` & `lookout_config-1.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lookout_config
-version = 1.2.0
+version = 1.2.1
 url = https://github.com/Greenroom-Robotics/lookout
 author = Greenroom Robotics
 author_email = team@greenroomrobotics.com
 maintainer = David Revay
 maintainer_email = david.revay@greenroomrobotics.com
 classifiers = 
 	Development Status :: 3 - Alpha
```

