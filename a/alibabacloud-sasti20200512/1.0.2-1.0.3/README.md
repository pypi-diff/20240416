# Comparing `tmp/alibabacloud_sasti20200512-1.0.2.tar.gz` & `tmp/alibabacloud_sasti20200512-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sasti20200512-1.0.2.tar", last modified: Mon Aug 21 08:23:18 2023, max compression
+gzip compressed data, was "dist/alibabacloud_sasti20200512-1.0.3.tar", last modified: Tue Apr 16 17:14:10 2024, max compression
```

## Comparing `alibabacloud_sasti20200512-1.0.2.tar` & `alibabacloud_sasti20200512-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      163 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2340 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10525 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/client.py
--rw-r--r--   0 root         (0) root         (0)    17028 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2340 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2621 2023-08-21 08:23:17.000000 alibabacloud_sasti20200512-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10525 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/client.py
+-rw-r--r--   0 root         (0) root         (0)    16518 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2621 2024-04-16 17:14:10.000000 alibabacloud_sasti20200512-1.0.3/setup.py
```

### Comparing `alibabacloud_sasti20200512-1.0.2/LICENSE` & `alibabacloud_sasti20200512-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512-1.0.2/PKG-INFO` & `alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_sasti20200512
-Version: 1.0.2
+Name: alibabacloud-sasti20200512
+Version: 1.0.3
 Summary: Alibaba Cloud Sasti (20200512) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/sasti-20200512/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_sasti20200512-1.0.2/README-CN.md` & `alibabacloud_sasti20200512-1.0.3/README-CN.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/sasti-20200512/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_sasti20200512-1.0.2/README.md` & `alibabacloud_sasti20200512-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/sasti-20200512/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/client.py` & `alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512/models.py` & `alibabacloud_sasti20200512-1.0.3/alibabacloud_sasti20200512/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,17 +156,14 @@
         body: DescribeDomainReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -302,17 +299,14 @@
         body: DescribeFileReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -478,17 +472,14 @@
         body: DescribeIpReportResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_sasti20200512-1.0.2/alibabacloud_sasti20200512.egg-info/PKG-INFO` & `alibabacloud_sasti20200512-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-sasti20200512
-Version: 1.0.2
+Name: alibabacloud_sasti20200512
+Version: 1.0.3
 Summary: Alibaba Cloud Sasti (20200512) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/sasti-20200512/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_sasti20200512-1.0.2/setup.py` & `alibabacloud_sasti20200512-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sasti20200512.
 
-Created on 21/08/2023
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sasti20200512"
 NAME = "alibabacloud_sasti20200512" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Sasti (20200512) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

