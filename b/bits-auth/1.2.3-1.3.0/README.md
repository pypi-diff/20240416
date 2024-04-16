# Comparing `tmp/bits-auth-1.2.3.tar.gz` & `tmp/bits_auth-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bits-auth-1.2.3.tar", last modified: Fri Jun  9 16:04:21 2023, max compression
+gzip compressed data, was "bits_auth-1.3.0.tar", max compression
```

## Comparing `bits-auth-1.2.3.tar` & `bits_auth-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,5 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.170493 bits-auth-1.2.3/
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-09 16:04:21.171929 bits-auth-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2019-07-08 19:13:08.000000 bits-auth-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.099113 bits-auth-1.2.3/bits/
--rw-r--r--   0 root         (0) root         (0)       89 2021-03-19 15:15:17.000000 bits-auth-1.2.3/bits/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.107076 bits-auth-1.2.3/bits/auth/
--rw-r--r--   0 root         (0) root         (0)    40416 2023-06-09 15:51:37.000000 bits-auth-1.2.3/bits/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 16:04:21.162705 bits-auth-1.2.3/bits_auth.egg-info/
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 15:58:54.000000 bits-auth-1.2.3/bits_auth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-09 16:04:21.000000 bits-auth-1.2.3/bits_auth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-09 16:04:21.177522 bits-auth-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-09 15:52:26.000000 bits-auth-1.2.3/setup.py
+-rw-r--r--   0        0        0       38 2024-04-16 17:52:32.183587 bits_auth-1.3.0/README.md
+-rw-r--r--   0        0        0       65 2024-04-16 17:52:32.183587 bits_auth-1.3.0/bits/__init__.py
+-rw-r--r--   0        0        0    40788 2024-04-16 17:52:32.183587 bits_auth-1.3.0/bits/auth/__init__.py
+-rw-r--r--   0        0        0     1096 2024-04-16 17:52:32.183587 bits_auth-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 bits_auth-1.3.0/PKG-INFO
```

### Comparing `bits-auth-1.2.3/bits/auth/__init__.py` & `bits_auth-1.3.0/bits/auth/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# -*- coding: utf-8 -*-
 """Auth class file."""
 import os
 import sys
 
 from bits.secrets import Secrets
 
 # import bits-api-python-client
 mypath = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(mypath, "bits-api-python-client"))
 
 # pylama: ignore=E402
 
 
-class Auth(object):
+class Auth:
     """Auth class."""
 
     def __init__(self, settings, verbose=False, yes=False):
         """Initialize an Auth class instance."""
         self.settings = settings
         self.verbose = verbose
         self.yes = yes
 
         self.smproject = 'broad-bits-vault'
         self.secrets = Secrets(default_project=self.smproject)
 
-    def accounts(
+    def accounts(  # noqa: PLR0913
             self,
             ad=None,
             google=None,
             mongo=None,
             nis=None,
             people=None,
             slack=None,
@@ -302,15 +301,15 @@
         from bits.cloudaccounts import CloudAccounts
         return CloudAccounts(self.google())
 
     def ccure(self):
         """Connect to CCURE DB."""
         from bitsapiclient.services.ccure import CCURE
         params = self.secrets.resolve({
-            'server': '%s:%s' % (
+            'server': '{}:{}'.format(
                 self.settings['mssql_servers']['ccure']['db_host'],
                 self.settings['mssql_servers']['ccure']['db_port'],
             ),
             'user': self.settings['mssql_servers']['ccure']['db_user'],
             'password': self.settings['mssql_servers']['ccure']['db_pass'],
             'database': self.settings['mssql_servers']['ccure']['db'],
             'credentials_file': self.settings['ccure']['credentials'],
@@ -322,15 +321,15 @@
         })
         return CCURE(**params)
 
     def ccure_dev(self):
         """Connect to CCURE dev DB."""
         from bitsapiclient.services.ccure import CCURE
         params = self.secrets.resolve({
-            'server': '%s:%s' % (
+            'server': '{}:{}'.format(
                 self.settings['mssql_servers']['ccure_dev']['db_host'],
                 self.settings['mssql_servers']['ccure_dev']['db_port'],
             ),
             'user': self.settings['mssql_servers']['ccure_dev']['db_user'],
             'password': self.settings['mssql_servers']['ccure_dev']['db_pass'],
             'database': self.settings['mssql_servers']['ccure_dev']['db'],
             'credentials_file': self.settings['ccure_dev']['credentials'],
@@ -342,15 +341,15 @@
         })
         return CCURE(**params)
 
     def ccure_prod(self):
         """Connect to CCURE prod DB."""
         from bitsapiclient.services.ccure import CCURE
         params = self.secrets.resolve({
-            'server': '%s:%s' % (
+            'server': '{}:{}'.format(
                 self.settings['mssql_servers']['ccure_prod']['db_host'],
                 self.settings['mssql_servers']['ccure_prod']['db_port'],
             ),
             'user': self.settings['mssql_servers']['ccure_prod']['db_user'],
             'password': self.settings['mssql_servers']['ccure_prod']['db_pass'],
             'database': self.settings['mssql_servers']['ccure_prod']['db'],
             'credentials_file': self.settings['ccure_prod']['credentials'],
@@ -681,14 +680,25 @@
             'mongo_uri': self.settings['mongo']['bitsdb_prod']['uri'],
             'mongo_db': self.settings['mongo']['bitsdb_prod']['db'],
             'auth': self,
             'verbose': self.verbose,
         })
         return Mongo(**params)
 
+    def mongo_bitsdb(self):
+        """Connect to BITSdb Mongo DB."""
+        from bits.mongo import Mongo
+        params = self.secrets.resolve({
+            'uri': self.settings['mongo']['bitsdb']['uri'],
+            'db': self.settings['mongo']['bitsdb']['db'],
+            'auth': self,
+            'verbose': self.verbose,
+        })
+        return Mongo(**params)
+
     def mx(self):
         """Return an MX instance."""
         from bits.mx import MX
         params = self.secrets.resolve({
             'aliases_puppetdir': self.settings['mx']['aliases_puppetdir'],
             'transports_puppetdir': self.settings['mx']['transports_puppetdir'],
             'extension': self.settings['mx']['extension'],
@@ -819,15 +829,15 @@
         })
         return RequestTracker(**params)
 
     def sap(self):
         """Connect to SAP DB."""
         from bitsapiclient.services.sap import SAP
         params = self.secrets.resolve({
-            'server': '%s:%s' % (
+            'server': '{}:{}'.format(
                 self.settings['mssql_servers']['sap']['db_host'],
                 self.settings['mssql_servers']['sap']['db_port'],
             ),
             'user': self.settings['mssql_servers']['sap']['db_user'],
             'password': self.settings['mssql_servers']['sap']['db_pass'],
             'db': self.settings['mssql_servers']['sap']['db'],
             'verbose': self.verbose,
```

