# Comparing `tmp/ecopipeline-0.2.5.tar.gz` & `tmp/ecopipeline-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.5.tar", last modified: Wed Apr 10 20:53:04 2024, max compression
+gzip compressed data, was "ecopipeline-0.2.6.tar", last modified: Tue Apr 16 19:11:14 2024, max compression
```

## Comparing `ecopipeline-0.2.5.tar` & `ecopipeline-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.299634 ecopipeline-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.299634 ecopipeline-0.2.5/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23669 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-10 20:52:35.000000 ecopipeline-0.2.5/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:53:04.303634 ecopipeline-0.2.5/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 20:53:04.000000 ecopipeline-0.2.5/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27209 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.151156 ecopipeline-0.2.6/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30169 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-16 19:10:43.000000 ecopipeline-0.2.6/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:11:14.155156 ecopipeline-0.2.6/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 19:11:14.000000 ecopipeline-0.2.6/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.5/PKG-INFO` & `ecopipeline-0.2.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.5
+Version: 0.2.6
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,14 +43,17 @@
     - site_info: name of the site information csv
     - 410a_info: name of the 410a information csv
     - superheat_info: name of the superheat infomation csv
 - output 
     - directory: diretory of the folder where any pipeline output should be written to
 - data
     - directory: diretory of the folder from which extract loads the raw sensor data
+    - fieldManager_api_usr: Username for Field Manager API if extracting data through that medium
+    - fieldManager_api_pw: Password for Field Manager API if extracting data through that medium
+    - fieldManager_device_id: Device ID for Field Manager API if extracting data through that medium
 ## Unit Testing
 To run Unit tests, run the following command in the terminal in the corresponding directory:
 ```bash
 python -m pytest
 ```
```

### Comparing `ecopipeline-0.2.5/README.md` & `ecopipeline-0.2.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     - site_info: name of the site information csv
     - 410a_info: name of the 410a information csv
     - superheat_info: name of the superheat infomation csv
 - output 
     - directory: diretory of the folder where any pipeline output should be written to
 - data
     - directory: diretory of the folder from which extract loads the raw sensor data
+    - fieldManager_api_usr: Username for Field Manager API if extracting data through that medium
+    - fieldManager_api_pw: Password for Field Manager API if extracting data through that medium
+    - fieldManager_device_id: Device ID for Field Manager API if extracting data through that medium
 ## Unit Testing
 To run Unit tests, run the following command in the terminal in the corresponding directory:
 ```bash
 python -m pytest
 ```
```

### Comparing `ecopipeline-0.2.5/setup.cfg` & `ecopipeline-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.5
+version = 0.2.6
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.5/src/ecopipeline/extract/extract.py` & `ecopipeline-0.2.6/src/ecopipeline/extract/extract.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import json
 from ecopipeline.utils.unit_convert import temp_c_to_f, divide_num_by_ten, windspeed_mps_to_knots, precip_cm_to_mm, conditions_index_to_desc
 from ecopipeline import ConfigManager
 import numpy as np
 import sys
 from pytz import timezone, utc
 import mysql.connector.errors as mysqlerrors
+import requests
 
 
 def get_last_full_day_from_db(config : ConfigManager) -> datetime:
     """
     Function retrieves the last line from the database with the most recent datetime 
     in local time.
     
@@ -328,14 +329,93 @@
      #group and sort index
      df = df.groupby(df.index).mean()
      
      df.sort_index(inplace = True)
 
      return df
 
+def fm_api_to_df(config: ConfigManager, startTime: datetime = None, endTime: datetime = None) -> pd.DataFrame:
+    """
+    Function connects to the field manager api to pull data and returns a dataframe.
+
+    Parameters
+    ----------  
+    config : ecopipeline.ConfigManager
+        The ConfigManager object that holds configuration data for the pipeline. The config manager
+        must contain information to connect to the api, i.e. the api user name and password as well as
+        the device id for the device the data is being pulled from.
+    startTime: datetime
+        The point in time for which we want to start the data extraction from. This 
+        is local time from the data's index. 
+    endTime: datetime
+        The point in time for which we want to end the data extraction. This 
+        is local time from the data's index. 
+    
+    Returns
+    ------- 
+    pd.DataFrame: 
+        Pandas Dataframe containing data from the API pull with column headers the same as the variable names in the data from the pull
+    """
+    api_token = config.get_fm_token()
+    device_id = config.get_fm_device_id()
+    url = f"https://www.fieldpop.io/rest/method/fieldpop-api/deviceDataLog?happn_token={api_token}&deviceID={device_id}"
+    if not startTime is None:
+        url = f"{url}&startUTCsec={startTime.timestamp()}"
+    else:
+        startTime = datetime(2000, 1, 1, 0, 0, 0)  # Jan 1, 2000
+    if not endTime is None:
+        url = f"{url}&endUTCsec={endTime.timestamp()}"
+    else:
+        endTime = datetime.now()
+
+    try:
+        response = requests.get(url)
+        if response.status_code == 200:
+            df = pd.DataFrame()
+            response = response.json()['data']
+            for key, value in response.items():
+                for sensor, data in value.items():
+                    sensor_object = []
+                    # sensor_string = f'{key}_{sensor}'
+                    sensor_string = f'{sensor}'
+                    for entry in data:
+                        sensor_object.append({
+                            'time_pt' : entry['time'],
+                            sensor_string : entry['value']
+                        })
+                    df = pd.concat([df, pd.DataFrame(sensor_object)])
+
+            # Convert 'time_pt' to datetime and set as index
+            if not df.empty:
+                df['time_pt'] = pd.to_datetime(df['time_pt'], unit='s')
+                df.set_index('time_pt', inplace=True)
+                df = df.sort_index()
+                df = df.groupby(df.index).mean()
+            return df
+        elif response.status_code == 500:
+            json_message = response.json()
+            string_to_match = 'The log size is too large - please try again with a smaller date range.'
+            if 'error' in json_message and 'message' in json_message['error'] and json_message['error']['message'] == string_to_match:
+                # Calculate the midpoint between the two datetimes
+                time_diff = endTime - startTime
+                midpointTime = startTime + time_diff / 2
+                # recursively construct the df
+                df_1 = fm_api_to_df(config, startTime, midpointTime)
+                df_2 = fm_api_to_df(config, midpointTime, endTime)
+                df = pd.concat([df_1, df_2])
+                df = df.sort_index()
+                df = df.groupby(df.index).mean()
+                return df
+            
+        print(f"Failed to make GET request. Status code: {response.status_code} {response.json()}")
+        return None
+    except Exception as e:
+        print(f"An error occurred: {e}")
+        return None
+
 def get_sub_dirs(dir: str) -> List[str]:
     """
     Function takes in a directory and returns a list of the paths to all immediate subfolders in that directory. 
     This is used when multiple sites are being ran in same pipeline. 
 
     Parameters
     ---------- 
@@ -374,23 +454,19 @@
     -------
     dict: 
         Dictionary with key as Station Name and Value as DF of Parsed Weather Data
     """
     formatted_dfs = {}
     weather_directory = config.get_weather_dir_path()
     try:
-        print("here 3")
         noaa_dictionary = _get_noaa_dictionary(weather_directory)
-        print("here 4")
         station_ids = {noaa_dictionary[station_name]
             : station_name for station_name in station_names if station_name in noaa_dictionary}
         noaa_filenames = _download_noaa_data(station_ids, weather_directory)
-        print("here 5")
         noaa_dfs = _convert_to_df(station_ids, noaa_filenames, weather_directory)
-        print("here 6")
         formatted_dfs = _format_df(station_ids, noaa_dfs)
     except:
         # temporary solution for NOAA ftp not including 2024
         noaa_df = pd.DataFrame(index=pd.date_range(start='2024-01-01', periods=10, freq='H'))
         noaa_df['conditions'] = None
         noaa_df['airTemp_F'] = None
         noaa_df['dewPoint_F'] = None
```

### Comparing `ecopipeline-0.2.5/src/ecopipeline/load/load.py` & `ecopipeline-0.2.6/src/ecopipeline/load/load.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.2.6/src/ecopipeline/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.2.6/src/ecopipeline/transform/bayview.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.2.6/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline/transform/transform.py` & `ecopipeline-0.2.6/src/ecopipeline/transform/transform.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.2.6/src/ecopipeline/utils/ConfigManager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import configparser
 import os
 import mysql.connector
 import mysql.connector.cursor
+import requests
 
 class ConfigManager:
     """
     A helpful object to manage configuration
 
     Attributes
     ----------
@@ -35,21 +36,41 @@
 
         configure = configparser.ConfigParser()
         configure.read(self.config_directory)
 
         # Directories are saved in config.ini with a relative directory to working directory
         self.input_directory = input_directory
         if self.input_directory is None:
-            self.input_directory = configure.get('input', 'directory')
+            if 'input' in configure and 'directory' in configure['input']:
+                self.input_directory = configure.get('input', 'directory')
+            else:
+                raise Exception('input section missing or incomplete in configuration file.')
         self.output_directory = output_directory
         if self.output_directory is None:
-            self.output_directory = configure.get('output', 'directory')
+            if 'input' in configure and 'directory' in configure['output']:
+                self.output_directory = configure.get('output', 'directory')
+            else:
+                raise Exception('output section missing or incomplete in configuration file.')
         self.data_directory = data_directory
+        self.api_usr = None
+        self.api_pw = None
+        self.api_device_id = None
         if self.data_directory is None:
-            self.data_directory = configure.get('data', 'directory')
+            configured_data_method = False
+            if 'data' in configure:
+                if 'directory' in configure['data']:
+                    self.data_directory = configure.get('data', 'directory')
+                    configured_data_method = True
+                if 'fieldManager_api_usr' in configure['data'] and 'fieldManager_api_pw' in configure['data'] and 'fieldManager_device_id' in configure['data']:
+                    self.api_usr = configure.get('data', 'fieldManager_api_usr')
+                    self.api_pw = configure.get('data', 'fieldManager_api_pw')
+                    self.api_device_id = configure.get('data','fieldManager_device_id')
+                    configured_data_method = True
+            if not configured_data_method:
+                raise Exception('data configuration section missing or incomplete in configuration file.')
 
         # If working on compute3, change directory (Ecotope specific)
         if eco_file_structure and os.name == 'posix':
             if self.input_directory[:2] == 'R:':
                 self.input_directory = '/storage/RBSA_secure' + self.input_directory[2:]
                 self.output_directory = '/storage/RBSA_secure' + self.output_directory[2:]
                 self.data_directory = '/storage/RBSA_secure' + self.data_directory[2:]
@@ -140,8 +161,30 @@
                 database=self.db_connection_info['database']
             )
         except mysql.connector.Error:
             print("Unable to connect to database with given credentials.")
             return None, None
 
         print(f"Successfully connected to database.")
-        return connection, connection.cursor()
+        return connection, connection.cursor()
+    
+    def get_fm_token(self) -> str:
+        if self.api_usr is None or self.api_pw is None:
+            raise Exception("Cannot retrieve Field Manager API token. Credentials were not provided in configuration file.")
+        url = f"https://www.fieldpop.io/rest/login?username={self.api_usr}&password={self.api_pw}"
+        try:
+            response = requests.get(url)
+            # Check if the request was successful (status code 200)
+            if response.status_code == 200:
+                response = response.json()  # Return the response data as JSON
+                return response['data']['token']
+            else:
+                print(f"Failed to make GET request. Status code: {response.status_code}")
+                return None
+        except Exception as e:
+            print(f"An error occurred: {e}")
+            return None
+        
+    def get_fm_device_id(self) -> str:
+        if self.api_device_id is None:
+            raise Exception("Field Manager device ID has not been configured.")
+        return self.api_device_id
```

### Comparing `ecopipeline-0.2.5/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.2.6/src/ecopipeline/utils/unit_convert.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.5/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.2.6/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.5
+Version: 0.2.6
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -43,14 +43,17 @@
     - site_info: name of the site information csv
     - 410a_info: name of the 410a information csv
     - superheat_info: name of the superheat infomation csv
 - output 
     - directory: diretory of the folder where any pipeline output should be written to
 - data
     - directory: diretory of the folder from which extract loads the raw sensor data
+    - fieldManager_api_usr: Username for Field Manager API if extracting data through that medium
+    - fieldManager_api_pw: Password for Field Manager API if extracting data through that medium
+    - fieldManager_device_id: Device ID for Field Manager API if extracting data through that medium
 ## Unit Testing
 To run Unit tests, run the following command in the terminal in the corresponding directory:
 ```bash
 python -m pytest
 ```
```

### Comparing `ecopipeline-0.2.5/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.2.6/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

