# Comparing `tmp/nanorpc-0.1.2.tar.gz` & `tmp/nanorpc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanorpc-0.1.2.tar", last modified: Sun Mar 24 09:26:51 2024, max compression
+gzip compressed data, was "nanorpc-0.1.3.tar", last modified: Tue Apr 16 08:14:42 2024, max compression
```

## Comparing `nanorpc-0.1.2.tar` & `nanorpc-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-03-24 09:26:51.919826 nanorpc-0.1.2/
--rw-r--r--   0 bl         (501) staff       (20)     3351 2024-03-24 09:26:51.919525 nanorpc-0.1.2/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)     2656 2024-01-14 16:43:31.000000 nanorpc-0.1.2/README.md
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-03-24 09:26:51.917361 nanorpc-0.1.2/nanorpc/
--rw-r--r--   0 bl         (501) staff       (20)       22 2024-01-24 13:32:29.000000 nanorpc-0.1.2/nanorpc/__init__.py
--rw-r--r--   0 bl         (501) staff       (20)    15996 2024-03-13 13:59:44.000000 nanorpc-0.1.2/nanorpc/client.py
--rw-r--r--   0 bl         (501) staff       (20)     4780 2024-03-13 13:59:44.000000 nanorpc-0.1.2/nanorpc/client_dynamic.py
--rw-r--r--   0 bl         (501) staff       (20)    19798 2024-03-13 14:00:04.000000 nanorpc-0.1.2/nanorpc/client_extended.py
--rw-r--r--   0 bl         (501) staff       (20)     4895 2024-03-24 09:25:41.000000 nanorpc-0.1.2/nanorpc/client_nanoto.py
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-03-24 09:26:51.919057 nanorpc-0.1.2/nanorpc/versions/
--rw-r--r--   0 bl         (501) staff       (20)        0 2024-01-14 16:43:31.000000 nanorpc-0.1.2/nanorpc/versions/__init__.py
--rw-r--r--   0 bl         (501) staff       (20)     1052 2024-03-13 13:59:44.000000 nanorpc-0.1.2/nanorpc/versions/handler.py
--rw-r--r--   0 bl         (501) staff       (20)     3243 2024-03-24 09:23:19.000000 nanorpc-0.1.2/nanorpc/versions/nano_to.py
--rw-r--r--   0 bl         (501) staff       (20)    10916 2024-01-23 09:51:50.000000 nanorpc-0.1.2/nanorpc/versions/v23_3.py
--rw-r--r--   0 bl         (501) staff       (20)     3369 2024-01-23 09:27:50.000000 nanorpc-0.1.2/nanorpc/versions/v24_0.py
--rw-r--r--   0 bl         (501) staff       (20)      503 2024-01-16 20:44:38.000000 nanorpc-0.1.2/nanorpc/versions/v25_0.py
-drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-03-24 09:26:51.919252 nanorpc-0.1.2/nanorpc.egg-info/
--rw-r--r--   0 bl         (501) staff       (20)     3351 2024-03-24 09:26:51.000000 nanorpc-0.1.2/nanorpc.egg-info/PKG-INFO
--rw-r--r--   0 bl         (501) staff       (20)      451 2024-03-24 09:26:51.000000 nanorpc-0.1.2/nanorpc.egg-info/SOURCES.txt
--rw-r--r--   0 bl         (501) staff       (20)        1 2024-03-24 09:26:51.000000 nanorpc-0.1.2/nanorpc.egg-info/dependency_links.txt
--rw-r--r--   0 bl         (501) staff       (20)       16 2024-03-24 09:26:51.000000 nanorpc-0.1.2/nanorpc.egg-info/requires.txt
--rw-r--r--   0 bl         (501) staff       (20)        8 2024-03-24 09:26:51.000000 nanorpc-0.1.2/nanorpc.egg-info/top_level.txt
--rw-r--r--   0 bl         (501) staff       (20)       38 2024-03-24 09:26:51.919882 nanorpc-0.1.2/setup.cfg
--rw-r--r--   0 bl         (501) staff       (20)      925 2024-03-24 09:25:50.000000 nanorpc-0.1.2/setup.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-04-16 08:14:42.144331 nanorpc-0.1.3/
+-rw-r--r--   0 bl         (501) staff       (20)     3351 2024-04-16 08:14:42.144006 nanorpc-0.1.3/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)     2656 2024-01-14 16:43:31.000000 nanorpc-0.1.3/README.md
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-04-16 08:14:42.140898 nanorpc-0.1.3/nanorpc/
+-rw-r--r--   0 bl         (501) staff       (20)       22 2024-01-24 13:32:29.000000 nanorpc-0.1.3/nanorpc/__init__.py
+-rw-r--r--   0 bl         (501) staff       (20)    16090 2024-04-15 19:59:03.000000 nanorpc-0.1.3/nanorpc/client.py
+-rw-r--r--   0 bl         (501) staff       (20)     4780 2024-03-13 13:59:44.000000 nanorpc-0.1.3/nanorpc/client_dynamic.py
+-rw-r--r--   0 bl         (501) staff       (20)    19798 2024-03-13 14:00:04.000000 nanorpc-0.1.3/nanorpc/client_extended.py
+-rw-r--r--   0 bl         (501) staff       (20)     4895 2024-03-24 21:33:00.000000 nanorpc-0.1.3/nanorpc/client_nanoto.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-04-16 08:14:42.143445 nanorpc-0.1.3/nanorpc/versions/
+-rw-r--r--   0 bl         (501) staff       (20)        0 2024-01-14 16:43:31.000000 nanorpc-0.1.3/nanorpc/versions/__init__.py
+-rw-r--r--   0 bl         (501) staff       (20)     1052 2024-03-13 13:59:44.000000 nanorpc-0.1.3/nanorpc/versions/handler.py
+-rw-r--r--   0 bl         (501) staff       (20)     3243 2024-03-24 09:23:19.000000 nanorpc-0.1.3/nanorpc/versions/nano_to.py
+-rw-r--r--   0 bl         (501) staff       (20)    10946 2024-04-15 19:57:47.000000 nanorpc-0.1.3/nanorpc/versions/v23_3.py
+-rw-r--r--   0 bl         (501) staff       (20)     3369 2024-01-23 09:27:50.000000 nanorpc-0.1.3/nanorpc/versions/v24_0.py
+-rw-r--r--   0 bl         (501) staff       (20)      503 2024-01-16 20:44:38.000000 nanorpc-0.1.3/nanorpc/versions/v25_0.py
+drwxr-xr-x   0 bl         (501) staff       (20)        0 2024-04-16 08:14:42.143773 nanorpc-0.1.3/nanorpc.egg-info/
+-rw-r--r--   0 bl         (501) staff       (20)     3351 2024-04-16 08:14:42.000000 nanorpc-0.1.3/nanorpc.egg-info/PKG-INFO
+-rw-r--r--   0 bl         (501) staff       (20)      451 2024-04-16 08:14:42.000000 nanorpc-0.1.3/nanorpc.egg-info/SOURCES.txt
+-rw-r--r--   0 bl         (501) staff       (20)        1 2024-04-16 08:14:42.000000 nanorpc-0.1.3/nanorpc.egg-info/dependency_links.txt
+-rw-r--r--   0 bl         (501) staff       (20)       16 2024-04-16 08:14:42.000000 nanorpc-0.1.3/nanorpc.egg-info/requires.txt
+-rw-r--r--   0 bl         (501) staff       (20)        8 2024-04-16 08:14:42.000000 nanorpc-0.1.3/nanorpc.egg-info/top_level.txt
+-rw-r--r--   0 bl         (501) staff       (20)       38 2024-04-16 08:14:42.144374 nanorpc-0.1.3/setup.cfg
+-rw-r--r--   0 bl         (501) staff       (20)      925 2024-04-16 08:13:42.000000 nanorpc-0.1.3/setup.py
```

### Comparing `nanorpc-0.1.2/PKG-INFO` & `nanorpc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanorpc
-Version: 0.1.2
+Version: 0.1.3
 Summary: async nano rpc library with dynamic method generation per node version
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanorpc-0.1.2/README.md` & `nanorpc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/client.py` & `nanorpc-0.1.3/nanorpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 class NanoRpcTyped:
     def __init__(self, url, username=None, password=None, wrap_json=False):
         #
         self.rpc = NanoRpc(url=url, username=username,
                            password=password, node_version=NodeVersion.V25_1, wrap_json=wrap_json)
 
-    async def account_balance(self, account):
-        return await self.rpc.account_balance(account)
+    async def account_balance(self, account, include_only_confirmed=True):
+        return await self.rpc.account_balance(account, include_only_confirmed=include_only_confirmed)
 
     async def account_info(self, account, representative=None, weight=None, receivable=None, pending=None, include_confirmed=None):
         return await self.rpc.account_info(account, representative=representative, weight=weight, receivable=receivable, pending=pending, include_confirmed=include_confirmed)
 
     async def account_get(self, key):
         return await self.rpc.account_get(key)
 
@@ -268,16 +268,16 @@
 
     async def wallet_change_seed(self, wallet, seed, count=None):
         return await self.rpc.wallet_change_seed(wallet, seed, count=count)
 
     async def wallet_contains(self, wallet, account):
         return await self.rpc.wallet_contains(wallet, account)
 
-    async def wallet_create(self, ):
-        return await self.rpc.wallet_create()
+    async def wallet_create(self, seed=None):
+        return await self.rpc.wallet_create(seed=seed)
 
     async def wallet_destroy(self, wallet):
         return await self.rpc.wallet_destroy(wallet)
 
     async def wallet_export(self, wallet):
         return await self.rpc.wallet_export(wallet)
```

### Comparing `nanorpc-0.1.2/nanorpc/client_dynamic.py` & `nanorpc-0.1.3/nanorpc/client_dynamic.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/client_extended.py` & `nanorpc-0.1.3/nanorpc/client_extended.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/client_nanoto.py` & `nanorpc-0.1.3/nanorpc/client_nanoto.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/versions/handler.py` & `nanorpc-0.1.3/nanorpc/versions/handler.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/versions/nano_to.py` & `nanorpc-0.1.3/nanorpc/versions/nano_to.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc/versions/v23_3.py` & `nanorpc-0.1.3/nanorpc/versions/v23_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 COMMANDS = {
     "account_balance": {
         "required": ["account"],
-        "optional": []
+        "optional": ["include_only_confirmed"]
     },
     "account_info": {
         "required": ["account"],
         "optional":
         ["representative", "weight", "pending", "include_confirmed"]
     },
     "account_get": {
@@ -371,15 +371,15 @@
     },
     "wallet_contains": {
         "required": ["wallet", "account"],
         "optional": []
     },
     "wallet_create": {
         "required": [],
-        "optional": []
+        "optional": ["seed"]
     },
     "wallet_destroy": {
         "required": ["wallet"],
         "optional": []
     },
     "wallet_export": {
         "required": ["wallet"],
```

### Comparing `nanorpc-0.1.2/nanorpc/versions/v24_0.py` & `nanorpc-0.1.3/nanorpc/versions/v24_0.py`

 * *Files identical despite different names*

### Comparing `nanorpc-0.1.2/nanorpc.egg-info/PKG-INFO` & `nanorpc-0.1.3/nanorpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanorpc
-Version: 0.1.2
+Version: 0.1.3
 Summary: async nano rpc library with dynamic method generation per node version
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nanorpc-0.1.2/setup.py` & `nanorpc-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='nanorpc',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=['aiohttp', 'asyncio'],
     python_requires='>=3.7',
     author='gr0vity',
     url="https://github.com/gr0vity-dev/nanomock",
     description='async nano rpc library with dynamic method generation per node version',
     long_description=long_description,
```

