# Comparing `tmp/ls2d-1.0.3.tar.gz` & `tmp/ls2d-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ls2d-1.0.3.tar", last modified: Thu Sep 28 11:31:38 2023, max compression
+gzip compressed data, was "ls2d-1.0.4.tar", last modified: Tue Apr 16 11:35:34 2024, max compression
```

## Comparing `ls2d-1.0.3.tar` & `ls2d-1.0.4.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.276036 ls2d-1.0.3/
--rw-r--r--   0 bart      (1000) bart      (1000)    35147 2021-05-26 07:47:37.000000 ls2d-1.0.3/LICENSE.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      153 2023-04-04 10:39:10.000000 ls2d-1.0.3/MANIFEST.in
--rw-r--r--   0 bart      (1000) bart      (1000)    44507 2023-09-28 11:31:38.276036 ls2d-1.0.3/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     3130 2023-09-28 11:30:31.000000 ls2d-1.0.3/README.md
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.269369 ls2d-1.0.3/examples/
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.272702 ls2d-1.0.3/examples/microhh/
--rw-r--r--   0 bart      (1000) bart      (1000)     1823 2021-05-26 07:47:37.000000 ls2d-1.0.3/examples/microhh/cabauw.ini.base
--rwxr-xr-x   0 bart      (1000) bart      (1000)      577 2023-04-04 09:43:40.000000 ls2d-1.0.3/examples/microhh/link_lookup_tables.sh
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.272702 ls2d-1.0.3/ls2d/
--rw-r--r--   0 bart      (1000) bart      (1000)     1083 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/__init__.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.272702 ls2d-1.0.3/ls2d/ecmwf/
--rw-r--r--   0 bart      (1000) bart      (1000)     7644 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/ecmwf/IFS_tools.py
--rw-r--r--   0 bart      (1000) bart      (1000)    11723 2021-05-03 14:13:15.000000 ls2d-1.0.3/ls2d/ecmwf/L137_grid.txt
--rw-r--r--   0 bart      (1000) bart      (1000)     5300 2021-09-16 10:54:45.000000 ls2d-1.0.3/ls2d/ecmwf/L60_grid.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      814 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/ecmwf/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)    16446 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/ecmwf/download_era5.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2846 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/ecmwf/era_tools.py
--rw-r--r--   0 bart      (1000) bart      (1000)    30294 2023-09-28 11:28:41.000000 ls2d-1.0.3/ls2d/ecmwf/read_era5.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.272702 ls2d-1.0.3/ls2d/src/
--rw-r--r--   0 bart      (1000) bart      (1000)        0 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1603 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/finite_difference.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4108 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/grid.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1822 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/messages.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7512 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/slurm.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2672 2023-04-01 13:15:27.000000 ls2d-1.0.3/ls2d/src/spatial_tools.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-09-28 11:31:38.272702 ls2d-1.0.3/ls2d.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)    44507 2023-09-28 11:31:38.000000 ls2d-1.0.3/ls2d.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      581 2023-09-28 11:31:38.000000 ls2d-1.0.3/ls2d.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-09-28 11:31:38.000000 ls2d-1.0.3/ls2d.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       61 2023-09-28 11:31:38.000000 ls2d-1.0.3/ls2d.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2023-09-28 11:31:38.000000 ls2d-1.0.3/ls2d.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)      990 2023-09-28 11:29:42.000000 ls2d-1.0.3/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-09-28 11:31:38.276036 ls2d-1.0.3/setup.cfg
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/
+-rw-r--r--   0 bart      (1000) bart      (1000)    35147 2021-05-26 07:47:37.000000 ls2d-1.0.4/LICENSE.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      153 2023-04-04 10:39:10.000000 ls2d-1.0.4/MANIFEST.in
+-rw-r--r--   0 bart      (1000) bart      (1000)    44507 2024-04-16 11:35:34.611221 ls2d-1.0.4/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     3130 2023-09-28 11:30:31.000000 ls2d-1.0.4/README.md
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.607887 ls2d-1.0.4/examples/
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/examples/microhh/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1823 2021-05-26 07:47:37.000000 ls2d-1.0.4/examples/microhh/cabauw.ini.base
+-rwxr-xr-x   0 bart      (1000) bart      (1000)      577 2023-04-04 09:43:40.000000 ls2d-1.0.4/examples/microhh/link_lookup_tables.sh
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/ls2d/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1154 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/__init__.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/ls2d/ecmwf/
+-rw-r--r--   0 bart      (1000) bart      (1000)     7891 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/IFS_tools.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11723 2021-05-03 14:13:15.000000 ls2d-1.0.4/ls2d/ecmwf/L137_grid.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)     5300 2021-09-16 10:54:45.000000 ls2d-1.0.4/ls2d/ecmwf/L60_grid.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      889 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11081 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/download_cams.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    16491 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/download_era5.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2949 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/era_tools.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     8197 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/read_cams.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    31162 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/ecmwf/read_era5.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/ls2d/src/
+-rw-r--r--   0 bart      (1000) bart      (1000)        0 2024-02-06 16:26:25.000000 ls2d-1.0.4/ls2d/src/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1603 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/src/finite_difference.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4108 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/src/grid.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1822 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/src/messages.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7512 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/src/slurm.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2672 2024-04-16 11:22:53.000000 ls2d-1.0.4/ls2d/src/spatial_tools.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-16 11:35:34.611221 ls2d-1.0.4/ls2d.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)    44507 2024-04-16 11:35:34.000000 ls2d-1.0.4/ls2d.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      633 2024-04-16 11:35:34.000000 ls2d-1.0.4/ls2d.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-16 11:35:34.000000 ls2d-1.0.4/ls2d.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       61 2024-04-16 11:35:34.000000 ls2d-1.0.4/ls2d.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-16 11:35:34.000000 ls2d-1.0.4/ls2d.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)      990 2024-04-16 11:35:17.000000 ls2d-1.0.4/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-16 11:35:34.611221 ls2d-1.0.4/setup.cfg
```

### Comparing `ls2d-1.0.3/LICENSE.txt` & `ls2d-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/PKG-INFO` & `ls2d-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls2d
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation
 Author-email: Bart van Stratum <bart.vanstratum@wur.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ls2d-1.0.3/README.md` & `ls2d-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/examples/microhh/cabauw.ini.base` & `ls2d-1.0.4/examples/microhh/cabauw.ini.base`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/examples/microhh/link_lookup_tables.sh` & `ls2d-1.0.4/examples/microhh/link_lookup_tables.sh`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/ls2d/__init__.py` & `ls2d-1.0.4/ls2d/ecmwf/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -14,19 +14,12 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with LS2D.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-# Ban Python 2.x:
-import sys
-if sys.version_info.major < 3:
-    from ls2d.src.messages import error
-    error('(LS)2D requires Python 3.x')
+from .download_era5 import download_era5
+from .download_cams import download_cams
 
-# Make packages directly available as e.g.:
-# ls2d.download_era5() instead of ls2d.ecmwf.download_era5()
-from ls2d.ecmwf import download_era5
-from ls2d.ecmwf import Read_era5
-
-from ls2d.src import grid
+from .read_era5 import Read_era5
+from .read_cams import Read_cams
```

### Comparing `ls2d-1.0.3/ls2d/ecmwf/IFS_tools.py` & `ls2d-1.0.4/ls2d/ecmwf/IFS_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -21,33 +21,38 @@
 # Python modules
 import pkg_resources
 import os
 
 # Third party modules
 import numpy as np
 
-class _IFS_tools:
+class IFS_tools:
     """
     Various tools to calculate e.g. properties of the vertical IFS/ERA grid,
     or the thermodynamics as used by IFS. Wrapped in a class, to prevent
     mixing up differences in methods/constants/.. between IFS and other models
     """
-    def __init__(self):
+    def __init__(self, grid_def='L137'):
 
         # Constants (see IFS part IV, chapter 12)
         self.grav  = 9.80665
         self.Rd    = 287.0597
         self.Rv    = 461.5250
         self.eps   = self.Rv/self.Rd-1.
         self.cpd   = 1004.7090
         self.Lv    = 2.5008e6
 
         # Read the table with the vertical grid properties/parameters
         # From: https://www.ecmwf.int/en/forecasts/documentation-and-support/137-model-levels
-        path = pkg_resources.resource_filename(__name__, 'L137_grid.txt')
+        if grid_def == 'L137':
+            path = pkg_resources.resource_filename(__name__, 'L137_grid.txt')
+        elif grid_def == 'L60':
+            path = pkg_resources.resource_filename(__name__, 'L60_grid.txt')
+        else:
+            sys.exit(f'Unknow grid definition \"{grid_def}\".')
         f = np.loadtxt(path)
 
         # Half and full level number
         self.nh  = f[:,0]
         self.nf  = 0.5 * (self.nh[1:] + self.nh[:-1])
 
         # Reverse all arrays (::-1) from top-to-bottom to bottom-to-top
@@ -202,18 +207,19 @@
         pl.semilogy(self.nf, np.abs((self.gpa-Zgf)/self.gpa))
         pl.xlabel('Level (-)')
         pl.ylabel('(-)')
 
         pl.tight_layout()
         pl.savefig('IFS_tools_validation.pdf')
 
-IFS_tools = _IFS_tools()
 
 if __name__ == "__main__":
     """ Test / example, only executed if script is called directly """
 
     import matplotlib.pyplot as pl
     pl.ion()
     pl.close('all')
 
+    ifs_tools = IFS_tools('L60')
+
     # Validate the IFS_tools conversion from surface pressure to model level pressure, height, etc.
-    IFS_tools.validate()
+    ifs_tools.validate()
```

### Comparing `ls2d-1.0.3/ls2d/ecmwf/L137_grid.txt` & `ls2d-1.0.4/ls2d/ecmwf/L137_grid.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/ls2d/ecmwf/L60_grid.txt` & `ls2d-1.0.4/ls2d/ecmwf/L60_grid.txt`

 * *Files identical despite different names*

### Comparing `ls2d-1.0.3/ls2d/ecmwf/download_era5.py` & `ls2d-1.0.4/ls2d/ecmwf/download_era5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -150,15 +150,18 @@
                     error('CDS request is no longer available online!', exit=False)
                     error('To continue, delete the previous request: {}'.format(pickle_file))
 
                 state = cds_request.reply['state']
 
                 if state == 'completed':
                     message('Request finished, downloading NetCDF file')
+
                     cds_request.download(nc_file)
+                    os.remove(pickle_file)
+
                     finished = True
 
                 elif state in ('queued', 'running'):
                     message('Request not finished, current status = \"{}\"'.format(state))
 
                 else:
                     error('Request failed, status = \"{}\"'.format(state), exit=False)
```

### Comparing `ls2d-1.0.3/ls2d/ecmwf/era_tools.py` & `ls2d-1.0.4/ls2d/ecmwf/era_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -37,24 +37,26 @@
 
     if return_dir:
         return era_dir, era_file
     else:
         return era_file
 
 
-def get_required_analysis(start, end):
+def get_required_analysis(start, end, freq=1):
 
     # One day datetime offset
     one_day = datetime.timedelta(days=1)
 
     # Analysis start at 00 UTC, so first analysis = start day
     first_analysis = datetime.datetime(start.year, start.month, start.day)
 
-    # If end time is after 23 UTC, include next day for the analysis files
-    if end.hour == 23 and end.minute > 0:
+    # If end time is after (24-freq) UTC, include next day for the analysis files.
+    # `freq` is typically 1 hour for ERA5, and 3 hours for CAMS.
+    hour = end.hour + end.minute / 60.
+    if hour > 24 - freq:
         last_analysis = datetime.datetime(end.year, end.month, end.day) + one_day
     else:
         last_analysis = datetime.datetime(end.year, end.month, end.day)
 
     # Create list of datetime objects:
     dates = [first_analysis + i*one_day for i in range((last_analysis-first_analysis).days + 1)]
```

### Comparing `ls2d-1.0.3/ls2d/ecmwf/read_era5.py` & `ls2d-1.0.4/ls2d/ecmwf/read_era5.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -37,14 +37,16 @@
 from ls2d.ecmwf.IFS_tools import IFS_tools
 
 # Constants
 Rd = 287.04
 Rv = 461.5
 ep = Rd/Rv
 
+ifs_tools = IFS_tools('L137')
+
 
 class Slice:
     def __init__(self, istart, iend, jstart, jend):
         self.istart = istart
         self.iend   = iend
         self.jstart = jstart
         self.jend   = jend
@@ -249,59 +251,59 @@
 
         self.theta_soil1 = get_variable(self.fsa, 'swvl1', s2d)  # Top soil layer moisture (-)
         self.theta_soil2 = get_variable(self.fsa, 'swvl2', s2d)  # 2nd soil layer moisture (-)
         self.theta_soil3 = get_variable(self.fsa, 'swvl3', s2d)  # 3rd soil layer moisture (-)
         self.theta_soil4 = get_variable(self.fsa, 'swvl4', s2d)  # Bottom soil layer moistsure (-)
 
         # Pressure level data:
-        self.z_p = get_variable(self.fpa, 'z', s3d) / IFS_tools.grav  # Geopotential height on pressure levels (m)
+        self.z_p = get_variable(self.fpa, 'z', s3d) / ifs_tools.grav  # Geopotential height on pressure levels (m)
         self.p_p = get_variable(self.fpa, 'level', s1d) * 100         # Pressure levels (Pa)
 
         # Convert ozone from mass mixing ratio to volume mixing ratio
         self.o3 = 28.9644 / 47.9982 * self.o3 * 1e6
 
 
     def calc_derived_data(self):
         """
         Calculate derived properties; conversion model levels to pressure/height,
         prognostic variables used by LES, etc.
         """
 
         self.ql  = self.qc + self.qi + self.qr + self.qs  # Total liquid/solid specific humidity (kg kg-1)
         self.qt  = self.q + self.ql                       # Total specific humidity (kg kg-1)
-        self.Tv  = IFS_tools.calc_virtual_temp(
+        self.Tv  = ifs_tools.calc_virtual_temp(
                 self.T, self.q, self.qc, self.qi, self.qr, self.qs)  # Virtual temp on full levels (K)
 
         # Calculate half level pressure and heights
         self.ph  = np.zeros((self.ntime, self.nhalf, self.nlat, self.nlon))  # Half level pressure (Pa)
         self.zh  = np.zeros((self.ntime, self.nhalf, self.nlat, self.nlon))  # Half level geopotential height (m)
 
         # TO-DO: remove loops
         for t in range(self.ntime):
             for la in range(self.nlat):
                 for lo in range(self.nlon):
-                    self.ph[t,:,la,lo] = IFS_tools.calc_half_level_pressure(self.ps[t,la,lo])
-                    self.zh[t,:,la,lo] = IFS_tools.calc_half_level_Zg(self.ph[t,:,la,lo], self.Tv[t,:,la,lo])
+                    self.ph[t,:,la,lo] = ifs_tools.calc_half_level_pressure(self.ps[t,la,lo])
+                    self.zh[t,:,la,lo] = ifs_tools.calc_half_level_Zg(self.ph[t,:,la,lo], self.Tv[t,:,la,lo])
 
         # Full level pressure and height as interpolation of the half level values
         self.p  = 0.5 * (self.ph[:,1:,:,:] + self.ph[:,:-1:,:])  # Full level pressure (Pa)
         self.z  = 0.5 * (self.zh[:,1:,:,:] + self.zh[:,:-1:,:])  # Full level height (m)
 
         # Other derived quantities
-        self.exn  = IFS_tools.calc_exner(self.p)  # Exner on full model levels (-)
+        self.exn  = ifs_tools.calc_exner(self.p)  # Exner on full model levels (-)
         self.th   = (self.T / self.exn)  # Potential temperature (K)
-        self.thl  = self.th - IFS_tools.Lv / (IFS_tools.cpd * self.exn) * self.ql  # Liquid water potential temperature (K)
-        self.rho  = self.p / (IFS_tools.Rd * self.Tv)  # Density at full levels (kg m-3)
-        self.wls  = -self.w / (self.rho * IFS_tools.grav)  # Vertical velocity (m s-1)
+        self.thl  = self.th - ifs_tools.Lv / (ifs_tools.cpd * self.exn) * self.ql  # Liquid water potential temperature (K)
+        self.rho  = self.p / (ifs_tools.Rd * self.Tv)  # Density at full levels (kg m-3)
+        self.wls  = -self.w / (self.rho * ifs_tools.grav)  # Vertical velocity (m s-1)
         self.U    = (self.u**2. + self.v**2)**0.5  # Absolute horizontal wind (m s-1)
 
-        self.Tvs  = IFS_tools.calc_virtual_temp(self.Ts, self.q[:,0])  # Estimate surface Tv using lowest model q (...)
-        self.rhos = self.ph[:,0] / (IFS_tools.Rd * self.Tvs)  # Surface density (kg m-3)
-        self.exns = IFS_tools.calc_exner(self.ps)  # Exner at surface (-)
-        self.wths = self.H / (self.rhos * IFS_tools.cpd * self.exns)  # Surface kinematic heat flux (K m s-1)
+        self.Tvs  = ifs_tools.calc_virtual_temp(self.Ts, self.q[:,0])  # Estimate surface Tv using lowest model q (...)
+        self.rhos = self.ph[:,0] / (ifs_tools.Rd * self.Tvs)  # Surface density (kg m-3)
+        self.exns = ifs_tools.calc_exner(self.ps)  # Exner at surface (-)
+        self.wths = self.H / (self.rhos * ifs_tools.cpd * self.exns)  # Surface kinematic heat flux (K m s-1)
 
         self.fc = 2 * 7.2921e-5 * np.sin(np.deg2rad(self.settings['central_lat']))  # Coriolis parameter
 
         # Store soil temperature, and moisture content, in 3D array
         self.z_soil = np.array([-0.035, -0.175, -0.64, -1.945])
         self.T_soil = np.zeros((self.ntime, 4, self.nlat, self.nlon))
         self.theta_soil = np.zeros((self.ntime, 4, self.nlat, self.nlon))
@@ -332,14 +334,20 @@
                 self.lons[self.i], self.lats[self.j],
                 self.settings['central_lon'], self.settings['central_lat'])
 
         message('Using nearest lat/lon = {0:.2f}/{1:.2f} (requested = {2:.2f}/{3:.2f}), distance ~= {4:.1f} km'\
                 .format(self.lats[self.j], self.lons[self.i],
                         self.settings['central_lat'], self.settings['central_lon'], distance/1000.))
 
+        # Print averaging area.
+        dlon = (1+2*n_av) * float(self.lons[1] - self.lons[0])
+        dlat = (1+2*n_av) * float(self.lats[1] - self.lats[0])
+        self.area = f'{dlon:.2f}°×{dlat:.2f}°'
+        message(f'Averaging ERA5 over a {self.area} spatial area.')
+
         # Start and end indices of averaging domain:
         istart = self.i - n_av
         iend   = self.i + n_av + 1
         jstart = self.j - n_av
         jend   = self.j + n_av + 1
 
         # Numpy slicing tuples for averaging domain
@@ -421,16 +429,16 @@
             self.dtu_advec_mean   = advec(self.u)
             self.dtv_advec_mean   = advec(self.v)
 
             # Geostrophic wind:
             dzdx = np.gradient(self.z_p, axis=3) / dxdi[None, None, :, :]
             dzdy = np.gradient(self.z_p, axis=2) / dydj[None, None, :, :]
 
-            self.ug_p = -IFS_tools.grav / self.fc * dzdy
-            self.vg_p =  IFS_tools.grav / self.fc * dzdx
+            self.ug_p = -ifs_tools.grav / self.fc * dzdy
+            self.vg_p =  ifs_tools.grav / self.fc * dzdx
 
             ug_p_mean = self.ug_p[center4d].mean(axis=(2,3))
             vg_p_mean = self.vg_p[center4d].mean(axis=(2,3))
 
             # Bonus for large domains; spatial (ug,vg) on model levels.
             # Use Scipy's interpolation, as it can extrapolate (in case ps > 1000 hPa)
             self.ug = np.zeros_like(self.u)
@@ -476,19 +484,19 @@
                     self.v[s(0,-2)], self.v[s(0,-1)], self.v[s(0,+1)], self.v[s(0,+2)], dx) \
                 -self.v[s(0,0)] * fd.grad4c(
                     self.v[s(-2,0)], self.v[s(-1,0)], self.v[s(+1,0)], self.v[s(+2,0)], dy)
                                   ).mean(axis=(2,3))
 
             # Geostrophic wind (gradient geopotential height on constant pressure levels)
             vg_p_mean = (
-                IFS_tools.grav / self.fc * fd.grad4c(
+                ifs_tools.grav / self.fc * fd.grad4c(
                     self.z_p[s(0,-2)], self.z_p[s(0,-1)], self.z_p[s(0,+1)], self.z_p[s(0,+2)], dx)
                         ).mean(axis=(2,3))
             ug_p_mean = (
-               -IFS_tools.grav / self.fc * fd.grad4c(
+               -ifs_tools.grav / self.fc * fd.grad4c(
                     self.z_p[s(-2,0)], self.z_p[s(-1,0)], self.z_p[s(+1,0)], self.z_p[s(+2,0)], dy)
                         ).mean(axis=(2,3))
 
 
         # Interpolate geostrophic wind onto model grid.
         # Use Scipy's interpolation, as it can extrapolate (in case ps > 1000 hPa)
         self.ug_mean = np.zeros_like(self.p_mean)
@@ -619,15 +627,15 @@
 
         add_ds_var(ds, 'p_lay', self.p_mean, ('time', 'lay'), 'full level pressure radiation', 'Pa')
         add_ds_var(ds, 'p_lev', self.ph_mean, ('time', 'lev'), 'half level pressure radiation', 'Pa')
 
         add_ds_var(ds, 't_lay', self.T_mean, ('time', 'lay'), 'full level temperature radiation', 'K')
         add_ds_var(ds, 't_lev', self.Th_mean, ('time', 'lev'), 'half level temperature radiation', 'K')
 
-        h2o_lay = self.qt_mean / (ep - ep*self.qt_mean)
+        h2o_lay = self.qt_mean / (ep - ep * self.qt_mean)
         add_ds_var(ds, 'h2o_lay', h2o_lay, ('time', 'lay'), 'moisture volume mixing ratio', '')
         add_ds_var(ds, 'o3_lay', self.o3_mean, ('time', 'lay'), 'ozone volume mixing ratio radiation', 'ppmv')
 
         # Soil variables
         add_ds_var(ds, 't_soil', self.T_soil_mean, ('time', 'zs'), 'soil temperature', 'K')
         add_ds_var(ds, 'theta_soil', self.theta_soil_mean, ('time', 'zs'), 'soil moisture content', 'm3 m-3')
         add_ds_var(ds, 'type_soil', self.soil_type_nn, None, 'ECMWF soil type (Fortran indexing!)', '-')
@@ -653,9 +661,15 @@
         add_ds_var(ds, 'sst', self.sst_mean, ('time'), 'sea surface temperature', 'K')
         add_ds_var(ds, 'ts', self.Ts_mean, ('time'), 'surface (skin) temperature', 'K')
         add_ds_var(ds, 'wth', self.wths_mean, ('time'), 'surface sensible heat flux', 'K m s-1')
         add_ds_var(ds, 'wq', self.wqs_mean, ('time'), 'surface latent heat flux', 'kg kg-1 m s-1')
 
         # Misc
         ds.attrs['fc'] = self.fc
+        ds.attrs['central_lon'] = self.settings['central_lon']
+        ds.attrs['central_lat'] = self.settings['central_lat']
+        ds.attrs['area'] = f'{self.area} spatial average'
+        ds.attrs['source'] = 'ERA5 + (LS)²D'
+        ds.attrs['description'] = 'Generated by (LS)²D: https://github.com/LS2D & https://pypi.org/project/ls2d)'
+        ds.attrs['reference'] = 'van Stratum et al. (2023). The benefits and challenges of downscaling a global reanalysis with doubly-periodic large-eddy simulations. JAMES, https://doi.org/10.1029/2023MS003750'
 
         return ds
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ls2d-1.0.3/ls2d/src/finite_difference.py` & `ls2d-1.0.4/ls2d/src/finite_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `ls2d-1.0.3/ls2d/src/grid.py` & `ls2d-1.0.4/ls2d/src/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `ls2d-1.0.3/ls2d/src/messages.py` & `ls2d-1.0.4/ls2d/src/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `ls2d-1.0.3/ls2d/src/slurm.py` & `ls2d-1.0.4/ls2d/src/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `ls2d-1.0.3/ls2d/src/spatial_tools.py` & `ls2d-1.0.4/ls2d/src/spatial_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is part of LS2D.
 #
-# Copyright (c) 2017-2023 Wageningen University & Research
+# Copyright (c) 2017-2024 Wageningen University & Research
 # Author: Bart van Stratum (WUR)
 #
 # LS2D is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `ls2d-1.0.3/ls2d.egg-info/PKG-INFO` & `ls2d-1.0.4/ls2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ls2d
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation
 Author-email: Bart van Stratum <bart.vanstratum@wur.nl>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ls2d-1.0.3/pyproject.toml` & `ls2d-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = [
     "ls2d",
     "ls2d.ecmwf",
     "ls2d.src"]
 
 [project]
 name = "ls2d"
-version = "1.0.3"
+version = "1.0.4"
 description = "Python toolkit to downscale ERA5 with doubly-periodic large-eddy simulation"
 readme = "README.md"
 authors = [{ name = "Bart van Stratum", email = "bart.vanstratum@wur.nl" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
```

