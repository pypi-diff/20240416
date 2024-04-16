# Comparing `tmp/amino_fix_fix-1.0.8.1.tar.gz` & `tmp/amino_fix_fix-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino_fix_fix-1.0.8.1.tar", last modified: Mon Apr 15 17:44:31 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `amino_fix_fix-1.0.8.1.tar` & `amino_fix_fix-1.1.tar`

### file list

```diff
@@ -1,35 +1,25 @@
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.169118 amino_fix_fix-1.0.8.1/
--rw-r--r--   0 josephattano   (501) staff       (20)     1075 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/LICENSE
--rw-r--r--   0 josephattano   (501) staff       (20)     4550 2024-04-15 17:44:31.169031 amino_fix_fix-1.0.8.1/PKG-INFO
--rw-r--r--   0 josephattano   (501) staff       (20)     3474 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/README.md
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.168349 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/
--rw-r--r--   0 josephattano   (501) staff       (20)     4550 2024-04-15 17:44:31.000000 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/PKG-INFO
--rw-r--r--   0 josephattano   (501) staff       (20)      799 2024-04-15 17:44:31.000000 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/SOURCES.txt
--rw-r--r--   0 josephattano   (501) staff       (20)        1 2024-04-15 17:44:31.000000 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/dependency_links.txt
--rw-r--r--   0 josephattano   (501) staff       (20)      227 2024-04-15 17:44:31.000000 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/requires.txt
--rw-r--r--   0 josephattano   (501) staff       (20)       12 2024-04-15 17:44:31.000000 amino_fix_fix-1.0.8.1/amino.fix.fix.egg-info/top_level.txt
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.164470 amino_fix_fix-1.0.8.1/aminofixfix/
--rw-r--r--   0 josephattano   (501) staff       (20)     1284 2024-04-14 22:54:03.000000 amino_fix_fix-1.0.8.1/aminofixfix/__init__.py
--rw-r--r--   0 josephattano   (501) staff       (20)    24271 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/acm.py
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.166107 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/
--rw-r--r--   0 josephattano   (501) staff       (20)     1270 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/__init__.py
--rw-r--r--   0 josephattano   (501) staff       (20)    16275 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/acm.py
--rw-r--r--   0 josephattano   (501) staff       (20)    98563 2024-04-15 17:43:21.000000 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/client.py
--rw-r--r--   0 josephattano   (501) staff       (20)    14887 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/socket.py
--rw-r--r--   0 josephattano   (501) staff       (20)   109970 2024-04-15 17:44:08.000000 amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/sub_client.py
--rw-r--r--   0 josephattano   (501) staff       (20)   105410 2024-04-15 17:39:45.000000 amino_fix_fix-1.0.8.1/aminofixfix/client.py
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.166988 amino_fix_fix-1.0.8.1/aminofixfix/lib/
--rw-r--r--   0 josephattano   (501) staff       (20)       95 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/__init__.py
--rw-r--r--   0 josephattano   (501) staff       (20)    33502 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/exceptions.py
-drwxr-xr-x   0 josephattano   (501) staff       (20)        0 2024-04-15 17:44:31.168170 amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/
--rw-r--r--   0 josephattano   (501) staff       (20)      243 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/__init__.py
--rw-r--r--   0 josephattano   (501) staff       (20)     3388 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/aiohttp.py
--rw-r--r--   0 josephattano   (501) staff       (20)     2610 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/requests.py
--rw-r--r--   0 josephattano   (501) staff       (20)      657 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/unsuccessful_import.py
--rw-r--r--   0 josephattano   (501) staff       (20)     5911 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/headers.py
--rw-r--r--   0 josephattano   (501) staff       (20)     5123 2024-04-15 17:43:52.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/helpers.py
--rw-r--r--   0 josephattano   (501) staff       (20)   200156 2024-04-14 22:46:06.000000 amino_fix_fix-1.0.8.1/aminofixfix/lib/objects.py
--rw-r--r--   0 josephattano   (501) staff       (20)    14885 2024-04-14 22:30:26.000000 amino_fix_fix-1.0.8.1/aminofixfix/socket.py
--rw-r--r--   0 josephattano   (501) staff       (20)   146160 2024-04-14 22:51:45.000000 amino_fix_fix-1.0.8.1/aminofixfix/sub_client.py
--rw-r--r--   0 josephattano   (501) staff       (20)       38 2024-04-15 17:44:31.169329 amino_fix_fix-1.0.8.1/setup.cfg
--rw-r--r--   0 josephattano   (501) staff       (20)     1363 2024-04-15 17:43:45.000000 amino_fix_fix-1.0.8.1/setup.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/__init__.py
+-rw-r--r--   0        0        0    24271 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/acm.py
+-rw-r--r--   0        0        0   105414 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/client.py
+-rw-r--r--   0        0        0    14295 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/socket.py
+-rw-r--r--   0        0        0   146160 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/sub_client.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/README.md
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/__init__.py
+-rw-r--r--   0        0        0    16275 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/acm.py
+-rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/client.py
+-rw-r--r--   0        0        0    14297 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/socket.py
+-rw-r--r--   0        0        0   109970 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/asyncfixfix/sub_client.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/__init__.py
+-rw-r--r--   0        0        0    33502 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/exceptions.py
+-rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/headers.py
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/helpers.py
+-rw-r--r--   0        0        0   200156 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/objects.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/__init__.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/aiohttp.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/requests.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/aminofixfix/lib/facades/unsuccessful_import.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/LICENSE
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/README.md
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/pyproject.toml
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 amino_fix_fix-1.1/PKG-INFO
```

### Comparing `amino_fix_fix-1.0.8.1/LICENSE` & `amino_fix_fix-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/PKG-INFO` & `amino_fix_fix-1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,57 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: amino.fix.fix
-Version: 1.0.8.1
-Summary: Library for Aminoapps
-Home-page: https://github.com/imperialwool/Amino.fix.fix
-Author: imperialwool
-Author-email: hi@iwool.dev
-License: MIT
-Keywords: aminoapps,amino.fix,amino.fix.fix,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,imperialwool
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Version: 1.1
+Summary: Unofficial library to work with Aminoapps
+Project-URL: Download, https://github.com/imperialwool/Amino.fix.fix.git
+Project-URL: Homepage, https://github.com/imperialwool/Amino.fix.fix
+Project-URL: Issues, https://github.com/imperialwool/Amino.fix.fix/issues
+Author-email: imperialwool <hi@iwool.dev>
+License-Expression: MIT
 License-File: LICENSE
+Keywords: amino,amino fix,amino fix fix,amino py,amino-bot,amino.fix,amino.fix.fix,aminoapps,aminofix,aminofixfix,api,imperialwool,medialab,minori,narvii,ndc,python,python3,python3.x
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.8
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: httpx[http2]
 Requires-Dist: httpx[socks]
-Requires-Dist: websocket-client>=1.3.1
 Requires-Dist: python-socks
-Requires-Dist: setuptools
-Provides-Extra: requests
-Requires-Dist: requests>=2.30.0; extra == "requests"
-Requires-Dist: requests[socks]; extra == "requests"
+Requires-Dist: websocket-client>=1.3.1
 Provides-Extra: aiohttp
-Requires-Dist: aiohttp>=3.9.0; extra == "aiohttp"
-Requires-Dist: aiohttp[speedups]; extra == "aiohttp"
-Requires-Dist: aiohttp_socks; extra == "aiohttp"
+Requires-Dist: aiohttp-socks; extra == 'aiohttp'
+Requires-Dist: aiohttp>=3.9.0; extra == 'aiohttp'
+Requires-Dist: aiohttp[speedups]; extra == 'aiohttp'
 Provides-Extra: dev
-Requires-Dist: setuptools; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
+Requires-Dist: wheel; extra == 'dev'
+Provides-Extra: requests
+Requires-Dist: requests>=2.30.0; extra == 'requests'
+Requires-Dist: requests[socks]; extra == 'requests'
+Description-Content-Type: text/markdown
 
 # Amino.fix.fix
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b4-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
-Fork of Amino.fix to improve this library.
+Fork of Amino.fix to improve this library. Also unofficial client to work with Aminoapps.
 
 ## Important notices
 
 - in subclient you should pass `client`, **not** `profile`
 - if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
 - `lib/util` -> `lib/`
 - if you have issues in pydroid, reinstall/update it
```

### Comparing `amino_fix_fix-1.0.8.1/README.md` & `amino_fix_fix-1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/amino.fix.fix.svg)](https://pypi.python.org/pypi/amino.fix.fix/)
 [![PyPi Preview](https://img.shields.io/badge/pypi_pre-v1.0.7b4-blue)](https://pypi.org/project/amino.fix.fix/#history)
 ![Python Version](https://img.shields.io/badge/python-%3E%3D3.8-orange)
 [![Issues](https://img.shields.io/github/issues-raw/imperialwool/amino.fix.fix.svg?maxAge=25000)](https://github.com/imperialwool/Amino.fix.fix/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr/imperialwool/amino.fix.fix.svg?style=flat)](https://github.com/imperialwool/Amino.fix.fix/pulls)
 
-Fork of Amino.fix to improve this library.
+Fork of Amino.fix to improve this library. Also unofficial client to work with Aminoapps.
 
 ## Important notices
 
 - in subclient you should pass `client`, **not** `profile`
 - if you have issues with HTTPX [let me know here](https://github.com/imperialwool/Amino.fix.fix/issues/3)
 - `lib/util` -> `lib/`
 - if you have issues in pydroid, reinstall/update it
```

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/acm.py` & `amino_fix_fix-1.1/aminofixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/acm.py` & `amino_fix_fix-1.1/aminofixfix/asyncfixfix/acm.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/client.py` & `amino_fix_fix-1.1/aminofixfix/asyncfixfix/client.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/socket.py` & `amino_fix_fix-1.1/aminofixfix/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,18 @@
 from random import randint
 from json import loads, dumps
 from datetime import datetime as dt
 
 from threading import Thread
 from sys import _getframe as getframe
 
-from ..lib import objects, helpers
-from ..lib.helpers import gen_deviceId, inttime
+from .lib import objects, helpers
+from .lib.helpers import gen_deviceId, inttime
 
 class SocketHandler:
-    '''
-        Sockets needs rewrite. Really.
-
-        It's hard to add new features or support it, because code is mess of useless functions and things.
-        It's LITTERALY a digital spaghetti that will poison you instead of healing you.
-
-        In next update if sockets will be rewritten,
-        just know that sockets was written from scratch using "websockets" library, not "websocket-client".
-
-        And please. DO NOT SEND any issues about websockets if they arent rewritten.
-        I will close it and ignore it. Just please. I'm asking you as human to you, human.
-    '''
     def __init__(self, client, socket_trace: bool = False, debug: bool = False):
         self.socket_url = f"wss://ws{randint(1,4)}.aminoapps.com"
         self.debug = debug
         self.socket = None
         self.active = False
         self.headers = None
         self.proxies = None
```

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/asyncfixfix/sub_client.py` & `amino_fix_fix-1.1/aminofixfix/asyncfixfix/sub_client.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/client.py` & `amino_fix_fix-1.1/aminofixfix/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         """
         Init client.
 
         Accepting:
         - deviceId: str
         - userAgent: str
         - proxies: str | dict 
-            - str support in beta
+            - from dict will be taken
         - socket_trace: bool = False
             - recieving all things that socket doing
         - socketDebugging: bool = False
             - socket printing results of its work
         - socket_enabled: bool = True
             - enabling socket or not
             - useful for scripts
```

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/exceptions.py` & `amino_fix_fix-1.1/aminofixfix/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/aiohttp.py` & `amino_fix_fix-1.1/aminofixfix/lib/facades/aiohttp.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/requests.py` & `amino_fix_fix-1.1/aminofixfix/lib/facades/requests.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/facades/unsuccessful_import.py` & `amino_fix_fix-1.1/aminofixfix/lib/facades/unsuccessful_import.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/headers.py` & `amino_fix_fix-1.1/aminofixfix/lib/headers.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/helpers.py` & `amino_fix_fix-1.1/aminofixfix/lib/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from hashlib import sha1
 from os import urandom
 from json import loads
 from uuid import uuid4
 from hmac import new
 import re
 
-LIBRARY_VERSION = "1.0.8.1"
-
 PREFIX = bytes.fromhex("19")
 SIG_KEY = bytes.fromhex("DFA5ED192DDA6E88A12FE12130DC6206B1251E44")
 DEVICE_KEY = bytes.fromhex("E7309ECC0953C6FA60005B2765F99DBBC965C8E9")
 
 IPHONE_IDS = [
     "11,2", "11,4", "11,6", "11,8",
     "12,1", "12,3", "12,5", "12,8",
```

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/lib/objects.py` & `amino_fix_fix-1.1/aminofixfix/lib/objects.py`

 * *Files identical despite different names*

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/socket.py` & `amino_fix_fix-1.1/aminofixfix/asyncfixfix/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,18 @@
 from random import randint
 from json import loads, dumps
 from datetime import datetime as dt
 
 from threading import Thread
 from sys import _getframe as getframe
 
-from .lib import objects, helpers
-from .lib.helpers import gen_deviceId, inttime
+from ..lib import objects, helpers
+from ..lib.helpers import gen_deviceId, inttime
 
 class SocketHandler:
-    '''
-        Sockets needs rewrite. Really.
-
-        It's hard to add new features or support it, because code is mess of useless functions and things.
-        It's LITTERALY a digital spaghetti that will poison you instead of healing you.
-
-        In next update if sockets will be rewritten,
-        just know that sockets was written from scratch using "websockets" library, not "websocket-client".
-
-        And please. DO NOT SEND any issues about websockets if they arent rewritten.
-        I will close it and ignore it. Just please. I'm asking you as human to you, human.
-    '''
     def __init__(self, client, socket_trace: bool = False, debug: bool = False):
         self.socket_url = f"wss://ws{randint(1,4)}.aminoapps.com"
         self.debug = debug
         self.socket = None
         self.active = False
         self.headers = None
         self.proxies = None
```

### Comparing `amino_fix_fix-1.0.8.1/aminofixfix/sub_client.py` & `amino_fix_fix-1.1/aminofixfix/sub_client.py`

 * *Files identical despite different names*

