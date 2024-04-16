# Comparing `tmp/wbx_workspaces-1.0.1.tar.gz` & `tmp/wbx_workspaces-1.1.1.tar.gz`

## Comparing `wbx_workspaces-1.0.1.tar` & `wbx_workspaces-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/src/wbx_workspaces/__init__.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/src/wbx_workspaces/__main__.py
--rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/src/wbx_workspaces/wbx.py
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/src/wbx_workspaces/wbx_dataframe.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/src/wbx_workspaces/wbx_utils.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/LICENSE
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 wbx_workspaces-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/__init__.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/__main__.py
+-rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_dataframe.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/src/wbx_workspaces/wbx_utils.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/LICENSE
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/README.md
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 wbx_workspaces-1.1.1/PKG-INFO
```

### Comparing `wbx_workspaces-1.0.1/src/wbx_workspaces/__main__.py` & `wbx_workspaces-1.1.1/src/wbx_workspaces/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,44 +17,29 @@
 
 ut=wbx_utils.UtilsTrc()
 wbxr=wbx.WbxRequest()
 
 # import variables in .env 
 # load_dotenv(os.getcwd() + "/.env")
 
-WBX_SCOPES = "spark-admin:workspaces_read spark-admin:devices_read workspace_metrics_read"
+WBX_SCOPES = "spark-admin:workspaces_read spark-admin:devices_read spark-admin:workspace_metrics_read"
 
 __version__ = my_name = "N/A"
 try:
     __version__ = importlib.metadata.version(__package__)
     my_name = __package__
 except:
     print("Local run")
 
 logging.basicConfig()
 
 ###################
-### UTILS functions 
+### Workspaces ### 
 ###################
 
-# print items array fields listed in 'il' 
-#
-def print_items(il, items):
-    for i in il:
-        print(i,",", end='', sep='')
-    print ("")        
-    for item in items:
-        for i in il:
-            try:
-                v=item[i]
-            except KeyError:
-                v=""
-            print (v, ",", end='', sep='')
-        print ("")
-
 @click.command()
 @click.option('-c', '--csvfile', help='Save results to CSV file.')
 @click.option('-r', '--rawdata', is_flag=True, help='Show json raw data')
 def locations(csvfile, rawdata):
     """ List locations IDs"""
     # get data   
     #
@@ -73,44 +58,68 @@
     #
     workspacesDF=wbxdf.workspacesDF(location_id)
     workspacesDF.print(csvfile)        
     if (rawdata):
         pprint(workspacesDF.jsonList)
 
 @click.command()
+@click.option('-l', '--location_id', help='Restrict list to location Id')
+@click.option('-c', '--csvfile', help='Save results to CSV file.')
+def devices(csvfile, location_id):
+    """ Get the list of devices in given location """
+    # get data   
+    #
+    devicesDF=wbxdf.devicesDF(location_id)
+    devicesDF.print(csvfile)        
+
+@click.command()
+@click.argument('device_id')
+@click.argument('name')
+def device_status(device_id, name):
+    """ Show device status """
+    # get data   
+    #
+    data=wbxr.get_wbx_data(f"xapi/status", f"?deviceId={device_id}&name={name}")
+    pprint(data)        
+
+def print_metrics(workspace_id, metric, fmt):
+    metricDF=wbxdf.metricsDF(workspace_id, metric)
+    metricDF.print(fmt)
+
+@click.command()
 @click.argument('metric')
 @click.option('-l', '--location_id', help='Get metrics data for all workspaces under location ID')
 @click.option('-w', '--workspace_id', help='Get metrics data for specific workspace ID')
-def metrics(metric, location_id="", workspace_id=""):
-    """ Gather yesterday's hourly peopleCount or timeUsed metric for a workspace or workspaces in a location"""
+@click.option('-f', '--fmt', help='Save to CSV or JSON file.')
+def metrics(metric, fmt, location_id="", workspace_id=""):
+    """ Gather yesteray's hourly peopleCount or timeUsed metric for a workspace or workspaces in a location"""
 
     if ( not (location_id or workspace_id) ):
+
         print ( "I need a location or a workspace ID")
         return (400)
     
     match metric:
         case 'peopleCount':
             pass
         case 'timeUsed':
             pass
         case _ :
             print(f"{metric} value not supported")
             return(400)
         
     if (workspace_id):
-        metricDF=wbxdf.metricsDF(workspace_id, metric)
-        metricDF.write_to_file()
+        print_metrics( workspace_id, metric, fmt )
 
     elif (location_id):
         workspacesDF=wbxdf.workspacesDF(location_id)
         workspace_items=workspacesDF.jsonList['items']
         for workspace in workspace_items :
             workspace_id = workspace['id']
-            metricDF=wbxdf.metricsDF(workspace_id, metric)
-            metricDF.write_to_file()
+            print_metrics( workspace_id, metric, fmt )
     
 #####################
 ### Top Lev       ###
 #####################
 
 @click.group()
 @click.version_option(__version__)
@@ -132,10 +141,12 @@
         else:
             sys.exit('No access token set. Use option -t or AUTH_BEARER env variable')
 
 
 cli.add_command(metrics)
 cli.add_command(locations)
 cli.add_command(workspaces)
+cli.add_command(devices)
+cli.add_command(device_status)
 
 if __name__ == '__main__':
     cli()
```

### Comparing `wbx_workspaces-1.0.1/src/wbx_workspaces/wbx.py` & `wbx_workspaces-1.1.1/src/wbx_workspaces/wbx.py`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.0.1/LICENSE` & `wbx_workspaces-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.0.1/README.md` & `wbx_workspaces-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wbx_workspaces-1.0.1/pyproject.toml` & `wbx_workspaces-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wbx-workspaces"
-version = "1.0.1"
+version = "1.1.1"
 description = "Commands to download Webex Workspaces stats"
 readme = "README.md"
 authors = [{ name = "Stephane Cohen", email = "stecohen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `wbx_workspaces-1.0.1/PKG-INFO` & `wbx_workspaces-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wbx-workspaces
-Version: 1.0.1
+Version: 1.1.1
 Summary: Commands to download Webex Workspaces stats
 Author-email: Stephane Cohen <stecohen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Stephane Cohen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

