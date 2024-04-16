# Comparing `tmp/fireblocks_sdk-2.8.0.tar.gz` & `tmp/fireblocks_sdk-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireblocks_sdk-2.8.0.tar", last modified: Sun Apr 14 11:56:05 2024, max compression
+gzip compressed data, was "fireblocks_sdk-2.8.1.tar", last modified: Tue Apr 16 09:44:12 2024, max compression
```

## Comparing `fireblocks_sdk-2.8.0.tar` & `fireblocks_sdk-2.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/fireblocks_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/api_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/ncw_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)   105849 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/sdk_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/tokenization_api_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-14 11:56:02.000000 fireblocks_sdk-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:44:12.565334 fireblocks_sdk-2.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 09:44:12.565334 fireblocks_sdk-2.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:44:12.565334 fireblocks_sdk-2.8.1/fireblocks_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/ncw_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107091 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/sdk_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-16 09:44:05.000000 fireblocks_sdk-2.8.1/fireblocks_sdk/tokenization_api_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:44:12.565334 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 09:44:12.000000 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-16 09:44:12.000000 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:44:12.000000 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 09:44:12.000000 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-16 09:44:12.000000 fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-16 09:44:12.565334 fireblocks_sdk-2.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-16 09:44:09.000000 fireblocks_sdk-2.8.1/setup.py
```

### Comparing `fireblocks_sdk-2.8.0/LICENSE.txt` & `fireblocks_sdk-2.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/PKG-INFO` & `fireblocks_sdk-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fireblocks_sdk
-Version: 2.8.0
+Version: 2.8.1
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.1.tar.gz
 License: MIT
 Keywords: Fireblocks,SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: PyJWT>=2.8.0
+Requires-Dist: PyJWT>=2.8.1
 Requires-Dist: cryptography>=2.7
 Requires-Dist: requests>=2.22.0
 
 Fireblocks python SDK
```

### Comparing `fireblocks_sdk-2.8.0/README.md` & `fireblocks_sdk-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk/api_types.py` & `fireblocks_sdk-2.8.1/fireblocks_sdk/api_types.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk/ncw_sdk.py` & `fireblocks_sdk-2.8.1/fireblocks_sdk/ncw_sdk.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk/sdk.py` & `fireblocks_sdk-2.8.1/fireblocks_sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -2927,45 +2927,74 @@
 
         if page_size:
             request_filter["pageSize"] = page_size
 
         if page_cursor:
             request_filter["pageCursor"] = page_cursor
 
-        return self._get_request("/v1/contract-registry/contracts", query_params=request_filter)
+        return self._get_request("/v1/tokenization/templates", query_params=request_filter)
 
     def upload_contract_template(self, request: ContractUploadRequest):
-        return self._post_request("/v1/contract-registry/contracts", request.to_dict())
+        return self._post_request("/v1/tokenization/templates", request.to_dict())
 
-    def get_contract_template(self, contract_id: str):
-        return self._get_request(f"/v1/contract-registry/contracts/{contract_id}")
+    def get_contract_template(self, template_id: str):
+        return self._get_request(f"/v1/tokenization/templates/{template_id}")
 
-    def get_contract_template_constructor(self, contract_id: str, with_docs: bool=False):
-        return self._get_request(f"/v1/contract-registry/contracts/{contract_id}/constructor?withDocs=${with_docs}")
+    def get_contract_template_constructor(self, template_id: str, with_docs: bool=False):
+        return self._get_request(f"/v1/tokenization/templates/{template_id}/constructor?withDocs=${with_docs}")
+    
+    def get_contract_template_deploy_function(self, template_id: str, with_docs: bool=False):
+        return self._get_request(f"/v1/tokenization/templates/{template_id}/deploy_function?withDocs=${with_docs}")
+    
+    def get_contract_template_supported_blockchains(self, template_id: str):
+        return self._get_request(f"/v1/tokenization/templates/{template_id}/supported_blockchains")
 
-    def delete_contract_template(self, contract_id: str):
-        return self._delete_request(f"/v1/contract-registry/contracts/{contract_id}")
+    def delete_contract_template(self, template_id: str):
+        return self._delete_request(f"/v1/tokenization/templates/{template_id}")
 
-    def deploy_contract(self, contract_id: str, request: ContractDeployRequest):
-        return self._post_request(f"/v1/contract-registry/contracts/{contract_id}/deploy", request.to_dict())
-    
-    def get_contracts_by_filter(self, templateId: str, blockchain_id: Optional[str] = None):
-        return self._get_request(f"/v1/contract-service/contracts?templateId={templateId}&blockchainId={blockchain_id}")
+    def deploy_contract(self, template_id: str, request: ContractDeployRequest):
+        return self._post_request(f"/v1/tokenization/templates/{template_id}/deploy", request.to_dict())
+
+    def get_contracts_by_filter(self, 
+                                contract_template_id: Optional[str] = None, 
+                                base_asset_id: Optional[str] = None, 
+                                contract_address: Optional[str] = None, 
+                                page_size: Optional[int] = None, 
+                                page_cursor: Optional[str] = None
+                                ):
+        request_filter = {}
+
+        if contract_template_id:
+            request_filter["contractTemplateId"] = contract_template_id
+
+        if base_asset_id:
+            request_filter["baseAssetId"] = base_asset_id
+
+        if contract_address:
+            request_filter["contractAddress"] = contract_address
+
+        if page_size:
+            request_filter["pageSize"] = page_size
+
+        if page_cursor:
+            request_filter["pageCursor"] = page_cursor
+
+        return self._get_request("/v1/tokenization/contracts", query_params=request_filter)
     
-    def get_contract_by_address(self, blockchain_id: str, contract_address: str):
-        return self._get_request(f"/v1/contract-service/contracts/{blockchain_id}/{contract_address}")
+    def get_contract_by_address(self, base_asset_id: str, contract_address: str):
+        return self._get_request(f"/v1/contract_interactions/base_asset_id/{base_asset_id}/contract_address/{contract_address}")
     
-    def get_contract_abi(self, blockchain_id: str, contract_address: str):
-        return self._get_request(f"/v1/contract-service/contracts/{blockchain_id}/{contract_address}/abi")
+    def get_contract_abi(self, base_asset_id: str, contract_address: str):
+        return self._get_request(f"/v1/contract_interactions/base_asset_id/{base_asset_id}/contract_address/{contract_address}/abi")
     
-    def read_contract_call_function(self, blockchain_id: str, contract_address: str, request: ReadCallFunction):
-        return self._post_request(f"/v1/contract-service/contracts/{blockchain_id}/{contract_address}/function/read", request.to_dict())
+    def read_contract_call_function(self, base_asset_id: str, contract_address: str, request: ReadCallFunction):
+        return self._post_request(f"/v1/contract_interactions/base_asset_id/{base_asset_id}/contract_address/{contract_address}/functions/read", request.to_dict())
 
-    def write_contract_call_function(self, blockchain_id: str, contract_address: str, request: WriteCallFunction):
-        return self._post_request(f"/v1/contract-service/contracts/{blockchain_id}/{contract_address}/function/write", request.to_dict())
+    def write_contract_call_function(self, base_asset_id: str, contract_address: str, request: WriteCallFunction):
+        return self._post_request(f"/v1/contract_interactions/base_asset_id/{base_asset_id}/contract_address/{contract_address}/functions/write", request.to_dict())
 
     def _get_request(self, path, page_mode=False, query_params: Dict = None):
         if query_params:
             path = path + "?" + urllib.parse.urlencode(query_params)
         token = self.token_provider.sign_jwt(path)
         headers = {"Authorization": f"Bearer {token}"}
         response = self.http_session.get(
```

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk/sdk_token_provider.py` & `fireblocks_sdk-2.8.1/fireblocks_sdk/sdk_token_provider.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk/tokenization_api_types.py` & `fireblocks_sdk-2.8.1/fireblocks_sdk/tokenization_api_types.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/PKG-INFO` & `fireblocks_sdk-2.8.1/fireblocks_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fireblocks_sdk
-Version: 2.8.0
+Version: 2.8.1
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.1.tar.gz
 License: MIT
 Keywords: Fireblocks,SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: PyJWT>=2.8.0
+Requires-Dist: PyJWT>=2.8.1
 Requires-Dist: cryptography>=2.7
 Requires-Dist: requests>=2.22.0
 
 Fireblocks python SDK
```

### Comparing `fireblocks_sdk-2.8.0/setup.py` & `fireblocks_sdk-2.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'fireblocks_sdk',
   packages = ['fireblocks_sdk'],
-  version = '2.8.0',
+  version = '2.8.1',
   license='MIT',
   description = 'Fireblocks python SDK',
   long_description="""Fireblocks python SDK""",
   long_description_content_type='text/markdown',
   url = 'https://github.com/fireblocks/fireblocks-sdk-py',
-  download_url = 'https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.0.tar.gz',
+  download_url = 'https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.1.tar.gz',
   keywords = ['Fireblocks', 'SDK'],
   install_requires=[
-          'PyJWT>=2.8.0',
+          'PyJWT>=2.8.1',
           'cryptography>=2.7',
           'requests>=2.22.0',
       ],
   classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development',
```

