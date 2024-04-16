# Comparing `tmp/alibabacloud_chatbot20220408_py2-1.2.0.tar.gz` & `tmp/alibabacloud_chatbot20220408_py2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.2.0.tar", last modified: Thu Feb 22 13:51:25 2024, max compression
+gzip compressed data, was "dist/alibabacloud_chatbot20220408_py2-1.3.0.tar", last modified: Tue Apr 16 17:14:09 2024, max compression
```

## Comparing `alibabacloud_chatbot20220408_py2-1.2.0.tar` & `alibabacloud_chatbot20220408_py2-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      880 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112764 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/client.py
--rw-r--r--   0 root         (0) root         (0)   454272 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2923 2024-02-22 13:51:25.000000 alibabacloud_chatbot20220408_py2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1612 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112878 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/client.py
+-rw-r--r--   0 root         (0) root         (0)   454816 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:14:09.000000 alibabacloud_chatbot20220408_py2-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2923 2024-04-16 17:14:08.000000 alibabacloud_chatbot20220408_py2-1.3.0/setup.py
```

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/LICENSE` & `alibabacloud_chatbot20220408_py2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_chatbot20220408_py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/README-CN.md` & `alibabacloud_chatbot20220408_py2-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/README.md` & `alibabacloud_chatbot20220408_py2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/client.py` & `alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1729,14 +1729,16 @@
             query['AgentName'] = request.agent_name
         if not UtilClient.is_unset(request.goods_codes):
             query['GoodsCodes'] = request.goods_codes
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.product_code):
+            query['ProductCode'] = request.product_code
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListAgent',
             version='2022-04-08',
             protocol='HTTPS',
```

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408/models.py` & `alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7136,19 +7136,20 @@
         if m.get('body') is not None:
             temp_model = LinkInstanceCategoryResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListAgentRequest(TeaModel):
-    def __init__(self, agent_name=None, goods_codes=None, page_number=None, page_size=None):
+    def __init__(self, agent_name=None, goods_codes=None, page_number=None, page_size=None, product_code=None):
         self.agent_name = agent_name  # type: str
         self.goods_codes = goods_codes  # type: str
         self.page_number = page_number  # type: int
         self.page_size = page_size  # type: int
+        self.product_code = product_code  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListAgentRequest, self).to_map()
         if _map is not None:
@@ -7159,34 +7160,39 @@
             result['AgentName'] = self.agent_name
         if self.goods_codes is not None:
             result['GoodsCodes'] = self.goods_codes
         if self.page_number is not None:
             result['PageNumber'] = self.page_number
         if self.page_size is not None:
             result['PageSize'] = self.page_size
+        if self.product_code is not None:
+            result['ProductCode'] = self.product_code
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AgentName') is not None:
             self.agent_name = m.get('AgentName')
         if m.get('GoodsCodes') is not None:
             self.goods_codes = m.get('GoodsCodes')
         if m.get('PageNumber') is not None:
             self.page_number = m.get('PageNumber')
         if m.get('PageSize') is not None:
             self.page_size = m.get('PageSize')
+        if m.get('ProductCode') is not None:
+            self.product_code = m.get('ProductCode')
         return self
 
 
 class ListAgentResponseBodyData(TeaModel):
-    def __init__(self, agent_id=None, agent_key=None, agent_name=None, instance_infos=None):
+    def __init__(self, agent_id=None, agent_key=None, agent_name=None, default_agent=None, instance_infos=None):
         self.agent_id = agent_id  # type: long
         self.agent_key = agent_key  # type: str
         self.agent_name = agent_name  # type: str
+        self.default_agent = default_agent  # type: bool
         self.instance_infos = instance_infos  # type: dict[str, any]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListAgentResponseBodyData, self).to_map()
@@ -7196,26 +7202,30 @@
         result = dict()
         if self.agent_id is not None:
             result['AgentId'] = self.agent_id
         if self.agent_key is not None:
             result['AgentKey'] = self.agent_key
         if self.agent_name is not None:
             result['AgentName'] = self.agent_name
+        if self.default_agent is not None:
+            result['DefaultAgent'] = self.default_agent
         if self.instance_infos is not None:
             result['InstanceInfos'] = self.instance_infos
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('AgentId') is not None:
             self.agent_id = m.get('AgentId')
         if m.get('AgentKey') is not None:
             self.agent_key = m.get('AgentKey')
         if m.get('AgentName') is not None:
             self.agent_name = m.get('AgentName')
+        if m.get('DefaultAgent') is not None:
+            self.default_agent = m.get('DefaultAgent')
         if m.get('InstanceInfos') is not None:
             self.instance_infos = m.get('InstanceInfos')
         return self
 
 
 class ListAgentResponseBody(TeaModel):
     def __init__(self, data=None, page_number=None, page_size=None, request_id=None, total_count=None):
```

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO` & `alibabacloud_chatbot20220408_py2-1.3.0/alibabacloud_chatbot20220408_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-chatbot20220408-py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud Chatbot (20220408) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_chatbot20220408_py2-1.2.0/setup.py` & `alibabacloud_chatbot20220408_py2-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_chatbot20220408_py2.
 
-Created on 22/02/2024
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_chatbot20220408"
 NAME = "alibabacloud_chatbot20220408_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Chatbot (20220408) SDK Library for Python2"
```

