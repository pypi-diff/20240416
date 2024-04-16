# Comparing `tmp/tsugu-0.4.7.tar.gz` & `tmp/tsugu-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.7.tar", last modified: Mon Apr 15 17:50:21 2024, max compression
+gzip compressed data, was "tsugu-0.4.8.tar", last modified: Tue Apr 16 01:05:33 2024, max compression
```

## Comparing `tsugu-0.4.7.tar` & `tsugu-0.4.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.291282 tsugu-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 17:50:12.000000 tsugu-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 17:50:21.291282 tsugu-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 17:50:12.000000 tsugu-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:50:21.291282 tsugu-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 17:50:12.000000 tsugu-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.287282 tsugu-0.4.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 17:50:12.000000 tsugu-0.4.7/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.287282 tsugu-0.4.7/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19371 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.291282 tsugu-0.4.7/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 01:05:21.000000 tsugu-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:05:33.777291 tsugu-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 01:05:21.000000 tsugu-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:05:33.777291 tsugu-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 01:05:21.000000 tsugu-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 01:05:21.000000 tsugu-0.4.8/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21196 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.7/LICENSE` & `tsugu-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.7/PKG-INFO` & `tsugu-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.7
+Version: 0.4.8
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.8 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.7/README.md` & `tsugu-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.7/setup.py` & `tsugu-0.4.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.7',
+    version='0.4.8',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
-            "requests",
+            "urllib3",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-0.4.7/test/test_main.py` & `tsugu-0.4.8/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.7/tsugu/bot.py` & `tsugu-0.4.8/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.7/tsugu/config.py` & `tsugu-0.4.8/tsugu/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 
 class Config:
     def __init__(self):
         # 设置默认值
         self.backend = "http://tsugubot.com:8080"
         self.user_data_backend = "http://tsugubot.com:8080"
+        self.backend_use_proxy = False
+        self.user_data_backend_use_proxy = False
+        self.submit_car_number_use_proxy = False
+        self.verify_player_bind_use_proxy = False
+        self.proxy_url = "http://localhost:7890"
         self.user_database_path = None
-
-        self.use_proxies = False
-        self.proxies = {
-            "http": "http://127.0.0.1:7890",
-            "https": "http://127.0.0.1:7890",
-        }
-
         self.token_name = "Tsugu"
         self.bandori_station_token = "ZtV4EX2K9Onb"
 
         self.use_easy_bg = True
         self.compress = True
 
         self.ban_gacha_simulate_group_data = []
@@ -283,20 +281,20 @@
         pass
         return None
 
     def output_config_json(self, path="./config.json"):
         config_pre_json = {
             "backend": "http://tsugubot.com:8080",
             "user_data_backend": "http://tsugubot.com:8080",
+            "backend_use_proxy": False,
+            "user_data_backend_use_proxy": False,
+            "submit_car_number_use_proxy": False,
+            "verify_player_bind_use_proxy": False,
+            "proxy_url": "http://localhost:7890",
             "user_database_path": None,
-            "use_proxies": False,
-            "proxies": {
-                "http": "http://localhost:7890",
-                "https": "http://localhost:7890",
-            },
             "token_name": "Tsugu",
             "bandori_station_token": "ZtV4EX2K9Onb",
             "use_easy_bg": True,
             "compress": True,
             "ban_gacha_simulate_group_data": [],
             "server_list": {
                 "0": "日服",
```

### Comparing `tsugu-0.4.7/tsugu/router.py` & `tsugu-0.4.8/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.7/tsugu/utils.py` & `tsugu-0.4.8/tsugu/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import requests
 from typing import List
 import re
 import json
 import sqlite3
 import os
 import sys
 import random
-from requests.exceptions import HTTPError
-# import atexit
+import urllib3
+from urllib3.exceptions import HTTPError
 
 from .config import config
 
 
 class DatabaseManager:
     def __init__(self, path):
         self.path = path
@@ -86,25 +85,52 @@
 
 def server_exists(server):
     if server or server == 0:
         return True
     return False
 
 
-def requests_post(url, data):
+def requests_post_for_user(url, data):
+    if config.user_data_backend_use_proxy:
+        http = urllib3.ProxyManager(config.proxy_url)
+    else:
+        http = urllib3.PoolManager()
     try:
-        if config.use_proxies:
-            response = requests.post(url, json=data, proxies=config.proxies)
-        else:
-            response = requests.post(url, json=data)
+        response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
 
         # 检查响应的状态码是否为 200
-        response.raise_for_status()
+        if response.status == 200:
+            return json.loads(response.data.decode('utf-8'))
+        else:
+            # 处理其他状态码
+            return text_response("服务器出现了问题，请稍后再试。")
 
-        return response.json()
+    except HTTPError as http_err:
+        print(f'HTTP 错误：{http_err}')
+        return text_response("服务器出现了问题，请稍后再试。")
+
+    except Exception as e:
+        print(f'发生异常：{e}')
+        return text_response("发生了未知错误。")
+
+
+def requests_post_for_backend(url, data):
+    if config.backend_use_proxy:
+        http = urllib3.ProxyManager(config.proxy_url)
+    else:
+        http = urllib3.PoolManager()
+    try:
+        response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
+
+        # 检查响应的状态码是否为 200
+        if response.status == 200:
+            return json.loads(response.data.decode('utf-8'))
+        else:
+            # 处理其他状态码
+            return text_response("服务器出现了问题，请稍后再试。")
 
     except HTTPError as http_err:
         print(f'HTTP 错误：{http_err}')
         return text_response("服务器出现了问题，请稍后再试。")
 
     except Exception as e:
         print(f'发生异常：{e}')
@@ -119,15 +145,15 @@
         "default_servers": default_servers,
         "server": server,
         "text": text,
         "useEasyBG": config.use_easy_bg,
         "compress": config.compress
     }
     # print(data)
-    res = requests_post(f"{config.backend}{path}", data)
+    res = requests_post_for_backend(f"{config.backend}{path}", data)
     return res
 
 
 def v2_api_command(message, command_matched, api, platform, user_id, channel_id):
     text = message[len(command_matched):].strip()
 
     if api in ['cardIllustration', 'ycm']:  # 无需验证server信息
@@ -143,14 +169,15 @@
     try:
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
         return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
     except Exception as e:
         return text_response('前端错误: ' + str(e))
 
+
 def submit_car_number_msg(message, user_id, platform=None):
     # 检查car_config['car']中的关键字
     for keyword in config.car_config["car"]:
         if str(keyword) in message:
             break
     else:
         return False
@@ -173,26 +200,38 @@
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
-        # 构建URL
+
+        # 构建 URL
         url = f"https://api.bandoristation.com/index.php?function=submit_room_number&number={car_id}&user_id={user_id}&raw_message={message}&source={config.token_name}&token={config.bandori_station_token}"
+
+        if config.submit_car_number_use_proxy:
+            http = urllib3.ProxyManager(config.proxy_url)
+        else:
+            http = urllib3.PoolManager()
+
         # 发送请求
-        response = requests.get(url)
-        if response.status_code != 200:
-            print(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status_code}")
+        response = http.request('GET', url)
+
+        # 检查响应的状态码是否为 200
+        if response.status == 200:
+            return True
+        else:
+            print(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status}")
             return True  # 虽然提交失败，但是确定了是车牌消息
-        return True
+
     except Exception as e:
         print(f"[Tsugu] 发生异常: {e}")
         return True  # 虽然提交失败，但是确定了是车牌消息
 
+
 def match_command(message, cmd_dict):
     for command, api_value in cmd_dict.items():
         if message.startswith(command):
             return command, api_value
     return None, None
 
 
@@ -381,17 +420,31 @@
         return text_response('请先获取验证代码')
     # 检测重复性
     game_ids = json.loads(user_data['data']['game_ids'])
     for i in game_ids:
         if i.get("game_id") == player_id and i.get("server") == server:
             return text_response('请勿重复绑定')
     server_s_name = config.server_index_to_s_name[str(server)]
+
+    # 构建 URL
     url = f'https://bestdori.com/api/player/{server_s_name}/{player_id}?mode=2'
-    response = requests.get(url)
-    data = response.json()
+    if config.verify_player_bind_use_proxy:
+        http = urllib3.ProxyManager(config.proxy_url)
+    else:
+        http = urllib3.PoolManager()
+    # 发送请求
+    response = http.request('GET', url)
+    # 检查响应的状态码是否为 200
+    if response.status == 200:
+        # 解析 JSON 响应数据
+        data = json.loads(response.data.decode('utf-8'))
+    else:
+        print(f"获取玩家数据失败，HTTP响应码: {response.status}")
+        return None
+
     if data.get("data").get("profile") is None or data.get("profile") == {}:
         return text_response('玩家ID不存在，请检查输入，或服务器是否对应')
     introduction = data.get("data", {}).get("profile", {}).get("introduction")
     deck_name = data.get("data", {}).get("profile", {}).get("mainUserDeck", {}).get("deckName")
     if verify_code != introduction and verify_code != deck_name:
         return text_response('验证失败，签名或者乐队编队名称与验证代码不匹配喵，可以检查后再次尝试(无需重复发送绑定玩家)')
     # 验证成功
@@ -450,38 +503,38 @@
 class Remote:
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         data = {
             'platform': platform,
             'user_id': user_id
         }
-        result = requests_post(f"{config.user_data_backend}/user/getUserData", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/getUserData", data)
         return result
 
     @staticmethod
     def bind_player_request(platform: str, user_id: str, server: int, bind_type: bool):
         data = {
             'platform': platform,
             'user_id': user_id,
             'server': server,
             'bindType': bind_type  # 布尔，表示绑定还是解绑
         }
-        result = requests_post(f"{config.user_data_backend}/user/bindPlayerRequest", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/bindPlayerRequest", data)
         return result
 
     @staticmethod
     def bind_player_verification(platform: str, user_id: str, server: int, player_id: str, bind_type: bool):
         data = {
             'platform': platform,
             'user_id': user_id,
             'server': server,
             'playerId': player_id,
             'bindType': bind_type  # 布尔，表示绑定还是解绑
         }
-        result = requests_post(f"{config.user_data_backend}/user/bindPlayerVerification", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/bindPlayerVerification", data)
         return result
 
     @staticmethod
     def player_status(user_id, platform, server=None):
         user_data = Remote.get_user_data(platform, user_id)
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
@@ -495,31 +548,31 @@
     @staticmethod
     def set_car_forward(platform, user_id, status):
         data = {
             'platform': platform,
             'user_id': user_id,
             'status': status
         }
-        result = requests_post(f"{config.user_data_backend}/user/changeUserData/setCarForwarding", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setCarForwarding", data)
         return result
 
     @staticmethod
     def set_default_server(platform, user_id, text):
         data = {
             'platform': platform,
             'user_id': user_id,
             'text': text
         }
-        result = requests_post(f"{config.user_data_backend}/user/changeUserData/setDefaultServer", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setDefaultServer", data)
         return result
 
     @staticmethod
     def set_server_mode(platform, user_id, text):
         data = {
             'platform': platform,
             'user_id': user_id,
             'text': text
         }
-        result = requests_post(f"{config.user_data_backend}/user/changeUserData/setServerMode", data)
+        result = requests_post_for_user(f"{config.user_data_backend}/user/changeUserData/setServerMode", data)
         return result
```

### Comparing `tsugu-0.4.7/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.8/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.7
+Version: 0.4.8
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.7 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.8 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

