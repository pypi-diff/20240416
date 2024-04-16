# Comparing `tmp/yoto_api-1.1.0.tar.gz` & `tmp/yoto_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.1.0.tar", last modified: Mon Apr 15 23:55:41 2024, max compression
+gzip compressed data, was "yoto_api-1.2.0.tar", last modified: Tue Apr 16 00:44:24 2024, max compression
```

## Comparing `yoto_api-1.1.0.tar` & `yoto_api-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.669992 yoto_api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-15 23:55:12.000000 yoto_api-1.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-15 23:55:12.000000 yoto_api-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 23:55:12.000000 yoto_api-1.1.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 23:55:12.000000 yoto_api-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 23:55:12.000000 yoto_api-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-15 23:55:41.669992 yoto_api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 23:55:12.000000 yoto_api-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:12.000000 yoto_api-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 23:55:41.669992 yoto_api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-15 23:55:34.000000 yoto_api-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:12.000000 yoto_api-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-15 23:55:12.000000 yoto_api-1.1.0/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    18901 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 23:55:12.000000 yoto_api-1.1.0/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:41.665992 yoto_api-1.1.0/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 23:55:41.000000 yoto_api-1.1.0/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-16 00:43:28.000000 yoto_api-1.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-16 00:43:28.000000 yoto_api-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 00:43:28.000000 yoto_api-1.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 00:43:28.000000 yoto_api-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-16 00:43:28.000000 yoto_api-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:44:24.062342 yoto_api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-16 00:43:28.000000 yoto_api-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:43:28.000000 yoto_api-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:44:24.062342 yoto_api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-16 00:44:07.000000 yoto_api-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 00:43:28.000000 yoto_api-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-16 00:43:28.000000 yoto_api-1.2.0/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19621 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 00:43:28.000000 yoto_api-1.2.0/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:44:24.062342 yoto_api-1.2.0/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:44:23.000000 yoto_api-1.2.0/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 00:44:24.000000 yoto_api-1.2.0/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.1.0/CONTRIBUTING.rst` & `yoto_api-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.1.0/LICENSE` & `yoto_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.1.0/PKG-INFO` & `yoto_api-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.1.0/README.rst` & `yoto_api-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.1.0/setup.py` & `yoto_api-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="yoto_api",
     name="yoto_api",
     packages=find_packages(include=["yoto_api", "yoto_api.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/cdnninja/yoto_api",
-    version="1.1.0",
+    version="1.2.0",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.1.0/yoto_api/Card.py` & `yoto_api-1.2.0/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.1.0/yoto_api/YotoAPI.py` & `yoto_api-1.2.0/yoto_api/YotoAPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         self.SCOPE: str = "YOUR_SCOPE"
         # self.MQTT_AUTH_NAME: str = "JwtAuthorizer_mGDDmvLsocFY"
         # self.MQTT_URL: str = "wss://aqrphjqbp3u2z-ats.iot.eu-west-2.amazonaws.com"
 
     def login(self, username: str, password: str) -> Token:
         url = self.TOKEN_URL
         payload = {}
-        # all the values here should be URL encoded - not sure if this is done automatically by requests
         payload["audience"] = self.BASE_URL
         payload["client_id"] = self.CLIENT_ID
         payload["grant_type"] = "password"
         payload["password"] = password
         payload["scope"] = "openid email profile offline_access"
         payload["username"] = username
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
@@ -66,18 +65,34 @@
 
     def update_library(self, token) -> list[Card]:
         cards = self._get_cards(token)
         return cards
         # TODO: parse the data and return a list of cards.
 
     def refresh_token(self, token: Token) -> Token:
-        # to do: add command to refresh token
         # audience=https%3A//api.yotoplay.com&client_id=FILL_THIS_IN&grant_type=refresh_token&refresh_token=FILL_THIS_IN&scope=openid%20email%20profile%20offline_access
-
-        return token
+        url = self.TOKEN_URL
+        payload = {}
+        payload["audience"] = self.BASE_URL
+        payload["client_id"] = self.CLIENT_ID
+        payload["grant_type"] = "refresh_token"
+        payload["refresh_token"] = token.refresh_token
+        payload["scope"] = "openid email profile offline_access"
+        headers = {"Content-Type": "application/x-www-form-urlencoded"}
+        response = requests.post(url, data=payload, headers=headers).json()
+        _LOGGER.debug(f"{DOMAIN} - Sign In Response {response}")
+        return Token(
+            username=token.username,
+            password=token.password,
+            access_token=response["access_token"],
+            refresh_token=response["refresh_token"],
+            token_type=response["token_type"],
+            scope=response["scope"],
+            valid_until=response["expires_in"],  # Needs to be adjusted to DT
+        )
 
     def _get_devices(self, token) -> None:
         url = self.BASE_URL + "/device-v2/devices/mine"
 
         headers = self._get_authenticated_headers(token)
 
         response = requests.get(url, headers=headers).json()
```

### Comparing `yoto_api-1.1.0/yoto_api/YotoManager.py` & `yoto_api-1.2.0/yoto_api/YotoManager.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.1.0/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.2.0/yoto_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

