# Comparing `tmp/mypylib-0.2.3.tar.gz` & `tmp/mypylib-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.3.tar", last modified: Tue Apr 16 11:41:10 2024, max compression
+gzip compressed data, was "mypylib-0.2.4.tar", last modified: Tue Apr 16 12:30:48 2024, max compression
```

## Comparing `mypylib-0.2.3.tar` & `mypylib-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/
--rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 11:41:10.509836 mypylib-0.2.3/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     3740 2023-11-06 13:42:12.000000 mypylib-0.2.3/README.md
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib/
--rw-rw-r--   0 william   (1000) william   (1000)     3184 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/MP_shioaji_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)    51135 2024-04-16 11:40:10.000000 mypylib-0.2.3/mypylib/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)     3364 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/binance.py
--rw-rw-r--   0 william   (1000) william   (1000)     7105 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/binance_copy_bot.py
--rw-rw-r--   0 william   (1000) william   (1000)     3421 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/chdbif.py
--rw-rw-r--   0 william   (1000) william   (1000)     5984 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/crawler.py
--rw-rw-r--   0 william   (1000) william   (1000)     1083 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/crypto.py
--rw-rw-r--   0 william   (1000) william   (1000)     5093 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/finmind.py
--rw-rw-r--   0 william   (1000) william   (1000)    87196 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/libexcel.py
--rw-rw-r--   0 william   (1000) william   (1000)    24435 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/mvp.py
--rw-rw-r--   0 william   (1000) william   (1000)      157 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/my_random_proxy.py
--rw-rw-r--   0 william   (1000) william   (1000)     3588 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/option_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     1109 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/rayin.py
--rw-rw-r--   0 william   (1000) william   (1000)      778 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_history_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)     2490 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_kline.py
--rw-rw-r--   0 william   (1000) william   (1000)     1312 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_ticks.py
--rw-rw-r--   0 william   (1000) william   (1000)    10696 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/sjtools.py
--rw-rw-r--   0 william   (1000) william   (1000)     1464 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tLineNotify.py
--rw-rw-r--   0 william   (1000) william   (1000)     7735 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/ti.py
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib/tmpDevelopment/
--rw-rw-r--   0 william   (1000) william   (1000)        0 2023-11-06 13:42:12.000000 mypylib-0.2.3/mypylib/tmpDevelopment/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)       37 2024-03-14 04:27:41.000000 mypylib-0.2.3/mypylib/tmpDevelopment/aa.py
--rw-rw-r--   0 william   (1000) william   (1000)     1958 2024-03-14 04:49:02.000000 mypylib-0.2.3/mypylib/tmpDevelopment/socket_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     1074 2023-11-06 13:42:12.000000 mypylib-0.2.3/mypylib/tmpDevelopment/warrant_test.py
--rw-rw-r--   0 william   (1000) william   (1000)     2543 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tplaysound.py
--rw-rw-r--   0 william   (1000) william   (1000)     8609 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tredis.py
--rw-rw-r--   0 william   (1000) william   (1000)    11313 2024-04-16 11:40:10.000000 mypylib-0.2.3/mypylib/warrant.py
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)      752 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        1 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)        8 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)       38 2024-04-16 11:41:10.509836 mypylib-0.2.3/setup.cfg
--rw-rw-r--   0 william   (1000) william   (1000)      846 2023-11-06 13:42:12.000000 mypylib-0.2.3/setup.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:30:48.573874 mypylib-0.2.4/
+-rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 12:30:48.573874 mypylib-0.2.4/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)     3740 2023-11-06 13:42:12.000000 mypylib-0.2.4/README.md
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:30:48.569874 mypylib-0.2.4/mypylib/
+-rw-rw-r--   0 william   (1000) william   (1000)     3184 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/MP_shioaji_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)    51171 2024-04-16 12:30:22.000000 mypylib-0.2.4/mypylib/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3364 2024-03-13 13:37:39.000000 mypylib-0.2.4/mypylib/binance.py
+-rw-rw-r--   0 william   (1000) william   (1000)     7105 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/binance_copy_bot.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3421 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/chdbif.py
+-rw-rw-r--   0 william   (1000) william   (1000)     5984 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/crawler.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1083 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/crypto.py
+-rw-rw-r--   0 william   (1000) william   (1000)     5093 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/finmind.py
+-rw-rw-r--   0 william   (1000) william   (1000)    87196 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/libexcel.py
+-rw-rw-r--   0 william   (1000) william   (1000)    24435 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/mvp.py
+-rw-rw-r--   0 william   (1000) william   (1000)      157 2024-03-13 13:37:39.000000 mypylib-0.2.4/mypylib/my_random_proxy.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3588 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/option_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1109 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/rayin.py
+-rw-rw-r--   0 william   (1000) william   (1000)      778 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/shioaji_history_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)     2490 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/shioaji_kline.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1312 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/shioaji_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)    10696 2024-03-13 13:37:39.000000 mypylib-0.2.4/mypylib/sjtools.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1464 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/tLineNotify.py
+-rw-rw-r--   0 william   (1000) william   (1000)     7735 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/ti.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:30:48.573874 mypylib-0.2.4/mypylib/tmpDevelopment/
+-rw-rw-r--   0 william   (1000) william   (1000)        0 2023-11-06 13:42:12.000000 mypylib-0.2.4/mypylib/tmpDevelopment/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)       37 2024-03-14 04:27:41.000000 mypylib-0.2.4/mypylib/tmpDevelopment/aa.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1958 2024-03-14 04:49:02.000000 mypylib-0.2.4/mypylib/tmpDevelopment/socket_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1074 2023-11-06 13:42:12.000000 mypylib-0.2.4/mypylib/tmpDevelopment/warrant_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     2543 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/tplaysound.py
+-rw-rw-r--   0 william   (1000) william   (1000)     8609 2023-11-06 13:43:07.000000 mypylib-0.2.4/mypylib/tredis.py
+-rw-rw-r--   0 william   (1000) william   (1000)    11658 2024-04-16 12:29:27.000000 mypylib-0.2.4/mypylib/warrant.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 12:30:48.573874 mypylib-0.2.4/mypylib.egg-info/
+-rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 12:30:48.000000 mypylib-0.2.4/mypylib.egg-info/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)      752 2024-04-16 12:30:48.000000 mypylib-0.2.4/mypylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        1 2024-04-16 12:30:48.000000 mypylib-0.2.4/mypylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        8 2024-04-16 12:30:48.000000 mypylib-0.2.4/mypylib.egg-info/top_level.txt
+-rw-rw-r--   0 william   (1000) william   (1000)       38 2024-04-16 12:30:48.573874 mypylib-0.2.4/setup.cfg
+-rw-rw-r--   0 william   (1000) william   (1000)      846 2023-11-06 13:42:12.000000 mypylib-0.2.4/setup.py
```

### Comparing `mypylib-0.2.3/README.md` & `mypylib-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.4/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/__init__.py` & `mypylib-0.2.4/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,17 +91,18 @@
     '2024/03/13: 0.1.97 fix get_punishment_list()',
     '2024/03/23: 0.1.98 add warrant_bible_convert_to_c_need()',
     '2024/03/24: 0.1.99 modify warrant_bible_convert_to_c_need() and save warrant_bible.txt',
     '2024/03/27: 0.2.00 fix get_punishment_list() date bug ',
     '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
     '2024/04/15: 0.2.02 add warrant_bible_do_all()',
     '2024/04/16: 0.2.03 change request to http.client',
+    '2024/04/16: 0.2.04 add proxy',
 }
 
-__version__ = '0.2.03'
+__version__ = '0.2.04'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.3/mypylib/binance.py` & `mypylib-0.2.4/mypylib/binance.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/binance_copy_bot.py` & `mypylib-0.2.4/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/chdbif.py` & `mypylib-0.2.4/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/crawler.py` & `mypylib-0.2.4/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/crypto.py` & `mypylib-0.2.4/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/finmind.py` & `mypylib-0.2.4/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/libexcel.py` & `mypylib-0.2.4/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/mvp.py` & `mypylib-0.2.4/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/option_test.py` & `mypylib-0.2.4/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/rayin.py` & `mypylib-0.2.4/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.4/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/shioaji_kline.py` & `mypylib-0.2.4/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/shioaji_ticks.py` & `mypylib-0.2.4/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/sjtools.py` & `mypylib-0.2.4/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/tLineNotify.py` & `mypylib-0.2.4/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/ti.py` & `mypylib-0.2.4/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/tmpDevelopment/socket_test.py` & `mypylib-0.2.4/mypylib/tmpDevelopment/socket_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.4/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/tplaysound.py` & `mypylib-0.2.4/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/tredis.py` & `mypylib-0.2.4/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/mypylib/warrant.py` & `mypylib-0.2.4/mypylib/warrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 import re
 import requests
 import os
 from os.path import expanduser
 from io import StringIO
 import shutil
 from loguru import logger
-import http.client
-from urllib.parse import urlparse
 
 headers = {'User-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/604.5.6 (KHTML, like Gecko) Version/11.0.3 Safari/604.5.6'}
 
 # 讀取新上市的權證標的
 # 從元富的網站讀取
 # 有些新上市的權證，當天不會出現在權證達人寶典上面，這樣跟單不會跟到，很可惜，因此在每天開盤之前，讀取當天新上市的權證
 # 資料來源: https://newjust.masterlink.com.tw/z/zx/zxc/zxc.djhtm?a=2&page=1
@@ -26,14 +24,31 @@
   3: '111/12/14',
   4: '111/12/16',
   5: "<!-- \tGenLink2stk('AS2014','中鴻'); //-->",
   6: '34.78'},
 '''
 
 
+def get_proxy_settings():
+    # Retrieve proxy settings using os.environ (like a dictionary)
+    http_proxy = os.environ.get('HTTP_PROXY') or os.environ.get('http_proxy')
+    https_proxy = os.environ.get('HTTPS_PROXY') or os.environ.get('https_proxy')
+
+    # Using os.getenv() method to specify a default value if the variable is not found
+    # Example: os.getenv('HTTP_PROXY', 'Default Value')
+
+    if http_proxy is None:
+        return None
+
+    return {
+        "HTTP Proxy": http_proxy,
+        "HTTPS Proxy": https_proxy
+    }
+
+
 #
 # 之後傳回 list
 # ('T' or 'N', symbol, name, 上市日期)
 
 def get_new_warrant_list():
     import pandas as pd
     from time import sleep
@@ -44,15 +59,15 @@
 
     for i in range(1, 9999):
         url = f'https://newjust.masterlink.com.tw/z/zx/zxc/zxc.djhtm?a=2&page={i}'
         # 元富把 pd.read_html() 檔掉了...，所以得用別的方式去讀取
         # ret = requests.get(url, headers={'User-agent': 'Mozilla/5.0'}).text
         # df_tmp = pd.read_html(requests.get(url, headers={'User-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/604.5.6 (KHTML, like Gecko) Version/11.0.3 Safari/604.5.6'}).text)
 
-        response = requests.get(url, headers=headers)
+        response = requests.get(url, headers=headers, proxies=get_proxy_settings())
         html_data = StringIO(response.text)
         df_tmp = pd.read_html(html_data)
 
         # sleep(1)
         df_tmp = df_tmp[2].iloc[2:]
         # df_tmp.columns = df_tmp.iloc[0]
 
@@ -227,28 +242,24 @@
 
     while True:
         str_date = day_now.strftime('%Y-%m-%d')
         target_file = f'/home/william/warrant/warrant-{str_date}.xls'
         url = f'http://iwarrant-mobile.capital.com.tw/wdataV2/canonical/capital-newvol/%E6%AC%8A%E8%AD%89%E9%81%94%E4%BA%BA%E5%AF%B6%E5%85%B8_NEWVOL_{str_date}.xls'
         logger.info(f'下載權證達人寶典: {url}')
 
-        parsed_url = urlparse(url)
-        host = parsed_url.netloc
-        path = parsed_url.path
-
         try:
-            conn = http.client.HTTPConnection(host)
-            conn.request("GET", path, headers=headers)
-            response = conn.getresponse()
-            if response.status != 200:
-                logger.info(f'Failed to download {url}')
-            else:
-                with open(target_file, 'wb') as f:
-                    shutil.copyfileobj(response, f)  # 將 response 寫入檔案
-                break
+            with requests.get(url, proxies=get_proxy_settings(), headers=headers) as r:
+                r.raise_for_status()
+            with open(target_file, '+wb') as f:
+                for chunk in r:
+                    if chunk:
+                        # logger.info(f'chunk: {chunk}')
+                        f.write(chunk)
+
+            break
         except Exception as e:
             logger.error(e)
 
         day_now -= datetime.timedelta(days=1)
 
 
 def get_last_warrant_bible_date():
```

### Comparing `mypylib-0.2.3/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.4/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.3/setup.py` & `mypylib-0.2.4/setup.py`

 * *Files identical despite different names*

