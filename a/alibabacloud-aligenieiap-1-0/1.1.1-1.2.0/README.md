# Comparing `tmp/alibabacloud_aligenieiap_1_0-1.1.1.tar.gz` & `tmp/alibabacloud_aligenieiap_1_0-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.1.1.tar", last modified: Thu Apr 11 09:59:27 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aligenieiap_1_0-1.2.0.tar", last modified: Tue Apr 16 17:16:09 2024, max compression
```

## Comparing `alibabacloud_aligenieiap_1_0-1.1.1.tar` & `alibabacloud_aligenieiap_1_0-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1112 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1197 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81284 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   164650 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2430 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 09:59:27.000000 alibabacloud_aligenieiap_1_0-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2024-04-11 09:59:26.000000 alibabacloud_aligenieiap_1_0-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      509 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93586 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   183098 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2024-04-16 17:16:09.000000 alibabacloud_aligenieiap_1_0-1.2.0/setup.py
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/LICENSE` & `alibabacloud_aligenieiap_1_0-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligenieiap_1_0
-Version: 1.1.1
+Version: 1.2.0
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/README-CN.md` & `alibabacloud_aligenieiap_1_0-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/README.md` & `alibabacloud_aligenieiap_1_0-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/client.py` & `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,258 @@
         self,
         request: ali_genieiap__1__0_models.AppUseTimeReportRequest,
     ) -> ali_genieiap__1__0_models.AppUseTimeReportResponse:
         runtime = util_models.RuntimeOptions()
         headers = ali_genieiap__1__0_models.AppUseTimeReportHeaders()
         return await self.app_use_time_report_with_options_async(request, headers, runtime)
 
+    def call_back_third_right_send_plan_with_options(
+        self,
+        tmp_req: ali_genieiap__1__0_models.CallBackThirdRightSendPlanRequest,
+        headers: ali_genieiap__1__0_models.CallBackThirdRightSendPlanHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse:
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
+            pathname=f'/1.0/iap/business/CallBackThirdRightSendPlan',
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
+    async def call_back_third_right_send_plan_with_options_async(
+        self,
+        tmp_req: ali_genieiap__1__0_models.CallBackThirdRightSendPlanRequest,
+        headers: ali_genieiap__1__0_models.CallBackThirdRightSendPlanHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse:
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
+            pathname=f'/1.0/iap/business/CallBackThirdRightSendPlan',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def call_back_third_right_send_plan(
+        self,
+        request: ali_genieiap__1__0_models.CallBackThirdRightSendPlanRequest,
+    ) -> ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CallBackThirdRightSendPlanHeaders()
+        return self.call_back_third_right_send_plan_with_options(request, headers, runtime)
+
+    async def call_back_third_right_send_plan_async(
+        self,
+        request: ali_genieiap__1__0_models.CallBackThirdRightSendPlanRequest,
+    ) -> ali_genieiap__1__0_models.CallBackThirdRightSendPlanResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CallBackThirdRightSendPlanHeaders()
+        return await self.call_back_third_right_send_plan_with_options_async(request, headers, runtime)
+
+    def check_third_right_send_plan_with_options(
+        self,
+        tmp_req: ali_genieiap__1__0_models.CheckThirdRightSendPlanRequest,
+        headers: ali_genieiap__1__0_models.CheckThirdRightSendPlanHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse:
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
+            pathname=f'/v1.0/iap/business/CheckThirdRightSendPlan',
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
+    async def check_third_right_send_plan_with_options_async(
+        self,
+        tmp_req: ali_genieiap__1__0_models.CheckThirdRightSendPlanRequest,
+        headers: ali_genieiap__1__0_models.CheckThirdRightSendPlanHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse:
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
+            pathname=f'/v1.0/iap/business/CheckThirdRightSendPlan',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def check_third_right_send_plan(
+        self,
+        request: ali_genieiap__1__0_models.CheckThirdRightSendPlanRequest,
+    ) -> ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CheckThirdRightSendPlanHeaders()
+        return self.check_third_right_send_plan_with_options(request, headers, runtime)
+
+    async def check_third_right_send_plan_async(
+        self,
+        request: ali_genieiap__1__0_models.CheckThirdRightSendPlanRequest,
+    ) -> ali_genieiap__1__0_models.CheckThirdRightSendPlanResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = ali_genieiap__1__0_models.CheckThirdRightSendPlanHeaders()
+        return await self.check_third_right_send_plan_with_options_async(request, headers, runtime)
+
     def create_reminder_with_options(
         self,
         tmp_req: ali_genieiap__1__0_models.CreateReminderRequest,
         headers: ali_genieiap__1__0_models.CreateReminderHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> ali_genieiap__1__0_models.CreateReminderResponse:
         UtilClient.validate_model(tmp_req)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0/models.py` & `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, List
+from typing import Dict, Any, List
 
 
 class AppUseTimeReportHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
@@ -370,14 +370,575 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AppUseTimeReportResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CallBackThirdRightSendPlanHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        biz_group: str = None,
+        biz_type: str = None,
+        card_type: int = None,
+        error_msg: str = None,
+        extend_info: Dict[str, Any] = None,
+        genie_open_id: str = None,
+        receive_status: int = None,
+        sn: str = None,
+        supplier_id: int = None,
+    ):
+        self.biz_group = biz_group
+        self.biz_type = biz_type
+        self.card_type = card_type
+        self.error_msg = error_msg
+        self.extend_info = extend_info
+        self.genie_open_id = genie_open_id
+        self.receive_status = receive_status
+        self.sn = sn
+        self.supplier_id = supplier_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        biz_group: str = None,
+        biz_type: str = None,
+        card_type: int = None,
+        error_msg: str = None,
+        extend_info_shrink: str = None,
+        genie_open_id: str = None,
+        receive_status: int = None,
+        sn: str = None,
+        supplier_id: int = None,
+    ):
+        self.biz_group = biz_group
+        self.biz_type = biz_type
+        self.card_type = card_type
+        self.error_msg = error_msg
+        self.extend_info_shrink = extend_info_shrink
+        self.genie_open_id = genie_open_id
+        self.receive_status = receive_status
+        self.sn = sn
+        self.supplier_id = supplier_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        ret_code: str = None,
+        ret_msg: str = None,
+        ret_value: bool = None,
+        request_id: str = None,
+    ):
+        self.ret_code = ret_code
+        self.ret_msg = ret_msg
+        self.ret_value = ret_value
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CallBackThirdRightSendPlanResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_aligenie_access_token: str = None,
+        authorization: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_aligenie_access_token = x_acs_aligenie_access_token
+        self.authorization = authorization
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        biz_group: str = None,
+        biz_type: str = None,
+        extend_info: Dict[str, Any] = None,
+        sn: str = None,
+        supplier_id: int = None,
+    ):
+        self.biz_group = biz_group
+        self.biz_type = biz_type
+        self.extend_info = extend_info
+        self.sn = sn
+        self.supplier_id = supplier_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        biz_group: str = None,
+        biz_type: str = None,
+        extend_info_shrink: str = None,
+        sn: str = None,
+        supplier_id: int = None,
+    ):
+        self.biz_group = biz_group
+        self.biz_type = biz_type
+        self.extend_info_shrink = extend_info_shrink
+        self.sn = sn
+        self.supplier_id = supplier_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        activate_date: str = None,
+        card_type: int = None,
+        channel_code: str = None,
+        channel_name: str = None,
+        extend_info: Dict[str, Any] = None,
+        request_id: str = None,
+        rights_expired_date: str = None,
+    ):
+        self.activate_date = activate_date
+        self.card_type = card_type
+        self.channel_code = channel_code
+        self.channel_name = channel_name
+        self.extend_info = extend_info
+        self.request_id = request_id
+        self.rights_expired_date = rights_expired_date
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        ret_code: int = None,
+        ret_msg: str = None,
+        ret_value: CheckThirdRightSendPlanResponseBodyRetValue = None,
+    ):
+        self.ret_code = ret_code
+        self.ret_msg = ret_msg
+        self.ret_value = ret_value
+
+    def validate(self):
+        if self.ret_value:
+            self.ret_value.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CheckThirdRightSendPlanResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_aligenie_access_token: str = None,
         authorization: str = None,
     ):
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO` & `alibabacloud_aligenieiap_1_0-1.2.0/alibabacloud_aligenieiap_1_0.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligenieiap-1-0
-Version: 1.1.1
+Version: 1.2.0
 Summary: Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligenieiap_1_0-1.1.1/setup.py` & `alibabacloud_aligenieiap_1_0-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligenieiap_1_0.
 
-Created on 11/04/2024
+Created on 16/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligenieiap_1_0"
 NAME = "alibabacloud_aligenieiap_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (iap_1_0) SDK Library for Python"
```

