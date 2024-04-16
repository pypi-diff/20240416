# Comparing `tmp/antchain_nftc-1.0.8.tar.gz` & `tmp/antchain_nftc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftc-1.0.8.tar", last modified: Wed Dec  6 05:42:10 2023, max compression
+gzip compressed data, was "dist/antchain_nftc-1.0.9.tar", last modified: Thu Dec 14 07:33:18 2023, max compression
```

## Comparing `antchain_nftc-1.0.8.tar` & `antchain_nftc-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      600 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_nftc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/antchain_sdk_nftc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/antchain_sdk_nftc/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43489 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/antchain_sdk_nftc/client.py
--rw-r--r--   0 root         (0) root         (0)    84654 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/antchain_sdk_nftc/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-06 05:42:10.000000 antchain_nftc-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2023-12-06 05:42:09.000000 antchain_nftc-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_nftc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_sdk_nftc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_sdk_nftc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43489 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_sdk_nftc/client.py
+-rw-r--r--   0 root         (0) root         (0)    85806 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/antchain_sdk_nftc/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-12-14 07:33:18.000000 antchain_nftc-1.0.9/setup.py
```

### Comparing `antchain_nftc-1.0.8/LICENSE` & `antchain_nftc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.8/PKG-INFO` & `antchain_nftc-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain NFTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftc-1.0.8/README-CN.md` & `antchain_nftc-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.8/README.md` & `antchain_nftc-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftc-1.0.8/antchain_nftc.egg-info/PKG-INFO` & `antchain_nftc-1.0.9/antchain_nftc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Ant Chain NFTC SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftc-1.0.8/antchain_sdk_nftc/client.py` & `antchain_nftc-1.0.9/antchain_sdk_nftc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'NFTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.8',
+                    'sdk_version': '1.0.9',
                     '_prod_code': 'NFTC',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_nftc-1.0.8/antchain_sdk_nftc/models.py` & `antchain_nftc-1.0.9/antchain_sdk_nftc/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,36 +159,48 @@
         self,
         deco_id: str = None,
         deco_name: str = None,
         web_ab_url: str = None,
         texture_url: str = None,
         thumbnail: str = None,
         avatar_pv_json: str = None,
+        android_ab_url: str = None,
+        ios_ab_url: str = None,
+        faling_texture_url: str = None,
     ):
         # 装扮id
         self.deco_id = deco_id
         # 装扮名称
         self.deco_name = deco_name
         # webGl ab包地址
         self.web_ab_url = web_ab_url
         # 贴图文件配置
         self.texture_url = texture_url
         # 缩略图
         self.thumbnail = thumbnail
         # json字符串，装扮额外属性信息
         # 如自定义头发颜色，性别等
         self.avatar_pv_json = avatar_pv_json
+        # 安卓ab包
+        self.android_ab_url = android_ab_url
+        # IOS AB 包
+        self.ios_ab_url = ios_ab_url
+        # 法令贴图文件
+        self.faling_texture_url = faling_texture_url
 
     def validate(self):
         self.validate_required(self.deco_id, 'deco_id')
         self.validate_required(self.deco_name, 'deco_name')
         self.validate_required(self.web_ab_url, 'web_ab_url')
         self.validate_required(self.texture_url, 'texture_url')
         self.validate_required(self.thumbnail, 'thumbnail')
         self.validate_required(self.avatar_pv_json, 'avatar_pv_json')
+        self.validate_required(self.android_ab_url, 'android_ab_url')
+        self.validate_required(self.ios_ab_url, 'ios_ab_url')
+        self.validate_required(self.faling_texture_url, 'faling_texture_url')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -200,14 +212,20 @@
             result['web_ab_url'] = self.web_ab_url
         if self.texture_url is not None:
             result['texture_url'] = self.texture_url
         if self.thumbnail is not None:
             result['thumbnail'] = self.thumbnail
         if self.avatar_pv_json is not None:
             result['avatar_pv_json'] = self.avatar_pv_json
+        if self.android_ab_url is not None:
+            result['android_ab_url'] = self.android_ab_url
+        if self.ios_ab_url is not None:
+            result['ios_ab_url'] = self.ios_ab_url
+        if self.faling_texture_url is not None:
+            result['faling_texture_url'] = self.faling_texture_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('deco_id') is not None:
             self.deco_id = m.get('deco_id')
         if m.get('deco_name') is not None:
@@ -216,14 +234,20 @@
             self.web_ab_url = m.get('web_ab_url')
         if m.get('texture_url') is not None:
             self.texture_url = m.get('texture_url')
         if m.get('thumbnail') is not None:
             self.thumbnail = m.get('thumbnail')
         if m.get('avatar_pv_json') is not None:
             self.avatar_pv_json = m.get('avatar_pv_json')
+        if m.get('android_ab_url') is not None:
+            self.android_ab_url = m.get('android_ab_url')
+        if m.get('ios_ab_url') is not None:
+            self.ios_ab_url = m.get('ios_ab_url')
+        if m.get('faling_texture_url') is not None:
+            self.faling_texture_url = m.get('faling_texture_url')
         return self
 
 
 class ExternalOrderItemDTO(TeaModel):
     def __init__(
         self,
         sku_id: int = None,
```

### Comparing `antchain_nftc-1.0.8/setup.py` & `antchain_nftc-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftc.
 
-Created on 06/12/2023
+Created on 14/12/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftc"
 NAME = "antchain_nftc" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTC SDK Library for Python"
```

