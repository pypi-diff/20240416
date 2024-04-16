# Comparing `tmp/alibabacloud_sasti20200512_py2-1.0.2.tar.gz` & `tmp/alibabacloud_sasti20200512_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_sasti20200512_py2-1.0.2.tar", last modified: Mon Aug 21 08:22:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_sasti20200512_py2-1.0.3.tar", last modified: Tue Apr 16 17:15:09 2024, max compression
```

## Comparing `alibabacloud_sasti20200512_py2-1.0.2.tar` & `alibabacloud_sasti20200512_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      163 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2484 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/client.py
--rw-r--r--   0 root         (0) root         (0)    17077 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2484 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      456 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2913 2023-08-21 08:22:34.000000 alibabacloud_sasti20200512_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/client.py
+-rw-r--r--   0 root         (0) root         (0)    16567 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2913 2024-04-16 17:15:09.000000 alibabacloud_sasti20200512_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/LICENSE` & `alibabacloud_sasti20200512_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/PKG-INFO` & `alibabacloud_sasti20200512_py2-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_sasti20200512_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Sasti (20200512) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/README-CN.md` & `alibabacloud_sasti20200512_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/README.md` & `alibabacloud_sasti20200512_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/client.py` & `alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512/models.py` & `alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,14 @@
 class DescribeDomainReportResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeDomainReportResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeDomainReportResponse, self).to_map()
         if _map is not None:
             return _map
@@ -259,17 +256,14 @@
 class DescribeFileReportResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeFileReportResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeFileReportResponse, self).to_map()
         if _map is not None:
             return _map
@@ -413,17 +407,14 @@
 class DescribeIpReportResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeIpReportResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeIpReportResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/alibabacloud_sasti20200512_py2.egg-info/PKG-INFO` & `alibabacloud_sasti20200512_py2-1.0.3/alibabacloud_sasti20200512_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-sasti20200512-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud Sasti (20200512) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_sasti20200512_py2-1.0.2/setup.py` & `alibabacloud_sasti20200512_py2-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_sasti20200512_py2.
 
-Created on 21/08/2023
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_sasti20200512"
 NAME = "alibabacloud_sasti20200512_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Sasti (20200512) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```

