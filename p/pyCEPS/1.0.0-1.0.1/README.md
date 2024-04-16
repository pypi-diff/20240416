# Comparing `tmp/pyCEPS-1.0.0.tar.gz` & `tmp/pyceps-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCEPS-1.0.0.tar", last modified: Wed Apr 10 11:13:06 2024, max compression
+gzip compressed data, was "pyceps-1.0.1.tar", last modified: Tue Apr 16 13:29:18 2024, max compression
```

## Comparing `pyCEPS-1.0.0.tar` & `pyceps-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyCEPS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 11:13:06.000000 pyCEPS-1.0.0/pyCEPS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.758434 pyCEPS-1.0.0/pyceps/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20595 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.758434 pyCEPS-1.0.0/pyceps/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/cartotypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/lesions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/precisiontypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    44950 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    21395 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/datatypes/surface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyceps/fileio/
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104812 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/cartoio.py
--rw-r--r--   0 runner    (1001) docker     (127)    25123 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/cartoutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/igb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/pathtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/precisionio.py
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/precisionutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/fileio/xmlio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/pyceps/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/colormaps.json
--rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashlayout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/pyceps/visualize/dashutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-10 11:12:58.000000 pyCEPS-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 11:13:06.762434 pyCEPS-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-10 11:13:04.000000 pyCEPS-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.232032 pyceps-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-16 13:29:11.000000 pyceps-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 13:29:11.000000 pyceps-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-16 13:29:18.232032 pyceps-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-16 13:29:11.000000 pyceps-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.232032 pyceps-1.0.1/pyCEPS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 13:29:18.000000 pyceps-1.0.1/pyCEPS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.228032 pyceps-1.0.1/pyceps/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20595 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.228032 pyceps-1.0.1/pyceps/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/cartotypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/lesions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/precisiontypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45815 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21395 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/datatypes/surface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.232032 pyceps-1.0.1/pyceps/fileio/
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105485 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/cartoio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25122 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/cartoutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11755 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/igb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11618 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/pathtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/precisionio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/precisionutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/fileio/xmlio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:29:18.232032 pyceps-1.0.1/pyceps/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   231836 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/colormaps.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30885 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/dashapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25578 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/dashelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/dashlayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-16 13:29:11.000000 pyceps-1.0.1/pyceps/visualize/dashutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 13:29:11.000000 pyceps-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:29:18.236033 pyceps-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-16 13:29:16.000000 pyceps-1.0.1/setup.py
```

### Comparing `pyCEPS-1.0.0/LICENSE.txt` & `pyceps-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/PKG-INFO` & `pyceps-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 1.0.0
+Version: 1.0.1
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
+Project-URL: Github, https://github.com/medunigraz/pyCEPS
+Project-URL: Changelog, https://github.com/medunigraz/pyCEPS/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pyCEPS-1.0.0/README.md` & `pyceps-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyCEPS.egg-info/PKG-INFO` & `pyceps-1.0.1/pyCEPS.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: pyCEPS
-Version: 1.0.0
+Version: 1.0.1
 Summary: pyceps provides methods for importing EP studies from commercial Clinical Mapping Systems and to export data to openCARP compatible data formats.
 Home-page: https://github.com/medunigraz/pyCEPS
 Author: Robert Arnold
 Author-email: robert.arnold@medunigraz.at
 License: GPLv3+
+Project-URL: Github, https://github.com/medunigraz/pyCEPS
+Project-URL: Changelog, https://github.com/medunigraz/pyCEPS/blob/main/CHANGELOG.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `pyCEPS-1.0.0/pyCEPS.egg-info/SOURCES.txt` & `pyceps-1.0.1/pyCEPS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/__init__.py` & `pyceps-1.0.1/pyceps/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/cli.py` & `pyceps-1.0.1/pyceps/cli.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/__init__.py` & `pyceps-1.0.1/pyceps/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/cartotypes.py` & `pyceps-1.0.1/pyceps/datatypes/cartotypes.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/lesions.py` & `pyceps-1.0.1/pyceps/datatypes/lesions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/precisiontypes.py` & `pyceps-1.0.1/pyceps/datatypes/precisiontypes.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/signals.py` & `pyceps-1.0.1/pyceps/datatypes/signals.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/study.py` & `pyceps-1.0.1/pyceps/datatypes/study.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,15 @@
             # add surface mesh
             xml_add_binary_surface(proc, cmap.surface)
 
             # add mapping points
             points = ET.SubElement(proc, 'Points',
                                    count=str(len(cmap.points))
                                    )
+            # export data from EPPoint baseclass only
             for key in list(EPPoint('dummy', parent=cmap).__dict__):
                 if key == 'parent':
                     # don't save this
                     continue
 
                 data = [getattr(p, key) for p in cmap.points]
                 # handle maps with no points
@@ -569,15 +570,16 @@
         Create surface parameter maps by interpolating EGM data on mesh
         surface points.
 
         Surface maps are added to the surface.
 
         Parameters:
             which : str
-                parameter to interpolate, options: ['uni', 'bip', 'act']
+                parameter to interpolate
+                options: ['uni', 'bip', 'lat', 'imp', 'frc']
 
         Raises:
             KeyError : If parameter to interpolate is unknown
 
         Returns:
             None
         """
@@ -605,19 +607,37 @@
         if which.lower() == 'lat':
             data = np.asarray([p.latAnnotation - p.refAnnotation
                                for p in valid_points])
         elif which.lower() == 'bip':
             data = np.asarray([p.bipVoltage for p in valid_points])
         elif which.lower() == 'uni':
             data = np.asarray([p.uniVoltage for p in valid_points])
+        elif which.lower() == 'imp':
+            data = np.asarray([p.impedance for p in valid_points])
+        elif which.lower() == 'frc':
+            data = np.asarray([p.force for p in valid_points])
         else:
             raise KeyError()
 
+        # check if there is data for interpolation
+        if np.isnan(data).all():
+            log.debug('found only NaN in data, cannot interpolate map {}'
+                      .format(which.upper())
+                      )
+            return
+
+        # remove data for redundant points
+        data = data[unique_ids]
+        # remove any points with NaN's before interpolation
+        mask = ~np.isnan(data)
+        data = data[mask]
+        unique_points = unique_points[mask]
+
         interpolated = inverse_distance_weighting(unique_points,
-                                                  data[unique_ids],
+                                                  data,
                                                   mesh_points,
                                                   k=7)
 
         # adjust array dims for compatibility
         interpolated = np.expand_dims(interpolated, 1)
 
         surf_map = SurfaceSignalMap(name=which.upper(),
@@ -834,23 +854,25 @@
                     for point in points]
             dat_file = basename + '.ptdata.LAT.pc.dat'
             writer.dump(dat_file, data)
             log.info('exported point data to {}'.format(dat_file))
 
         if "IMP" in which:
             data = [point.impedance for point in points]
-            dat_file = basename + '.ptdata.IMP.pc.dat'
-            writer.dump(dat_file, data)
-            log.info('exported point data to {}'.format(dat_file))
+            if not np.isnan(data).all():
+                dat_file = basename + '.ptdata.IMP.pc.dat'
+                writer.dump(dat_file, data)
+                log.info('exported point data to {}'.format(dat_file))
 
         if "FRC" in which:
             data = [point.force for point in points]
-            dat_file = basename + '.ptdata.FRC.pc.dat'
-            writer.dump(dat_file, data)
-            log.info('exported point data to {}'.format(dat_file))
+            if not np.isnan(data).all():
+                dat_file = basename + '.ptdata.FRC.pc.dat'
+                writer.dump(dat_file, data)
+                log.info('exported point data to {}'.format(dat_file))
 
         return
 
     def export_point_info(self, basename='', points=None):
         """
         Export additional point info.
```

### Comparing `pyCEPS-1.0.0/pyceps/datatypes/surface.py` & `pyceps-1.0.1/pyceps/datatypes/surface.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/exceptions.py` & `pyceps-1.0.1/pyceps/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/__init__.py` & `pyceps-1.0.1/pyceps/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/cartoio.py` & `pyceps-1.0.1/pyceps/fileio/cartoio.py`

 * *Files 0% similar despite different names*

```diff
@@ -661,15 +661,15 @@
         self.name = root.get('name')
         self.studyXML = root.get('studyXML')
         units = root.find('Units')
         self.units = CartoUnits(units.get('distance'), units.get('angle'))
 
         # load additional meshes
         mesh_item = root.find('AdditionalMeshes')
-        if int(mesh_item.get('count')) > 0:
+        if mesh_item:
             _, reg_matrix = xml_load_binary_data(
                 [x for x in mesh_item.findall('DataArray')
                  if x.get('name') == 'registrationMatrix'][0]
             )
             _, file_names = xml_load_binary_data(
                 [x for x in mesh_item.findall('DataArray')
                  if x.get('name') == 'fileNames'][0]
@@ -702,32 +702,33 @@
             new_map.lesions = xml_load_binary_lesion(proc.find('Lesions'))
 
             # load EGM points
             p_data = {}
             points_item = proc.find('Points')
             num_points = int(points_item.get('count'))
 
-            for arr in points_item.findall('DataArray'):
-                d_name, data = xml_load_binary_data(arr)
-                p_data[d_name] = data
-            for arr in points_item.findall('Traces'):
-                d_name, data = xml_load_binary_trace(arr)
-                p_data[d_name] = data
-
-            points = []
-            for i in range(num_points):
-                new_point = CartoPoint('dummy', parent=new_map)
-                for key, value in p_data.items():
-                    if hasattr(new_point, key):
-                        setattr(new_point, key, value[i])
-                    else:
-                        log.warning('cannot set attribute "{}" for CartoPoint'
-                                    .format(key))
-                points.append(new_point)
-            new_map.points = points
+            if num_points > 0:
+                for arr in points_item.findall('DataArray'):
+                    d_name, data = xml_load_binary_data(arr)
+                    p_data[d_name] = data
+                for arr in points_item.findall('Traces'):
+                    d_name, data = xml_load_binary_trace(arr)
+                    p_data[d_name] = data
+
+                points = []
+                for i in range(num_points):
+                    new_point = CartoPoint('dummy', parent=new_map)
+                    for key, value in p_data.items():
+                        if hasattr(new_point, key):
+                            setattr(new_point, key, value[i])
+                        else:
+                            log.warning('cannot set attribute "{}" for CartoPoint'
+                                        .format(key))
+                    points.append(new_point)
+                new_map.points = points
 
             # now we can add the procedure to the study
             self.maps[name] = new_map
 
         # try to set root if explicitly given
         if repo_path:
             if self.set_repository(os.path.abspath(repo_path)):
@@ -1189,14 +1190,16 @@
         self.points = self.load_points(
             study_tags=self.parent.mappingParams.TagsTable,
             egm_names_from_pos=egm_names_from_pos)
         # build surface maps
         self.interpolate_data('lat')
         self.interpolate_data('bip')
         self.interpolate_data('uni')
+        self.interpolate_data('imp')
+        self.interpolate_data('frc')
         self.bsecg = self.get_map_ecg(method=['median', 'mse', 'ccf'])
 
     def load_mesh(self):
         """
         Load a Carto3 triangulated anatomical shell from file. Overrides
         BaseClass method.
 
@@ -1951,16 +1954,18 @@
         uniX : ndarray (3, )
             cartesian coordinates of the second unipolar recording electrode
             NOTE: coordinates of second unipolar electrode are same as recX if
             position cannot be determined
         forceFile : str
             name of the points contact force file
             <map_name>_<point_name>_Contact_Force.txt
-        force : PointForce
-            contact force data for this point
+        forceData : PointForce
+            full contact force data for this point
+        impedanceData : PointImpedance
+            full impedance data for this point
 
     Methods:
         is_valid()
             check if point has LAT annotation within WOI
         load(egm_names_from_pos=False)
             load all data associated with this point
         import_ecg(channel_names)
@@ -1993,18 +1998,19 @@
 
         super().__init__(name, coordinates=coordinates, parent=parent)
 
         # add Carto3 specific attributes
         self.pointFile = ''
         self.barDirection = None
         self.tags = tags
-        self.ecgFile = None
+        self.ecgFile = ''
         self.uniX = np.full(3, np.nan, dtype=np.float32)
-        self.forceFile = None
+        self.forceFile = ''
         self.forceData = None
+        self.impedanceData = None
 
     def import_point(self, point_file, egm_names_from_pos=False):
         """
         Load data associated with this point.
 
         Parameters:
             point_file : str
@@ -2054,16 +2060,20 @@
         if n_impedance_values > 0:
             impedance_value = np.empty(n_impedance_values, dtype=np.float32)
             impedance_time = np.empty(n_impedance_values, dtype=np.float32)
             for i, x in enumerate(impedance_item.findall('Impedance')):
                 impedance_time[i] = x.get('Time')
                 impedance_value[i] = x.get('Value')
 
-            self.impedance = PointImpedance(time=impedance_time,
-                                            value=impedance_value)
+            self.impedanceData = PointImpedance(time=impedance_time,
+                                                value=impedance_value)
+            # update base class impedance value with the one closest to LAT
+            self.impedance = impedance_value[
+                np.nanargmin(np.abs(impedance_time - self.latAnnotation))
+            ]
 
         self.ecgFile = root.find('ECG').get('FileName')
 
         # get egm names from ECG file
         ecg_file = self.parent.parent.repository.join(self.ecgFile)
         with self.parent.parent.repository.open(ecg_file) as fid:
             ecg_file_header = read_ecg_file_header(
@@ -2121,27 +2131,28 @@
                             .format(self.name, closest))
             self.prjX = np.array(closest[0], dtype=np.float32)
             self.prjDistance = distance[0]
             self.barDirection = direct[0]
 
         # now get the force data for this point
         log.debug('reading force file for point {}'.format(self.name))
-        self.forceFile = (self.pointFile.split('_Point_Export')[0]
-                          + '_ContactForce.txt'
-                          )
-
-        if self.parent.parent.repository.is_file(self.forceFile):
-            with self.parent.parent.repository.open(self.forceFile) as fid:
-                self.forceData = read_force_file(
-                    fid, encoding=self.parent.parent.encoding
-                )
-            # update base class force value
-            self.force = self.forceData.force
-        else:
-            log.debug('No force file found for point {}'.format(self.name))
+        try:
+            self.forceFile = root.find('ContactForce').get('FileName')
+            force_file = self.parent.parent.repository.join(self.forceFile)
+            if self.parent.parent.repository.is_file(force_file):
+                with self.parent.parent.repository.open(force_file) as fid:
+                    self.forceData = read_force_file(
+                        fid, encoding=self.parent.parent.encoding
+                    )
+                # update base class force value with the one closest to LAT
+                self.force = self.forceData.force
+            else:
+                log.debug('No force file found for point {}'.format(self.name))
+        except AttributeError:
+            log.debug('No force data saved for point {}'.format(self.name))
 
     def is_valid(self):
         """
         Check if LAT annotation is within the WOI.
 
         Raises:
             ValueError : If no WOI or reference annotation is found or there
```

### Comparing `pyCEPS-1.0.0/pyceps/fileio/cartoutils.py` & `pyceps-1.0.1/pyceps/fileio/cartoutils.py`

 * *Files identical despite different names*

```diff
@@ -522,15 +522,14 @@
                   'lateralAngle': np.nan,
                   't_time': np.empty(0),
                   't_force': np.empty(0),
                   't_axialAngle': np.empty(0),
                   't_lateralAngle': np.empty(0),
                   'systemTime': np.empty(0)}
 
-
     # read file version
     version = fid.readline().decode(encoding=encoding).rstrip()
     if not version.lower().endswith('contactforce.txt_2.0'):
         log.warning('version in Carto3 point force file is not supported')
         return PointForces()
 
     line = fid.readline().decode(encoding=encoding).rstrip()
```

### Comparing `pyCEPS-1.0.0/pyceps/fileio/igb.py` & `pyceps-1.0.1/pyceps/fileio/igb.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/pathtools.py` & `pyceps-1.0.1/pyceps/fileio/pathtools.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/precisionio.py` & `pyceps-1.0.1/pyceps/fileio/precisionio.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/precisionutils.py` & `pyceps-1.0.1/pyceps/fileio/precisionutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/writer.py` & `pyceps-1.0.1/pyceps/fileio/writer.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/fileio/xmlio.py` & `pyceps-1.0.1/pyceps/fileio/xmlio.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/interpolation.py` & `pyceps-1.0.1/pyceps/interpolation.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/utils.py` & `pyceps-1.0.1/pyceps/utils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/__init__.py` & `pyceps-1.0.1/pyceps/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/colormaps.json` & `pyceps-1.0.1/pyceps/visualize/colormaps.json`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/dashapp.py` & `pyceps-1.0.1/pyceps/visualize/dashapp.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/dashelements.py` & `pyceps-1.0.1/pyceps/visualize/dashelements.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/dashlayout.py` & `pyceps-1.0.1/pyceps/visualize/dashlayout.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/pyceps/visualize/dashutils.py` & `pyceps-1.0.1/pyceps/visualize/dashutils.py`

 * *Files identical despite different names*

### Comparing `pyCEPS-1.0.0/setup.py` & `pyceps-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,19 @@
                'openCARP compatible data formats.'
                )
 LICENSE = 'GPLv3+'
 URL = 'https://github.com/medunigraz/pyCEPS'
 EMAIL = 'robert.arnold@medunigraz.at'
 AUTHOR = 'Robert Arnold'
 REQUIRES_PYTHON = '>=3.8'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
+PROJECT_URLS = {
+    'Github': 'https://github.com/medunigraz/pyCEPS',
+    'Changelog': 'https://github.com/medunigraz/pyCEPS/blob/main/CHANGELOG.md',
+}
 CLASSIFIERS = [
     # Trove classifiers
     # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
     'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
@@ -91,14 +95,15 @@
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
+    project_urls=PROJECT_URLS,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['pyceps'],
     entry_points={
         # command = package.module:function
         'console_scripts': ['pyceps=pyceps.cli:run'],
     },
```

