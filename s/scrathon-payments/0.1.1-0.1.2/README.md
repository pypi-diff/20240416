# Comparing `tmp/scrathon_payments-0.1.1.tar.gz` & `tmp/scrathon_payments-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.1.1.tar", last modified: Sun Apr 14 15:21:10 2024, max compression
+gzip compressed data, was "scrathon_payments-0.1.2.tar", last modified: Tue Apr 16 08:10:24 2024, max compression
```

## Comparing `scrathon_payments-0.1.1.tar` & `scrathon_payments-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:21:10.033915 scrathon_payments-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 15:21:03.000000 scrathon_payments-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-14 15:21:10.033915 scrathon_payments-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 15:21:03.000000 scrathon_payments-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:21:10.033915 scrathon_payments-0.1.1/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 15:21:03.000000 scrathon_payments-0.1.1/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:21:10.033915 scrathon_payments-0.1.1/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-14 15:21:10.000000 scrathon_payments-0.1.1/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-14 15:21:10.000000 scrathon_payments-0.1.1/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:21:10.000000 scrathon_payments-0.1.1/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 15:21:10.000000 scrathon_payments-0.1.1/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-14 15:21:10.000000 scrathon_payments-0.1.1/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:21:10.033915 scrathon_payments-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-14 15:21:03.000000 scrathon_payments-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:10:24.331348 scrathon_payments-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-16 08:10:18.000000 scrathon_payments-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-16 08:10:24.331348 scrathon_payments-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 08:10:18.000000 scrathon_payments-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:10:24.331348 scrathon_payments-0.1.2/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-16 08:10:18.000000 scrathon_payments-0.1.2/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:10:24.331348 scrathon_payments-0.1.2/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-16 08:10:24.000000 scrathon_payments-0.1.2/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 08:10:24.000000 scrathon_payments-0.1.2/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:10:24.000000 scrathon_payments-0.1.2/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 08:10:24.000000 scrathon_payments-0.1.2/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-16 08:10:24.000000 scrathon_payments-0.1.2/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:10:24.331348 scrathon_payments-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-16 08:10:18.000000 scrathon_payments-0.1.2/setup.py
```

### Comparing `scrathon_payments-0.1.1/LICENSE` & `scrathon_payments-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.1.1/PKG-INFO` & `scrathon_payments-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.1.1
+Version: 0.1.2
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.1.1/ScrathonPayments/__init__.py` & `scrathon_payments-0.1.2/ScrathonPayments/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-import json
-import re
+import scratchattach as scratch3
 import requests
 
-
 class Scrathon():
 
     def __init__(self, username):
-        self.username = str(username)
+        self.username = "None"
+        try:
+            scratch3.get_user(username)
+            userexists = True
+        except scratch3.exceptions.UserNotFound:
+            userexists = False
+        if userexists:
+            if requests.post("https://scrathon.justablock.online:1111/userexist/", json={"username": username}).json == {"userexist": "True"}:
+                self.username = str(username)
+            else:
+                print("User {} did not use Scrathon before!".format(username))
+        else:
+            print("User {} does not exist on scratch!".format(username))
 
-        print("Started Scrathon as {}! All funds earned will go to mentioned user".format(username))
+        if self.username != "None":
+            print("Started Scrathon as {}! All funds earned will go to mentioned user".format(self.username))
 
     def purchase(self, price, user):
-        request = requests.post("https://scrathon.justablock.online/transaction", json={
+        request = requests.post("https://scrathon.justablock.online:1111/transaction", json={
             "price": price,
             "buyer": user,
             "seller": self.username
         })
 
         return request.content
     
     def purchasecheck(self, price, user):
-        request = requests.post("https://scrathon.justablock.online/checkpurchase", json={
+        request = requests.post("https://scrathon.justablock.online:1111/checkpurchase", json={
             "price": price,
             "buyer": user,
             "seller": self.username
         })
 
         return request.content
```

### Comparing `scrathon_payments-0.1.1/scrathon_payments.egg-info/PKG-INFO` & `scrathon_payments-0.1.2/scrathon_payments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.1.1
+Version: 0.1.2
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.1.1/setup.py` & `scrathon_payments-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.1.1',
+    version='0.1.2',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```

