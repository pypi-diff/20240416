# Comparing `tmp/antchain_realperson-1.8.0.tar.gz` & `tmp/antchain_realperson-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_realperson-1.8.0.tar", last modified: Tue Sep  6 12:31:10 2022, max compression
+gzip compressed data, was "dist/antchain_realperson-1.9.0.tar", last modified: Tue Nov 22 02:51:01 2022, max compression
```

## Comparing `antchain_realperson-1.8.0.tar` & `antchain_realperson-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:31:10.000000 antchain_realperson-1.8.0/
--rw-r--r--   0 root         (0) root         (0)      600 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2204 2022-09-06 12:31:10.000000 antchain_realperson-1.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1011 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:31:10.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2204 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_realperson.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:31:10.000000 antchain_realperson-1.8.0/antchain_sdk_realperson/
--rw-r--r--   0 root         (0) root         (0)       21 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_sdk_realperson/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55453 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_sdk_realperson/client.py
--rw-r--r--   0 root         (0) root         (0)   100698 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/antchain_sdk_realperson/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-09-06 12:31:10.000000 antchain_realperson-1.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2523 2022-09-06 12:31:09.000000 antchain_realperson-1.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2204 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1011 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2204 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_realperson.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/antchain_sdk_realperson/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/antchain_sdk_realperson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62043 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/antchain_sdk_realperson/client.py
+-rw-r--r--   0 root         (0) root         (0)   119623 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/antchain_sdk_realperson/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2022-11-22 02:51:01.000000 antchain_realperson-1.9.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2523 2022-11-22 02:51:00.000000 antchain_realperson-1.9.0/setup.py
```

### Comparing `antchain_realperson-1.8.0/LICENSE` & `antchain_realperson-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_realperson-1.8.0/PKG-INFO` & `antchain_realperson-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_realperson
-Version: 1.8.0
+Version: 1.9.0
 Summary: Ant Chain REALPERSON SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_realperson-1.8.0/README-CN.md` & `antchain_realperson-1.9.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_realperson-1.8.0/README.md` & `antchain_realperson-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_realperson-1.8.0/antchain_realperson.egg-info/PKG-INFO` & `antchain_realperson-1.9.0/antchain_realperson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-realperson
-Version: 1.8.0
+Version: 1.9.0
 Summary: Ant Chain REALPERSON SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_realperson-1.8.0/antchain_sdk_realperson/client.py` & `antchain_realperson-1.9.0/antchain_sdk_realperson/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.0',
+                    'sdk_version': '1.9.0',
                     '_prod_code': 'REALPERSON',
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
-                    'sdk_version': '1.8.0',
+                    'sdk_version': '1.9.0',
                     '_prod_code': 'REALPERSON',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1201,14 +1201,182 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             realperson_models.QueryThreemetaOnlinetimeResponse(),
             await self.do_request_async('1.0', 'di.realperson.threemeta.onlinetime.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def init_facevrf_zim(
+        self,
+        request: realperson_models.InitFacevrfZimRequest,
+    ) -> realperson_models.InitFacevrfZimResponse:
+        """
+        Description: 客户端初始化认证(OEM专用)
+        Summary: 客户端初始化认证(OEM专用)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.init_facevrf_zim_ex(request, headers, runtime)
+
+    async def init_facevrf_zim_async(
+        self,
+        request: realperson_models.InitFacevrfZimRequest,
+    ) -> realperson_models.InitFacevrfZimResponse:
+        """
+        Description: 客户端初始化认证(OEM专用)
+        Summary: 客户端初始化认证(OEM专用)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.init_facevrf_zim_ex_async(request, headers, runtime)
+
+    def init_facevrf_zim_ex(
+        self,
+        request: realperson_models.InitFacevrfZimRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.InitFacevrfZimResponse:
+        """
+        Description: 客户端初始化认证(OEM专用)
+        Summary: 客户端初始化认证(OEM专用)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.InitFacevrfZimResponse(),
+            self.do_request('1.0', 'di.realperson.facevrf.zim.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def init_facevrf_zim_ex_async(
+        self,
+        request: realperson_models.InitFacevrfZimRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.InitFacevrfZimResponse:
+        """
+        Description: 客户端初始化认证(OEM专用)
+        Summary: 客户端初始化认证(OEM专用)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.InitFacevrfZimResponse(),
+            await self.do_request_async('1.0', 'di.realperson.facevrf.zim.init', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def verify_facevrf_zim(
+        self,
+        request: realperson_models.VerifyFacevrfZimRequest,
+    ) -> realperson_models.VerifyFacevrfZimResponse:
+        """
+        Description: 客户端人脸验证(OEM专用)
+        Summary: 客户端人脸验证(OEM专用)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.verify_facevrf_zim_ex(request, headers, runtime)
+
+    async def verify_facevrf_zim_async(
+        self,
+        request: realperson_models.VerifyFacevrfZimRequest,
+    ) -> realperson_models.VerifyFacevrfZimResponse:
+        """
+        Description: 客户端人脸验证(OEM专用)
+        Summary: 客户端人脸验证(OEM专用)
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.verify_facevrf_zim_ex_async(request, headers, runtime)
+
+    def verify_facevrf_zim_ex(
+        self,
+        request: realperson_models.VerifyFacevrfZimRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.VerifyFacevrfZimResponse:
+        """
+        Description: 客户端人脸验证(OEM专用)
+        Summary: 客户端人脸验证(OEM专用)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.VerifyFacevrfZimResponse(),
+            self.do_request('1.0', 'di.realperson.facevrf.zim.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def verify_facevrf_zim_ex_async(
+        self,
+        request: realperson_models.VerifyFacevrfZimRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.VerifyFacevrfZimResponse:
+        """
+        Description: 客户端人脸验证(OEM专用)
+        Summary: 客户端人脸验证(OEM专用)
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.VerifyFacevrfZimResponse(),
+            await self.do_request_async('1.0', 'di.realperson.facevrf.zim.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def recognize_doc_individualcard(
+        self,
+        request: realperson_models.RecognizeDocIndividualcardRequest,
+    ) -> realperson_models.RecognizeDocIndividualcardResponse:
+        """
+        Description: 卡证OCR
+        Summary: 卡证OCR
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.recognize_doc_individualcard_ex(request, headers, runtime)
+
+    async def recognize_doc_individualcard_async(
+        self,
+        request: realperson_models.RecognizeDocIndividualcardRequest,
+    ) -> realperson_models.RecognizeDocIndividualcardResponse:
+        """
+        Description: 卡证OCR
+        Summary: 卡证OCR
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.recognize_doc_individualcard_ex_async(request, headers, runtime)
+
+    def recognize_doc_individualcard_ex(
+        self,
+        request: realperson_models.RecognizeDocIndividualcardRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.RecognizeDocIndividualcardResponse:
+        """
+        Description: 卡证OCR
+        Summary: 卡证OCR
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.RecognizeDocIndividualcardResponse(),
+            self.do_request('1.0', 'di.realperson.doc.individualcard.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def recognize_doc_individualcard_ex_async(
+        self,
+        request: realperson_models.RecognizeDocIndividualcardRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> realperson_models.RecognizeDocIndividualcardResponse:
+        """
+        Description: 卡证OCR
+        Summary: 卡证OCR
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            realperson_models.RecognizeDocIndividualcardResponse(),
+            await self.do_request_async('1.0', 'di.realperson.doc.individualcard.recognize', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_antcloud_gatewayx_file_upload(
         self,
         request: realperson_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> realperson_models.CreateAntcloudGatewayxFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
```

### Comparing `antchain_realperson-1.8.0/antchain_sdk_realperson/models.py` & `antchain_realperson-1.9.0/antchain_sdk_realperson/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -2567,14 +2567,517 @@
         if m.get('length_code') is not None:
             self.length_code = m.get('length_code')
         if m.get('extern_info') is not None:
             self.extern_info = m.get('extern_info')
         return self
 
 
+class InitFacevrfZimRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_data: str = None,
+        channel: str = None,
+        merchant: str = None,
+        meta_info: str = None,
+        produce_node: str = None,
+        product_name: str = None,
+        zim_id: str = None,
+        zim_principal: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务参数
+        self.biz_data = biz_data
+        # 渠道
+        self.channel = channel
+        # 商户
+        self.merchant = merchant
+        # 环境参数
+        self.meta_info = meta_info
+        # 产品节点
+        self.produce_node = produce_node
+        # 产品名称
+        self.product_name = product_name
+        # 实人认证id
+        # 
+        self.zim_id = zim_id
+        # 身份信息参数
+        # 
+        self.zim_principal = zim_principal
+
+    def validate(self):
+        self.validate_required(self.meta_info, 'meta_info')
+        self.validate_required(self.zim_id, 'zim_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_data is not None:
+            result['biz_data'] = self.biz_data
+        if self.channel is not None:
+            result['channel'] = self.channel
+        if self.merchant is not None:
+            result['merchant'] = self.merchant
+        if self.meta_info is not None:
+            result['meta_info'] = self.meta_info
+        if self.produce_node is not None:
+            result['produce_node'] = self.produce_node
+        if self.product_name is not None:
+            result['product_name'] = self.product_name
+        if self.zim_id is not None:
+            result['zim_id'] = self.zim_id
+        if self.zim_principal is not None:
+            result['zim_principal'] = self.zim_principal
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_data') is not None:
+            self.biz_data = m.get('biz_data')
+        if m.get('channel') is not None:
+            self.channel = m.get('channel')
+        if m.get('merchant') is not None:
+            self.merchant = m.get('merchant')
+        if m.get('meta_info') is not None:
+            self.meta_info = m.get('meta_info')
+        if m.get('produce_node') is not None:
+            self.produce_node = m.get('produce_node')
+        if m.get('product_name') is not None:
+            self.product_name = m.get('product_name')
+        if m.get('zim_id') is not None:
+            self.zim_id = m.get('zim_id')
+        if m.get('zim_principal') is not None:
+            self.zim_principal = m.get('zim_principal')
+        return self
+
+
+class InitFacevrfZimResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        ext_params: str = None,
+        message: str = None,
+        protocol: str = None,
+        ret_code: str = None,
+        ret_code_sub: str = None,
+        ret_message_sub: str = None,
+        zim_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 预留扩展结果
+        # 
+        self.ext_params = ext_params
+        # 描述
+        self.message = message
+        # 协议
+        self.protocol = protocol
+        # 返回码
+        self.ret_code = ret_code
+        # 明细返回码
+        self.ret_code_sub = ret_code_sub
+        # 明细返回码对应的文案
+        self.ret_message_sub = ret_message_sub
+        # 实人认证id
+        self.zim_id = zim_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.ext_params is not None:
+            result['ext_params'] = self.ext_params
+        if self.message is not None:
+            result['message'] = self.message
+        if self.protocol is not None:
+            result['protocol'] = self.protocol
+        if self.ret_code is not None:
+            result['ret_code'] = self.ret_code
+        if self.ret_code_sub is not None:
+            result['ret_code_sub'] = self.ret_code_sub
+        if self.ret_message_sub is not None:
+            result['ret_message_sub'] = self.ret_message_sub
+        if self.zim_id is not None:
+            result['zim_id'] = self.zim_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('ext_params') is not None:
+            self.ext_params = m.get('ext_params')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        if m.get('protocol') is not None:
+            self.protocol = m.get('protocol')
+        if m.get('ret_code') is not None:
+            self.ret_code = m.get('ret_code')
+        if m.get('ret_code_sub') is not None:
+            self.ret_code_sub = m.get('ret_code_sub')
+        if m.get('ret_message_sub') is not None:
+            self.ret_message_sub = m.get('ret_message_sub')
+        if m.get('zim_id') is not None:
+            self.zim_id = m.get('zim_id')
+        return self
+
+
+class VerifyFacevrfZimRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        extern_param: str = None,
+        zim_data: str = None,
+        zim_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 扩展信息,Map的json格式
+        self.extern_param = extern_param
+        # 人脸业务参数
+        self.zim_data = zim_data
+        # 7501f6c2dd57e06fe0d4202d3aaab58e
+        self.zim_id = zim_id
+
+    def validate(self):
+        self.validate_required(self.zim_data, 'zim_data')
+        self.validate_required(self.zim_id, 'zim_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.extern_param is not None:
+            result['extern_param'] = self.extern_param
+        if self.zim_data is not None:
+            result['zim_data'] = self.zim_data
+        if self.zim_id is not None:
+            result['zim_id'] = self.zim_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('extern_param') is not None:
+            self.extern_param = m.get('extern_param')
+        if m.get('zim_data') is not None:
+            self.zim_data = m.get('zim_data')
+        if m.get('zim_id') is not None:
+            self.zim_id = m.get('zim_id')
+        return self
+
+
+class VerifyFacevrfZimResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        ext_params: str = None,
+        has_next: str = None,
+        next_protocol: str = None,
+        product_ret_code: str = None,
+        ret_code_sub: str = None,
+        ret_message_sub: str = None,
+        validation_ret_code: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 预留扩展结果
+        self.ext_params = ext_params
+        # ""
+        self.has_next = has_next
+        # ""
+        self.next_protocol = next_protocol
+        # 产品返回明细码
+        self.product_ret_code = product_ret_code
+        # 明细返回码
+        self.ret_code_sub = ret_code_sub
+        # 明细返回码对应的文案
+        self.ret_message_sub = ret_message_sub
+        # 验证返回明细码
+        self.validation_ret_code = validation_ret_code
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.ext_params is not None:
+            result['ext_params'] = self.ext_params
+        if self.has_next is not None:
+            result['has_next'] = self.has_next
+        if self.next_protocol is not None:
+            result['next_protocol'] = self.next_protocol
+        if self.product_ret_code is not None:
+            result['product_ret_code'] = self.product_ret_code
+        if self.ret_code_sub is not None:
+            result['ret_code_sub'] = self.ret_code_sub
+        if self.ret_message_sub is not None:
+            result['ret_message_sub'] = self.ret_message_sub
+        if self.validation_ret_code is not None:
+            result['validation_ret_code'] = self.validation_ret_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('ext_params') is not None:
+            self.ext_params = m.get('ext_params')
+        if m.get('has_next') is not None:
+            self.has_next = m.get('has_next')
+        if m.get('next_protocol') is not None:
+            self.next_protocol = m.get('next_protocol')
+        if m.get('product_ret_code') is not None:
+            self.product_ret_code = m.get('product_ret_code')
+        if m.get('ret_code_sub') is not None:
+            self.ret_code_sub = m.get('ret_code_sub')
+        if m.get('ret_message_sub') is not None:
+            self.ret_message_sub = m.get('ret_message_sub')
+        if m.get('validation_ret_code') is not None:
+            self.validation_ret_code = m.get('validation_ret_code')
+        return self
+
+
+class RecognizeDocIndividualcardRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        out_order_no: str = None,
+        card_type: str = None,
+        data_type: str = None,
+        data_content: str = None,
+        req_enc_type: str = None,
+        resp_enc_type: str = None,
+        resp_enc_token: str = None,
+        extern_param: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 长度不超过32位的0-9A-Za-z字符串。
+        # 外部请求ID，由调用方自行生成并自行保证唯一，以便问题定位。
+        self.out_order_no = out_order_no
+        # 待识别的卡类型。取值约束：ID_CARD（身份证）;EEP_TO_ML_CARD（港澳来往大陆通行证）;BANK_CARD（银行卡）
+        self.card_type = card_type
+        # 传入的图片是base64编码的图片还是图片的URL。取值约束：BASE64（类型为base64）；URL（类型为URL）
+        self.data_type = data_type
+        # 传入的图片的具体内容，需要与data_type的选择保持一致。
+        self.data_content = data_content
+        # 入参data_content是否经公钥RSA加密。不填默认不加密。取值约束：0（不加密）；1（加密）
+        self.req_enc_type = req_enc_type
+        # 出参ocr_info是否经AES加密。不填默认不加密。取值约束：0（不加密）；1（加密）
+        self.resp_enc_type = resp_enc_type
+        # 经过公钥RSA加密的AES密钥，用于对出参ocr_info加密。当resp_enc_type =1时必填。
+        self.resp_enc_token = resp_enc_token
+        # 扩展信息JSON串。
+        self.extern_param = extern_param
+
+    def validate(self):
+        self.validate_required(self.out_order_no, 'out_order_no')
+        self.validate_required(self.card_type, 'card_type')
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.data_content, 'data_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.out_order_no is not None:
+            result['out_order_no'] = self.out_order_no
+        if self.card_type is not None:
+            result['card_type'] = self.card_type
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.data_content is not None:
+            result['data_content'] = self.data_content
+        if self.req_enc_type is not None:
+            result['req_enc_type'] = self.req_enc_type
+        if self.resp_enc_type is not None:
+            result['resp_enc_type'] = self.resp_enc_type
+        if self.resp_enc_token is not None:
+            result['resp_enc_token'] = self.resp_enc_token
+        if self.extern_param is not None:
+            result['extern_param'] = self.extern_param
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('out_order_no') is not None:
+            self.out_order_no = m.get('out_order_no')
+        if m.get('card_type') is not None:
+            self.card_type = m.get('card_type')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('data_content') is not None:
+            self.data_content = m.get('data_content')
+        if m.get('req_enc_type') is not None:
+            self.req_enc_type = m.get('req_enc_type')
+        if m.get('resp_enc_type') is not None:
+            self.resp_enc_type = m.get('resp_enc_type')
+        if m.get('resp_enc_token') is not None:
+            self.resp_enc_token = m.get('resp_enc_token')
+        if m.get('extern_param') is not None:
+            self.extern_param = m.get('extern_param')
+        return self
+
+
+class RecognizeDocIndividualcardResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        ret_code: str = None,
+        ret_code_sub: str = None,
+        ret_message_sub: str = None,
+        ocr_info: str = None,
+        ext_info: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 返回结果码
+        self.ret_code = ret_code
+        # 错误码
+        self.ret_code_sub = ret_code_sub
+        # 错误信息
+        self.ret_message_sub = ret_message_sub
+        # 识别结果，为JSON串。如果入参resp_enc_type=1则是经过AES加密后的JSON串。
+        self.ocr_info = ocr_info
+        # 扩展信息JSON串。
+        self.ext_info = ext_info
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.ret_code is not None:
+            result['ret_code'] = self.ret_code
+        if self.ret_code_sub is not None:
+            result['ret_code_sub'] = self.ret_code_sub
+        if self.ret_message_sub is not None:
+            result['ret_message_sub'] = self.ret_message_sub
+        if self.ocr_info is not None:
+            result['ocr_info'] = self.ocr_info
+        if self.ext_info is not None:
+            result['ext_info'] = self.ext_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('ret_code') is not None:
+            self.ret_code = m.get('ret_code')
+        if m.get('ret_code_sub') is not None:
+            self.ret_code_sub = m.get('ret_code_sub')
+        if m.get('ret_message_sub') is not None:
+            self.ret_message_sub = m.get('ret_message_sub')
+        if m.get('ocr_info') is not None:
+            self.ocr_info = m.get('ocr_info')
+        if m.get('ext_info') is not None:
+            self.ext_info = m.get('ext_info')
+        return self
+
+
 class CreateAntcloudGatewayxFileUploadRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         api_code: str = None,
         file_label: str = None,
         file_metadata: str = None,
```

### Comparing `antchain_realperson-1.8.0/setup.py` & `antchain_realperson-1.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_realperson.
 
-Created on 06/09/2022
+Created on 22/11/2022
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_realperson"
 NAME = "antchain_realperson" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain REALPERSON SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

