# Comparing `tmp/yoto_api-1.2.0.tar.gz` & `tmp/yoto_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.2.0.tar", last modified: Tue Apr 16 00:44:24 2024, max compression
+gzip compressed data, was "yoto_api-1.2.1.tar", last modified: Tue Apr 16 00:57:11 2024, max compression
```

## Comparing `yoto_api-1.2.0.tar` & `yoto_api-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 00:43:28.000000 yoto_api-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 00:43:28.000000 yoto_api-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 00:43:28.000000 yoto_api-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 00:43:28.000000 yoto_api-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 00:43:28.000000 yoto_api-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:44:24.062342 yoto_api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 00:43:28.000000 yoto_api-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:43:28.000000 yoto_api-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:44:24.062342 yoto_api-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 00:44:07.000000 yoto_api-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:43:28.000000 yoto_api-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 00:43:28.000000 yoto_api-1.2.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:44:23.000000 yoto_api-1.2.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:57:11.064826 yoto_api-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 00:56:49.000000 yoto_api-1.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 00:56:49.000000 yoto_api-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 00:56:49.000000 yoto_api-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 00:56:49.000000 yoto_api-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 00:56:49.000000 yoto_api-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:57:11.064826 yoto_api-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 00:56:49.000000 yoto_api-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:56:49.000000 yoto_api-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:57:11.064826 yoto_api-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 00:57:05.000000 yoto_api-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:57:11.060826 yoto_api-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:56:49.000000 yoto_api-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 00:56:49.000000 yoto_api-1.2.1/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:57:11.060826 yoto_api-1.2.1/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19641 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 00:56:49.000000 yoto_api-1.2.1/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:57:11.064826 yoto_api-1.2.1/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:57:11.000000 yoto_api-1.2.1/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 00:57:11.000000 yoto_api-1.2.1/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:57:11.000000 yoto_api-1.2.1/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:57:10.000000 yoto_api-1.2.1/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 00:57:11.000000 yoto_api-1.2.1/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.2.0/CONTRIBUTING.rst` & `yoto_api-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.0/LICENSE` & `yoto_api-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.0/PKG-INFO` & `yoto_api-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.2.0/README.rst` & `yoto_api-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.0/setup.py` & `yoto_api-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.2.0",
+    version="1.2.1",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.2.0/yoto_api/Card.py` & `yoto_api-1.2.1/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.0/yoto_api/YotoAPI.py` & `yoto_api-1.2.1/yoto_api/YotoAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """API Methods"""
 
 import requests
 import logging
 import datetime
+import pytz
 from .const import DOMAIN
 from .Token import Token
 from .Card import Card
 from .YotoPlayer import YotoPlayer
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -52,15 +53,15 @@
         result = {}
         for device in response["devices"]:
             player: YotoPlayer = YotoPlayer(
                 id=device["deviceId"],
                 name=device["name"],
                 deviceType=device["deviceType"],
                 online=device["online"],
-                last_updated_at=datetime.datetime.now()
+                last_updated_at=datetime.datetime.now(pytz.utc)
             )
             result[player.id] = player
 
         return result
         # TODO: parse the data and return a list of yoto devices.
 
     def update_library(self, token) -> list[Card]:
```

### Comparing `yoto_api-1.2.0/yoto_api/YotoManager.py` & `yoto_api-1.2.1/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.2.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.2.1/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

