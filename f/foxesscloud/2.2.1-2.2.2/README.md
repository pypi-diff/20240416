# Comparing `tmp/foxesscloud-2.2.1.tar.gz` & `tmp/foxesscloud-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-rjjzde6s\foxesscloud-2.2.1.tar", last modified: Mon Apr 15 11:21:29 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-thxz69pi\foxesscloud-2.2.2.tar", last modified: Mon Apr 15 18:36:05 2024, max compression
```

## Comparing `foxesscloud-2.2.1.tar` & `foxesscloud-2.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.1/LICENCE
--rw-rw-rw-   0        0        0    39391 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    38836 2024-04-15 11:18:57.000000 foxesscloud-2.2.1/README.md
--rw-rw-rw-   0        0        0      635 2024-04-15 11:08:55.000000 foxesscloud-2.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud/
--rw-rw-rw-   0        0        0   175247 2024-04-15 11:11:43.000000 foxesscloud-2.2.1/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   169540 2024-04-15 11:11:43.000000 foxesscloud-2.2.1/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    39391 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 11:21:29.000000 foxesscloud-2.2.1/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.2/LICENCE
+-rw-rw-rw-   0        0        0    39478 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    38923 2024-04-15 18:27:39.000000 foxesscloud-2.2.2/README.md
+-rw-rw-rw-   0        0        0      635 2024-04-15 18:26:07.000000 foxesscloud-2.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud/
+-rw-rw-rw-   0        0        0   175401 2024-04-15 18:31:50.000000 foxesscloud-2.2.2/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   169694 2024-04-15 18:31:50.000000 foxesscloud-2.2.2/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    39478 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 18:36:05.000000 foxesscloud-2.2.2/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.1/LICENCE` & `foxesscloud-2.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.1/PKG-INFO` & `foxesscloud-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.1
+Version: 2.2.2
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -665,15 +665,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.1.<br>
+2.2.2.<br>
+Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.1 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.2 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -457,18 +457,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.1.
-Ensure output is generated if get_battery() fails using battery_info(). Update
-f.avg() to include calculation of averages in lists containng None values.
-Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.2.
+Fix key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.1/README.md` & `foxesscloud-2.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -651,15 +651,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.1.<br>
+2.2.2.<br>
+Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
```

#### html2text {}

```diff
@@ -450,18 +450,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.1.
-Ensure output is generated if get_battery() fails using battery_info(). Update
-f.avg() to include calculation of averages in lists containng None values.
-Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.2.
+Fix key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

### Comparing `foxesscloud-2.2.1/pyproject.toml` & `foxesscloud-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.1/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.2/src/foxesscloud/foxesscloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.3.3"
+version = "1.3.4"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -830,19 +830,19 @@
         volt_n = 0
         volt_keys = []
         for p in remote_settings['parameters']:
             if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
                 volt_n += 1
                 volt_keys.append(p['key'])
                 if volt_n == 3:
-                    named_settings['BatteryVolt'] = {'key': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
+                    named_settings['BatteryVolt'] = {'keys': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
                 elif volt_n > 3:
                     print(f"** get_ui(): more than 3 groups found for BatteryVolt")
             elif p['name'][:11] == 'BatteryTemp':
-                named_settings['BatteryTemp'] = {'key': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
+                named_settings['BatteryTemp'] = {'keys': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
             else:
                 items = []
                 block = p['block'] and len(p['properties']) > 1
                 for e in p['properties']:
                     valueType = e['elemType']['valueType']
                     item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
                     if e['elemType'].get('uiItems') is not None:
@@ -909,17 +909,19 @@
             result.append(get_named_settings(n))
         return result
     if named_settings is None or named_settings.get(name) is None:
         output(f"** get_named_settings(): {name} was not recognised")
         return None
     keys = named_settings[name].get('keys')
     if keys is None:
+        output(f"** get_named_settings(): no keys for name: {name}")
         return None
     result = get_remote_settings(keys)
     if result is None:
+        output(f"** get_named_settings(): no result for {name} using key: {keys}")
         return None
     result_type = named_settings[name].get('type')
     value_type = named_settings[name].get('valueType')
     if result_type is None:
         v = result.get([k for k in result.keys()][0])
         return v if value_type is None else c_float(v) if value_type == 'float' else c_int(v)
     if result_type == 'list':
```

### Comparing `foxesscloud-2.2.1/src/foxesscloud/openapi.py` & `foxesscloud-2.2.2/src/foxesscloud/openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.1"
+version = "2.2.2"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -787,19 +787,19 @@
         volt_n = 0
         volt_keys = []
         for p in remote_settings['parameters']:
             if p['name'][:11] == 'BatteryVolt':    # merge BatteryVolts
                 volt_n += 1
                 volt_keys.append(p['key'])
                 if volt_n == 3:
-                    named_settings['BatteryVolt'] = {'key': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
+                    named_settings['BatteryVolt'] = {'keys': volt_keys, 'type': 'list', 'valueType': 'float', 'unit': p['properties'][0]['unit']}
                 elif volt_n > 3:
                     print(f"** get_ui(): more than 3 groups found for BatteryVolt")
             elif p['name'][:11] == 'BatteryTemp':
-                named_settings['BatteryTemp'] = {'key': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
+                named_settings['BatteryTemp'] = {'keys': p['key'], 'type': 'list', 'valueType': 'int', 'unit': p['properties'][0]['unit']}
             else:
                 items = []
                 block = p['block'] and len(p['properties']) > 1
                 for e in p['properties']:
                     valueType = e['elemType']['valueType']
                     item = {'name': e['key'].replace(protocol,'')} if block else {'key': e['key']} #, 'group': p['name']}
                     if e['elemType'].get('uiItems') is not None:
@@ -866,17 +866,19 @@
             result.append(get_named_settings(n))
         return result
     if named_settings is None or named_settings.get(name) is None:
         output(f"** get_named_settings(): {name} was not recognised")
         return None
     keys = named_settings[name].get('keys')
     if keys is None:
+        output(f"** get_named_settings(): no keys for name: {name}")
         return None
     result = get_remote_settings(keys)
     if result is None:
+        output(f"** get_named_settings(): no result for {name} using key: {keys}")
         return None
     result_type = named_settings[name].get('type')
     value_type = named_settings[name].get('valueType')
     if result_type is None:
         v = result.get([k for k in result.keys()][0])
         return v if value_type is None else c_float(v) if value_type == 'float' else c_int(v)
     if result_type == 'list':
```

### Comparing `foxesscloud-2.2.1/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.2/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.1
+Version: 2.2.2
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -665,15 +665,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.1.<br>
+2.2.2.<br>
+Fix key error when accessing cell volts and temps using an agent / installer account.
 Ensure output is generated if get_battery() fails using battery_info().
 Update f.avg() to include calculation of averages in lists containng None values.
 Added 'data_wrap' to charge_config.
 
 
 2.1.9<br>
 Update get_history() to use GMT or BST when plotting instead of mixed time zones.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.1 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.2 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -457,18 +457,19 @@
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.1.
-Ensure output is generated if get_battery() fails using battery_info(). Update
-f.avg() to include calculation of averages in lists containng None values.
-Added 'data_wrap' to charge_config. 2.1.9
+(verbose) # Version Info 2.2.2.
+Fix key error when accessing cell volts and temps using an agent / installer
+account. Ensure output is generated if get_battery() fails using battery_info
+(). Update f.avg() to include calculation of averages in lists containng None
+values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
 relation to work mode. Better reporting of reason for http error code. Template
 code for get_named_settings() added - not functional in this version due to
 Open API limitations. Update set_pvoutput() to allow push=2. Fix problem in
 set_pvoutput() sending summary to pushover when tou=1. Improve accuracy of time
```

