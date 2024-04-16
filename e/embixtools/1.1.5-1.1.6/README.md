# Comparing `tmp/embixtools-1.1.5.tar.gz` & `tmp/embixtools-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embixtools-1.1.5.tar", last modified: Tue Apr 16 15:37:44 2024, max compression
+gzip compressed data, was "embixtools-1.1.6.tar", last modified: Tue Apr 16 15:44:52 2024, max compression
```

## Comparing `embixtools-1.1.5.tar` & `embixtools-1.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:37:44.489198 embixtools-1.1.5/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)      272 2024-04-16 14:20:50.000000 embixtools-1.1.5/README.md
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/embixtools/
--rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.5/embixtools/dataquality.py
--rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.5/embixtools/errors.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/logs.py
--rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/main.py
--rw-r--r--   0 embix     (1000) embix     (1000)     7473 2024-04-16 15:37:16.000000 embixtools-1.1.5/embixtools/opinum_client.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/retry.py
--rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/schedule.py
--rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/vpn.py
--rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.5/embixtools/yaml_read.py
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:37:44.489198 embixtools-1.1.5/embixtools.egg-info/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)      385 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/SOURCES.txt
--rw-r--r--   0 embix     (1000) embix     (1000)        1 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/dependency_links.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       48 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/requires.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       11 2024-04-16 15:37:44.000000 embixtools-1.1.5/embixtools.egg-info/top_level.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       38 2024-04-16 15:37:44.489198 embixtools-1.1.5/setup.cfg
--rw-r--r--   0 embix     (1000) embix     (1000)      287 2024-04-16 15:37:34.000000 embixtools-1.1.5/setup.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:44:52.899198 embixtools-1.1.6/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:44:52.899198 embixtools-1.1.6/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)      272 2024-04-16 14:20:50.000000 embixtools-1.1.6/README.md
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:44:52.899198 embixtools-1.1.6/embixtools/
+-rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.6/embixtools/dataquality.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.6/embixtools/errors.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/logs.py
+-rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/main.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     7535 2024-04-16 15:44:26.000000 embixtools-1.1.6/embixtools/opinum_client.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/retry.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/schedule.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/vpn.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.6/embixtools/yaml_read.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 15:44:52.899198 embixtools-1.1.6/embixtools.egg-info/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 15:44:52.000000 embixtools-1.1.6/embixtools.egg-info/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)      385 2024-04-16 15:44:52.000000 embixtools-1.1.6/embixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)        1 2024-04-16 15:44:52.000000 embixtools-1.1.6/embixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       48 2024-04-16 15:44:52.000000 embixtools-1.1.6/embixtools.egg-info/requires.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       11 2024-04-16 15:44:52.000000 embixtools-1.1.6/embixtools.egg-info/top_level.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       38 2024-04-16 15:44:52.899198 embixtools-1.1.6/setup.cfg
+-rw-r--r--   0 embix     (1000) embix     (1000)      287 2024-04-16 15:44:43.000000 embixtools-1.1.6/setup.py
```

### Comparing `embixtools-1.1.5/embixtools/logs.py` & `embixtools-1.1.6/embixtools/logs.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.5/embixtools/opinum_client.py` & `embixtools-1.1.6/embixtools/opinum_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return self.request('GET','variables').json()
 
     @property
     def timeseries(self):
         sources = self.sources
         variables = self.variables
         return {
-            variable['id']: ( source['siteName'], source['name'], variable['name'] )
+            variable['id']: { "site": source['siteName'], "source": source['name'], "variable": variable['name'] }
             for source in sources
             for variable in variables
             if variable['sourceId'] == source['id']
         }
         
     def auth(self):
         oauth = OAuth2Session(
@@ -60,26 +60,26 @@
         oauth.close()
         return self.token
     
     def var(self, site, source, variable):
         try:
             return [
                 i for i, ts in self.timeseries.items() 
-                if ts == (site, source, variable)
+                if tuple(ts.values()) == (site, source, variable)
             ][0]
         except:
             return -1
 
     def vars(self, var_ids):
         tss = self.timeseries
         try:
             ids = []
             for ssi1 in var_ids:
                 for i, ssi2 in tss.items():
-                    if ssi1 == ssi2:
+                    if ssi1 == tuple(ssi2.values()):
                         ids += [i]
             return ids
         except:
             return []
 
     def token_required(func):
         @wraps(func)
```

### Comparing `embixtools-1.1.5/embixtools/retry.py` & `embixtools-1.1.6/embixtools/retry.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.5/embixtools/schedule.py` & `embixtools-1.1.6/embixtools/schedule.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.5/embixtools/vpn.py` & `embixtools-1.1.6/embixtools/vpn.py`

 * *Files identical despite different names*

