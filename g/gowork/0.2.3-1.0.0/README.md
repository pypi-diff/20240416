# Comparing `tmp/gowork-0.2.3.tar.gz` & `tmp/gowork-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gowork-0.2.3.tar", last modified: Thu May 18 17:00:29 2023, max compression
+gzip compressed data, was "gowork-1.0.0.tar", last modified: Tue Apr 16 20:15:06 2024, max compression
```

## Comparing `gowork-0.2.3.tar` & `gowork-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 17:00:29.822595 gowork-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-18 17:00:18.000000 gowork-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork/safe/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-18 17:00:18.000000 gowork-0.2.3/gowork/safe/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:00:29.822595 gowork-0.2.3/gowork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 17:00:29.000000 gowork-0.2.3/gowork.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:00:29.822595 gowork-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-18 17:00:18.000000 gowork-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 20:15:05.996420 gowork-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-16 20:14:54.000000 gowork-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork/safe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-16 20:14:54.000000 gowork-1.0.0/gowork/safe/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:15:05.996420 gowork-1.0.0/gowork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 20:15:05.000000 gowork-1.0.0/gowork.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:15:05.996420 gowork-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-16 20:14:54.000000 gowork-1.0.0/setup.py
```

### Comparing `gowork-0.2.3/README.rst` & `gowork-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `gowork-0.2.3/gowork/databases.py` & `gowork-1.0.0/gowork/databases.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from sqlalchemy import create_engine
 import pandas as pd
 import glob
 import pathlib
 import base64
 import platform
 
+
 class AthenaGo:
     def __init__(self, name_connection: str):
         self.__decode(name_connection)
         self.__con = connect(aws_access_key_id=self.__cred['aws_access_key_id'],
                              aws_secret_access_key=self.__cred['aws_secret_access_key'],
                              s3_staging_dir=self.__cred['s3_staging_dir'],
                              region_name=self.__cred['region_name'])
```

### Comparing `gowork-0.2.3/gowork/handler.py` & `gowork-1.0.0/gowork/handler.py`

 * *Files identical despite different names*

### Comparing `gowork-0.2.3/gowork/monitor.py` & `gowork-1.0.0/gowork/monitor.py`

 * *Files identical despite different names*

### Comparing `gowork-0.2.3/gowork/safe/configs.py` & `gowork-1.0.0/gowork/safe/configs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,57 @@
 import gowork
 import json
 import os
 import base64
 import platform
+import pathlib
+
 
 class Credentials:
     def __init__(self):
         self.__platform = '\\' if platform.system().__str__() == 'Windows' else '/'
         self.__root = self.__platform.join(gowork.__file__.split(self.__platform)[:-1] + ['safe', 'secret_keys.json'])
         self.__creds = {}
+        self.__project = pathlib.Path().resolve().__str__()
 
     def insert(self, name: str, connector: str, credentials: dict, encode=[]):
         name = name.lower()
         connector = connector.lower()
 
         self.__load()
         if connector not in self.__creds.keys():
             self.__creds[connector] = {}
         if len(encode) > 0:
             credentials = self.__encode(credentials, encode)
         self.__creds[connector][name] = credentials
         with open(self.__root, 'w', encoding='utf-8') as file:
             file.write(json.dumps(self.__creds, indent=4))
 
+    def export_credentials(self):
+        try:
+            os.popen(f'cp {self.__root} {self.__project + self.__platform + "gowork_secret_keys.json"}')
+            print('Exported successfully')
+        except:
+            print('Exported failed')
+
+    def import_credentials(self, path='.'):
+        try:
+            os.popen(f'cp {self.__project + self.__platform + path + self.__platform + "gowork_secret_keys.json"} {self.__root}')
+            print('Imported successfully')
+        except:
+            print('File not found')
+
+    def get_credentials(self) -> dict:
+        self.__load()
+        creds = {}
+        for k in self.__creds.keys():
+            for sk in self.__creds[k].keys():
+                creds[k] = sk
+        return creds
+
     def select(self, connector: str, name: str):
         name = name.lower()
         connector = connector.lower()
 
         self.__load()
         if connector in self.__creds:
             if name in self.__creds[connector]:
```

### Comparing `gowork-0.2.3/setup.py` & `gowork-1.0.0/setup.py`

 * *Files identical despite different names*

