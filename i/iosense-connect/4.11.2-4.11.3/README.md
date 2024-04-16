# Comparing `tmp/iosense_connect-4.11.2.tar.gz` & `tmp/iosense_connect-4.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iosense_connect-4.11.2.tar", last modified: Wed Mar 20 11:33:51 2024, max compression
+gzip compressed data, was "iosense_connect-4.11.3.tar", last modified: Tue Apr 16 06:51:35 2024, max compression
```

## Comparing `iosense_connect-4.11.2.tar` & `iosense_connect-4.11.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 dhruti    (1000) dhruti    (1000)        0 2024-03-20 11:33:51.195201 iosense_connect-4.11.2/
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)     1067 2024-01-31 06:54:11.000000 iosense_connect-4.11.2/LICENSE.txt
--rw-r--r--   0 dhruti    (1000) dhruti    (1000)     1451 2024-03-20 11:33:51.195201 iosense_connect-4.11.2/PKG-INFO
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)      653 2024-01-31 06:54:11.000000 iosense_connect-4.11.2/README.md
-drwxrwxr-x   0 dhruti    (1000) dhruti    (1000)        0 2024-03-20 11:33:51.191201 iosense_connect-4.11.2/iosense_connect/
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)       72 2024-03-14 11:27:34.000000 iosense_connect-4.11.2/iosense_connect/__init__.py
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)    68010 2024-03-20 11:28:42.000000 iosense_connect-4.11.2/iosense_connect/data_access.py
-drwxrwxr-x   0 dhruti    (1000) dhruti    (1000)        0 2024-03-20 11:33:51.195201 iosense_connect-4.11.2/iosense_connect.egg-info/
--rw-r--r--   0 dhruti    (1000) dhruti    (1000)     1451 2024-03-20 11:33:51.000000 iosense_connect-4.11.2/iosense_connect.egg-info/PKG-INFO
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)      283 2024-03-20 11:33:51.000000 iosense_connect-4.11.2/iosense_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)        1 2024-03-20 11:33:51.000000 iosense_connect-4.11.2/iosense_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)      183 2024-03-20 11:33:51.000000 iosense_connect-4.11.2/iosense_connect.egg-info/requires.txt
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)       16 2024-03-20 11:33:51.000000 iosense_connect-4.11.2/iosense_connect.egg-info/top_level.txt
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)       38 2024-03-20 11:33:51.195201 iosense_connect-4.11.2/setup.cfg
--rw-rw-r--   0 dhruti    (1000) dhruti    (1000)      994 2024-03-20 11:28:42.000000 iosense_connect-4.11.2/setup.py
+drwxrwxr-x   0 samarth   (1000) samarth   (1000)        0 2024-04-16 06:51:35.474886 iosense_connect-4.11.3/
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)     1349 2024-04-16 06:51:35.474886 iosense_connect-4.11.3/PKG-INFO
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)      653 2024-04-16 06:45:48.000000 iosense_connect-4.11.3/README.md
+drwxrwxr-x   0 samarth   (1000) samarth   (1000)        0 2024-04-16 06:51:35.474886 iosense_connect-4.11.3/iosense_connect/
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)       72 2024-04-16 06:45:48.000000 iosense_connect-4.11.3/iosense_connect/__init__.py
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)    68669 2024-04-16 06:51:23.000000 iosense_connect-4.11.3/iosense_connect/data_access.py
+drwxrwxr-x   0 samarth   (1000) samarth   (1000)        0 2024-04-16 06:51:35.474886 iosense_connect-4.11.3/iosense_connect.egg-info/
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)     1349 2024-04-16 06:51:35.000000 iosense_connect-4.11.3/iosense_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)      271 2024-04-16 06:51:35.000000 iosense_connect-4.11.3/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)        1 2024-04-16 06:51:35.000000 iosense_connect-4.11.3/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)      183 2024-04-16 06:51:35.000000 iosense_connect-4.11.3/iosense_connect.egg-info/requires.txt
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)       16 2024-04-16 06:51:35.000000 iosense_connect-4.11.3/iosense_connect.egg-info/top_level.txt
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)       38 2024-04-16 06:51:35.474886 iosense_connect-4.11.3/setup.cfg
+-rw-rw-r--   0 samarth   (1000) samarth   (1000)      994 2024-04-16 06:49:52.000000 iosense_connect-4.11.3/setup.py
```

### Comparing `iosense_connect-4.11.2/README.md` & `iosense_connect-4.11.3/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-4.11.2/iosense_connect/data_access.py` & `iosense_connect-4.11.3/iosense_connect/data_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Disable urllib3's warning about insecure requests
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class DataAccess:
     """Class for accessing data from an API."""
-    __version__ = "4.11.2"
+    __version__ = "4.11.3 "
 
     def __init__(self, userid, url, key):
         """
         Initialize DataAccess instance.
 
         Args:
             userid (str): User ID for accessing the API.
@@ -908,14 +908,25 @@
                                                               end_time=end_time, sensors=sensors, echo=True,
                                                               onpremise=False, IST=True)
                                     df = pd.concat([df, df1])
                                     df.reset_index(drop=True, inplace=True)
 
                                 if IST is False:
                                     df['time'] = pd.to_datetime(df['time']) - timedelta(hours=5.5)
+
+                        else:
+                            df_devices = DataAccess.get_device_details(self, onpremise=onpremise)
+                            device_list = df_devices['devID'].tolist()
+                            if device_id in device_list:
+                                df = DataAccess.influxdb(self, device_id, sensors, start_time, end_time=end_time,
+                                                        onpremise=onpremise,
+                                                        IST=IST, echo=True)
+                            else:
+                                raise Exception('Message: Device not added in account')
+
                     else:
                         df_devices = DataAccess.get_device_details(self, onpremise=onpremise)
                         device_list = df_devices['devID'].tolist()
                         if device_id in device_list:
                             df = DataAccess.influxdb(self, device_id, sensors, start_time, end_time=end_time,
                                                      onpremise=onpremise,
                                                      IST=IST, echo=True)
```

### Comparing `iosense_connect-4.11.2/setup.py` & `iosense_connect-4.11.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "4.11.2",
+    version = "4.11.3",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     install_requires=[
```

