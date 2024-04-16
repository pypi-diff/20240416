# Comparing `tmp/dtcv2_util-0.1.4.tar.gz` & `tmp/dtcv2_util-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtcv2_util-0.1.4.tar", last modified: Tue Apr 16 14:49:16 2024, max compression
+gzip compressed data, was "dtcv2_util-0.1.5.tar", last modified: Tue Apr 16 15:00:37 2024, max compression
```

## Comparing `dtcv2_util-0.1.4.tar` & `dtcv2_util-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.902703 dtcv2_util-0.1.4/
--rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 14:49:16.902544 dtcv2_util-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1588 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.901319 dtcv2_util-0.1.4/dtcv2_util/
--rw-r--r--   0 root         (0) staff       (20)      221 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1407 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/log_management.py
--rw-r--r--   0 root         (0) staff       (20)    19994 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/meteo_utils.py
--rw-r--r--   0 root         (0) staff       (20)     9602 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/dtcv2_util/validate_inp.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 14:49:16.902343 dtcv2_util-0.1.4/dtcv2_util.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      292 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       58 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       11 2024-04-16 14:49:16.000000 dtcv2_util-0.1.4/dtcv2_util.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2024-04-16 14:49:16.902752 dtcv2_util-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1323 2024-04-16 14:42:26.000000 dtcv2_util-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 15:00:37.946781 dtcv2_util-0.1.5/
+-rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 15:00:37.946634 dtcv2_util-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     1588 2024-04-16 14:42:26.000000 dtcv2_util-0.1.5/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 15:00:37.945719 dtcv2_util-0.1.5/dtcv2_util/
+-rw-r--r--   0 root         (0) staff       (20)      221 2024-04-16 14:42:26.000000 dtcv2_util-0.1.5/dtcv2_util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1407 2024-04-16 14:42:26.000000 dtcv2_util-0.1.5/dtcv2_util/log_management.py
+-rw-r--r--   0 root         (0) staff       (20)    20023 2024-04-16 15:00:36.000000 dtcv2_util-0.1.5/dtcv2_util/meteo_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     9602 2024-04-16 14:42:26.000000 dtcv2_util-0.1.5/dtcv2_util/validate_inp.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-16 15:00:37.946449 dtcv2_util-0.1.5/dtcv2_util.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     2148 2024-04-16 15:00:37.000000 dtcv2_util-0.1.5/dtcv2_util.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      292 2024-04-16 15:00:37.000000 dtcv2_util-0.1.5/dtcv2_util.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-16 15:00:37.000000 dtcv2_util-0.1.5/dtcv2_util.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       58 2024-04-16 15:00:37.000000 dtcv2_util-0.1.5/dtcv2_util.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       11 2024-04-16 15:00:37.000000 dtcv2_util-0.1.5/dtcv2_util.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-16 15:00:37.946834 dtcv2_util-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1323 2024-04-16 15:00:36.000000 dtcv2_util-0.1.5/setup.py
```

### Comparing `dtcv2_util-0.1.4/PKG-INFO` & `dtcv2_util-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtcv2_util
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for workflow management
 Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
 Author: Alejandra Guerrero - DTGEO
 Author-email: aguerrero@geo3bcn.csic.es
 License: MIT
 Description: # DTCV2-utils
```

### Comparing `dtcv2_util-0.1.4/README.md` & `dtcv2_util-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.4/dtcv2_util/log_management.py` & `dtcv2_util-0.1.5/dtcv2_util/log_management.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.4/dtcv2_util/meteo_utils.py` & `dtcv2_util-0.1.5/dtcv2_util/meteo_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
             #Dates (dtart-end) Hours (min max in the day 0-23 default)
             [date, times, step]=self.time.time_ERA5(self.options,self.file_manager.log_file_path)
             
             #Area
             self.area.areas(self.options,self.areas_file_path,self.file_manager.log_file_path)
             [lonmin,lonmax,latmin,latmax]=[self.area.lonmin,self.area.lonmax,self.area.latmin,self.area.latmax]
             verbose=1
-            
+            output=self.options["OUTPUT"]
             #Server predetermined values 
             api_key=self.options["API_KEY"]
             server=self.server.serverERA5(self.servers_file,self.file_manager.log_file_path)
             try:
                 meteo=Meteo(date=date,times=times,step=step,latmin=latmin,latmax=latmax,lonmin=lonmin,lonmax=lonmax,res=res, output=output,verbose=verbose,project_path=os.path.join(self.file_manager.project_path,self.file_manager.meteo_folder),server=server,log_file=self.file_manager.log_file_path,api_key=api_key)
                 
             except Exception as e:
```

### Comparing `dtcv2_util-0.1.4/dtcv2_util/validate_inp.py` & `dtcv2_util-0.1.5/dtcv2_util/validate_inp.py`

 * *Files identical despite different names*

### Comparing `dtcv2_util-0.1.4/dtcv2_util.egg-info/PKG-INFO` & `dtcv2_util-0.1.5/dtcv2_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtcv2-util
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library for workflow management
 Home-page: https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs
 Author: Alejandra Guerrero - DTGEO
 Author-email: aguerrero@geo3bcn.csic.es
 License: MIT
 Description: # DTCV2-utils
```

### Comparing `dtcv2_util-0.1.4/setup.py` & `dtcv2_util-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.4' #First version 
+VERSION = '0.1.5' #First version 
 PACKAGE_NAME = 'dtcv2_util' #For DTGEO general 
 AUTHOR = 'Alejandra Guerrero - DTGEO' 
 AUTHOR_EMAIL = 'aguerrero@geo3bcn.csic.es' 
 URL = 'https://gitlab.geo3bcn.csic.es/dtgeo/dtc-v2/meteo-gfs' 
 LICENSE = 'MIT' 
 DESCRIPTION = 'Library for workflow management' #DTC-V2
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
```

