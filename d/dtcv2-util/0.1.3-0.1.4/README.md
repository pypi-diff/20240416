# Comparing `tmp/dtcv2_util-0.1.3.tar.gz` & `tmp/dtcv2_util-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtcv2_util-0.1.3.tar", last modified: Thu Apr 11 09:16:36 2024, max compression
+gzip compressed data, was "dtcv2_util-0.1.4.tar", last modified: Tue Apr 16 14:49:16 2024, max compression
```

## Comparing `dtcv2_util-0.1.3.tar` & `dtcv2_util-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/
--rw-r--r--   0 root         (0) root         (0)     1897 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1588 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.053982 dtcv2_util-0.1.3/dtcv2_util/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/log_management.py
--rw-rw-rw-   0 root         (0) root         (0)    20362 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/meteo_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     9602 2024-03-20 14:52:59.000000 dtcv2_util-0.1.3/dtcv2_util/validate_inp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 09:16:36.053982 dtcv2_util-0.1.3/dtcv2_util.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1897 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2024-04-11 09:16:36.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-11 09:16:35.000000 dtcv2_util-0.1.3/dtcv2_util.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 09:16:36.057982 dtcv2_util-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-11 09:16:25.000000 dtcv2_util-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.902703 dtcv2_util-0.1.4/
+-rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 14:49:16.902544 dtcv2_util-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1588 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.901319 dtcv2_util-0.1.4/dtcv2_util/
+-rw-r--r--   0 root         (0) staff       (20)      221 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1407 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/log_management.py
+-rw-r--r--   0 root         (0) staff       (20)    19994 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/meteo_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     9602 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/validate_inp.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.902343 dtcv2_util-0.1.4/dtcv2_util.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      292 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       58 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-16 14:49:16.902752 dtcv2_util-0.1.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1323 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/setup.py
```

### Comparing `dtcv2_util-0.1.3/PKG-INFO` & `dtcv2_util-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: dtcv2_util
-Version: 0.1.3
-Summary: Library for workflow management
-Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
-Author: Alejandra Guerrero - DTGEO
-Author-email: aguerrero@geo3bcn.csic.es
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # DTCV2-utils
 
 
 This is a library with utilities developed in DTGEO project in DTCV2 for general purpose. This library contains scripts and functions required for:
 - ****Input file validation:****  through a json file definition of variables
 - ****Log (error) file manager:**** creates and writes the log_file
 - ****Meteo utils:**** utilities for meteorological download
@@ -35,9 +24,7 @@
 
 ## License
 
 The information of the license is avavilable in the [File](LICENSE.md)
 
 ## Project status
 In progress
-
-
```

### Comparing `dtcv2_util-0.1.3/README.md` & `dtcv2_util-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,41 @@
-# DTCV2-utils
-
-
-This is a library with utilities developed in DTGEO project in DTCV2 for general purpose. This library contains scripts and functions required for:
-- ****Input file validation:****  through a json file definition of variables
-- ****Log (error) file manager:**** creates and writes the log_file
-- ****Meteo utils:**** utilities for meteorological download
-- ****ESP utils:**** utilities for Eruption Source Parameters 
-
-For more information related to this package please consult the [Wiki](https://gitlab.geo3bcn.csic.es/dtgeo/WP5-general/dtcv2-utils-base/-/wikis/WP5-utilities) 
-## Input file validation
-
-The meteo_inp.py Python script serves as a data validation tool to ensure that input files adhere to predefined criteria specified in an options configuration file (`options.json`). The script validates variables for dependencies, types, and values according to the specifications outlined in the options file.
-
-## Log (error) file manager 
-
-The function constructs a JSON object containing the log message details, including the description, hour, date, type, locator, and code. It then appends this object to the specified log file.
-
-If the log file directory does not exist, a "FATAL ERROR" message is printed, and the script exits.
-
-## Meteo utils
-
-The Python code is part of a system for managing meteorological data and resources. It includes several classes and functions to handle various aspects of the meteorological data retrieval process.
-
-## License
-
-The information of the license is avavilable in the [File](LICENSE.md)
-
-## Project status
-In progress
+Metadata-Version: 2.1
+Name: dtcv2_util
+Version: 0.1.4
+Summary: Library for workflow management
+Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
+Author: Alejandra Guerrero - DTGEO
+Author-email: aguerrero@geo3bcn.csic.es
+License: MIT
+Description: # DTCV2-utils
+        
+        
+        This is a library with utilities developed in DTGEO project in DTCV2 for general purpose. This library contains scripts and functions required for:
+        - ****Input file validation:****  through a json file definition of variables
+        - ****Log (error) file manager:**** creates and writes the log_file
+        - ****Meteo utils:**** utilities for meteorological download
+        - ****ESP utils:**** utilities for Eruption Source Parameters 
+        
+        For more information related to this package please consult the [Wiki](https://gitlab.geo3bcn.csic.es/dtgeo/WP5-general/dtcv2-utils-base/-/wikis/WP5-utilities) 
+        ## Input file validation
+        
+        The meteo_inp.py Python script serves as a data validation tool to ensure that input files adhere to predefined criteria specified in an options configuration file (`options.json`). The script validates variables for dependencies, types, and values according to the specifications outlined in the options file.
+        
+        ## Log (error) file manager 
+        
+        The function constructs a JSON object containing the log message details, including the description, hour, date, type, locator, and code. It then appends this object to the specified log file.
+        
+        If the log file directory does not exist, a "FATAL ERROR" message is printed, and the script exits.
+        
+        ## Meteo utils
+        
+        The Python code is part of a system for managing meteorological data and resources. It includes several classes and functions to handle various aspects of the meteorological data retrieval process.
+        
+        ## License
+        
+        The information of the license is avavilable in the [File](LICENSE.md)
+        
+        ## Project status
+        In progress
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `dtcv2_util-0.1.3/dtcv2_util/log_management.py` & `dtcv2_util-0.1.4/dtcv2_util/log_management.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.3/dtcv2_util/meteo_utils.py` & `dtcv2_util-0.1.4/dtcv2_util/meteo_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,21 +357,15 @@
     def init_ERA5(self):
             #Files and folders manegem
             
             #Resolution of the GRID 
             res=self.options["RESOLUTION"]
             #Dates (dtart-end) Hours (min max in the day 0-23 default)
             [date, times, step]=self.time.time_ERA5(self.options,self.file_manager.log_file_path)
-            #Output       
-            if self.options["OUTPUT"].upper()=="AUTO":
-                output = "ERA5{date1}-to-{date2}.grb".format(date1  = date[0].strftime("%Y%m%d"),date2  = date[1].strftime("%Y%m%d"))
-            else:
-                output=self.options["OUTPUT"]
-                if not output.endswith('.grb'):
-                    output = output.strip() + '.grb'
+            
             #Area
             self.area.areas(self.options,self.areas_file_path,self.file_manager.log_file_path)
             [lonmin,lonmax,latmin,latmax]=[self.area.lonmin,self.area.lonmax,self.area.latmin,self.area.latmax]
             verbose=1
             
             #Server predetermined values 
             api_key=self.options["API_KEY"]
```

### Comparing `dtcv2_util-0.1.3/dtcv2_util/validate_inp.py` & `dtcv2_util-0.1.4/dtcv2_util/validate_inp.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.3/dtcv2_util.egg-info/PKG-INFO` & `dtcv2_util-0.1.4/dtcv2_util.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: dtcv2-util
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library for workflow management
 Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
 Author: Alejandra Guerrero - DTGEO
 Author-email: aguerrero@geo3bcn.csic.es
 License: MIT
+Description: # DTCV2-utils
+        
+        
+        This is a library with utilities developed in DTGEO project in DTCV2 for general purpose. This library contains scripts and functions required for:
+        - ****Input file validation:****  through a json file definition of variables
+        - ****Log (error) file manager:**** creates and writes the log_file
+        - ****Meteo utils:**** utilities for meteorological download
+        - ****ESP utils:**** utilities for Eruption Source Parameters 
+        
+        For more information related to this package please consult the [Wiki](https://gitlab.geo3bcn.csic.es/dtgeo/WP5-general/dtcv2-utils-base/-/wikis/WP5-utilities) 
+        ## Input file validation
+        
+        The meteo_inp.py Python script serves as a data validation tool to ensure that input files adhere to predefined criteria specified in an options configuration file (`options.json`). The script validates variables for dependencies, types, and values according to the specifications outlined in the options file.
+        
+        ## Log (error) file manager 
+        
+        The function constructs a JSON object containing the log message details, including the description, hour, date, type, locator, and code. It then appends this object to the specified log file.
+        
+        If the log file directory does not exist, a "FATAL ERROR" message is printed, and the script exits.
+        
+        ## Meteo utils
+        
+        The Python code is part of a system for managing meteorological data and resources. It includes several classes and functions to handle various aspects of the meteorological data retrieval process.
+        
+        ## License
+        
+        The information of the license is avavilable in the [File](LICENSE.md)
+        
+        ## Project status
+        In progress
+        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-
-# DTCV2-utils
-
-
-This is a library with utilities developed in DTGEO project in DTCV2 for general purpose. This library contains scripts and functions required for:
-- ****Input file validation:****  through a json file definition of variables
-- ****Log (error) file manager:**** creates and writes the log_file
-- ****Meteo utils:**** utilities for meteorological download
-- ****ESP utils:**** utilities for Eruption Source Parameters 
-
-For more information related to this package please consult the [Wiki](https://gitlab.geo3bcn.csic.es/dtgeo/WP5-general/dtcv2-utils-base/-/wikis/WP5-utilities) 
-## Input file validation
-
-The meteo_inp.py Python script serves as a data validation tool to ensure that input files adhere to predefined criteria specified in an options configuration file (`options.json`). The script validates variables for dependencies, types, and values according to the specifications outlined in the options file.
-
-## Log (error) file manager 
-
-The function constructs a JSON object containing the log message details, including the description, hour, date, type, locator, and code. It then appends this object to the specified log file.
-
-If the log file directory does not exist, a "FATAL ERROR" message is printed, and the script exits.
-
-## Meteo utils
-
-The Python code is part of a system for managing meteorological data and resources. It includes several classes and functions to handle various aspects of the meteorological data retrieval process.
-
-## License
-
-The information of the license is avavilable in the [File](LICENSE.md)
-
-## Project status
-In progress
-
-
```

### Comparing `dtcv2_util-0.1.3/setup.py` & `dtcv2_util-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.3' #First version 
+VERSION = '0.1.4' #First version 
 PACKAGE_NAME = 'dtcv2_util' #For DTGEO general 
 AUTHOR = 'Alejandra Guerrero - DTGEO' 
 AUTHOR_EMAIL = 'aguerrero@geo3bcn.csic.es' 
 URL = 'https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs' 
 LICENSE = 'MIT' 
 DESCRIPTION = 'Library for workflow management' #DTC-V2
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
```

