# Comparing `tmp/embixtools-1.1.3.tar.gz` & `tmp/embixtools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embixtools-1.1.3.tar", last modified: Wed Nov 29 09:54:47 2023, max compression
+gzip compressed data, was "embixtools-1.1.4.tar", last modified: Tue Apr 16 14:18:53 2024, max compression
```

## Comparing `embixtools-1.1.3.tar` & `embixtools-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2023-11-29 09:54:47.467070 embixtools-1.1.3/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2023-11-29 09:54:47.467070 embixtools-1.1.3/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)       79 2023-03-31 12:52:32.000000 embixtools-1.1.3/README.md
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2023-11-29 09:54:47.467070 embixtools-1.1.3/embixtools/
--rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.3/embixtools/dataquality.py
--rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.3/embixtools/errors.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/logs.py
--rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/main.py
--rw-r--r--   0 embix     (1000) embix     (1000)     4958 2023-11-29 09:53:19.000000 embixtools-1.1.3/embixtools/opinum_client.py
--rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/retry.py
--rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/schedule.py
--rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/vpn.py
--rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.3/embixtools/yaml_read.py
-drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2023-11-29 09:54:47.467070 embixtools-1.1.3/embixtools.egg-info/
--rw-r--r--   0 embix     (1000) embix     (1000)      188 2023-11-29 09:54:47.000000 embixtools-1.1.3/embixtools.egg-info/PKG-INFO
--rw-r--r--   0 embix     (1000) embix     (1000)      385 2023-11-29 09:54:47.000000 embixtools-1.1.3/embixtools.egg-info/SOURCES.txt
--rw-r--r--   0 embix     (1000) embix     (1000)        1 2023-11-29 09:54:47.000000 embixtools-1.1.3/embixtools.egg-info/dependency_links.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       48 2023-11-29 09:54:47.000000 embixtools-1.1.3/embixtools.egg-info/requires.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       11 2023-11-29 09:54:47.000000 embixtools-1.1.3/embixtools.egg-info/top_level.txt
--rw-r--r--   0 embix     (1000) embix     (1000)       38 2023-11-29 09:54:47.467070 embixtools-1.1.3/setup.cfg
--rw-r--r--   0 embix     (1000) embix     (1000)      287 2023-11-29 09:53:51.000000 embixtools-1.1.3/setup.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 14:18:53.429198 embixtools-1.1.4/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)       79 2023-03-31 12:52:32.000000 embixtools-1.1.4/README.md
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/embixtools/
+-rw-r--r--   0 embix     (1000) embix     (1000)        0 2023-03-31 13:01:53.000000 embixtools-1.1.4/embixtools/dataquality.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      324 2023-04-25 15:20:36.000000 embixtools-1.1.4/embixtools/errors.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1075 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/logs.py
+-rw-r--r--   0 embix     (1000) embix     (1000)       33 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/main.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     5859 2024-04-16 14:09:28.000000 embixtools-1.1.4/embixtools/opinum_client.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     1555 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/retry.py
+-rw-r--r--   0 embix     (1000) embix     (1000)     3172 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/schedule.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      990 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/vpn.py
+-rw-r--r--   0 embix     (1000) embix     (1000)      447 2022-11-08 14:28:52.000000 embixtools-1.1.4/embixtools/yaml_read.py
+drwxr-xr-x   0 embix     (1000) embix     (1000)        0 2024-04-16 14:18:53.429198 embixtools-1.1.4/embixtools.egg-info/
+-rw-r--r--   0 embix     (1000) embix     (1000)      188 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/PKG-INFO
+-rw-r--r--   0 embix     (1000) embix     (1000)      385 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)        1 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       48 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/requires.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       11 2024-04-16 14:18:53.000000 embixtools-1.1.4/embixtools.egg-info/top_level.txt
+-rw-r--r--   0 embix     (1000) embix     (1000)       38 2024-04-16 14:18:53.429198 embixtools-1.1.4/setup.cfg
+-rw-r--r--   0 embix     (1000) embix     (1000)      287 2024-04-16 14:10:12.000000 embixtools-1.1.4/setup.py
```

### Comparing `embixtools-1.1.3/embixtools/logs.py` & `embixtools-1.1.4/embixtools/logs.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.3/embixtools/opinum_client.py` & `embixtools-1.1.4/embixtools/opinum_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,25 +30,21 @@
     def variables(self):
         return self.request('GET','variables').json()
 
     @property
     def timeseries(self):
         sources = self.sources
         variables = self.variables
-        return [
-            {
-                'id': variable['id'],
-                'site': source['siteName'],
-                'source': source['name'],
-                'name': variable['name'],
-            }
+        return {
+            variable['id']: ( source['siteName'], source['name'], variable['name'] )
             for source in sources
-            for variable in variables if variable['sourceId'] == source['id']
-        ]
-
+            for variable in variables
+            if variable['sourceId'] == source['id']
+        }
+        
     def auth(self):
         oauth = OAuth2Session(
             client = LegacyApplicationClient(client_id=self.client_id)
         )
         token = oauth.fetch_token(
             token_url = 'https://identity.opinum.com/connect/token',
             scope = 'opisense-api push-data',
@@ -62,20 +58,32 @@
         self.token_expiration = dt.utcnow() + td(seconds=60)
         oauth.close()
         return self.token
     
     def var(self, site, source, variable):
         try:
             return [
-                ts['id'] for ts in self.timeseries 
-                if all((ts['site'] == site, ts['source'] == source, ts['name'] == variable))
+                i for i, ts in self.timeseries.items() 
+                if ts == (site, source, variable)
             ][0]
         except:
             return -1
 
+    def vars(self, var_ids):
+        tss = self.timeseries
+        try:
+            ids = []
+            for ssi1 in var_ids:
+                for i, ssi2 in tss.items():
+                    if ssi1 == ssi2:
+                        ids += [i]
+            return ids
+        except:
+            return []
+
     def token_required(func):
         @wraps(func)
         def wrapper(self, *args, **kwargs):
             if dt.utcnow() > self.token_expiration:
                 self.auth()
             return func(self, *args, **kwargs)
         return wrapper
@@ -142,8 +150,29 @@
     @token_required
     def push_ts(self, site, source, variable, dps=None):
         try: 
             data = pd.DataFrame({ "date": dps.index.values, "value": dps.values })
             data["date"] = data["date"].dt.strftime(iso)
             data = data.to_dict(orient="records")
             return self.push_dps(site, source, variable=variable, dps=data)
-        except: return
+        except: return
+
+    @token_required
+    def delete(self, vars_ssi, interval=None, confirm=False):
+        vars_ids = self.vars(vars_ssi)
+        tss = self.timeseries
+        params = {
+            "variableIds": vars_ids,
+            "whatIf": (not confirm)
+        }
+        if not interval is None:
+            params["fromDateUtc"] = interval[0].strftime(iso)
+            params["toDateUtc"] = interval[1].strftime(iso)
+        resp = self.request("DELETE", "/data", params)
+        if confirm:
+            for v in resp.json()["results"]:
+                i = v["variableId"]
+                logging.info(f"""Opinum Datahub : deleting {v["datapointCount"]} datapoints from {tss[i]} ...""")
+        return resp.json()
+            
+
+
```

### Comparing `embixtools-1.1.3/embixtools/retry.py` & `embixtools-1.1.4/embixtools/retry.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.3/embixtools/schedule.py` & `embixtools-1.1.4/embixtools/schedule.py`

 * *Files identical despite different names*

### Comparing `embixtools-1.1.3/embixtools/vpn.py` & `embixtools-1.1.4/embixtools/vpn.py`

 * *Files identical despite different names*

