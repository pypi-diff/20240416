# Comparing `tmp/sparkproxy-0.4.2.tar.gz` & `tmp/sparkproxy-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkproxy-0.4.2.tar", last modified: Thu Apr 11 08:09:59 2024, max compression
+gzip compressed data, was "sparkproxy-0.4.3.tar", last modified: Tue Apr 16 14:03:00 2024, max compression
```

## Comparing `sparkproxy-0.4.2.tar` & `sparkproxy-0.4.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.403334 sparkproxy-0.4.2/
--rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.4.2/LICENSE
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-11 08:09:59.403159 sparkproxy-0.4.2/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)     4831 2024-04-11 07:31:06.000000 sparkproxy-0.4.2/README.md
--rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-11 08:09:59.403385 sparkproxy-0.4.2/setup.cfg
--rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.4.2/setup.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.399149 sparkproxy-0.4.2/sparkproxy/
--rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-11 08:09:08.000000 sparkproxy-0.4.2/sparkproxy/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.4.2/sparkproxy/auth.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.4.2/sparkproxy/compat.py
--rw-r--r--   0 huanghy    (501) staff       (20)     1278 2024-04-11 08:07:58.000000 sparkproxy-0.4.2/sparkproxy/config.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.400701 sparkproxy-0.4.2/sparkproxy/http/
--rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.4.2/sparkproxy/http/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.4.2/sparkproxy/http/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.401646 sparkproxy-0.4.2/sparkproxy/http/middleware/
--rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.4.2/sparkproxy/http/middleware/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.4.2/sparkproxy/http/middleware/base.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.4.2/sparkproxy/http/middleware/retry_domains.py
--rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.4.2/sparkproxy/http/middleware/ua.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.4.2/sparkproxy/http/response.py
--rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.4.2/sparkproxy/rsa.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.401981 sparkproxy-0.4.2/sparkproxy/services/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.2/sparkproxy/services/__init__.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.402209 sparkproxy-0.4.2/sparkproxy/services/openapi/
--rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.2/sparkproxy/services/openapi/__init__.py
--rw-r--r--   0 huanghy    (501) staff       (20)     7388 2024-04-11 07:46:36.000000 sparkproxy-0.4.2/sparkproxy/services/openapi/client.py
-drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-11 08:09:59.400014 sparkproxy-0.4.2/sparkproxy.egg-info/
--rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/PKG-INFO
--rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/SOURCES.txt
--rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/dependency_links.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/entry_points.txt
--rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/requires.txt
--rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-11 08:09:59.000000 sparkproxy-0.4.2/sparkproxy.egg-info/top_level.txt
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.533330 sparkproxy-0.4.3/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1063 2024-04-09 02:02:16.000000 sparkproxy-0.4.3/LICENSE
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-16 14:03:00.533170 sparkproxy-0.4.3/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)     4831 2024-04-11 07:31:06.000000 sparkproxy-0.4.3/README.md
+-rw-r--r--   0 huanghy    (501) staff       (20)       38 2024-04-16 14:03:00.533376 sparkproxy-0.4.3/setup.cfg
+-rw-r--r--   0 huanghy    (501) staff       (20)     2362 2024-04-09 03:18:58.000000 sparkproxy-0.4.3/setup.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.529661 sparkproxy-0.4.3/sparkproxy/
+-rw-r--r--   0 huanghy    (501) staff       (20)      346 2024-04-16 13:53:34.000000 sparkproxy-0.4.3/sparkproxy/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     3098 2024-04-10 04:59:43.000000 sparkproxy-0.4.3/sparkproxy/auth.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1666 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/compat.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     1341 2024-04-16 14:01:23.000000 sparkproxy-0.4.3/sparkproxy/config.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.531231 sparkproxy-0.4.3/sparkproxy/http/
+-rw-r--r--   0 huanghy    (501) staff       (20)     3137 2024-04-10 05:00:18.000000 sparkproxy-0.4.3/sparkproxy/http/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     5000 2024-04-08 13:48:17.000000 sparkproxy-0.4.3/sparkproxy/http/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532183 sparkproxy-0.4.3/sparkproxy/http/middleware/
+-rw-r--r--   0 huanghy    (501) staff       (20)      246 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      875 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/base.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2611 2024-04-08 13:48:17.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/retry_domains.py
+-rw-r--r--   0 huanghy    (501) staff       (20)      608 2024-04-08 15:18:23.000000 sparkproxy-0.4.3/sparkproxy/http/middleware/ua.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2520 2024-04-08 15:21:24.000000 sparkproxy-0.4.3/sparkproxy/http/response.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     2973 2024-04-10 05:09:23.000000 sparkproxy-0.4.3/sparkproxy/rsa.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532516 sparkproxy-0.4.3/sparkproxy/services/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/services/__init__.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.532726 sparkproxy-0.4.3/sparkproxy/services/openapi/
+-rw-r--r--   0 huanghy    (501) staff       (20)        0 2024-04-08 13:34:09.000000 sparkproxy-0.4.3/sparkproxy/services/openapi/__init__.py
+-rw-r--r--   0 huanghy    (501) staff       (20)     8299 2024-04-16 13:58:07.000000 sparkproxy-0.4.3/sparkproxy/services/openapi/client.py
+drwxr-xr-x   0 huanghy    (501) staff       (20)        0 2024-04-16 14:03:00.530610 sparkproxy-0.4.3/sparkproxy.egg-info/
+-rw-r--r--   0 huanghy    (501) staff       (20)     1128 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/PKG-INFO
+-rw-r--r--   0 huanghy    (501) staff       (20)      677 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/SOURCES.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)        1 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/dependency_links.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       54 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/entry_points.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)      209 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/requires.txt
+-rw-r--r--   0 huanghy    (501) staff       (20)       11 2024-04-16 14:03:00.000000 sparkproxy-0.4.3/sparkproxy.egg-info/top_level.txt
```

### Comparing `sparkproxy-0.4.2/LICENSE` & `sparkproxy-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/PKG-INFO` & `sparkproxy-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.4.2/README.md` & `sparkproxy-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/setup.py` & `sparkproxy-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/auth.py` & `sparkproxy-0.4.3/sparkproxy/auth.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/compat.py` & `sparkproxy-0.4.3/sparkproxy/compat.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/config.py` & `sparkproxy-0.4.3/sparkproxy/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 
 API_HOST = 'http://8.130.48.76:16801'  # 数据处理操作Host
+# API_HOST = 'http://127.0.0.1:8080'  # 数据处理操作Host
 
 _config = {
     'default_api_host': API_HOST,
     'connection_timeout': 30,  # 链接超时为时间为30s
     'connection_retries': 3,  # 链接重试次数为3次
     'connection_pool': 10  # 链接池个数为10
 }
```

### Comparing `sparkproxy-0.4.2/sparkproxy/http/__init__.py` & `sparkproxy-0.4.3/sparkproxy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/http/client.py` & `sparkproxy-0.4.3/sparkproxy/http/client.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/http/middleware/base.py` & `sparkproxy-0.4.3/sparkproxy/http/middleware/base.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/http/middleware/retry_domains.py` & `sparkproxy-0.4.3/sparkproxy/http/middleware/retry_domains.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/http/middleware/ua.py` & `sparkproxy-0.4.3/sparkproxy/http/middleware/ua.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/http/response.py` & `sparkproxy-0.4.3/sparkproxy/http/response.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/rsa.py` & `sparkproxy-0.4.3/sparkproxy/rsa.py`

 * *Files identical despite different names*

### Comparing `sparkproxy-0.4.2/sparkproxy/services/openapi/client.py` & `sparkproxy-0.4.3/sparkproxy/services/openapi/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,49 +54,64 @@
             except ValueError as e:
                 raise ValueError("使用本地私钥解密失败")
             received_msg = to_string(received_decrypted_msg)
             return msg == received_msg, None
 
         return False, info
 
-    def get_product_stock(self, proxy_type, country_code=None, city_code=None):
+    def get_product_stock(self, proxy_type, country_code=None, area_code=None, city_code=None):
         """获取商品库存
 
         列出当前所有在售的商品及其库存信息。
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回服务组列表[<product1>, <product1>, ...]，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
         return self.__post('GetProductStock',
-                           {"proxyType": proxy_type, "countryCode": country_code, "cityCode": city_code})
+                           {"proxyType": proxy_type, "countryCode": country_code, "areaCode": area_code, "cityCode": city_code})
 
-    def create_proxy(self, req_order_no, sku, amount, duration, unit, country_code, city_code):
+    def get_product_stock2(self, proxy_type, country_code=None, area_code=None, city_code=None):
+        """获取商品库存
+
+        列出当前所有在售的商品及其库存信息。
+
+        Returns:
+            返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
+            - result          成功返回服务组列表[<product1>, <product1>, ...]，失败返回{"error": "<errMsg string>"}
+            - ResponseInfo    请求的Response信息
+        """
+        return self.__post('GetProductStock',
+                           {"proxyType": proxy_type, "countryCode": country_code, "areaCode": area_code, "cityCode": city_code},
+                           version="2024-04-16")
+
+    def create_proxy(self, req_order_no, sku, amount, duration, unit, country_code, area_code, city_code):
         """创建代理实例
 
         创建新代理实例，返回订单信息
 
         Args:
             - req_order_no: 请求方订单ID
             - sku:  商品ID
             - amount: IP数量
             - duration: 必要 时长 0无限制
             - unit: 单位 1 天;2 周（7天）;3 月(自然月; 4年(自然年365，366）
             - country_code: 必要,国家代码 3位 iso标准
+            - area_code: 必要,州代码 3位 iso标准
             - city_code: 必要,城市代码 向我方提取
 
         Returns:
             返回一个tuple对象，其格式为(<result>, <ResponseInfo>)
             - result          成功返回空dict{}，失败返回{"error": "<errMsg string>"}
             - ResponseInfo    请求的Response信息
         """
-        return self.__post('CreateProxy', {"reqOrderNo": req_order_no, "sku": sku, "amount": amount,
+        return self.__post('CreateProxy', {"reqOrderNo": req_order_no, "productId": sku, "amount": amount,
                                            "duration": duration, "unit": unit, "countryCode": country_code,
-                                           "cityCode": city_code})
+                                           "areaCode": area_code, "cityCode": city_code})
 
     def renew_proxy(self, req_order_no, instances):
         """续费代理实例
 
         续费新代理实例，返回新订单信息
 
         Args:
@@ -170,24 +185,24 @@
         if ret is not None and 'code' in ret and ret['code'] == 200 and 'data' in ret:
             data = ret['data']
             password = data["password"] if 'password' in data else ''
             if len(password) > 0:
                 data["password"] = self.auth.decrypt_using_private_key(password)
         return ret, info
 
-    def __request_params(self, method, args):
+    def __request_params(self, method, version, args):
         base_params = {
             "method": method,
-            "version": "2024-04-08",
+            "version": version if version is not None else "2024-04-08",
             "reqId": str(uuid.uuid4()),
             "timestamp": int(time.time()),
             "supplierNo": self.auth.get_supplier_no(),
             "sign": "",
             "params": args
         }
         base_params["sign"] = self.auth.token_of_request(base_params)
         return base_params
 
-    def __post(self, method, data=None):
+    def __post(self, method, data=None, version=None):
         url = '{0}/v1/open/api'.format(self.host)
-        req = self.__request_params(method, data)
+        req = self.__request_params(method, version, data)
         return http._post(url, req)
```

### Comparing `sparkproxy-0.4.2/sparkproxy.egg-info/PKG-INFO` & `sparkproxy-0.4.3/sparkproxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparkproxy
-Version: 0.4.2
+Version: 0.4.3
 Summary: Spark proxy OpenApi SDK
 Home-page: https://github.com/yungoo/spark-sdk-python
 Author: Spark Proxy Co., Ltd.
 Author-email: sdk@sparkproxy.com
 Maintainer-email: support@sparkproxy.com
 License: MIT
 Platform: any
```

### Comparing `sparkproxy-0.4.2/sparkproxy.egg-info/SOURCES.txt` & `sparkproxy-0.4.3/sparkproxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

