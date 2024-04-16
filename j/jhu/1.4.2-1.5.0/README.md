# Comparing `tmp/jhu-1.4.2.tar.gz` & `tmp/jhu-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhu-1.4.2.tar", last modified: Fri Apr 12 09:08:49 2024, max compression
+gzip compressed data, was "jhu-1.5.0.tar", last modified: Tue Apr 16 09:34:22 2024, max compression
```

## Comparing `jhu-1.4.2.tar` & `jhu-1.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.854325 jhu-1.4.2/
--rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.4.2/LICENSE
--rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-12 09:08:49.853584 jhu-1.4.2/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)     1706 2024-04-12 08:24:25.000000 jhu-1.4.2/README.md
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.849614 jhu-1.4.2/jhu/
--rw-r--r--   0 hujian     (501) staff       (20)       21 2024-04-12 09:07:47.000000 jhu-1.4.2/jhu/__init__.py
--rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-01-05 07:00:28.000000 jhu-1.4.2/jhu/auth.py
--rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.4.2/jhu/email.py
--rw-r--r--   0 hujian     (501) staff       (20)     2620 2024-04-12 09:05:59.000000 jhu-1.4.2/jhu/security.py
--rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.4.2/jhu/webhook.py
-drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-12 09:08:49.852937 jhu-1.4.2/jhu.egg-info/
--rw-r--r--   0 hujian     (501) staff       (20)      596 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/PKG-INFO
--rw-r--r--   0 hujian     (501) staff       (20)      254 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/SOURCES.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/dependency_links.txt
--rw-r--r--   0 hujian     (501) staff       (20)       42 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/requires.txt
--rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-12 09:08:49.000000 jhu-1.4.2/jhu.egg-info/top_level.txt
--rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.4.2/jhu.egg-info/zip-safe
--rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-12 09:08:49.854451 jhu-1.4.2/setup.cfg
--rwxr-xr-x   0 hujian     (501) staff       (20)     1592 2024-04-12 08:23:43.000000 jhu-1.4.2/setup.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-16 09:34:22.767527 jhu-1.5.0/
+-rw-r--r--   0 hujian     (501) staff       (20)     1066 2023-03-06 05:42:40.000000 jhu-1.5.0/LICENSE
+-rw-r--r--   0 hujian     (501) staff       (20)      622 2024-04-16 09:34:22.767072 jhu-1.5.0/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)     1706 2024-04-12 08:24:25.000000 jhu-1.5.0/README.md
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-16 09:34:22.761936 jhu-1.5.0/jhu/
+-rw-r--r--   0 hujian     (501) staff       (20)       21 2024-04-16 08:42:12.000000 jhu-1.5.0/jhu/__init__.py
+-rw-r--r--   0 hujian     (501) staff       (20)     5039 2024-04-16 08:37:49.000000 jhu-1.5.0/jhu/auth.py
+-rw-r--r--   0 hujian     (501) staff       (20)     2828 2024-04-16 09:34:09.000000 jhu-1.5.0/jhu/data.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4487 2023-12-19 06:05:59.000000 jhu-1.5.0/jhu/email.py
+-rw-r--r--   0 hujian     (501) staff       (20)     2620 2024-04-16 08:39:07.000000 jhu-1.5.0/jhu/security.py
+-rw-r--r--   0 hujian     (501) staff       (20)     4408 2024-01-08 01:29:05.000000 jhu-1.5.0/jhu/webhook.py
+drwxr-xr-x   0 hujian     (501) staff       (20)        0 2024-04-16 09:34:22.766568 jhu-1.5.0/jhu.egg-info/
+-rw-r--r--   0 hujian     (501) staff       (20)      622 2024-04-16 09:34:22.000000 jhu-1.5.0/jhu.egg-info/PKG-INFO
+-rw-r--r--   0 hujian     (501) staff       (20)      266 2024-04-16 09:34:22.000000 jhu-1.5.0/jhu.egg-info/SOURCES.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2024-04-16 09:34:22.000000 jhu-1.5.0/jhu.egg-info/dependency_links.txt
+-rw-r--r--   0 hujian     (501) staff       (20)       53 2024-04-16 09:34:22.000000 jhu-1.5.0/jhu.egg-info/requires.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        4 2024-04-16 09:34:22.000000 jhu-1.5.0/jhu.egg-info/top_level.txt
+-rw-r--r--   0 hujian     (501) staff       (20)        1 2023-03-06 05:44:18.000000 jhu-1.5.0/jhu.egg-info/zip-safe
+-rw-r--r--   0 hujian     (501) staff       (20)       38 2024-04-16 09:34:22.767625 jhu-1.5.0/setup.cfg
+-rwxr-xr-x   0 hujian     (501) staff       (20)     1630 2024-04-16 08:42:07.000000 jhu-1.5.0/setup.py
```

### Comparing `jhu-1.4.2/LICENSE` & `jhu-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jhu-1.4.2/PKG-INFO` & `jhu-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.2
+Version: 1.5.0
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-jose
 Requires-Dist: bcrypt
 Requires-Dist: pycryptodomex
+Requires-Dist: sqlalchemy
```

### Comparing `jhu-1.4.2/README.md` & `jhu-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jhu-1.4.2/jhu/auth.py` & `jhu-1.5.0/jhu/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from urllib.parse import quote_plus
 from enum import Enum
 from requests import post, get
 
 
 class AuthType(Enum):
-    DINGDING = 0
+    DINGTALK = 0
     FEISHU = 1
 
 
 def dingding_user_info_get(ak: str, sk: str, auth_code: str) -> dict:
     # 获取Access_token
     ACCESS_TOKEN_URL = 'https://api.dingtalk.com/v1.0/oauth2/userAccessToken'
     data = dict(clientId=ak, clientSecret=sk,
@@ -55,15 +55,15 @@
 class ThridAuth:
     def __init__(self, ak: str, sk: str, auth_type: AuthType) -> None:
         """三方扫码登录初始化
 
         Args:
             ak:str,应用的appkey
             sk:str,应用的secretkey
-            auth_type:AuthType,应用类型,当前支持 钉钉:AuthType.DINGDING,飞书:AuthType.FEISHU
+            auth_type:AuthType,应用类型,当前支持 钉钉:AuthType.DINGTALK,飞书:AuthType.FEISHU
         """
         self.auth_type = auth_type
         self.ak = ak
         self.sk = sk
 
     def login_url_generate(self, redirect_url: str, state: str = None) -> str:
         """生成三方扫码登录的url地址
@@ -72,16 +72,16 @@
             redirect_url:str,扫码通过后,回调的地址
             state:str,生成地址用的state
 
         Return:
             三方扫码登录的url地址:str
         """
         match(self.auth_type):
-            case AuthType.DINGDING:
-                state = state or 'JHU_DINGDING'
+            case AuthType.DINGTALK:
+                state = state or 'JHU_DINGTALK'
                 # 钉钉三方登录网页地址拼接
                 prefix_url = 'https://login.dingtalk.com/oauth2/challenge.htm'
                 data = dict(
                     redirect_uri=quote_plus(redirect_url),
                     client_id=self.ak,
                     response_type='code', scope='openid', state=state, prompt='consent'
                 )
@@ -108,27 +108,27 @@
         Args:
             auth_code:str,三方登录连接返回的auth_code
 
         Return:
             用户的json信息:dict
         """
         match(self.auth_type):
-            case AuthType.DINGDING:
+            case AuthType.DINGTALK:
                 result = dingding_user_info_get(self.ak, self.sk, auth_code)
             case AuthType.FEISHU:
                 result = feishu_user_info_get(self.ak, self.sk, auth_code)
             case _:
                 raise Exception('认证类型类型错误')
         return result
 
 
 if __name__ == '__main__':
     ding_ak = 'ding_ak'
     ding_sk = 'ding_sk'
-    d = ThridAuth(ding_ak, ding_sk, AuthType.DINGDING)
+    d = ThridAuth(ding_ak, ding_sk, AuthType.DINGTALK)
     d.login_url_generate('http://localhost:9000/')
     # 这里的code从redirect_url返回的code中获取
     d.get_user_info('74f4f8d7dcdc3942ac11ef963f8fc76d')
 
     feishu_ak = 'feishu_ak'
     feishu_sk = 'feishu_sk'
     f = ThridAuth(feishu_ak, feishu_sk, AuthType.FEISHU)
```

### Comparing `jhu-1.4.2/jhu/email.py` & `jhu-1.5.0/jhu/email.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.2/jhu/security.py` & `jhu-1.5.0/jhu/security.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.2/jhu/webhook.py` & `jhu-1.5.0/jhu/webhook.py`

 * *Files identical despite different names*

### Comparing `jhu-1.4.2/jhu.egg-info/PKG-INFO` & `jhu-1.5.0/jhu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: jhu
-Version: 1.4.2
+Version: 1.5.0
 Summary: jhu是一个工具包,简化或自动化的做一些任务
 Home-page: https://github.com/joestarhu/jhu
 Author: J.Hu
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-jose
 Requires-Dist: bcrypt
 Requires-Dist: pycryptodomex
+Requires-Dist: sqlalchemy
```

### Comparing `jhu-1.4.2/setup.py` & `jhu-1.5.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     password = # 这里改成放申请下来的token
 6. twine upload dist/* 可上传安装,需要输入pypi的用户名和密码
 """
 from setuptools import setup, find_packages
 
 setup(
     name='jhu',  # 包的名称
-    version='1.4.2',  # 包的版本,每次更新或升级包都需要更新它
+    version='1.5.0',  # 包的版本,每次更新或升级包都需要更新它
     description='jhu是一个工具包,简化或自动化的做一些任务',  # 包的描述
     author='J.Hu',  # 作者
     email='joestarhu@163.com',  # 作者邮箱
     url='https://github.com/joestarhu/jhu',  # 项目地址
     packages=find_packages(
         exclude=['test', 'examples', 'script', 'tutorials']),   # 包内不需要引用的文件
     classifiers=[
@@ -33,10 +33,11 @@
         'Programming Language :: Python :: 3.12',
     ],
     install_requires=[
         'requests',         # auth webhook
         'python-jose',      # security.py
         'bcrypt',           # security.py
         'pycryptodomex',    # security.py
+        'sqlalchemy',       # data.py
         ],  # 依赖的包
     zip_safe=True
 )
```

