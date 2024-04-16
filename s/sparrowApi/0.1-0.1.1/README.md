# Comparing `tmp/sparrowApi-0.1.tar.gz` & `tmp/sparrowApi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowApi-0.1.tar", last modified: Mon Apr 15 02:46:39 2024, max compression
+gzip compressed data, was "sparrowApi-0.1.1.tar", last modified: Mon Apr 15 08:52:51 2024, max compression
```

## Comparing `sparrowApi-0.1.tar` & `sparrowApi-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 02:46:39.815048 sparrowApi-0.1/
--rw-rw-rw-   0        0        0      115 2024-04-15 02:46:39.814304 sparrowApi-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-15 02:46:39.815497 sparrowApi-0.1/setup.cfg
--rw-rw-rw-   0        0        0      236 2024-04-15 02:10:14.000000 sparrowApi-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:46:39.806137 sparrowApi-0.1/sparrowApi/
--rw-rw-rw-   0        0        0      504 2024-04-15 01:27:32.000000 sparrowApi-0.1/sparrowApi/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-04-15 02:36:18.000000 sparrowApi-0.1/sparrowApi/api.py
--rw-rw-rw-   0        0        0      825 2024-04-12 08:45:23.000000 sparrowApi-0.1/sparrowApi/constant.py
--rw-rw-rw-   0        0        0     5357 2024-04-15 02:46:23.000000 sparrowApi-0.1/sparrowApi/tool_class.py
-drwxrwxrwx   0        0        0        0 2024-04-15 02:46:39.812553 sparrowApi-0.1/sparrowApi.egg-info/
--rw-rw-rw-   0        0        0      115 2024-04-15 02:46:39.000000 sparrowApi-0.1/sparrowApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 02:46:39.000000 sparrowApi-0.1/sparrowApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 02:46:39.000000 sparrowApi-0.1/sparrowApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-15 02:46:39.000000 sparrowApi-0.1/sparrowApi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 08:52:51.841982 sparrowApi-0.1.1/
+-rw-rw-rw-   0        0        0      142 2024-04-15 08:52:51.840811 sparrowApi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:52:51.842130 sparrowApi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      248 2024-04-15 08:52:42.000000 sparrowApi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:52:51.829764 sparrowApi-0.1.1/sparrowApi/
+-rw-rw-rw-   0        0        0      504 2024-04-15 01:27:32.000000 sparrowApi-0.1.1/sparrowApi/__init__.py
+-rw-rw-rw-   0        0        0    18118 2024-04-15 08:52:20.000000 sparrowApi-0.1.1/sparrowApi/api.py
+-rw-rw-rw-   0        0        0      825 2024-04-12 08:45:23.000000 sparrowApi-0.1.1/sparrowApi/constant.py
+-rw-rw-rw-   0        0        0     5357 2024-04-15 02:46:23.000000 sparrowApi-0.1.1/sparrowApi/tool_class.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:52:51.838974 sparrowApi-0.1.1/sparrowApi.egg-info/
+-rw-rw-rw-   0        0        0      142 2024-04-15 08:52:51.000000 sparrowApi-0.1.1/sparrowApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-15 08:52:51.000000 sparrowApi-0.1.1/sparrowApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:52:51.000000 sparrowApi-0.1.1/sparrowApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 08:52:51.000000 sparrowApi-0.1.1/sparrowApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-15 08:52:51.000000 sparrowApi-0.1.1/sparrowApi.egg-info/top_level.txt
```

### Comparing `sparrowApi-0.1/sparrowApi/api.py` & `sparrowApi-0.1.1/sparrowApi/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         :param save_data: 需要记录的日志内容
         :return:
         """
         if self.is_save_log:
             with open(self.log_file, 'a', encoding='utf-8') as f:
                 f.write(f"{save_data}\n")
 
-    def _register_(self, path, func, method, content_type):
+    def _register_(self, path: str, func, method: str, content_type: dict, cors: list) -> None:
         """
         路由注册
         :param path: 路由
         :param func: 与路由绑定的方法
         :param method: 此路由的请求方法
         :param content_type: content_type的类型
         :return:
@@ -46,149 +46,181 @@
             content_type_str += f"{k}: {v}\r\n"
         if f"{path}" in self._routes_.keys():
             if method in self._routes_[path].keys():
                 raise Exception(
                     f"{str(datetime.datetime.now()).split('.')[0]} path:{path} -> function:{func.__name__}() not _register_ because {self._routes_[path]['methods'][method].__name__}() use {method} method already in {self._name_}")
             else:
                 self._show_routes_.append({path: method})
-                self._routes_[path][method] = {"func": func, "content_type": content_type_str}
+                self._routes_[path][method] = {"func": func, "content_type": content_type_str, "cors": cors}
                 self._routes_[path][method]['func'] = func
                 self._routes_[path][method]['content_type'] = content_type_str
+                self._routes_[path][method]['cors'] = cors
         else:
             self._show_routes_.append({path: method})
-            self._routes_[path] = {method: {"func": func, "content_type": content_type_str}}
+            self._routes_[path] = {method: {"func": func, "content_type": content_type_str, "cors": cors}}
 
-    def route(self, path='/', methods=None, content_type=None):
+    def route(self, path: str = '/', methods: list = None, content_type: dict = None, cors: list = None):
         """
         基础路由设置
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param methods: 默认请求方法为GET，POST，PUT，DELETE，PATCH，HEAD，OPTIONS
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if methods is None:
             methods = ['GET', 'POST', 'PUT', 'DELETE', 'PATCH', 'HEAD', 'OPTIONS']
         if content_type is None:
             content_type = self._content_type_
-
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
         def decorator(func):
             for method in methods:
-                self._register_(path, func, method, content_type)
+                self._register_(path, func, method, content_type, cors)
             return func
 
         return decorator
 
-    def get(self, path='/', content_type=None):
+    def get(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为GET
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "GET", content_type)
+            self._register_(path, func, "GET", content_type, cors)
             return func
 
         return decorator
 
-    def post(self, path='/', content_type=None):
+    def post(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为POST
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "POST", content_type)
+            self._register_(path, func, "POST", content_type, cors)
             return func
 
         return decorator
 
-    def head(self, path='/', content_type=None):
+    def head(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为HEAD
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "HEAD", content_type)
+            self._register_(path, func, "HEAD", content_type, cors)
             return func
 
         return decorator
 
-    def options(self, path='/', content_type=None):
+    def options(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为OPTIONS
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "OPTIONS", content_type)
+            self._register_(path, func, "OPTIONS", content_type, cors)
             return func
 
         return decorator
 
-    def put(self, path='/', content_type=None):
+    def put(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为PUT
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "PUT", content_type)
+            self._register_(path, func, "PUT", content_type, cors)
             return func
 
         return decorator
 
-    def delete(self, path='/', content_type=None):
+    def delete(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为DELETE
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "DELETE", content_type)
+            self._register_(path, func, "DELETE", content_type, cors)
             return func
 
         return decorator
 
-    def patch(self, path='/', content_type=None):
+    def patch(self, path: str = '/', content_type: dict = None, cors: list = None):
         """
         路由设置，请求方法为PATCH
+        :param cors: 跨域信息
         :param path: 默认路由地址为/
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
         :return:
         """
         if content_type is None:
             content_type = self._content_type_
+        if cors is not None:
+            if type(cors) is not list:
+                raise TypeError('cors must be a list')
 
         def decorator(func):
-            self._register_(path, func, "PATCH", content_type)
+            self._register_(path, func, "PATCH", content_type, cors)
             return func
 
         return decorator
 
     def _return_(self, request, client_socket, path_, address, handler, content_type, headers, method):
         """
         解析数据以及返回数据
@@ -234,15 +266,15 @@
             response = handler(data=data, headers=headers, args=new_body)
         response = f"HTTP/1.1 200 OK\r\n{content_type}\r\n{response}"
         client_socket.sendall(response.encode('utf-8'))
         message = f"{str(datetime.datetime.now()).split('.')[0]} from {address[0]}:{address[1]} to http://{self._host_}:{self._port_}{path_} {method} successful"
         print(message)
         self._log_(message)
 
-    def run(self, host="127.0.0.1", port=7012, try_model: bool = True, show_error: bool = True,
+    def run(self, host: str = "127.0.0.1", port: int = 7012, try_model: bool = True, show_error: bool = True,
             log_file: str = "%s.log", default_listen: int = Main.MAX_LISTEN, is_save_log: bool = True,
             content_type: dict = ContentType.TEXT, show_register: bool = False):
         """
         sparrowApi启动程序
         :param is_save_log: 是否进行日志记录
         :param show_register: 运行时是否输出已注册的路由路径
         :param content_type: 发送的数据类型，默认为text，基础类型在ContentType中，可以自定义，同时也为所有的请求头，传入类型为dict
@@ -341,14 +373,24 @@
         if path == "/favicon.ico":
             pass
         else:
             if path in self._routes_.keys():
                 if http_method in self._routes_[path].keys():
                     handler = self._routes_.get(path).get(http_method).get("func")
                     content_type = self._routes_.get(path).get(http_method).get("content_type")
+                    cors = self._routes_.get(path).get(http_method).get("cors")
+                    print(address)
+                    print(cors)
+                    if cors is not None:
+                        if cors[0] == "*":
+                            content_type += "Access-Control-Allow-Origin: *"
+                        else:
+                            if address[0] in cors:
+                                content_type += f"Access-Control-Allow-Origin: {address[0]}"
+                    print(content_type)
                     self._return_(request, client_socket, path_, address, handler, content_type, headers, http_method)
                 else:
                     response = 'HTTP/1.1 404 Not Found\r\nContent-Type: */*\r\n\r\nMethod Is Error'
                     client_socket.sendall(response.encode('utf-8'))
                     message = f"{str(datetime.datetime.now()).split('.')[0]} from {address[0]}:{address[1]} to http://{self._host_}:{self._port_}{path_} {http_method} unsuccessful"
                     print(message)
                     self._log_(message)
```

### Comparing `sparrowApi-0.1/sparrowApi/constant.py` & `sparrowApi-0.1.1/sparrowApi/constant.py`

 * *Files identical despite different names*

### Comparing `sparrowApi-0.1/sparrowApi/tool_class.py` & `sparrowApi-0.1.1/sparrowApi/tool_class.py`

 * *Files identical despite different names*

