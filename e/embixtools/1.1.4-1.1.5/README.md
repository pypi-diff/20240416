# Comparing `tmp/embixtools-1.1.4.tar.gz` & `tmp/embixtools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embixtools-1.1.4.tar", last modified: Tue Apr 16 14:18:53 2024, max compression
+gzip compressed data, was "embixtools-1.1.5.tar", last modified: Tue Apr 16 15:37:44 2024, max compression
```

## Comparing `embixtools-1.1.4.tar` & `embixtools-1.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 14:18:53.429198 embixtools-1.1.4/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)       79 2023-03-31 12:52:32.000000 embixtools-1.1.4/README.md
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/embixtools/
--rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.4/embixtools/dataquality.py
--rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.4/embixtools/errors.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/logs.py
--rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/main.py
--rw-r--r--   0 embix     (1000) embix     (1000)     5859 2024-04-16 14:09:28.000000 embixtools-1.1.4/embixtools/opinum_client.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/retry.py
--rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/schedule.py
--rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/vpn.py
--rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/yaml_read.py
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/embixtools.egg-info/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)      385 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/SOURCES.txt
--rw-r--r--   0 embix     (1000) embix     (1000)        1 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/dependency_links.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       48 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/requires.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       11 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/top_level.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       38 2024-04-16 14:18:53.429198 embixtools-1.1.4/setup.cfg
--rw-r--r--   0 embix     (1000) embix     (1000)      287 2024-04-16 14:10:12.000000 embixtools-1.1.4/setup.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:37:44.489198 embixtools-1.1.5/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)      272 2024-04-16 14:20:50.000000 embixtools-1.1.5/README.md
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/embixtools/
+-rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.5/embixtools/dataquality.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.5/embixtools/errors.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/logs.py
+-rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/main.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     7473 2024-04-16 15:37:16.000000 embixtools-1.1.5/embixtools/opinum_client.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/retry.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/schedule.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/vpn.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/yaml_read.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/embixtools.egg-info/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)      385 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)        1 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       48 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/requires.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       11 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/top_level.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       38 2024-04-16 15:37:44.489198 embixtools-1.1.5/setup.cfg
+-rw-r--r--   0 embix     (1000) embix     (1000)      287 2024-04-16 15:37:34.000000 embixtools-1.1.5/setup.py
```

### Comparing `embixtools-1.1.4/embixtools/logs.py` & `embixtools-1.1.5/embixtools/logs.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.4/embixtools/opinum_client.py` & `embixtools-1.1.5/embixtools/opinum_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 from oauthlib.oauth2 import LegacyApplicationClient
 from requests_oauthlib import OAuth2Session
 from functools import wraps
 from datetime import datetime as dt, timedelta as td
 import logging
 import pandas as pd
+import re
 
 iso = "%Y-%m-%dT%H:%M:%S"
 
 class Opinum(object):
     
     def __init__(self, usr, pwd, client_id, client_secret):
         self.username = usr
@@ -169,10 +170,56 @@
             params["toDateUtc"] = interval[1].strftime(iso)
         resp = self.request("DELETE", "/data", params)
         if confirm:
             for v in resp.json()["results"]:
                 i = v["variableId"]
                 logging.info(f"""Opinum Datahub : deleting {v["datapointCount"]} datapoints from {tss[i]} ...""")
         return resp.json()
-            
-
-    
+    
+    def create_variable(self, site, source, variable, unit=None, granularity=None, quantity_type=None, calculated=False):
+        if unit is None: 
+            unit_id = 0
+        else:
+            unit_id = {
+                "W": 1,
+                "VA": 2,
+                "kW": 4,
+                "Wh": 7,
+                "kWh": 8,
+                "L": 18,
+                "m3": 19,
+                "°C": 28,
+                "%": 31,
+                "kVA": 39,
+                "€": 48,
+                "Wh/m2": 50,
+                "€/MWh": 57,
+                "tCO2": 61,
+                "kgCO2": 62,
+                "kWh/m2": 68,
+            }[unit]
+        if granularity is None: 
+            granularity = 0
+        else:
+            res = re.search("([0-9]+)([YmdHT])", granularity)
+            granularity_value = res.group(1)
+            granularity_timebase = {
+                "T": 2,
+                "H": 3,
+                "d": 4,
+                "m": 5,
+                "Y": 6,
+            }[res.group(2)]
+        if quantity_type is None: 
+            quantity_type = "Instantaneous"
+        source_id = [s["id"] for s in self.sources if (s["siteName"]==site and s["name"]==source)][0]
+        payload = {
+            "name": variable,
+            "unitId": unit_id,
+            "granularity": granularity_value,
+            "granularityTimeBase": granularity_timebase,
+            "quantityType": quantity_type,
+        }
+        if calculated: 
+            payload["calculated"] = {}
+        resp = self.request("POST", f"""/variables/source/{source_id}""", payload)
+        return resp.json()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `embixtools-1.1.4/embixtools/retry.py` & `embixtools-1.1.5/embixtools/retry.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.4/embixtools/schedule.py` & `embixtools-1.1.5/embixtools/schedule.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.4/embixtools/vpn.py` & `embixtools-1.1.5/embixtools/vpn.py`

 * *Files identical despite different names*

