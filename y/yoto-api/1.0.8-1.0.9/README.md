# Comparing `tmp/yoto_api-1.0.8.tar.gz` & `tmp/yoto_api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoto_api-1.0.8.tar", last modified: Sun Apr 14 20:36:23 2024, max compression
+gzip compressed data, was "yoto_api-1.0.9.tar", last modified: Sun Apr 14 21:59:16 2024, max compression
```

## Comparing `yoto_api-1.0.8.tar` & `yoto_api-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:36:23.465222 yoto_api-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 20:35:56.000000 yoto_api-1.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-14 20:35:56.000000 yoto_api-1.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 20:35:56.000000 yoto_api-1.0.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 20:35:56.000000 yoto_api-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 20:35:56.000000 yoto_api-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 20:36:23.465222 yoto_api-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-14 20:35:56.000000 yoto_api-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:35:56.000000 yoto_api-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:36:23.465222 yoto_api-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-14 20:36:16.000000 yoto_api-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:36:23.461223 yoto_api-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:35:56.000000 yoto_api-1.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-14 20:35:56.000000 yoto_api-1.0.8/tests/login_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:36:23.461223 yoto_api-1.0.8/yoto_api/
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/YotoAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/YotoManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/YotoPlayer.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 20:35:56.000000 yoto_api-1.0.8/yoto_api/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:36:23.465222 yoto_api-1.0.8/yoto_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 20:36:23.000000 yoto_api-1.0.8/yoto_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 20:36:23.000000 yoto_api-1.0.8/yoto_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:36:23.000000 yoto_api-1.0.8/yoto_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:36:23.000000 yoto_api-1.0.8/yoto_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 20:36:23.000000 yoto_api-1.0.8/yoto_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 21:58:54.000000 yoto_api-1.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-14 21:58:54.000000 yoto_api-1.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 21:58:54.000000 yoto_api-1.0.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 21:58:54.000000 yoto_api-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-14 21:58:54.000000 yoto_api-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 21:59:16.304932 yoto_api-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-14 21:58:54.000000 yoto_api-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:58:54.000000 yoto_api-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:59:16.304932 yoto_api-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-14 21:59:10.000000 yoto_api-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.300932 yoto_api-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:58:54.000000 yoto_api-1.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-14 21:58:54.000000 yoto_api-1.0.9/tests/login_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/yoto_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/YotoPlayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 21:58:54.000000 yoto_api-1.0.9/yoto_api/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:59:16.304932 yoto_api-1.0.9/yoto_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 21:59:16.000000 yoto_api-1.0.9/yoto_api.egg-info/top_level.txt
```

### Comparing `yoto_api-1.0.8/CONTRIBUTING.rst` & `yoto_api-1.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.8/LICENSE` & `yoto_api-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.8/PKG-INFO` & `yoto_api-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `yoto_api-1.0.8/README.rst` & `yoto_api-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.8/setup.py` & `yoto_api-1.0.9/setup.py`

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
-    version="1.0.8",
+    version="1.0.9",
     zip_safe=False,
 )
```

### Comparing `yoto_api-1.0.8/yoto_api/Card.py` & `yoto_api-1.0.9/yoto_api/Card.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.8/yoto_api/YotoAPI.py` & `yoto_api-1.0.9/yoto_api/YotoAPI.py`

 * *Files identical despite different names*

### Comparing `yoto_api-1.0.8/yoto_api/YotoManager.py` & `yoto_api-1.0.9/yoto_api/YotoManager.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,19 +23,19 @@
         self.library: list = None
         self.initialize()
 
     def initialize(self) -> None:
         self.update_player_status(self.token)
         self.update_cards(self.token)
 
-    def update_player_status(self, token) -> None:
+    def update_player_status(self) -> None:
         # TODO: Should update the self.players object with a current dict of players. Below isn't complete
         self.players = self.api.update_devices(self.token)
 
-    def update_cards(self, token) -> None:
+    def update_cards(self) -> None:
         # TODO: Should update the self.library object with a current dict of players. Should it do details for all cards too or separate?
         self.library = self.api.update_library(self.token)
 
     def check_and_refresh_token(self) -> bool:
         if self.token is None:
             self.initialize()
         if self.token.valid_until <= dt.datetime.now(pytz.utc):
```

### Comparing `yoto_api-1.0.8/yoto_api.egg-info/PKG-INFO` & `yoto_api-1.0.9/yoto_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yoto_api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/cdnninja/yoto_api
 Author: cdnninja
 Author-email: 
 License: MIT license
 Keywords: yoto_api
 Classifier: Development Status :: 2 - Pre-Alpha
```

