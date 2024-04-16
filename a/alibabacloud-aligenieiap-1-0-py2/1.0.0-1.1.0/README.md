# Comparing `tmp/alibabacloud_aligenieiap_1_0_py2-1.0.0.tar.gz` & `tmp/alibabacloud_aligenieiap_1_0_py2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0_py2-1.0.0.tar", last modified: Fri Dec 15 06:06:25 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0_py2-1.1.0.tar", last modified: Tue Apr 16 17:15:19 2024, max compression
```

## Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0.tar` & `alibabacloud_aligenieiap_1_0_py2-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2497 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1129 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33019 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155250 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2497 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      459 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2874 2023-12-15 06:06:25.000000 alibabacloud_aligenieiap_1_0_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1129 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41474 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   183861 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2927 2024-04-16 17:15:19.000000 alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.py
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/LICENSE` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/PKG-INFO` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieiap_1_0_py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/README-CN.md` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/README.md` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/client.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 from __future__ import unicode_literals
 
 from Tea.core import TeaCore
 
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_tea_util.client import Client as UtilClient
+from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_aligenieiap_1_0 import models as ali_genieiap__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(self, config):
         super(Client, self).__init__(config)
         self._endpoint_rule = ''
-        if UtilClient.empty(self._endpoint):
-            self._endpoint = 'openapi.aligenie.com/v1.0/iap'
+        self.check_config(config)
+        self._endpoint = self.get_endpoint('aligenie', self._region_id, self._endpoint_rule, self._network, self._suffix, self._endpoint_map, self._endpoint)
+
+    def get_endpoint(self, product_id, region_id, endpoint_rule, network, suffix, endpoint_map, endpoint):
+        if not UtilClient.empty(endpoint):
+            return endpoint
+        if not UtilClient.is_unset(endpoint_map) and not UtilClient.empty(endpoint_map.get(region_id)):
+            return endpoint_map.get(region_id)
+        return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def app_use_time_report_with_options(self, tmp_req, headers, runtime):
         UtilClient.validate_model(tmp_req)
         request = ali_genieiap__1__0_models.AppUseTimeReportShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
             request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
@@ -67,14 +75,120 @@
         )
 
     def app_use_time_report(self, request):
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.AppUseTimeReportHeaders()
         return self.app_use_time_report_with_options(request, headers, runtime)
 
+    def call_back_third_right_send_plan_with_options(self, tmp_req, headers, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = ali_genieiap__1__0_models.CallBackThirdRightSendPlanShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.extend_info):
+            request.extend_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.extend_info, 'ExtendInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.biz_group):
+            query['BizGroup'] = request.biz_group
+        if not UtilClient.is_unset(request.biz_type):
+            query['BizType'] = request.biz_type
+        if not UtilClient.is_unset(request.card_type):
+            query['CardType'] = request.card_type
+        if not UtilClient.is_unset(request.error_msg):
+            query['ErrorMsg'] = request.error_msg
+        if not UtilClient.is_unset(request.extend_info_shrink):
+            query['ExtendInfo'] = request.extend_info_shrink
+        if not UtilClient.is_unset(request.genie_open_id):
+            query['GenieOpenId'] = request.genie_open_id
+        if not UtilClient.is_unset(request.receive_status):
+            query['ReceiveStatus'] = request.receive_status
+        if not UtilClient.is_unset(request.sn):
+            query['Sn'] = request.sn
+        if not UtilClient.is_unset(request.supplier_id):
+            query['SupplierId'] = request.supplier_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CallBackThirdRightSendPlan',
+            version='iap_1.0',
+            protocol='HTTPS',
+            pathname='/1.0/iap/business/CallBackThirdRightSendPlan',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def call_back_third_right_send_plan(self, request):
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CallBackThirdRightSendPlanHeaders()
+        return self.call_back_third_right_send_plan_with_options(request, headers, runtime)
+
+    def check_third_right_send_plan_with_options(self, tmp_req, headers, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = ali_genieiap__1__0_models.CheckThirdRightSendPlanShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.extend_info):
+            request.extend_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.extend_info, 'ExtendInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.biz_group):
+            query['BizGroup'] = request.biz_group
+        if not UtilClient.is_unset(request.biz_type):
+            query['BizType'] = request.biz_type
+        if not UtilClient.is_unset(request.extend_info_shrink):
+            query['ExtendInfo'] = request.extend_info_shrink
+        if not UtilClient.is_unset(request.sn):
+            query['Sn'] = request.sn
+        if not UtilClient.is_unset(request.supplier_id):
+            query['SupplierId'] = request.supplier_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CheckThirdRightSendPlan',
+            version='iap_1.0',
+            protocol='HTTPS',
+            pathname='/v1.0/iap/business/CheckThirdRightSendPlan',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def check_third_right_send_plan(self, request):
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CheckThirdRightSendPlanHeaders()
+        return self.check_third_right_send_plan_with_options(request, headers, runtime)
+
     def create_reminder_with_options(self, tmp_req, headers, runtime):
         UtilClient.validate_model(tmp_req)
         request = ali_genieiap__1__0_models.CreateReminderShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
             request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.payload):
@@ -214,14 +328,63 @@
         )
 
     def get_account_for_app(self, request):
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.GetAccountForAppHeaders()
         return self.get_account_for_app_with_options(request, headers, runtime)
 
+    def get_bus_app_config_with_options(self, tmp_req, headers, runtime):
+        UtilClient.validate_model(tmp_req)
+        request = ali_genieiap__1__0_models.GetBusAppConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.device_info):
+            request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
+        if not UtilClient.is_unset(tmp_req.payload):
+            request.payload_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.payload, 'Payload', 'json')
+        if not UtilClient.is_unset(tmp_req.user_info):
+            request.user_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.user_info, 'UserInfo', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.device_info_shrink):
+            query['DeviceInfo'] = request.device_info_shrink
+        if not UtilClient.is_unset(request.payload_shrink):
+            query['Payload'] = request.payload_shrink
+        if not UtilClient.is_unset(request.user_info_shrink):
+            query['UserInfo'] = request.user_info_shrink
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_aligenie_access_token):
+            real_headers['x-acs-aligenie-access-token'] = UtilClient.to_jsonstring(headers.x_acs_aligenie_access_token)
+        if not UtilClient.is_unset(headers.authorization):
+            real_headers['Authorization'] = UtilClient.to_jsonstring(headers.authorization)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetBusAppConfig',
+            version='iap_1.0',
+            protocol='HTTPS',
+            pathname='/v1.0/iap/app/config/get',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.GetBusAppConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_bus_app_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.GetBusAppConfigHeaders()
+        return self.get_bus_app_config_with_options(request, headers, runtime)
+
     def get_phone_number_with_options(self, tmp_req, headers, runtime):
         UtilClient.validate_model(tmp_req)
         request = ali_genieiap__1__0_models.GetPhoneNumberShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.device_info):
             request.device_info_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.device_info, 'DeviceInfo', 'json')
         if not UtilClient.is_unset(tmp_req.user_info):
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0/models.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -293,17 +293,14 @@
 class AppUseTimeReportResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: AppUseTimeReportResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(AppUseTimeReportResponse, self).to_map()
         if _map is not None:
             return _map
@@ -325,14 +322,502 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AppUseTimeReportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CallBackThirdRightSendPlanHeaders(TeaModel):
+    def __init__(self, common_headers=None, x_acs_aligenie_access_token=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token  # type: str
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CallBackThirdRightSendPlanHeaders, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class CallBackThirdRightSendPlanRequest(TeaModel):
+    def __init__(self, biz_group=None, biz_type=None, card_type=None, error_msg=None, extend_info=None,
+                 genie_open_id=None, receive_status=None, sn=None, supplier_id=None):
+        self.biz_group = biz_group  # type: str
+        self.biz_type = biz_type  # type: str
+        self.card_type = card_type  # type: int
+        self.error_msg = error_msg  # type: str
+        self.extend_info = extend_info  # type: dict[str, any]
+        self.genie_open_id = genie_open_id  # type: str
+        self.receive_status = receive_status  # type: int
+        self.sn = sn  # type: str
+        self.supplier_id = supplier_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CallBackThirdRightSendPlanRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['BizGroup'] = self.biz_group
+        if self.biz_type is not None:
+            result['BizType'] = self.biz_type
+        if self.card_type is not None:
+            result['CardType'] = self.card_type
+        if self.error_msg is not None:
+            result['ErrorMsg'] = self.error_msg
+        if self.extend_info is not None:
+            result['ExtendInfo'] = self.extend_info
+        if self.genie_open_id is not None:
+            result['GenieOpenId'] = self.genie_open_id
+        if self.receive_status is not None:
+            result['ReceiveStatus'] = self.receive_status
+        if self.sn is not None:
+            result['Sn'] = self.sn
+        if self.supplier_id is not None:
+            result['SupplierId'] = self.supplier_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BizGroup') is not None:
+            self.biz_group = m.get('BizGroup')
+        if m.get('BizType') is not None:
+            self.biz_type = m.get('BizType')
+        if m.get('CardType') is not None:
+            self.card_type = m.get('CardType')
+        if m.get('ErrorMsg') is not None:
+            self.error_msg = m.get('ErrorMsg')
+        if m.get('ExtendInfo') is not None:
+            self.extend_info = m.get('ExtendInfo')
+        if m.get('GenieOpenId') is not None:
+            self.genie_open_id = m.get('GenieOpenId')
+        if m.get('ReceiveStatus') is not None:
+            self.receive_status = m.get('ReceiveStatus')
+        if m.get('Sn') is not None:
+            self.sn = m.get('Sn')
+        if m.get('SupplierId') is not None:
+            self.supplier_id = m.get('SupplierId')
+        return self
+
+
+class CallBackThirdRightSendPlanShrinkRequest(TeaModel):
+    def __init__(self, biz_group=None, biz_type=None, card_type=None, error_msg=None, extend_info_shrink=None,
+                 genie_open_id=None, receive_status=None, sn=None, supplier_id=None):
+        self.biz_group = biz_group  # type: str
+        self.biz_type = biz_type  # type: str
+        self.card_type = card_type  # type: int
+        self.error_msg = error_msg  # type: str
+        self.extend_info_shrink = extend_info_shrink  # type: str
+        self.genie_open_id = genie_open_id  # type: str
+        self.receive_status = receive_status  # type: int
+        self.sn = sn  # type: str
+        self.supplier_id = supplier_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CallBackThirdRightSendPlanShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['BizGroup'] = self.biz_group
+        if self.biz_type is not None:
+            result['BizType'] = self.biz_type
+        if self.card_type is not None:
+            result['CardType'] = self.card_type
+        if self.error_msg is not None:
+            result['ErrorMsg'] = self.error_msg
+        if self.extend_info_shrink is not None:
+            result['ExtendInfo'] = self.extend_info_shrink
+        if self.genie_open_id is not None:
+            result['GenieOpenId'] = self.genie_open_id
+        if self.receive_status is not None:
+            result['ReceiveStatus'] = self.receive_status
+        if self.sn is not None:
+            result['Sn'] = self.sn
+        if self.supplier_id is not None:
+            result['SupplierId'] = self.supplier_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BizGroup') is not None:
+            self.biz_group = m.get('BizGroup')
+        if m.get('BizType') is not None:
+            self.biz_type = m.get('BizType')
+        if m.get('CardType') is not None:
+            self.card_type = m.get('CardType')
+        if m.get('ErrorMsg') is not None:
+            self.error_msg = m.get('ErrorMsg')
+        if m.get('ExtendInfo') is not None:
+            self.extend_info_shrink = m.get('ExtendInfo')
+        if m.get('GenieOpenId') is not None:
+            self.genie_open_id = m.get('GenieOpenId')
+        if m.get('ReceiveStatus') is not None:
+            self.receive_status = m.get('ReceiveStatus')
+        if m.get('Sn') is not None:
+            self.sn = m.get('Sn')
+        if m.get('SupplierId') is not None:
+            self.supplier_id = m.get('SupplierId')
+        return self
+
+
+class CallBackThirdRightSendPlanResponseBody(TeaModel):
+    def __init__(self, ret_code=None, ret_msg=None, ret_value=None, request_id=None):
+        self.ret_code = ret_code  # type: str
+        self.ret_msg = ret_msg  # type: str
+        self.ret_value = ret_value  # type: bool
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CallBackThirdRightSendPlanResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ret_code is not None:
+            result['RetCode'] = self.ret_code
+        if self.ret_msg is not None:
+            result['RetMsg'] = self.ret_msg
+        if self.ret_value is not None:
+            result['RetValue'] = self.ret_value
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RetCode') is not None:
+            self.ret_code = m.get('RetCode')
+        if m.get('RetMsg') is not None:
+            self.ret_msg = m.get('RetMsg')
+        if m.get('RetValue') is not None:
+            self.ret_value = m.get('RetValue')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class CallBackThirdRightSendPlanResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CallBackThirdRightSendPlanResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CallBackThirdRightSendPlanResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CallBackThirdRightSendPlanResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CheckThirdRightSendPlanHeaders(TeaModel):
+    def __init__(self, common_headers=None, x_acs_aligenie_access_token=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token  # type: str
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanHeaders, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class CheckThirdRightSendPlanRequest(TeaModel):
+    def __init__(self, biz_group=None, biz_type=None, extend_info=None, sn=None, supplier_id=None):
+        self.biz_group = biz_group  # type: str
+        self.biz_type = biz_type  # type: str
+        self.extend_info = extend_info  # type: dict[str, any]
+        self.sn = sn  # type: str
+        self.supplier_id = supplier_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['BizGroup'] = self.biz_group
+        if self.biz_type is not None:
+            result['BizType'] = self.biz_type
+        if self.extend_info is not None:
+            result['ExtendInfo'] = self.extend_info
+        if self.sn is not None:
+            result['Sn'] = self.sn
+        if self.supplier_id is not None:
+            result['SupplierId'] = self.supplier_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BizGroup') is not None:
+            self.biz_group = m.get('BizGroup')
+        if m.get('BizType') is not None:
+            self.biz_type = m.get('BizType')
+        if m.get('ExtendInfo') is not None:
+            self.extend_info = m.get('ExtendInfo')
+        if m.get('Sn') is not None:
+            self.sn = m.get('Sn')
+        if m.get('SupplierId') is not None:
+            self.supplier_id = m.get('SupplierId')
+        return self
+
+
+class CheckThirdRightSendPlanShrinkRequest(TeaModel):
+    def __init__(self, biz_group=None, biz_type=None, extend_info_shrink=None, sn=None, supplier_id=None):
+        self.biz_group = biz_group  # type: str
+        self.biz_type = biz_type  # type: str
+        self.extend_info_shrink = extend_info_shrink  # type: str
+        self.sn = sn  # type: str
+        self.supplier_id = supplier_id  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.biz_group is not None:
+            result['BizGroup'] = self.biz_group
+        if self.biz_type is not None:
+            result['BizType'] = self.biz_type
+        if self.extend_info_shrink is not None:
+            result['ExtendInfo'] = self.extend_info_shrink
+        if self.sn is not None:
+            result['Sn'] = self.sn
+        if self.supplier_id is not None:
+            result['SupplierId'] = self.supplier_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('BizGroup') is not None:
+            self.biz_group = m.get('BizGroup')
+        if m.get('BizType') is not None:
+            self.biz_type = m.get('BizType')
+        if m.get('ExtendInfo') is not None:
+            self.extend_info_shrink = m.get('ExtendInfo')
+        if m.get('Sn') is not None:
+            self.sn = m.get('Sn')
+        if m.get('SupplierId') is not None:
+            self.supplier_id = m.get('SupplierId')
+        return self
+
+
+class CheckThirdRightSendPlanResponseBodyRetValue(TeaModel):
+    def __init__(self, activate_date=None, card_type=None, channel_code=None, channel_name=None, extend_info=None,
+                 request_id=None, rights_expired_date=None):
+        self.activate_date = activate_date  # type: str
+        self.card_type = card_type  # type: int
+        self.channel_code = channel_code  # type: str
+        self.channel_name = channel_name  # type: str
+        self.extend_info = extend_info  # type: dict[str, any]
+        self.request_id = request_id  # type: str
+        self.rights_expired_date = rights_expired_date  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanResponseBodyRetValue, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.activate_date is not None:
+            result['ActivateDate'] = self.activate_date
+        if self.card_type is not None:
+            result['CardType'] = self.card_type
+        if self.channel_code is not None:
+            result['ChannelCode'] = self.channel_code
+        if self.channel_name is not None:
+            result['ChannelName'] = self.channel_name
+        if self.extend_info is not None:
+            result['ExtendInfo'] = self.extend_info
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.rights_expired_date is not None:
+            result['RightsExpiredDate'] = self.rights_expired_date
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ActivateDate') is not None:
+            self.activate_date = m.get('ActivateDate')
+        if m.get('CardType') is not None:
+            self.card_type = m.get('CardType')
+        if m.get('ChannelCode') is not None:
+            self.channel_code = m.get('ChannelCode')
+        if m.get('ChannelName') is not None:
+            self.channel_name = m.get('ChannelName')
+        if m.get('ExtendInfo') is not None:
+            self.extend_info = m.get('ExtendInfo')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RightsExpiredDate') is not None:
+            self.rights_expired_date = m.get('RightsExpiredDate')
+        return self
+
+
+class CheckThirdRightSendPlanResponseBody(TeaModel):
+    def __init__(self, ret_code=None, ret_msg=None, ret_value=None):
+        self.ret_code = ret_code  # type: int
+        self.ret_msg = ret_msg  # type: str
+        self.ret_value = ret_value  # type: CheckThirdRightSendPlanResponseBodyRetValue
+
+    def validate(self):
+        if self.ret_value:
+            self.ret_value.validate()
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ret_code is not None:
+            result['RetCode'] = self.ret_code
+        if self.ret_msg is not None:
+            result['RetMsg'] = self.ret_msg
+        if self.ret_value is not None:
+            result['RetValue'] = self.ret_value.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RetCode') is not None:
+            self.ret_code = m.get('RetCode')
+        if m.get('RetMsg') is not None:
+            self.ret_msg = m.get('RetMsg')
+        if m.get('RetValue') is not None:
+            temp_model = CheckThirdRightSendPlanResponseBodyRetValue()
+            self.ret_value = temp_model.from_map(m['RetValue'])
+        return self
+
+
+class CheckThirdRightSendPlanResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CheckThirdRightSendPlanResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CheckThirdRightSendPlanResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CheckThirdRightSendPlanResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateReminderHeaders(TeaModel):
     def __init__(self, common_headers=None, x_acs_aligenie_access_token=None, authorization=None):
         self.common_headers = common_headers  # type: dict[str, str]
         self.x_acs_aligenie_access_token = x_acs_aligenie_access_token  # type: str
         self.authorization = authorization  # type: str
 
     def validate(self):
@@ -680,17 +1165,14 @@
 class CreateReminderResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateReminderResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateReminderResponse, self).to_map()
         if _map is not None:
             return _map
@@ -980,17 +1462,14 @@
 class DeleteReminderResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteReminderResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteReminderResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1316,17 +1795,14 @@
 class GetAccountForAppResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetAccountForAppResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetAccountForAppResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1348,14 +1824,352 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetAccountForAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetBusAppConfigHeaders(TeaModel):
+    def __init__(self, common_headers=None, x_acs_aligenie_access_token=None, authorization=None):
+        self.common_headers = common_headers  # type: dict[str, str]
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token  # type: str
+        self.authorization = authorization  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigHeaders, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_aligenie_access_token is not None:
+            result['x-acs-aligenie-access-token'] = self.x_acs_aligenie_access_token
+        if self.authorization is not None:
+            result['Authorization'] = self.authorization
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-aligenie-access-token') is not None:
+            self.x_acs_aligenie_access_token = m.get('x-acs-aligenie-access-token')
+        if m.get('Authorization') is not None:
+            self.authorization = m.get('Authorization')
+        return self
+
+
+class GetBusAppConfigRequestDeviceInfo(TeaModel):
+    def __init__(self, encode_key=None, encode_type=None, id=None, id_type=None, organization_id=None):
+        self.encode_key = encode_key  # type: str
+        self.encode_type = encode_type  # type: str
+        self.id = id  # type: str
+        self.id_type = id_type  # type: str
+        self.organization_id = organization_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigRequestDeviceInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.id_type is not None:
+            result['IdType'] = self.id_type
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdType') is not None:
+            self.id_type = m.get('IdType')
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        return self
+
+
+class GetBusAppConfigRequestPayload(TeaModel):
+    def __init__(self, origin_uuid=None, phone=None):
+        self.origin_uuid = origin_uuid  # type: str
+        self.phone = phone  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigRequestPayload, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.origin_uuid is not None:
+            result['originUuid'] = self.origin_uuid
+        if self.phone is not None:
+            result['phone'] = self.phone
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('originUuid') is not None:
+            self.origin_uuid = m.get('originUuid')
+        if m.get('phone') is not None:
+            self.phone = m.get('phone')
+        return self
+
+
+class GetBusAppConfigRequestUserInfo(TeaModel):
+    def __init__(self, encode_key=None, encode_type=None, id=None, id_type=None, organization_id=None):
+        self.encode_key = encode_key  # type: str
+        self.encode_type = encode_type  # type: str
+        self.id = id  # type: str
+        self.id_type = id_type  # type: str
+        self.organization_id = organization_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigRequestUserInfo, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.encode_key is not None:
+            result['EncodeKey'] = self.encode_key
+        if self.encode_type is not None:
+            result['EncodeType'] = self.encode_type
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.id_type is not None:
+            result['IdType'] = self.id_type
+        if self.organization_id is not None:
+            result['OrganizationId'] = self.organization_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EncodeKey') is not None:
+            self.encode_key = m.get('EncodeKey')
+        if m.get('EncodeType') is not None:
+            self.encode_type = m.get('EncodeType')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('IdType') is not None:
+            self.id_type = m.get('IdType')
+        if m.get('OrganizationId') is not None:
+            self.organization_id = m.get('OrganizationId')
+        return self
+
+
+class GetBusAppConfigRequest(TeaModel):
+    def __init__(self, device_info=None, payload=None, user_info=None):
+        self.device_info = device_info  # type: GetBusAppConfigRequestDeviceInfo
+        self.payload = payload  # type: GetBusAppConfigRequestPayload
+        self.user_info = user_info  # type: GetBusAppConfigRequestUserInfo
+
+    def validate(self):
+        if self.device_info:
+            self.device_info.validate()
+        if self.payload:
+            self.payload.validate()
+        if self.user_info:
+            self.user_info.validate()
+
+    def to_map(self):
+        _map = super(GetBusAppConfigRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_info is not None:
+            result['DeviceInfo'] = self.device_info.to_map()
+        if self.payload is not None:
+            result['Payload'] = self.payload.to_map()
+        if self.user_info is not None:
+            result['UserInfo'] = self.user_info.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DeviceInfo') is not None:
+            temp_model = GetBusAppConfigRequestDeviceInfo()
+            self.device_info = temp_model.from_map(m['DeviceInfo'])
+        if m.get('Payload') is not None:
+            temp_model = GetBusAppConfigRequestPayload()
+            self.payload = temp_model.from_map(m['Payload'])
+        if m.get('UserInfo') is not None:
+            temp_model = GetBusAppConfigRequestUserInfo()
+            self.user_info = temp_model.from_map(m['UserInfo'])
+        return self
+
+
+class GetBusAppConfigShrinkRequest(TeaModel):
+    def __init__(self, device_info_shrink=None, payload_shrink=None, user_info_shrink=None):
+        self.device_info_shrink = device_info_shrink  # type: str
+        self.payload_shrink = payload_shrink  # type: str
+        self.user_info_shrink = user_info_shrink  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigShrinkRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.device_info_shrink is not None:
+            result['DeviceInfo'] = self.device_info_shrink
+        if self.payload_shrink is not None:
+            result['Payload'] = self.payload_shrink
+        if self.user_info_shrink is not None:
+            result['UserInfo'] = self.user_info_shrink
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DeviceInfo') is not None:
+            self.device_info_shrink = m.get('DeviceInfo')
+        if m.get('Payload') is not None:
+            self.payload_shrink = m.get('Payload')
+        if m.get('UserInfo') is not None:
+            self.user_info_shrink = m.get('UserInfo')
+        return self
+
+
+class GetBusAppConfigResponseBodyRetValue(TeaModel):
+    def __init__(self, cashier=None, shopping_bar=None, shopping_window=None, vip_label=None):
+        self.cashier = cashier  # type: str
+        self.shopping_bar = shopping_bar  # type: str
+        self.shopping_window = shopping_window  # type: str
+        self.vip_label = vip_label  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetBusAppConfigResponseBodyRetValue, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.cashier is not None:
+            result['Cashier'] = self.cashier
+        if self.shopping_bar is not None:
+            result['ShoppingBar'] = self.shopping_bar
+        if self.shopping_window is not None:
+            result['ShoppingWindow'] = self.shopping_window
+        if self.vip_label is not None:
+            result['VipLabel'] = self.vip_label
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Cashier') is not None:
+            self.cashier = m.get('Cashier')
+        if m.get('ShoppingBar') is not None:
+            self.shopping_bar = m.get('ShoppingBar')
+        if m.get('ShoppingWindow') is not None:
+            self.shopping_window = m.get('ShoppingWindow')
+        if m.get('VipLabel') is not None:
+            self.vip_label = m.get('VipLabel')
+        return self
+
+
+class GetBusAppConfigResponseBody(TeaModel):
+    def __init__(self, ret_code=None, ret_msg=None, ret_value=None):
+        self.ret_code = ret_code  # type: int
+        self.ret_msg = ret_msg  # type: str
+        self.ret_value = ret_value  # type: GetBusAppConfigResponseBodyRetValue
+
+    def validate(self):
+        if self.ret_value:
+            self.ret_value.validate()
+
+    def to_map(self):
+        _map = super(GetBusAppConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ret_code is not None:
+            result['RetCode'] = self.ret_code
+        if self.ret_msg is not None:
+            result['RetMsg'] = self.ret_msg
+        if self.ret_value is not None:
+            result['RetValue'] = self.ret_value.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RetCode') is not None:
+            self.ret_code = m.get('RetCode')
+        if m.get('RetMsg') is not None:
+            self.ret_msg = m.get('RetMsg')
+        if m.get('RetValue') is not None:
+            temp_model = GetBusAppConfigResponseBodyRetValue()
+            self.ret_value = temp_model.from_map(m['RetValue'])
+        return self
+
+
+class GetBusAppConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetBusAppConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetBusAppConfigResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetBusAppConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetPhoneNumberHeaders(TeaModel):
     def __init__(self, common_headers=None, x_acs_aligenie_access_token=None, authorization=None):
         self.common_headers = common_headers  # type: dict[str, str]
         self.x_acs_aligenie_access_token = x_acs_aligenie_access_token  # type: str
         self.authorization = authorization  # type: str
 
     def validate(self):
@@ -1564,17 +2378,14 @@
 class GetPhoneNumberResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetPhoneNumberResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetPhoneNumberResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2035,17 +2846,14 @@
 class GetReminderResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GetReminderResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GetReminderResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2501,17 +3309,14 @@
 class ListRemindersResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: ListRemindersResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(ListRemindersResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2796,17 +3601,14 @@
 class PullCashierResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: PullCashierResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(PullCashierResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3037,16 +3839,15 @@
 
 class PushNotificationsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
+        pass
 
     def to_map(self):
         _map = super(PushNotificationsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -3360,16 +4161,15 @@
 
 class SendNotificationsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
+        pass
 
     def to_map(self):
         _map = super(SendNotificationsResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -3744,17 +4544,14 @@
 class UpdateReminderResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateReminderResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateReminderResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4075,17 +4872,14 @@
 class VideoAppReportResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: VideoAppReportResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(VideoAppReportResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4228,16 +5022,15 @@
 
 class WakeUpAppResponse(TeaModel):
     def __init__(self, headers=None, status_code=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
+        pass
 
     def to_map(self):
         _map = super(WakeUpAppResponse, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/alibabacloud_aligenieiap_1_0_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieiap-1-0-py2
-Version: 1.0.0
+Version: 1.1.0
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0_py2-1.0.0/setup.py` & `alibabacloud_aligenieiap_1_0_py2-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,31 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieiap_1_0_py2.
 
-Created on 15/12/2023
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieiap_1_0"
 NAME = "alibabacloud_aligenieiap_1_0_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0"
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
+    "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
         with open("README.md") as fp:
```

