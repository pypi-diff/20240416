# Comparing `tmp/tsugu-0.4.8.tar.gz` & `tmp/tsugu-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.8.tar", last modified: Tue Apr 16 01:05:33 2024, max compression
+gzip compressed data, was "tsugu-0.4.9.tar", last modified: Tue Apr 16 01:13:29 2024, max compression
```

## Comparing `tsugu-0.4.8.tar` & `tsugu-0.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 01:05:21.000000 tsugu-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:05:33.777291 tsugu-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 01:05:21.000000 tsugu-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:05:33.777291 tsugu-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 01:05:21.000000 tsugu-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 01:05:21.000000 tsugu-0.4.8/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    21196 2024-04-16 01:05:21.000000 tsugu-0.4.8/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:05:33.777291 tsugu-0.4.8/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 01:05:33.000000 tsugu-0.4.8/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 01:13:20.000000 tsugu-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:13:29.890428 tsugu-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 01:13:20.000000 tsugu-0.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:13:29.890428 tsugu-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 01:13:20.000000 tsugu-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 01:13:20.000000 tsugu-0.4.9/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21225 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.8/LICENSE` & `tsugu-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/PKG-INFO` & `tsugu-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.8
+Version: 0.4.9
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.8 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.9 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.8/README.md` & `tsugu-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/setup.py` & `tsugu-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.8',
+    version='0.4.9',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.8/test/test_main.py` & `tsugu-0.4.9/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/tsugu/bot.py` & `tsugu-0.4.9/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/tsugu/config.py` & `tsugu-0.4.9/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/tsugu/router.py` & `tsugu-0.4.9/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.8/tsugu/utils.py` & `tsugu-0.4.9/tsugu/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import random
 import urllib3
 from urllib3.exceptions import HTTPError
 
 from .config import config
 
 
+urllib3.disable_warnings()
+
+
 class DatabaseManager:
     def __init__(self, path):
         self.path = path
         self.conn = None
         self.cursor = None
         self.init_db(self.path)
```

### Comparing `tsugu-0.4.8/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.9/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.8
+Version: 0.4.9
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.8 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.9 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

