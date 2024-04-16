# Comparing `tmp/nasa_pace_data_reader-0.0.4.9.tar.gz` & `tmp/nasa_pace_data_reader-0.0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nasa_pace_data_reader-0.0.4.9.tar", last modified: Fri Mar 29 04:36:32 2024, max compression
+gzip compressed data, was "nasa_pace_data_reader-0.0.5.0.tar", last modified: Tue Apr 16 17:41:51 2024, max compression
```

## Comparing `nasa_pace_data_reader-0.0.4.9.tar` & `nasa_pace_data_reader-0.0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-03-29 04:36:32.312707 nasa_pace_data_reader-0.0.4.9/
--rw-r--r--   0 aputhukkudy   (501) staff       (20)     1061 2024-03-07 17:10:21.000000 nasa_pace_data_reader-0.0.4.9/LICENSE
--rw-r--r--   0 aputhukkudy   (501) staff       (20)     5673 2024-03-29 04:36:32.312469 nasa_pace_data_reader-0.0.4.9/PKG-INFO
--rw-r--r--   0 aputhukkudy   (501) staff       (20)     4932 2024-03-29 04:36:18.000000 nasa_pace_data_reader-0.0.4.9/README.md
--rw-r--r--   0 aputhukkudy   (501) staff       (20)      781 2024-03-29 04:35:04.000000 nasa_pace_data_reader-0.0.4.9/pyproject.toml
--rw-r--r--   0 aputhukkudy   (501) staff       (20)       38 2024-03-29 04:36:32.312756 nasa_pace_data_reader-0.0.4.9/setup.cfg
-drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-03-29 04:36:32.309593 nasa_pace_data_reader-0.0.4.9/src/
-drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-03-29 04:36:32.311195 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/
--rw-r--r--   0 aputhukkudy   (501) staff       (20)    13620 2024-03-19 02:17:49.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/L1.py
--rw-r--r--   0 aputhukkudy   (501) staff       (20)      210 2024-02-13 01:59:05.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/L2.py
--rw-r--r--   0 aputhukkudy   (501) staff       (20)        0 2024-02-13 00:06:45.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/__init__.py
--rw-r--r--   0 aputhukkudy   (501) staff       (20)    47427 2024-03-29 03:41:03.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/plot.py
-drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-03-29 04:36:32.312218 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/
--rw-r--r--   0 aputhukkudy   (501) staff       (20)     5673 2024-03-29 04:36:32.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/PKG-INFO
--rw-r--r--   0 aputhukkudy   (501) staff       (20)      412 2024-03-29 04:36:32.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/SOURCES.txt
--rw-r--r--   0 aputhukkudy   (501) staff       (20)        1 2024-03-29 04:36:32.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/dependency_links.txt
--rw-r--r--   0 aputhukkudy   (501) staff       (20)       90 2024-03-29 04:36:32.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/requires.txt
--rw-r--r--   0 aputhukkudy   (501) staff       (20)       22 2024-03-29 04:36:32.000000 nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/top_level.txt
+drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-04-16 17:41:51.374166 nasa_pace_data_reader-0.0.5.0/
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)     1061 2024-03-07 17:10:21.000000 nasa_pace_data_reader-0.0.5.0/LICENSE
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)     6034 2024-04-16 17:41:51.373900 nasa_pace_data_reader-0.0.5.0/PKG-INFO
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)     5293 2024-04-16 17:40:57.000000 nasa_pace_data_reader-0.0.5.0/README.md
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)      781 2024-04-16 17:39:14.000000 nasa_pace_data_reader-0.0.5.0/pyproject.toml
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)       38 2024-04-16 17:41:51.374217 nasa_pace_data_reader-0.0.5.0/setup.cfg
+drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-04-16 17:41:51.369173 nasa_pace_data_reader-0.0.5.0/src/
+drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-04-16 17:41:51.371477 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)    13966 2024-04-16 02:01:30.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/L1.py
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)    11752 2024-04-02 03:27:50.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/L2.py
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)        0 2024-02-13 00:06:45.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/__init__.py
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)    49899 2024-04-04 19:39:54.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/plot.py
+drwxr-xr-x   0 aputhukkudy   (501) staff       (20)        0 2024-04-16 17:41:51.373589 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)     6034 2024-04-16 17:41:51.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/PKG-INFO
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)      412 2024-04-16 17:41:51.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)        1 2024-04-16 17:41:51.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)       90 2024-04-16 17:41:51.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/requires.txt
+-rw-r--r--   0 aputhukkudy   (501) staff       (20)       22 2024-04-16 17:41:51.000000 nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/top_level.txt
```

### Comparing `nasa_pace_data_reader-0.0.4.9/LICENSE` & `nasa_pace_data_reader-0.0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nasa_pace_data_reader-0.0.4.9/PKG-INFO` & `nasa_pace_data_reader-0.0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa_pace_data_reader
-Version: 0.0.4.9
+Version: 0.0.5.0
 Summary: A package for reading NASA PACE data files.
 Author-email: Anin Puthukkudy <aputhukkudy@umbc.edu>
 Project-URL: Homepage, https://github.com/aninramesh/nasa-pace-data-reader
 Project-URL: Issues, https://github.com/aninramesh/nasa-pace-data-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -132,15 +132,21 @@
 plt_.projectVar('u',  viewAngle=-35)
 
 ```
 ---
 
 ## Change Log:
 ---
-### v0.0.4.9
+### v0.0.5.0
+- Apply this version for data from OBDAAC that is after April 11th, 2024.
+- Updated OCI L1C variable names to ensure consistency with all other instruments.
+- Resolved the projection issue with SPEXOne data.
+- Option to read HARP2 (GRASP-Anin) L2 product has been added. See `Examples/L2-HARP2-GRASP-example.py` to understand how it can be used.
+
+### v0.0.4.10
 - Fixed the projection issue at -180 to 180 longitude transition line
 
 ### v0.0.4.8
 - Added option to plot `highRes` blue marble
 
 ### v0.0.4.7
 - The bug concerning the `projectRGB()` function has been resolved. Users can now input `float` values for `normFactor` and `scale`, whereas previously only `int` values were permitted. (Issue: https://github.com/aninramesh/nasa-pace-data-reader/issues/2)
```

### Comparing `nasa_pace_data_reader-0.0.4.9/README.md` & `nasa_pace_data_reader-0.0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,21 @@
 plt_.projectVar('u',  viewAngle=-35)
 
 ```
 ---
 
 ## Change Log:
 ---
-### v0.0.4.9
+### v0.0.5.0
+- Apply this version for data from OBDAAC that is after April 11th, 2024.
+- Updated OCI L1C variable names to ensure consistency with all other instruments.
+- Resolved the projection issue with SPEXOne data.
+- Option to read HARP2 (GRASP-Anin) L2 product has been added. See `Examples/L2-HARP2-GRASP-example.py` to understand how it can be used.
+
+### v0.0.4.10
 - Fixed the projection issue at -180 to 180 longitude transition line
 
 ### v0.0.4.8
 - Added option to plot `highRes` blue marble
 
 ### v0.0.4.7
 - The bug concerning the `projectRGB()` function has been resolved. Users can now input `float` values for `normFactor` and `scale`, whereas previously only `int` values were permitted. (Issue: https://github.com/aninramesh/nasa-pace-data-reader/issues/2)
```

### Comparing `nasa_pace_data_reader-0.0.4.9/pyproject.toml` & `nasa_pace_data_reader-0.0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nasa_pace_data_reader"
-version = "0.0.4.9"
+version = "0.0.5.0"
 authors = [
   { name="Anin Puthukkudy", email="aputhukkudy@umbc.edu" },
 ]
 description = "A package for reading NASA PACE data files."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/L1.py` & `nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/L1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from netCDF4 import Dataset
+from netCDF4 import Dataset # type: ignore
 import datetime
 
 
 class L1C:
     """Class for reading
         NASA PACE Level 1C data files.
         
@@ -85,19 +85,21 @@
                                 'height', 'rotation_angle']
                 
                 
                 self.obsNames = ['i', 'q', 'u', 'q_over_i', 'u_over_i', 'dolp']
                 self.wavelengthsStr = 'intensity_wavelength'
                 self.F0Str = 'intensity_f0'
                 self.VAStr = 'sensor_view_angle'
+                self.PolWav = 'polarization_wavelength'
+                self.PolF0 = 'polarization_f0'
 
             case 'oci':
                 self.instrument = 'OCI'
-                self.geoNames = ['latitude', 'longitude', 'scattering_angle', 'solar_zenith', 
-                                'solar_azimuth', 'sensor_zenith', 'sensor_azimuth',
+                self.geoNames = ['latitude', 'longitude', 'scattering_angle', 'solar_zenith_angle', 
+                                'solar_azimuth_angle', 'sensor_zenith_angle', 'sensor_azimuth_angle',
                                 'height']
                 
                 self.obsNames = ['i']
                 self.wavelengthsStr = 'intensity_wavelength'
                 self.F0Str = 'intensity_f0'
                 self.VAStr = 'sensor_view_angle'
 
@@ -180,16 +182,18 @@
             data['_units']['F0'] = sensor_data.variables[self.F0Str].units
             self.unit(var, obs_data.variables[var].units)
 
             # read the band angles and wavelengths
             data['view_angles'] = sensor_data.variables[self.VAStr][:]
             data['intensity_wavelength'] = sensor_data.variables[self.wavelengthsStr][:]
 
-            # FIXME: Polarization based F0 might be needed for SPEXone, since their spectral response is polarization dependent
-
+            # Polarization based F0 might be needed for SPEXone, since their spectral response is polarization dependent
+            if self.instrument == 'SPEXone':
+                data['polarization_wavelength'] = sensor_data.variables[self.PolWav][:]
+                data['polarization_f0'] = sensor_data.variables[self.PolF0][:]
 
             # close the netCDF file
             dataNC.close()
 
             return data
 
         except KeyError as e:
```

### Comparing `nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader/plot.py` & `nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import numpy as np
 from scipy import interpolate
 
 # cartopy related imports
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 from cartopy.mpl.gridliner import LONGITUDE_FORMATTER, LATITUDE_FORMATTER
-from cartopy.util import add_cyclic
 
 class Plot:
     def __init__(self, data, instrument='HARP2'):
         self.data = data
         self.plotDPI = 240
         self.xAxis = 'scattering_angle'
         if instrument.lower() == 'harp2':
@@ -64,15 +63,15 @@
         """Set the band angles for the plot.
         Args:
             bandAngles (list): The band angles for the plot.
 
         Returns:
             None
         """
-        band = self.band if band == None else band
+        band = self.band if band is None else band
         if self.instrument == 'HARP2':
             band_angle_ranges = {
                 'blue': range(80, 90),
                 'green': range(0, 10),
                 'red': range(10, 70),
                 'nir': range(70, 80)
             }
@@ -87,57 +86,62 @@
         Args:
             band (str): The band for the plot.
 
         Returns:
             None
         """
         band_ = band.lower()
-        assert band_ in ['blue', 'green', 'red', 'nir', 'swir1', 'swir2',  'all'], 'Invalid band'
+        assert band_ in ['blue', 'green', 'red', 'nir', 'swir1', 'swir2',  'all', 'harp2'], 'Invalid band'
         self.band = band_
 
         # set the angle specification based on the instrument
         self.setBandAngles(self.band) if self.instrument == 'HARP2' else None
 
         # for oci, set the wavelength index
         if self.instrument == 'OCI':
             if self.band == 'blue':
                 self.wavIndex = np.argmin(np.abs(self.data['intensity_wavelength']-440)) 
             elif self.band == 'all':
                 self.wavIndex = range(0, self.data['intensity_wavelength'].shape[1])
             # self.setBandAngles(band=self.band)
         elif self.instrument == 'SPEXone':
-            self.wavIndex = range(0, self.data['intensity_wavelength'].shape[1], 20)
+            if self.band == 'all':
+                self.wavIndex = range(0, self.data['intensity_wavelength'].shape[1], 20)
+            elif self.band.lower() == 'harp2':
+                self.wavIndex = [63, 170, 285]
+                self.wavIndexDolp = [10, 25, 39]
+                self.bands = ['blue', 'green', 'red']
         else:
             self.wavIndex = 0
 
         print(f'...Band set to {self.band}') if verbose else None
 
 
     def setDPI(self, dpi):
         """Set the DPI for the plot.
         Args:
             dpi (int): The DPI for the plot.
 
         Returns:
             None
         """
-        self.plotDPI = dpi if not dpi==None else None
+        self.plotDPI = dpi if dpi is not None else None
         print('setting dpi to %d ppi' %self.plotDPI)
         plt.rcParams['figure.dpi'] = self.plotDPI
 
 
     def setInstrument(self, instrument=None):
         """Set the instrument for the plot.
         Args:
             instrument (str): The instrument for the plot.
 
         Returns:
             None
         """
-        if instrument == None:
+        if instrument is None:
             instrument = self.instrument
         else:
             assert instrument.lower() in ['harp2', 'spexone', 'oci'], 'Invalid instrument'
             self.instrument = instrument
 
         if self.instrument == 'HARP2':
             self.bands = ['blue', 'green', 'red', 'nir']
@@ -174,20 +178,20 @@
             y (int): The y coordinate of the pixel.
             dataVar (str): The variable to plot.
             xAxis (str): The x-axis variable.
 
         Returns:
             None
         """
-        xAxis = self.xAxis if xAxis == None else xAxis
+        xAxis = self.xAxis if xAxis is None else xAxis
         assert xAxis in ['scattering_angle', 'view_angles', 'intensity_wavelength'], 'Invalid x-axis variable'
         xData_, dataVar_, unit_ = self.physicalQuantity(x, y, dataVar, xAxis=xAxis, maskFlag=maskFlag)
 
         # Plot the data
-        fig_, ax_ = plt.subplots(figsize=(6, 4)) if axis == None else (None, axis)
+        fig_, ax_ = plt.subplots(figsize=(6, 4)) if axis is None else (None, axis)
         ax_.plot(xData_, dataVar_, **kwargs)
         if axisLabel:
             plt.xlabel(xAxis)
             if unit_:
                 plt.ylabel(f'{dataVar}\n{unit_}')
             elif dataVar != 'dolp':
                 plt.ylabel(r'R$_{%s}$' % dataVar)
@@ -225,15 +229,15 @@
 
         Returns:
             xData_ (np.ndarray): The x-axis data.
             dataVar_ (np.ndarray): The y-axis data.
             unit_ (str): The unit of the data.
         """
 
-        if x == None and y == None:
+        if x is None and y is None:
             x, y = 100, 200 # default values
 
         # plot reflectance or radiance
         if self.instrument == 'HARP2':
             if self.reflectance and dataVar.lower() in self.vars2plot and dataVar.lower() not in ['dolp']:
                 # πI/F0
                 dataVar_ = self.data[dataVar][x, y, self.bandAngles,
@@ -243,30 +247,33 @@
                 dataVar_ = self.data[dataVar][x, y, self.bandAngles, self.wavIndex]
                 unit_ = '('+self.data['_units'][dataVar]+')' if not dataVar == 'dolp' else ''
 
         elif self.instrument == 'OCI':
             # find if all values in a 2d array is masked
             if self.reflectance and dataVar in self.vars2plot:
                 # πI/F0
-                for i in self.bandAngles:
-                    if not np.all(np.ma.getmask(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])):
-                        if maskFlag:
-                            dataVar_ = np.ma.getdata(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])*np.pi/self.data['F0'][self.bandAngles[i], self.wavIndex]
-                        else:
-                            dataVar_ = np.ma.getdata(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])*np.pi/np.ma.getdata(self.data['F0'][self.bandAngles[i], self.wavIndex])
-                        continue
+
+                if self.bandAngles is not None:
+                    for i in self.bandAngles:
+                        if self.data[dataVar] is not None and not np.all(np.ma.getmask(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])):
+                            if maskFlag:
+                                dataVar_ = np.ma.getdata(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])*np.pi/self.data['F0'][self.bandAngles[i], self.wavIndex]
+                            else:
+                                dataVar_ = np.ma.getdata(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])*np.pi/np.ma.getdata(self.data['F0'][self.bandAngles[i], self.wavIndex])
+                            continue
                 unit_= ''
             else:
-                for i in self.bandAngles:
-                    # check if the data is masked, for the case of OCI only one viewing angle at a time
-                    if not np.all(np.ma.getmask(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])):
-                        dataVar_ = self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex]
-                        continue
+                if self.bandAngles is not None:
+                    for i in self.bandAngles:
+                        # check if the data is masked, for the case of OCI only one viewing angle at a time
+                        if not np.all(np.ma.getmask(self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex])):
+                            dataVar_ = self.data[dataVar][x, y, self.bandAngles[i], self.wavIndex]
+                            continue
                 # check any valid data found
-                if not 'dataVar_' in locals():
+                if 'dataVar_' not in locals():
                     print(f'...No valid data found for the variable {dataVar} at the pixel ({x}, {y})')
                     # end the script
                     return None, None, None
                 unit_ = '('+self.data['_units'][dataVar]+')' if not dataVar == 'dolp' else ''
         elif self.instrument == 'SPEXone':
             waveIndex = self.wavIndex if dataVar in ['i'] else self.wavIndexDolp
             if self.reflectance and dataVar in self.vars2plot and dataVar.lower() not in ['dolp']:
@@ -280,15 +287,15 @@
         # for the scattering angle
         if xAxis == 'scattering_angle':
             xData_ = self.data[xAxis][x, y, self.bandAngles]
         # for the view angles
         elif xAxis == 'view_angles':
             xData_ = self.data[xAxis][self.bandAngles]
         elif xAxis == 'intensity_wavelength':
-            xData_ = self.data[xAxis][self.bandAngles[i]] if self.instrument == 'OCI' else self.data[xAxis][self.bandAngles]
+            xData_ = self.data[xAxis][self.bandAngles[i]] if self.instrument == 'OCI' else self.data[xAxis][self.bandAngles] # type: ignore
 
         return xData_, dataVar_, unit_
 
     def setFigure(self, figsize=(10, 5), **kwargs):
         """Set the figure size for the plot.
         Args:
             figsize (tuple): The figure size for the plot.
@@ -329,25 +336,26 @@
         Returns:
             None
         """
         assert xAxis in ['scattering_angle', 'view_angles'], 'Invalid x-axis variable'
         if bands is None:
             self.plotAll = True
         self.bands2plot = self.bands if bands is None else bands
+        tempBands = self.bands
 
         # based on the instrument, set the band angles 
         if axis is None:
             # Define the size of each subplot
             subplot_size = (2, 1.5)
             rows = len(self.vars2plot)
             cols = len(self.bands2plot)
 
             # Calculate the figure size to keep a good aspect ratio
             figsize = (subplot_size[0] * cols, subplot_size[1] * rows)
-            figAll, axAll = self.setFigure(figsize=figsize)
+            figAll, axAll = self.setFigure(figsize=figsize) # type: ignore
         else:
             axAll = axis
 
         # define color strings based on the length of the bands try to preserve the color
         colors = ['C%d' %i for i in range(cols)]
         
         # plot the data over different bands and variables
@@ -358,14 +366,17 @@
 
                 # set the band and angles
                 self.setBand(band, verbose=self.verbose)
 
                 # get the physical quantity
                 xData_, dataVar_, unit_ = self.physicalQuantity(x, y, vars, xAxis=xAxis)
 
+                if self.instrument == 'SPEXone':
+                    dataVar_ = dataVar_[:, j]
+
                 # plot the data
                 axAll[i,j].plot(xData_, dataVar_,
                                 '%so-' %colors[j],
                                 label= vars if j ==0 else None, **kwargs)
                 
                 # set the labels
                 if axisLabel and j == 0:
@@ -376,18 +387,22 @@
                     else:
                         axAll[i,j].set_ylabel(vars)
                     axAll[i,j].yaxis.set_label_coords(-0.25,0.5)
 
                 if axisLabel and i == len(self.vars2plot)-1:
                     axAll[i,j].set_xlabel(xAxis)
 
-        plt.suptitle(f'Pixel ({x}, {y}) of the instrument {self.instrument}')
+        plt.suptitle(f'{self.data["date_time"]} \nPixel ({x}, {y}) of the instrument {self.instrument}')
         plt.tight_layout()
         plt.show()
 
+        # if SPEXOne, change the band back to all
+        if self.instrument == 'SPEXone':
+            self.bands = tempBands
+
         # if saveFig is True, save the figure
         if saveFig:
             location = f'./{self.instrument}_pixel_{x}_{y}.png'
             figAll.savefig(location, dpi=self.plotDPI)
 
     def plotRGB(self, var='i', viewAngleIdx=[38, 4, 84],
                  scale= 1, normFactor=200, returnRGB=False, autoNorm=False,
@@ -418,40 +433,57 @@
                 assert len(idx) == 1, 'Invalid number of indices'
             else:
                 if np.nanmean(self.data['latitude']) > 0:
                     viewAngleIdx = [1]
                 else:
                     viewAngleIdx = [0]
                 assert len(viewAngleIdx) == 1, 'Invalid number of indices'
+        elif self.instrument == 'SPEXone':
+            assert len(idx) == 3, 'Invalid number of indices'
+            # the viewAngleIdx is the index of the wavelength should be between 0 to 5
+            assert np.all(np.array(idx) < 5), 'Invalid viewAngleIdx'
 
         # Create a 3D array to store the RGB data
         rgb = np.zeros((self.data[var].shape[0], self.data[var].shape[1], 3), dtype=np.float16)
 
         # if the instrument is HARP2
         if self.instrument == 'HARP2':
             if rgb_dolp:
                 rgb[:, :, 0] = self.data['i'][:,:,idx[0],0]*self.data[var][:,:,idx[0],0]
                 rgb[:, :, 1] = self.data['i'][:,:,idx[1],0]*self.data[var][:,:,idx[1],0]
                 rgb[:, :, 2] = self.data['i'][:,:,idx[2],0]*self.data[var][:,:,idx[2],0]
             else:
                 rgb[:, :, 0] = self.data[var][:,:,idx[0],0]
                 rgb[:, :, 1] = self.data[var][:,:,idx[1],0]
                 rgb[:, :, 2] = self.data[var][:,:,idx[2],0]
-        elif self.instrument == 'OCI':
+        elif self.instrument == 'OCI' or self.instrument == 'SPEXone':
             # for the case of OCI, the variable is the intensity
-
+            if self.instrument == 'SPEXone' and var == 'dolp':
+                var_wav = 'polarization_wavelength'
+            else:
+                var_wav = 'intensity_wavelength'
             # find wavelength index close tor R, G, B
             #self.data['intensity_wavelength']-440
-            idxB = np.argmin(np.abs(self.data['intensity_wavelength']-440))
-            idxG = np.argmin(np.abs(self.data['intensity_wavelength']-550))
-            idxR = np.argmin(np.abs(self.data['intensity_wavelength']-650))
-            
-            rgb[:, :, 0] = self.data[var][:,:,viewAngleIdx[0],idxR]
-            rgb[:, :, 1] = self.data[var][:,:,viewAngleIdx[0],idxG]
-            rgb[:, :, 2] = self.data[var][:,:,viewAngleIdx[0],idxB]
+            idxB = np.argmin(np.abs(self.data[var_wav]-440))
+            idxG = np.argmin(np.abs(self.data[var_wav]-550))
+            idxR = np.argmin(np.abs(self.data[var_wav]-670))
+            if var == 'dolp':
+                rgb[:, :, 0] = self.data['i'][:,:,idx[0],idxR]*self.data[var][:,:,idx[0],idxR]
+                rgb[:, :, 1] = self.data['i'][:,:,idx[1],idxG]*self.data[var][:,:,idx[1],idxG]
+                rgb[:, :, 2] = self.data['i'][:,:,idx[2],idxB]*self.data[var][:,:,idx[2],idxB]
+            else:
+                
+                if self.instrument == 'SPEXone':
+                    rgb[:, :, 0] = self.data[var][:,:,idx[0],idxR]
+                    rgb[:, :, 1] = self.data[var][:,:,idx[1],idxG]
+                    rgb[:, :, 2] = self.data[var][:,:,idx[2],idxB]
+                else: # for OCI
+                    rgb[:, :, 0] = self.data[var][:,:,viewAngleIdx[0],idxR]
+                    rgb[:, :, 1] = self.data[var][:,:,viewAngleIdx[0],idxG]
+                    rgb[:, :, 2] = self.data[var][:,:,viewAngleIdx[0],idxB]
 
         # Normalize the RGB image
         if autoNorm:
 
             # calculate the normFactor for each band
             normFactor = np.zeros(3)
 
@@ -474,20 +506,26 @@
                         rgb = rgb/normFactor*scale
                     else:
                         for i in range(3):
                             rgb[:, :, i] = rgb[:, :, i]/normFactor*scale[i]
                 except Exception as e:
                     print(f'...Error in normalizing the RGB image {e}')
                     print('normFactor and scale shoulshould be an integer', normFactor)
-        # copy the rgb to a new variable
+        # Floor the rgb values to 0-1
+        rgb = np.clip(rgb, 0, 1)
 
         # Plot the RGB image
         if plot:
             plt.imshow(rgb, origin='lower')
-            plt.title(f'RGB image of the instrument {self.instrument}\n using "{var}" variable at angles {idx[0]}, {idx[1]}, {idx[2]}')
+            if self.instrument == 'HARP2':
+                plt.title(f'{self.data["date_time"]} \nRGB image of the instrument {self.instrument}\n using "{var}" variable at angles {idx[0]}, {idx[1]}, {idx[2]}', fontsize=8)
+            elif self.instrument == 'OCI':
+                plt.title(f'{self.data["date_time"]} \nRGB image of the instrument {self.instrument}\n using "{var}" variable at angle {viewAngleIdx[0]}', fontsize=8)
+            elif self.instrument == 'SPEXone':
+                plt.title(f'{self.data["date_time"]} \nRGB image of the instrument {self.instrument}\n using "{var}" variable at angles {idx[0]}, {idx[1]}, {idx[2]}', fontsize=8)
             plt.show()
 
         if returnRGB:
             self.rgb = rgb
 
         if saveFig:
             location = f'./{self.instrument}_RGB.png'
@@ -565,15 +603,15 @@
             for key, value in kwargs.items():
                 if key in kwargs:
                     kwargs[key] = value
                 if key in ['figsize']:
                     figsize = value
 
         # Prepare figure and axes
-        figsize_ = figsize if figsize_ == None else figsize_
+        figsize_ = figsize if figsize_ is None else figsize_
         if ax is None:
             fig = plt.figure(figsize=figsize_)
         
         if proj == 'PlateCarree':
             if ax is None:
                 if transitionFlag:
                     ax = plt.axes(projection=ccrs.PlateCarree(central_longitude=lon_center))
@@ -592,72 +630,67 @@
 
         elif proj == 'Orthographic':
             ax = plt.axes(projection=ccrs.Orthographic(central_longitude=lon_center, central_latitude=lat_center))
         else:
             print('Invalid projection method')
         
         # setup the gridlines
-        ax.coastlines()
-        ax.set_global()
-        ax.set_extent([lon.min(), lon.max(), lat.min(), lat.max()], crs=ccrs.PlateCarree())
-        if not highResStockImage:
-            ax.stock_img() if stockImage else ax.add_feature(cfeature.OCEAN, zorder=0) ; ax.add_feature(cfeature.LAND, zorder=0, edgecolor='black')
-        else:
-            ax.background_img(name='NaturalEarthRelief', resolution='high')
-        # Add coastline feature
-        ax.add_feature(cfeature.COASTLINE, edgecolor='black', linewidth=1, alpha=0.5)
-        ax.add_feature(cfeature.LAKES, edgecolor='black', linewidth=1, alpha=0.5) if lakes else None
-        ax.add_feature(cfeature.RIVERS, edgecolor='black', linewidth=1, alpha=0.5) if rivers else None
+        if ax is not None:
+            ax.coastlines()
+            ax.set_global()
+            ax.set_extent([lon.min(), lon.max(), lat.min(), lat.max()], crs=ccrs.PlateCarree())
+            if not highResStockImage:
+                ax.stock_img() if stockImage else ax.add_feature(cfeature.OCEAN, zorder=0)
+                ax.add_feature(cfeature.LAND, zorder=0, edgecolor='black')
+            else:
+                ax.background_img(name='NaturalEarthRelief', resolution='high')
+            # Add coastline feature
+            ax.add_feature(cfeature.COASTLINE, edgecolor='black', linewidth=1, alpha=0.5)
+            ax.add_feature(cfeature.LAKES, edgecolor='black', linewidth=1, alpha=0.5) if lakes else None
+            ax.add_feature(cfeature.RIVERS, edgecolor='black', linewidth=1, alpha=0.5) if rivers else None
         
         # plot the data with alpha value
         if varAlpha:
             kwargs['alpha'] = varAlpha
 
         # if reflectance is True, plot the reflectance
         if level.lower() == 'l1b':
             data_ = self.data[var][viewAngleIdx,:,:]
 
-            im = plt.contourf(lon, lat,
+            plt.contourf(lon, lat,
                             data_, 60,
                             transform=ccrs.PlateCarree(), **kwargs)
 
         else:
             if self.reflectance and var in ['i', 'q', 'u']:
                 # πI/F0
                 data_ = self.data[var][:,:,viewAngleIdx,0]*np.pi/self.data['F0'][viewAngleIdx, 0]
             else:
                 data_ = self.data[var][:,:,viewAngleIdx,0]
 
-            im = plt.contourf(lon, lat,
+            plt.contourf(lon, lat,
                             data_, 60,
                             transform=ccrs.PlateCarree(), **kwargs)
         
         # select var and units
         var, unit_ = self.reflectanceChange(var) if self.reflectance else (var, self.data['_units'][var])
         # var = '%s_' %var
         # add colorbar with same size as the y axis length and set the label
-        if colorbar:
-            cax = fig.add_axes([ax.get_position().x1+0.01,ax.get_position().y0,0.02,ax.get_position().height])
-            plt.colorbar(im, cax=cax)
-
-            # add the label to the colorbar
-            cax.set_ylabel(f'${var}{{({self.band})}}$ ({unit_})')
-
-        # set a margin around the data
-        ax.set_xmargin(0.05)
-        ax.set_ymargin(0.05)
+        if ax is not None:
+            ax.set_xmargin(0.05)
+            ax.set_ymargin(0.05)
 
-        # round the view angle to 2 decimal places
-        ax.set_title(f'${var}{{({self.band})}}$ at {round(float(viewAngle), 2)}° viewing angle \nof the instrument {self.instrument}')
-        plt.show()
+            # round the view angle to 2 decimal places
+            ax.set_title(f'${var}{{({self.band})}}$ at {round(float(viewAngle), 2)}° viewing angle \nof the instrument {self.instrument}')
+            plt.show()
 
-        if saveFig:
-            location = f'./{self.instrument}_viewAngle_{viewAngle}.png'
-            fig.savefig(location, dpi=self.plotDPI)
-            print(f'...Figure saved at {location}')
+            if saveFig:
+                location = f'./{self.instrument}_viewAngle_{viewAngle}.png'
+                fig.savefig(location, dpi=self.plotDPI)
+                print(f'...Figure saved at {location}')
 
     def reflectanceChange(self, var):
         """Change the variable to reflectance if reflectance is True.
 
         Args:
             var (str): The variable to change.
 
@@ -675,15 +708,15 @@
 
 
     # Plot projected RGB using Cartopy
     def projectedRGB(self, rgb=None, scale=1, ax=None, fig=None,
                      var='i', viewAngleIdx=[36, 4, 84],
                      normFactor=200, proj='PlateCarree',
                      saveFig=False, noShow=False, rivers=False, lakes=False,
-                     rgb_dolp=False, figsize=None, savePath=None, dpi=300, setTitle=True,
+                     rgb_dolp=False, figsize=None, savePath=None, dpi=None, setTitle=True,
                      returnRGB=False, lon_0=None, lat_0=None, black_background=True,
                      proj_size=None, returnTransitionFlag=False, highResStockImage=False,
                      **kwargs):
         """Plot the projected RGB image of the instrument using Cartopy.
 
         Args:
             rgb (np.ndarray, optional): The RGB data. Defaults to None.
@@ -695,15 +728,15 @@
             proj (str, optional): The projection method. Defaults to 'PlateCarree'.
             **kwargs: Variable length argument list to pass to the plot function.
 
         Returns:
             None
         """
         assert proj.lower() in ['platecarree', 'orthographic', 'none'], 'Invalid projection method currently only PlateCarree and Orthographic are supported'
-
+        self.plotDPI = dpi if dpi is not None else self.plotDPI
         if self.instrument == 'OCI':
             if np.nanmean(self.data['latitude']) > 0:
                 viewAngleIdx = [1]
             else:
                 viewAngleIdx = [0]
             assert len(viewAngleIdx) == 1, 'Invalid number of indices'
 
@@ -733,25 +766,28 @@
         proj_size=(900,400) if proj_size is None else proj_size
 
         if transitionFlag:
             # Interpolate the RGB values onto a regular grid via function applying scale factor in advance
             rgb_new, rgb_extent = self.GridRGB(lon, lat, dateline=True, proj_size=proj_size)
 
         else:
+            # rgb_new, rgb_extent = self.GridRGB(lon, lat, dateline=False, proj_size=proj_size)
             rgb_new, nlon, nlat = self.meshgridRGB(lon, lat, return_mapdata=False, proj_size=proj_size) #Created projection image
-            rgb_extent = [nlon.min(), nlon.max(), nlat.min(), nlat.max()]        
+            rgb_extent = [nlon.min(), nlon.max(), nlat.min(), nlat.max()]         # type: ignore
 
         # Prepare figure and axes
         if ax is None and proj.lower() != 'none':
             print('...Creating a new figure')
             if figsize is None:
                 fig = plt.figure(figsize=(4, 5), dpi=self.plotDPI) if fig is None else fig
                 # print('...Setting the figure size to (4, 5)')
             else:
                 if fig is None:
+                    print(f'...Creating a new figure with figsize {figsize}')
+                    print(f'...Setting the figure dpi to {self.plotDPI}')
                     fig = plt.figure(figsize=figsize, dpi=self.plotDPI)
                 else:
                     fig = fig
                 # print(f'...Setting the figure size to {figsize}')
 
         # Check the projection type
         if proj == 'Orthographic':
@@ -760,20 +796,16 @@
                 ax = plt.axes(projection=ccrs.Orthographic(lon_center, lat_center))
             else:
                 ax = ax
             if highResStockImage:
                 ax.background_img(name='BlueMarble', resolution='high')
             else:
                 ax.stock_img()
-            ax.set_global()
-
-            if black_background:
-                # Set the background color to black
+            if fig is not None:
                 fig.patch.set_facecolor('black')
-                # set the font color to white
 
             # mask the black pane
             rgb_new = np.ma.masked_where(rgb_new == 0, rgb_new)
 
             # Display the image in the projection
             ax.imshow(rgb_new, origin='lower',  extent=rgb_extent, transform=ccrs.PlateCarree(), **kwargs)
             ax.add_feature(cfeature.COASTLINE, edgecolor='black', linewidth=0.2, alpha=0.5)
@@ -812,30 +844,33 @@
                 print('...No projection method selected')
             else:
                 print('Invalid projection method')
 
         # These operations are common to both projections but not needed for just getting the RGB interpolated data
         if proj.lower() != 'none':
             # set a margin around the data
-            ax.set_xmargin(0.05)
-            ax.set_ymargin(0.05)
+            if ax is not None:
+                ax.set_xmargin(0.05)
+                ax.set_ymargin(0.05)
 
             if setTitle:
                 # set the title using the date_time
                 fontColor = 'tan' if black_background else 'black'
-                ax.set_title(f'RGB image of the instrument {self.instrument}\n {self.data["date_time"]} at viewing angles {str(self.data["view_angles"][viewAngleIdx[0]])}', color=fontColor)
-                
+                if ax is not None:
+                    ax.set_title(f'RGB image of the instrument {self.instrument}\n {self.data["date_time"]} at viewing angles {str(self.data["view_angles"][viewAngleIdx[0]])}', color=fontColor)
+
             plt.box(on=None)
             plt.show() if not noShow else None
 
             if saveFig:
                 location = f'./{self.instrument}_RGB_{str(viewAngleIdx[0])}_proj_{proj}.png'
                 if savePath is not None:
                     location = savePath
-                fig.savefig(location, dpi=self.plotDPI)
+                if fig is not None:  # Check if fig is not None
+                    fig.savefig(location, dpi=self.plotDPI)
                 print(f'...Figure saved at {location}')
 
         # return the figure and axes and the projected RGB
         if returnRGB:
             if proj.lower() == 'none':
                 if proj.lower() == 'none' and returnTransitionFlag:
                     return rgb_new, rgb_extent, transitionFlag
@@ -920,15 +955,15 @@
 
         # Calculate the midpoint of the latitude and longitude
         lat0 = 1/2.*(mn_lat+mx_lat)
         # if the transitionFlag is True, calculate the midpoint of the longitude using the cosine of the longitude
         lon0 = 1/2.*(mn_lon+mx_lon)
 
         # Set the size of the new projected image
-        x_new = proj_size[1]
+        x_new = proj_size[0]
         y_new = proj_size[0]
 
         # Create 1D arrays of evenly spaced values between the min and max longitude and latitude
         xx = np.linspace(mn_lon,mx_lon,x_new)
         yy = np.linspace(mn_lat,mx_lat,y_new)
 
         # Create a 2D grid of coordinates
```

### Comparing `nasa_pace_data_reader-0.0.4.9/src/nasa_pace_data_reader.egg-info/PKG-INFO` & `nasa_pace_data_reader-0.0.5.0/src/nasa_pace_data_reader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nasa_pace_data_reader
-Version: 0.0.4.9
+Version: 0.0.5.0
 Summary: A package for reading NASA PACE data files.
 Author-email: Anin Puthukkudy <aputhukkudy@umbc.edu>
 Project-URL: Homepage, https://github.com/aninramesh/nasa-pace-data-reader
 Project-URL: Issues, https://github.com/aninramesh/nasa-pace-data-reader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -132,15 +132,21 @@
 plt_.projectVar('u',  viewAngle=-35)
 
 ```
 ---
 
 ## Change Log:
 ---
-### v0.0.4.9
+### v0.0.5.0
+- Apply this version for data from OBDAAC that is after April 11th, 2024.
+- Updated OCI L1C variable names to ensure consistency with all other instruments.
+- Resolved the projection issue with SPEXOne data.
+- Option to read HARP2 (GRASP-Anin) L2 product has been added. See `Examples/L2-HARP2-GRASP-example.py` to understand how it can be used.
+
+### v0.0.4.10
 - Fixed the projection issue at -180 to 180 longitude transition line
 
 ### v0.0.4.8
 - Added option to plot `highRes` blue marble
 
 ### v0.0.4.7
 - The bug concerning the `projectRGB()` function has been resolved. Users can now input `float` values for `normFactor` and `scale`, whereas previously only `int` values were permitted. (Issue: https://github.com/aninramesh/nasa-pace-data-reader/issues/2)
```

