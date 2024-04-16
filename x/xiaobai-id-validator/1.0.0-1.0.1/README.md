# Comparing `tmp/xiaobai_id_validator-1.0.0.tar.gz` & `tmp/xiaobai_id_validator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaobai_id_validator-1.0.0.tar", last modified: Fri Jan  5 09:14:01 2024, max compression
+gzip compressed data, was "xiaobai_id_validator-1.0.1.tar", last modified: Tue Apr 16 05:14:04 2024, max compression
```

## Comparing `xiaobai_id_validator-1.0.0.tar` & `xiaobai_id_validator-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-01-05 09:14:01.855520 xiaobai_id_validator-1.0.0/
--rw-r--r--   0 zrx        (501) staff       (20)      309 2024-01-05 09:14:01.855403 xiaobai_id_validator-1.0.0/PKG-INFO
--rw-r--r--   0 zrx        (501) staff       (20)        0 2024-01-05 08:40:07.000000 xiaobai_id_validator-1.0.0/README.md
--rw-r--r--   0 zrx        (501) staff       (20)       38 2024-01-05 09:14:01.855566 xiaobai_id_validator-1.0.0/setup.cfg
--rw-r--r--   0 zrx        (501) staff       (20)      550 2024-01-05 08:32:23.000000 xiaobai_id_validator-1.0.0/setup.py
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-01-05 09:14:01.854807 xiaobai_id_validator-1.0.0/xiaobai_id_validator/
--rw-r--r--   0 zrx        (501) staff       (20)       46 2024-01-05 08:55:52.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/__init__.py
--rw-r--r--   0 zrx        (501) staff       (20)   689350 2024-01-05 09:13:06.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/data.py
--rw-r--r--   0 zrx        (501) staff       (20)     1073 2024-01-05 08:20:10.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/func.py
--rw-r--r--   0 zrx        (501) staff       (20)     9998 2024-01-05 08:20:10.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/helper.py
--rw-r--r--   0 zrx        (501) staff       (20)      935 2024-01-05 08:20:10.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/utils.py
--rw-r--r--   0 zrx        (501) staff       (20)     3448 2024-01-05 08:20:10.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator/validator.py
-drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-01-05 09:14:01.855244 xiaobai_id_validator-1.0.0/xiaobai_id_validator.egg-info/
--rw-r--r--   0 zrx        (501) staff       (20)      309 2024-01-05 09:14:01.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator.egg-info/PKG-INFO
--rw-r--r--   0 zrx        (501) staff       (20)      380 2024-01-05 09:14:01.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator.egg-info/SOURCES.txt
--rw-r--r--   0 zrx        (501) staff       (20)        1 2024-01-05 09:14:01.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator.egg-info/dependency_links.txt
--rw-r--r--   0 zrx        (501) staff       (20)       21 2024-01-05 09:14:01.000000 xiaobai_id_validator-1.0.0/xiaobai_id_validator.egg-info/top_level.txt
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:14:04.849542 xiaobai_id_validator-1.0.1/
+-rw-r--r--   0 zrx        (501) staff       (20)      264 2024-04-16 05:14:04.849344 xiaobai_id_validator-1.0.1/PKG-INFO
+-rw-r--r--   0 zrx        (501) staff       (20)        0 2024-01-05 08:40:07.000000 xiaobai_id_validator-1.0.1/README.md
+-rw-r--r--   0 zrx        (501) staff       (20)       38 2024-04-16 05:14:04.849591 xiaobai_id_validator-1.0.1/setup.cfg
+-rw-r--r--   0 zrx        (501) staff       (20)      550 2024-01-05 08:32:23.000000 xiaobai_id_validator-1.0.1/setup.py
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:14:04.848561 xiaobai_id_validator-1.0.1/xiaobai_id_validator/
+-rw-r--r--   0 zrx        (501) staff       (20)       46 2024-04-16 03:17:28.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/__init__.py
+-rw-r--r--   0 zrx        (501) staff       (20)   689350 2024-01-05 09:15:22.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/data.py
+-rw-r--r--   0 zrx        (501) staff       (20)     1073 2024-04-16 02:55:09.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/func.py
+-rw-r--r--   0 zrx        (501) staff       (20)     9939 2024-04-16 05:12:10.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/helper.py
+-rw-r--r--   0 zrx        (501) staff       (20)     1024 2024-04-16 03:08:09.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/utils.py
+-rw-r--r--   0 zrx        (501) staff       (20)     3353 2024-04-16 05:12:46.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator/validator.py
+drwxr-xr-x   0 zrx        (501) staff       (20)        0 2024-04-16 05:14:04.849108 xiaobai_id_validator-1.0.1/xiaobai_id_validator.egg-info/
+-rw-r--r--   0 zrx        (501) staff       (20)      264 2024-04-16 05:14:04.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator.egg-info/PKG-INFO
+-rw-r--r--   0 zrx        (501) staff       (20)      380 2024-04-16 05:14:04.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 zrx        (501) staff       (20)        1 2024-04-16 05:14:04.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 zrx        (501) staff       (20)       21 2024-04-16 05:14:04.000000 xiaobai_id_validator-1.0.1/xiaobai_id_validator.egg-info/top_level.txt
```

### Comparing `xiaobai_id_validator-1.0.0/setup.py` & `xiaobai_id_validator-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xiaobai_id_validator-1.0.0/xiaobai_id_validator/data.py` & `xiaobai_id_validator-1.0.1/xiaobai_id_validator/data.py`

 * *Files identical despite different names*

### Comparing `xiaobai_id_validator-1.0.0/xiaobai_id_validator/func.py` & `xiaobai_id_validator-1.0.1/xiaobai_id_validator/func.py`

 * *Files identical despite different names*

### Comparing `xiaobai_id_validator-1.0.0/xiaobai_id_validator/helper.py` & `xiaobai_id_validator-1.0.1/xiaobai_id_validator/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import re
 import random
 import datetime
+
 from . import data
 from . import func
 
 
 def generator_address_code(address=None):
     """
     生成地址码
@@ -107,24 +108,18 @@
 
 def generator_check_bit(body):
     """
     生成校验码
     :param body:
     :return:
     """
-    pos_weight = {}
     weight_list = range(2, 19)[::-1]
-    for i in weight_list:
-        weight = pow(2, i - 1) % 11
-        pos_weight[i] = weight
-
-    body_sum = 0
-    body_list = list(body)
-    count = len(body)
+    pos_weight = {i: pow(2, i - 1) % 11 for i in weight_list}
 
+    body_sum, body_list, count = 0, list(body), len(body)
     for j in range(count):
         body_sum += int(body_list[j], 10) * pos_weight[18 - j]
 
     check_bit = (12 - (body_sum % 11)) % 11
 
     if check_bit == 10:
         check_bit = 'X'
```

### Comparing `xiaobai_id_validator-1.0.0/xiaobai_id_validator/utils.py` & `xiaobai_id_validator-1.0.1/xiaobai_id_validator/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,10 +43,12 @@
     :return:
     """
 
     @functools.wraps(func)
     def decorator(*args, **kwargs):
         if len(args[0]) != 15 and len(args[0]) != 18:
             return False
+        elif len(args[0]) == 18 and not args[0][:-1].isdigit():
+            return False
         return func(*args, **kwargs)
 
     return decorator
```

### Comparing `xiaobai_id_validator-1.0.0/xiaobai_id_validator/validator.py` & `xiaobai_id_validator-1.0.1/xiaobai_id_validator/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 #!/usr/bin/env python
 # encoding: utf-8
-
-from . import utils
-from . import helper
-from . import data
 import random
 from datetime import datetime
+from . import data, helper, utils
 
 
 @utils.check_for_none
 @utils.check_empty_string
 @utils.check_id_card_length
 def is_valid(id_card, strict_mode=False):
     """
@@ -52,22 +49,23 @@
     id_card = str(id_card)
 
     if not is_valid(id_card, strict_mode):
         return False
 
     code = helper.get_id_argument(id_card)
     address_info = helper.get_address_info(code['address_code'], code['birthday_code'], strict_mode)
+
     info = dict()
     info['address_code'] = code['address_code']
     info['abandoned'] = helper.check_abandoned(code['address_code'])
     info['address'] = address_info['province'] + address_info['city'] + address_info['district']
     info['address_tree'] = [address_info['province'], address_info['city'], address_info['district']]
     info['age'] = datetime.now().year - int(code['birthday_code'][0:4])
-    info['birthday_code'] = code['birthday_code'][0:4] + '-' + code['birthday_code'][4:6] + '-' + code['birthday_code'][
-                                                                                                  6:8]
+    info['birthday_code'] = code['birthday_code'][0:4] + '-' + code['birthday_code'][4:6] + '-' + \
+                            code['birthday_code'][6:8]
     info['constellation'] = helper.get_constellation(code['birthday_code'])
     info['chinese_zodiac'] = helper.get_chinese_zodiac(code['birthday_code'])
     info['sex'] = 0 if int(code['order_code']) % 2 == 0 else 1
     info['length'] = code['type']
     info['check_bit'] = code['check_bit']
 
     return info
```

