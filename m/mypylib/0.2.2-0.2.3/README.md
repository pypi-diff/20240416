# Comparing `tmp/mypylib-0.2.2.tar.gz` & `tmp/mypylib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.2.2.tar", last modified: Mon Apr 15 05:43:53 2024, max compression
+gzip compressed data, was "mypylib-0.2.3.tar", last modified: Tue Apr 16 11:41:10 2024, max compression
```

## Comparing `mypylib-0.2.2.tar` & `mypylib-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.880657 mypylib-0.2.2/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-15 05:43:53.880272 mypylib-0.2.2/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2023-10-11 03:37:07.000000 mypylib-0.2.2/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.873740 mypylib-0.2.2/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    51079 2024-04-15 05:42:08.000000 mypylib-0.2.2/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3417 2024-01-25 14:54:07.000000 mypylib-0.2.2/mypylib/binance.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5984 2023-12-14 09:03:23.000000 mypylib-0.2.2/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      157 2023-12-27 08:05:41.000000 mypylib-0.2.2/mypylib/my_random_proxy.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1109 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/rayin.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    10696 2023-12-27 08:14:26.000000 mypylib-0.2.2/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.879556 mypylib-0.2.2/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3085 2023-10-18 03:05:27.000000 mypylib-0.2.2/mypylib/tmpDevelopment/arping.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1892 2023-10-17 13:34:43.000000 mypylib-0.2.2/mypylib/tmpDevelopment/tmp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2023-10-11 03:37:07.000000 mypylib-0.2.2/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2024-03-19 15:35:40.000000 mypylib-0.2.2/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8609 2023-10-16 13:50:29.000000 mypylib-0.2.2/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    10618 2024-04-15 05:41:25.000000 mypylib-0.2.2/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2024-04-15 05:43:53.876632 mypylib-0.2.2/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      310 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      748 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2024-04-15 05:43:53.000000 mypylib-0.2.2/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2024-04-15 05:43:53.880840 mypylib-0.2.2/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2023-10-11 03:37:07.000000 mypylib-0.2.2/setup.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/
+-rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 11:41:10.509836 mypylib-0.2.3/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)     3740 2023-11-06 13:42:12.000000 mypylib-0.2.3/README.md
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib/
+-rw-rw-r--   0 william   (1000) william   (1000)     3184 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/MP_shioaji_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)    51135 2024-04-16 11:40:10.000000 mypylib-0.2.3/mypylib/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3364 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/binance.py
+-rw-rw-r--   0 william   (1000) william   (1000)     7105 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/binance_copy_bot.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3421 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/chdbif.py
+-rw-rw-r--   0 william   (1000) william   (1000)     5984 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/crawler.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1083 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/crypto.py
+-rw-rw-r--   0 william   (1000) william   (1000)     5093 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/finmind.py
+-rw-rw-r--   0 william   (1000) william   (1000)    87196 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/libexcel.py
+-rw-rw-r--   0 william   (1000) william   (1000)    24435 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/mvp.py
+-rw-rw-r--   0 william   (1000) william   (1000)      157 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/my_random_proxy.py
+-rw-rw-r--   0 william   (1000) william   (1000)     3588 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/option_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1109 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/rayin.py
+-rw-rw-r--   0 william   (1000) william   (1000)      778 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_history_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)     2490 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_kline.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1312 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/shioaji_ticks.py
+-rw-rw-r--   0 william   (1000) william   (1000)    10696 2024-03-13 13:37:39.000000 mypylib-0.2.3/mypylib/sjtools.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1464 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tLineNotify.py
+-rw-rw-r--   0 william   (1000) william   (1000)     7735 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/ti.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib/tmpDevelopment/
+-rw-rw-r--   0 william   (1000) william   (1000)        0 2023-11-06 13:42:12.000000 mypylib-0.2.3/mypylib/tmpDevelopment/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)       37 2024-03-14 04:27:41.000000 mypylib-0.2.3/mypylib/tmpDevelopment/aa.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1958 2024-03-14 04:49:02.000000 mypylib-0.2.3/mypylib/tmpDevelopment/socket_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1074 2023-11-06 13:42:12.000000 mypylib-0.2.3/mypylib/tmpDevelopment/warrant_test.py
+-rw-rw-r--   0 william   (1000) william   (1000)     2543 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tplaysound.py
+-rw-rw-r--   0 william   (1000) william   (1000)     8609 2023-11-06 13:43:07.000000 mypylib-0.2.3/mypylib/tredis.py
+-rw-rw-r--   0 william   (1000) william   (1000)    11313 2024-04-16 11:40:10.000000 mypylib-0.2.3/mypylib/warrant.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2024-04-16 11:41:10.509836 mypylib-0.2.3/mypylib.egg-info/
+-rw-rw-r--   0 william   (1000) william   (1000)      310 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)      752 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/SOURCES.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        1 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/dependency_links.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        8 2024-04-16 11:41:10.000000 mypylib-0.2.3/mypylib.egg-info/top_level.txt
+-rw-rw-r--   0 william   (1000) william   (1000)       38 2024-04-16 11:41:10.509836 mypylib-0.2.3/setup.cfg
+-rw-rw-r--   0 william   (1000) william   (1000)      846 2023-11-06 13:42:12.000000 mypylib-0.2.3/setup.py
```

### Comparing `mypylib-0.2.2/README.md` & `mypylib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/MP_shioaji_ticks.py` & `mypylib-0.2.3/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/__init__.py` & `mypylib-0.2.3/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,18 @@
     '2024/03/11: 0.1.96 修正處置股資料。必須要看是否在期限內',
     '2024/03/13: 0.1.97 fix get_punishment_list()',
     '2024/03/23: 0.1.98 add warrant_bible_convert_to_c_need()',
     '2024/03/24: 0.1.99 modify warrant_bible_convert_to_c_need() and save warrant_bible.txt',
     '2024/03/27: 0.2.00 fix get_punishment_list() date bug ',
     '2024/04/11: 0.2.01 fix warrant_bible_convert_to_c_need() bug',
     '2024/04/15: 0.2.02 add warrant_bible_do_all()',
+    '2024/04/16: 0.2.03 change request to http.client',
 }
 
-__version__ = '0.2.02'
+__version__ = '0.2.03'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.2.2/mypylib/binance.py` & `mypylib-0.2.3/mypylib/binance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Org binance data path: https://data.binance.vision/
-
 import requests
 import xmltodict
 import json
 import wget
 from enum import Enum
 import os
 
@@ -85,21 +83,21 @@
     return True
 
 
 if __name__ == '__main__':
     list_targets = binance_get_history_list_targets(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines)
     print(list_targets)
 
-    list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, list_targets[0], Period._5m)
+    list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, list_targets[0], Period._15m)
     print(list_files)
 
     binance_get_history_download_file(list_files[0], list_files[0].split('/')[-1])
 
     for target in list_targets:
-        list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, target, Period._5m)
+        list_files = binance_get_history_list_files_by_target(Future_option_spot.future, Cm_um.um, Daily_monthly.monthly, Klines_others.klines, target, Period._15m)
         for file_url in list_files:
             if not file_url.endswith('.zip'):
                 continue
             file_name = file_url.split('/')[-1]
 
             if os.path.isfile(file_name):
                 continue
```

### Comparing `mypylib-0.2.2/mypylib/binance_copy_bot.py` & `mypylib-0.2.3/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/chdbif.py` & `mypylib-0.2.3/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/crawler.py` & `mypylib-0.2.3/mypylib/crawler.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/crypto.py` & `mypylib-0.2.3/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/finmind.py` & `mypylib-0.2.3/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/libexcel.py` & `mypylib-0.2.3/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/mvp.py` & `mypylib-0.2.3/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/option_test.py` & `mypylib-0.2.3/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/rayin.py` & `mypylib-0.2.3/mypylib/rayin.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/shioaji_history_ticks.py` & `mypylib-0.2.3/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/shioaji_kline.py` & `mypylib-0.2.3/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/shioaji_ticks.py` & `mypylib-0.2.3/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/sjtools.py` & `mypylib-0.2.3/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/tLineNotify.py` & `mypylib-0.2.3/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/ti.py` & `mypylib-0.2.3/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.2.3/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/tplaysound.py` & `mypylib-0.2.3/mypylib/tplaysound.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+
 import threading
 import queue
 import os
 from playsound import playsound
 from loguru import logger
 import datetime
 from collections import defaultdict
 
+
 if os.name == 'nt':
     import winsound
 
 _MYPYLIB_ROOT = os.path.abspath(os.path.dirname(__file__))
 
-
 class tplaysound(threading.Thread):
 
     def __init__(self):
         threading.Thread.__init__(self)
 
         self.time_block = 2
 
         self.queue = queue.Queue()
         self.queue.maxsize = 2
 
+
         self.file_sound_alert = f'{_MYPYLIB_ROOT}/../data/alert.wav'
 
         self.start()
 
         self.dict_filename_to_datetime = defaultdict(datetime.datetime.now)
 
     def block_or_not(self, filename):
@@ -79,14 +81,15 @@
         self.queue.put(('stop', 'stop'))
 
 
 
 if __name__ == '__main__':
     from time import sleep
 
+
     tps = tplaysound()
     index = 0
     while True:
         tps.play_file()
         tps.play_file()
         tps.play_file()
         tps.play_file()
```

### Comparing `mypylib-0.2.2/mypylib/tredis.py` & `mypylib-0.2.3/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.2.2/mypylib/warrant.py` & `mypylib-0.2.3/mypylib/warrant.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 import datetime
 import re
 import requests
 import os
 from os.path import expanduser
 from io import StringIO
 import shutil
+from loguru import logger
+import http.client
+from urllib.parse import urlparse
+
+headers = {'User-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/604.5.6 (KHTML, like Gecko) Version/11.0.3 Safari/604.5.6'}
 
 # 讀取新上市的權證標的
 # 從元富的網站讀取
 # 有些新上市的權證，當天不會出現在權證達人寶典上面，這樣跟單不會跟到，很可惜，因此在每天開盤之前，讀取當天新上市的權證
 # 資料來源: https://newjust.masterlink.com.tw/z/zx/zxc/zxc.djhtm?a=2&page=1
 # 讀取進來之後轉換成
 '''
@@ -39,30 +44,30 @@
 
     for i in range(1, 9999):
         url = f'https://newjust.masterlink.com.tw/z/zx/zxc/zxc.djhtm?a=2&page={i}'
         # 元富把 pd.read_html() 檔掉了...，所以得用別的方式去讀取
         # ret = requests.get(url, headers={'User-agent': 'Mozilla/5.0'}).text
         # df_tmp = pd.read_html(requests.get(url, headers={'User-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/604.5.6 (KHTML, like Gecko) Version/11.0.3 Safari/604.5.6'}).text)
 
-        response = requests.get(url, headers={'User-agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_3) AppleWebKit/604.5.6 (KHTML, like Gecko) Version/11.0.3 Safari/604.5.6'})
+        response = requests.get(url, headers=headers)
         html_data = StringIO(response.text)
         df_tmp = pd.read_html(html_data)
 
         # sleep(1)
         df_tmp = df_tmp[2].iloc[2:]
         # df_tmp.columns = df_tmp.iloc[0]
 
-        # print(f'{i} {df_tmp.shape}')
+        # logger.info(f'{i} {df_tmp.shape}')
         if df_tmp.shape[0] == 1:
             count_no_data += 1
             if count_no_data > 3:
                 break
             else:
                 continue
-        # print(df_tmp)
+        # logger.info(df_tmp)
         df = pd.concat([df, df_tmp])
 
     df = df.dropna()
     df_list = df.to_dict('records')
 
     list_new_warrants = []
     for d in df_list:
@@ -70,18 +75,18 @@
         if isinstance(d[5], str) and d[5][0] == '<':
             ret = re.search(r'.*GenLink2stk\((\'AS(.*)\',\'(.*)\')\)', d[5])
             if ret is None:
                 continue
             symbol = ret.group(2)
             name = ret.group(3)
             list_new_warrants.append(('T', d[0], d[1], d[2], symbol, name, d[4]))
-            # print('T', symbol, name, d[4])
+            # logger.info('T', symbol, name, d[4])
         else:
             list_new_warrants.append(('N', d[0], d[1], d[2], d[5], d[5], d[4]))
-            # print('N', d[5], d[4])
+            # logger.info('N', d[5], d[4])
 
     return list_new_warrants
 
 
 #
 # 0 日期：
 # 1
@@ -138,15 +143,15 @@
         date_due = datetime.datetime.strptime(dict_warrant_to_info[x]['到期日期'], '%Y/%m/%d')
         days_number_due = (date_due - date_today).days
         dict_warrant_to_info[x]['到期天數'] = days_number_due
         dict_warrant_to_info[x]['Volume'] = 0
         code = dict_warrant_to_info[x]['標的代碼']
         dict_stock_to_warrant[code].append(x)
 
-    # print(stock_warrant_map)
+    # logger.info(stock_warrant_map)
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
 def add_new_issued_warrant_to_bible(dict_warrant_to_info, dict_stock_to_warrant, list_new_warrants):
     # ('T', '06227P', '南電麥證26售01', '認售', '8046', '南電', '111/12/22')
     # ('N', '06228P', '臺股指麥證26售15', '認售', '加權指數', '加權指數', '111/12/22')
 
@@ -156,15 +161,15 @@
         if x[3] != '認購':
             continue
         if x[1] not in dict_warrant_to_info.keys():
             year, month, day = x[6].split('/')
             year = int(year) + 1911
             date_to_file = f'{year}/{month}/{day}'
 
-            print(f'新權證: {x[1]} {x[2]} {x[6]} {date_to_file}')
+            logger.info(f'新權證: {x[1]} {x[2]} {x[6]} {date_to_file}')
 
             dict_warrant_to_info[x[1]] = {
                 '權證名稱': x[2],
                 '發行券商': x[2],
                 '權證價格': 0,
                 '權證漲跌': 0,
                 '權證漲跌幅': 0,
@@ -207,71 +212,86 @@
             }
 
             dict_stock_to_warrant[x[4]].append(x[1])
     return dict_warrant_to_info, dict_stock_to_warrant
 
 
 def warrant_bible_convert_to_c_need(dict_warrant_to_info):
-    target_file = f'{expanduser("~")}/warrant/warrant_bible.txt'
+    target_file = f'/home/william/warrant/warrant_bible.txt'
     with open(target_file, "w+") as fp:
         for warrant in dict_warrant_to_info:
             fp.write(f'{warrant}\t{dict_warrant_to_info[warrant]["標的代碼"]}\t{dict_warrant_to_info[warrant]["認購/售類別"]}\n')
 
 
 def download_latest_warrant_bible():
     day_now = datetime.datetime.now()
 
     while True:
         str_date = day_now.strftime('%Y-%m-%d')
-        target_file = f'{expanduser("~")}/warrant/warrant-{str_date}.xls'
+        target_file = f'/home/william/warrant/warrant-{str_date}.xls'
         url = f'http://iwarrant-mobile.capital.com.tw/wdataV2/canonical/capital-newvol/%E6%AC%8A%E8%AD%89%E9%81%94%E4%BA%BA%E5%AF%B6%E5%85%B8_NEWVOL_{str_date}.xls'
-        print(f'下載權證達人寶典: {url}')
+        logger.info(f'下載權證達人寶典: {url}')
 
-        r = requests.get(url, headers={'User-agent': 'Mozilla/5.0'}, stream=True)
-        if r.status_code == 200:
-            with open(target_file, 'wb') as f:
-                f.write(r.content)
-            break
-        else:
-            print(f'找不到 {url}')
-            day_now -= datetime.timedelta(days=1)
+        parsed_url = urlparse(url)
+        host = parsed_url.netloc
+        path = parsed_url.path
+
+        try:
+            conn = http.client.HTTPConnection(host)
+            conn.request("GET", path, headers=headers)
+            response = conn.getresponse()
+            if response.status != 200:
+                logger.info(f'Failed to download {url}')
+            else:
+                with open(target_file, 'wb') as f:
+                    shutil.copyfileobj(response, f)  # 將 response 寫入檔案
+                break
+        except Exception as e:
+            logger.error(e)
+
+        day_now -= datetime.timedelta(days=1)
 
 
 def get_last_warrant_bible_date():
-    files = os.listdir(f'{expanduser("~")}/warrant')
+    files = os.listdir(f'/home/william/warrant')
     files.sort(reverse=True)
     file = ''
     for file in files:
         if file.startswith('warrant') and file.endswith('.xls'):
             bool_found = True
             # warrant-2024-04-12.xls
             return file[8:18]
     return None
 
 
 def warrant_bible_do_all():
-    import datetime
+    logger.info('download_latest_warrant_bible')
     download_latest_warrant_bible()
+    logger.info('get_last_warrant_bible_date')
     date_str = get_last_warrant_bible_date()
-    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'{expanduser("~")}/warrant/warrant-{date_str}.xls')
+    logger.info('read_warrant_bible')
+    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'/home/william/warrant/warrant-{date_str}.xls')
+    logger.info('get_new_warrant_list')
     list_new_warrants = get_new_warrant_list()
+    logger.info('add_new_issued_warrant_to_bible')
     dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
                                                                                   dict_stock_to_warrant,
                                                                                   list_new_warrants)
+    logger.info('warrant_bible_convert_to_c_need')
     warrant_bible_convert_to_c_need(dict_warrant_to_info)
 
 
 if __name__ == '__main__':
     import datetime
 
     download_latest_warrant_bible()
 
     # 2024-04-12
     date_str = get_last_warrant_bible_date()
 
-    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'{expanduser("~")}/warrant/warrant-{date_str}.xls')
+    dict_warrant_to_info, dict_stock_to_warrant = read_warrant_bible(f'/home/william/warrant/warrant-{date_str}.xls')
     list_new_warrants = get_new_warrant_list()
 
     dict_warrant_to_info, dict_stock_to_warrant = add_new_issued_warrant_to_bible(dict_warrant_to_info,
                                                                                   dict_stock_to_warrant,
                                                                                   list_new_warrants)
     warrant_bible_convert_to_c_need(dict_warrant_to_info)
```

### Comparing `mypylib-0.2.2/mypylib.egg-info/SOURCES.txt` & `mypylib-0.2.3/mypylib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 mypylib/tredis.py
 mypylib/warrant.py
 mypylib.egg-info/PKG-INFO
 mypylib.egg-info/SOURCES.txt
 mypylib.egg-info/dependency_links.txt
 mypylib.egg-info/top_level.txt
 mypylib/tmpDevelopment/__init__.py
-mypylib/tmpDevelopment/arping.py
-mypylib/tmpDevelopment/tmp.py
+mypylib/tmpDevelopment/aa.py
+mypylib/tmpDevelopment/socket_test.py
 mypylib/tmpDevelopment/warrant_test.py
```

### Comparing `mypylib-0.2.2/setup.py` & `mypylib-0.2.3/setup.py`

 * *Files identical despite different names*

