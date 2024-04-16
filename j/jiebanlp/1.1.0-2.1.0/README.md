# Comparing `tmp/jiebanlp-1.1.0.tar.gz` & `tmp/jiebanlp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiebanlp-1.1.0.tar", last modified: Mon Apr 15 08:22:14 2024, max compression
+gzip compressed data, was "jiebanlp-2.1.0.tar", last modified: Tue Apr 16 09:51:12 2024, max compression
```

## Comparing `jiebanlp-1.1.0.tar` & `jiebanlp-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 08:22:14.184929 jiebanlp-1.1.0/
--rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 jiebanlp-1.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      404 2024-04-15 08:22:14.182967 jiebanlp-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 08:22:14.159157 jiebanlp-1.1.0/jiebanlp/
--rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-1.1.0/jiebanlp/__init__.py
--rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-1.1.0/jiebanlp/constant.py
--rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-1.1.0/jiebanlp/manager.py
--rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-1.1.0/jiebanlp/predict.py
--rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-1.1.0/jiebanlp/scheduler.py
--rw-rw-rw-   0        0        0     1235 2024-04-15 07:14:26.000000 jiebanlp-1.1.0/jiebanlp/service.py
-drwxrwxrwx   0        0        0        0 2024-04-15 08:22:14.177573 jiebanlp-1.1.0/jiebanlp.egg-info/
--rw-rw-rw-   0        0        0      404 2024-04-15 08:22:14.000000 jiebanlp-1.1.0/jiebanlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2024-04-15 08:22:14.000000 jiebanlp-1.1.0/jiebanlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 08:22:14.000000 jiebanlp-1.1.0/jiebanlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-15 08:22:14.000000 jiebanlp-1.1.0/jiebanlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 08:22:14.185071 jiebanlp-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      646 2024-04-15 08:21:32.000000 jiebanlp-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:51:12.234310 jiebanlp-2.1.0/
+-rw-rw-rw-   0        0        0      469 2024-04-14 08:16:37.000000 jiebanlp-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-04-15 03:10:57.000000 jiebanlp-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:51:12.232090 jiebanlp-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       21 2024-04-15 03:10:31.000000 jiebanlp-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 09:51:12.204043 jiebanlp-2.1.0/jiebanlp/
+-rw-rw-rw-   0        0        0        0 2024-04-12 16:09:58.000000 jiebanlp-2.1.0/jiebanlp/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-04-15 03:16:25.000000 jiebanlp-2.1.0/jiebanlp/constant.py
+-rw-rw-rw-   0        0        0     1629 2024-04-15 05:37:23.000000 jiebanlp-2.1.0/jiebanlp/manager.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 03:21:31.000000 jiebanlp-2.1.0/jiebanlp/predict.py
+-rw-rw-rw-   0        0        0      296 2024-04-15 05:10:11.000000 jiebanlp-2.1.0/jiebanlp/scheduler.py
+-rw-rw-rw-   0        0        0     1357 2024-04-16 09:50:37.000000 jiebanlp-2.1.0/jiebanlp/service.py
+drwxrwxrwx   0        0        0        0 2024-04-16 09:51:12.225053 jiebanlp-2.1.0/jiebanlp.egg-info/
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:51:12.000000 jiebanlp-2.1.0/jiebanlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2024-04-16 09:51:12.000000 jiebanlp-2.1.0/jiebanlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 09:51:12.000000 jiebanlp-2.1.0/jiebanlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 09:51:12.000000 jiebanlp-2.1.0/jiebanlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 09:51:12.234310 jiebanlp-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      646 2024-04-16 09:50:49.000000 jiebanlp-2.1.0/setup.py
```

### Comparing `jiebanlp-1.1.0/jiebanlp/constant.py` & `jiebanlp-2.1.0/jiebanlp/constant.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-1.1.0/jiebanlp/manager.py` & `jiebanlp-2.1.0/jiebanlp/manager.py`

 * *Files identical despite different names*

### Comparing `jiebanlp-1.1.0/jiebanlp/service.py` & `jiebanlp-2.1.0/jiebanlp/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from flask import Flask, request, jsonify
+from flask import Flask, request, jsonify, make_response
 from mysql.connector import Error
 
 default_config = {
     'host': '0.0.0.0',
     'port': 5000,
     'debug': False,
 }
@@ -38,15 +38,16 @@
         return request.args
 
 # 发送数据
 def send_data(code=0, msg="数据获取成功。", data=None):
     response_content = {"code": code, "msg": msg}
     if data is not None:
         response_content["data"] = data
-    
     status = 200 if code == 0 else code
-    return jsonify(response_content), status
+    response = make_response(jsonify(response_content), status)
+    response.headers['Content-Type'] = 'application/json; charset=utf-8'
+    return response
 
 # 运行服务
 def run(app, config = default_config):
     final_config = {**default_config, **config}
     app.run(**final_config)
```

### Comparing `jiebanlp-1.1.0/setup.py` & `jiebanlp-2.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jiebanlp',
-    version="1.1.0",
+    version="2.1.0",
     packages=find_packages(),
     include_package_data=True,
     author="xl",
     author_email="123456@qq.com",
     description="A short description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

