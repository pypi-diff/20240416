# Comparing `tmp/yoto_api-1.0.9.tar.gz` & `tmp/yoto_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.0.9.tar", last modified: Sun Apr 14 21:59:16 2024, max compression
+gzip compressed data, was "yoto_api-1.1.0.tar", last modified: Mon Apr 15 23:55:41 2024, max compression
```

## Comparing `yoto_api-1.0.9.tar` & `yoto_api-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 21:58:54.000000 yoto_api-1.0.9/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-14 21:58:54.000000 yoto_api-1.0.9/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 21:58:54.000000 yoto_api-1.0.9/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 21:58:54.000000 yoto_api-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 21:58:54.000000 yoto_api-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 21:59:16.304932 yoto_api-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-14 21:58:54.000000 yoto_api-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:58:54.000000 yoto_api-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:59:16.304932 yoto_api-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-14 21:59:10.000000 yoto_api-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.300932 yoto_api-1.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:58:54.000000 yoto_api-1.0.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-14 21:58:54.000000 yoto_api-1.0.9/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.669992 yoto_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 23:55:12.000000 yoto_api-1.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-15 23:55:12.000000 yoto_api-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 23:55:12.000000 yoto_api-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 23:55:12.000000 yoto_api-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 23:55:12.000000 yoto_api-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-15 23:55:41.669992 yoto_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 23:55:12.000000 yoto_api-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:12.000000 yoto_api-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:55:41.669992 yoto_api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 23:55:34.000000 yoto_api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:12.000000 yoto_api-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-15 23:55:12.000000 yoto_api-1.1.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.0.9/CONTRIBUTING.rst` & `yoto_api-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.9/LICENSE` & `yoto_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.9/PKG-INFO` & `yoto_api-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Introduction
 ============
 
-Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far. 
+Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far.
 
 To run this code for test I am doing::
 
     from pathlib import Path
     import logging
     import sys
     import os
@@ -32,8 +32,10 @@
     sys.path.append(str(path_root))
     from yoto_api import \*
 
     logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format='%(asctime)s %(name)s %(levelname)s:%(message)s')
     logger = logging.getLogger(**name**)
 
     ym = YotoManager(username="username", password="password")
+    ym.check_and_refresh_token()
+    ym.update_player_status()
     print (ym.players)
```

### Comparing `yoto_api-1.0.9/setup.py` & `yoto_api-1.1.0/setup.py`

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
-    version="1.0.9",
+    version="1.1.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.0.9/yoto_api/Card.py` & `yoto_api-1.1.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.9/yoto_api/YotoAPI.py` & `yoto_api-1.1.0/yoto_api/YotoAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """API Methods"""
 
 import requests
 import logging
+import datetime
 from .const import DOMAIN
 from .Token import Token
 from .Card import Card
 from .YotoPlayer import YotoPlayer
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -43,25 +44,26 @@
             scope=response["scope"],
             valid_until=response["expires_in"],  # Needs to be adjusted to DT
         )
 
     # pass='audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=password&password=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access&username=FILL_THIS_IN%40gmail.com'
     # curl -d "$pass" https://api.yotoplay.com/auth/token | jq '.access_token'
 
-    def update_devices(self, token) -> list[YotoPlayer]:
+    def update_devices(self, token) -> dict[YotoPlayer]:
         response = self._get_devices(token)
-        result = []
+        result = {}
         for device in response["devices"]:
             player: YotoPlayer = YotoPlayer(
                 id=device["deviceId"],
                 name=device["name"],
                 deviceType=device["deviceType"],
                 online=device["online"],
+                last_updated_at=datetime.datetime.now()
             )
-            result.append(player)
+            result[player.id] = player
 
         return result
         # TODO: parse the data and return a list of yoto devices.
 
     def update_library(self, token) -> list[Card]:
         cards = self._get_cards(token)
         return cards
```

### Comparing `yoto_api-1.0.9/yoto_api/YotoManager.py` & `yoto_api-1.1.0/yoto_api/YotoManager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """YotoManager.py"""
 
 import logging
-import datetime as dt
-import pytz
 from .YotoAPI import YotoAPI
 from .Token import Token
-from .const import DOMAIN
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class YotoManager:
     def __init__(self, username: str, password: str) -> None:
         self.username: str = username
         self.password: str = password
         self.api: YotoAPI = YotoAPI()
         self.players: dict = {}
         self.token: Token = None
-
-        self.token: Token = self.api.login(self.username, self.password)
         self.players: list = None
         self.library: list = None
-        self.initialize()
 
     def initialize(self) -> None:
-        self.update_player_status(self.token)
-        self.update_cards(self.token)
+        self.token: Token = self.api.login(self.username, self.password)
+        self.update_player_status()
+        self.update_cards()
 
     def update_player_status(self) -> None:
-        # TODO: Should update the self.players object with a current dict of players. Below isn't complete
+        # Updates the data with current player data.
         self.players = self.api.update_devices(self.token)
 
     def update_cards(self) -> None:
+        # Updates library and all card data.  Typically only required on startup.
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.library = self.api.update_library(self.token)
 
     def check_and_refresh_token(self) -> bool:
         if self.token is None:
             self.initialize()
-        if self.token.valid_until <= dt.datetime.now(pytz.utc):
-            _LOGGER.debug(f"{DOMAIN} - Refresh token expired")
-            self.token: Token = self.api.refresh_token(self.token)
-            return True
-        return False
+        # Check if valid and correct if not
+        # if self.token.valid_until <= dt.datetime.now(pytz.utc):
+        # _LOGGER.debug(f"{DOMAIN} - Refresh token expired")
+        # self.token: Token = self.api.refresh_token(self.token)
+        return True
+        # return False
```

### Comparing `yoto_api-1.0.9/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.1.0/yoto_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Requires-Python: >=3.9
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 Introduction
 ============
 
-Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far. 
+Early days of this API. Plan is to use this for home assistant. Basics are only item build for auth so far.
 
 To run this code for test I am doing::
 
     from pathlib import Path
     import logging
     import sys
     import os
@@ -32,8 +32,10 @@
     sys.path.append(str(path_root))
     from yoto_api import \*
 
     logging.basicConfig(stream=sys.stdout, level=logging.DEBUG, format='%(asctime)s %(name)s %(levelname)s:%(message)s')
     logger = logging.getLogger(**name**)
 
     ym = YotoManager(username="username", password="password")
+    ym.check_and_refresh_token()
+    ym.update_player_status()
     print (ym.players)
```

