# Comparing `tmp/tokive-1.4.tar.gz` & `tmp/tokive-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokive-1.4.tar", last modified: Thu Apr 11 03:22:08 2024, max compression
+gzip compressed data, was "tokive-1.5.tar", last modified: Tue Apr 16 05:16:55 2024, max compression
```

## Comparing `tokive-1.4.tar` & `tokive-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:08.573993 tokive-1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 03:22:08.573993 tokive-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 03:22:04.000000 tokive-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 03:22:08.573993 tokive-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-11 03:22:04.000000 tokive-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:08.573993 tokive-1.4/tokhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-11 03:22:04.000000 tokive-1.4/tokhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 03:22:04.000000 tokive-1.4/tokhelper/captchaCheck_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-11 03:22:04.000000 tokive-1.4/tokhelper/solve_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    58572 2024-04-11 03:22:04.000000 tokive-1.4/tokhelper/tiktok_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-11 03:22:04.000000 tokive-1.4/tokhelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 03:22:04.000000 tokive-1.4/tokive
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:22:08.573993 tokive-1.4/tokive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 03:22:08.000000 tokive-1.4/tokive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-11 03:22:08.000000 tokive-1.4/tokive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:22:08.000000 tokive-1.4/tokive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 03:22:08.000000 tokive-1.4/tokive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 03:22:08.000000 tokive-1.4/tokive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.884127 tokive-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 05:16:55.884127 tokive-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 05:16:48.000000 tokive-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 05:16:55.884127 tokive-1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-16 05:16:48.000000 tokive-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.880127 tokive-1.5/tokhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/captchaCheck_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/solve_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58756 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/tiktok_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-16 05:16:48.000000 tokive-1.5/tokhelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-16 05:16:48.000000 tokive-1.5/tokive
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:16:55.880127 tokive-1.5/tokive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 05:16:55.000000 tokive-1.5/tokive.egg-info/top_level.txt
```

### Comparing `tokive-1.4/setup.py` & `tokive-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='tokive',
-    version='1.4',
+    version='1.5',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of tokive",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/AutoWinTeam/tokive",
     packages=setuptools.find_packages(),
```

### Comparing `tokive-1.4/tokhelper/captchaCheck_pb2.py` & `tokive-1.5/tokhelper/captchaCheck_pb2.py`

 * *Files identical despite different names*

### Comparing `tokive-1.4/tokhelper/solve_captcha.py` & `tokive-1.5/tokhelper/solve_captcha.py`

 * *Files identical despite different names*

### Comparing `tokive-1.4/tokhelper/tiktok_main.py` & `tokive-1.5/tokhelper/tiktok_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 import json, sys
 from tokhelper import captchaCheck_pb2
 from tokhelper.solve_captcha import TikTokCaptchaSolver
 from urllib.parse import urlencode
 import traceback
 URL_SESSION="https://autolive.vip/api/tiktok/commit"
 
-P_VERSION_CODE="0.52.4"
-P_BROWSER_VERSION="5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.52.4 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
-H_USER_AGENT="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.52.4 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
+P_VERSION_CODE="0.54.0"
+P_WEBCAST_VERSION="540"
+P_BROWSER_VERSION="5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.54.0 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
+H_USER_AGENT="Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) TikTokLIVEStudio/0.54.0 Chrome/104.0.5112.102 Electron/20.1.0-tt.8.release.main.35 TTElectron/20.1.0-tt.8.release.main.35 Safari/537.36"
 
 def load_tiktok_acc(id):
     url = f"https://autolive.vip/api/tiktok/load?id={id}"
     data = None
     try:
         headers={"platform":"Autolive"}
         res = requests.get(url, headers=headers).json()
@@ -120,15 +121,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version':424,
+            'webcast_sdk_version':P_WEBCAST_VERSION,
             'live_mode':6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -384,15 +385,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version':424,
+            'webcast_sdk_version':P_WEBCAST_VERSION,
             'live_mode':6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -464,15 +465,15 @@
         "browser_platform": "Win32",
         "browser_name": "Mozilla",
         "browser_version": P_BROWSER_VERSION,
         "language": "en",
         "app_language": "en",
         "webcast_language": "en",
         "priority_region": acc['priority_region'],
-        "webcast_sdk_version": "424",
+        "webcast_sdk_version": P_WEBCAST_VERSION,
         "live_mode": "6"
     }
     print(params)
     headers = {
         'accept': 'application/x-protobuf',
         'accept-language': 'en-US',
         'content-type': 'application/x-protobuf',
@@ -521,15 +522,15 @@
             "browser_platform": "Win32",
             "browser_name": "Mozilla",
             "browser_version": P_BROWSER_VERSION,
             "language": "en",
             "app_language": "en",
             "webcast_language": "en",
             "priority_region": acc['priority_region'],
-            "webcast_sdk_version": "424",
+            "webcast_sdk_version": P_WEBCAST_VERSION,
             "live_mode": "6"
         }
         print(params)
         headers = {
             'accept': 'application/x-protobuf',
             'accept-language': 'en-US',
             'content-type': 'application/x-protobuf',
@@ -577,15 +578,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version': 424,
+            'webcast_sdk_version': P_WEBCAST_VERSION,
             'live_mode': 6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -638,15 +639,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version': 424,
+            'webcast_sdk_version': P_WEBCAST_VERSION,
             'live_mode': 6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -688,15 +689,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version': 424,
+            'webcast_sdk_version': P_WEBCAST_VERSION,
             'live_mode': 6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -747,15 +748,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version': 424,
+            'webcast_sdk_version': P_WEBCAST_VERSION,
             'live_mode': 6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -791,15 +792,15 @@
             "browser_platform": "Win32",
             "browser_name": "Mozilla",
             "browser_version": P_BROWSER_VERSION,
             "language": "en",
             "app_language": "en",
             "webcast_language": "en",
             "priority_region": acc['priority_region'],
-            "webcast_sdk_version": "424",
+            "webcast_sdk_version": P_WEBCAST_VERSION,
             "live_mode": "6"
         }
         headers = {
             'accept': 'application/json',
             'accept-language': 'en-US',
             'content-type': 'application/x-protobuf',
             'sec-fetch-dest': 'empty',
@@ -836,15 +837,15 @@
             "browser_platform": "Win32",
             "browser_name": "Mozilla",
             "browser_version": P_BROWSER_VERSION,
             "language": "en",
             "app_language": "en",
             "webcast_language": "en",
             "priority_region": acc['priority_region'],
-            "webcast_sdk_version": "424",
+            "webcast_sdk_version": P_WEBCAST_VERSION,
             "live_mode": "6"
         }
         headers = {
             'accept': 'application/json',
             'accept-language': 'en-US',
             'content-type': 'application/x-protobuf',
             'sec-fetch-dest': 'empty',
@@ -1020,15 +1021,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version':424,
+            'webcast_sdk_version':P_WEBCAST_VERSION,
             'live_mode':6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
@@ -1402,15 +1403,15 @@
             'browser_platform': 'Win32',
             'browser_name': 'Mozilla',
             'browser_version': P_BROWSER_VERSION,
             'language': 'en',
             'app_language': 'en',
             'webcast_language': 'en',
             'priority_region': acc['priority_region'],
-            'webcast_sdk_version': 424,
+            'webcast_sdk_version': P_WEBCAST_VERSION,
             'live_mode': 6
         }
         headers = {
             'accept': 'application/json, text/plain, */*',
             'accept-language': 'en-US',
             'content-type': 'application/x-www-form-urlencoded; charset=UTF-8',
             'sec-fetch-dest': 'empty',
```

### Comparing `tokive-1.4/tokhelper/utils.py` & `tokive-1.5/tokhelper/utils.py`

 * *Files identical despite different names*

### Comparing `tokive-1.4/tokive` & `tokive-1.5/tokive`

 * *Files identical despite different names*

