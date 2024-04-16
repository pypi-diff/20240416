# Comparing `tmp/tsugu-0.4.6.tar.gz` & `tmp/tsugu-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.6.tar", last modified: Mon Apr 15 03:05:22 2024, max compression
+gzip compressed data, was "tsugu-0.4.7.tar", last modified: Mon Apr 15 17:50:21 2024, max compression
```

## Comparing `tsugu-0.4.6.tar` & `tsugu-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.057525 tsugu-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 03:05:10.000000 tsugu-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 03:05:22.057525 tsugu-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 03:05:10.000000 tsugu-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:05:22.057525 tsugu-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 03:05:10.000000 tsugu-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.053525 tsugu-0.4.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 03:05:10.000000 tsugu-0.4.6/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.053525 tsugu-0.4.6/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.057525 tsugu-0.4.6/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 03:05:22.000000 tsugu-0.4.6/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.291282 tsugu-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 17:50:12.000000 tsugu-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 17:50:21.291282 tsugu-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 17:50:12.000000 tsugu-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:50:21.291282 tsugu-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 17:50:12.000000 tsugu-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.287282 tsugu-0.4.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 17:50:12.000000 tsugu-0.4.7/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.287282 tsugu-0.4.7/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19371 2024-04-15 17:50:12.000000 tsugu-0.4.7/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:50:21.291282 tsugu-0.4.7/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 17:50:21.000000 tsugu-0.4.7/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.6/LICENSE` & `tsugu-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/PKG-INFO` & `tsugu-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.6
+Version: 0.4.7
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.6 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.7 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.6/README.md` & `tsugu-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/setup.py` & `tsugu-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.6',
+    version='0.4.7',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.6/test/test_main.py` & `tsugu-0.4.7/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/tsugu/bot.py` & `tsugu-0.4.7/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/tsugu/config.py` & `tsugu-0.4.7/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/tsugu/router.py` & `tsugu-0.4.7/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.6/tsugu/utils.py` & `tsugu-0.4.7/tsugu/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import requests
 from typing import List
 import re
 import json
 import sqlite3
-import atexit
 import os
 import sys
 import random
+from requests.exceptions import HTTPError
+# import atexit
 
 from .config import config
 
 
 class DatabaseManager:
     def __init__(self, path):
         self.path = path
@@ -91,19 +92,27 @@
 
 def requests_post(url, data):
     try:
         if config.use_proxies:
             response = requests.post(url, json=data, proxies=config.proxies)
         else:
             response = requests.post(url, json=data)
+
+        # 检查响应的状态码是否为 200
+        response.raise_for_status()
+
         return response.json()
+
+    except HTTPError as http_err:
+        print(f'HTTP 错误：{http_err}')
+        return text_response("服务器出现了问题，请稍后再试。")
+
     except Exception as e:
-        print(response, response.text)
-        # raise e
-        return text_response(f"发生异常: {str(response)}")
+        print(f'发生异常：{e}')
+        return text_response("发生了未知错误。")
 
 
 def v2api_from_backend(api, text, default_servers: List[int] = None, server=3):
     if default_servers is None:
         default_servers = [3, 0]
     path = f"/v2/{api}"
     data = {
```

### Comparing `tsugu-0.4.6/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.7/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.6
+Version: 0.4.7
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.6 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.7 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

