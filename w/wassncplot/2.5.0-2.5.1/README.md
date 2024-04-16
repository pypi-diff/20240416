# Comparing `tmp/wassncplot-2.5.tar.gz` & `tmp/wassncplot-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-0udbdbcl/wassncplot-2.5.tar", last modified: Fri Apr 12 21:50:42 2024, max compression
+gzip compressed data, was "/home/fibe/projects/wassncplot/dist/.tmp-mx_jjtzu/wassncplot-2.5.1.tar", last modified: Tue Apr 16 12:39:45 2024, max compression
```

## Comparing `wassncplot-2.5.tar` & `wassncplot-2.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 21:50:42.788569 wassncplot-2.5/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-12 21:50:42.788569 wassncplot-2.5/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.5/README.md
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.5/pyproject.toml
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-12 21:50:42.788569 wassncplot-2.5/setup.cfg
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 21:50:42.784569 wassncplot-2.5/src/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 21:50:42.784569 wassncplot-2.5/src/wassncplot/
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 21:50:42.784569 wassncplot-2.5/src/wassncplot/WaveFieldVisualize/
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.5/src/wassncplot/WaveFieldVisualize/__init__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.5/src/wassncplot/WaveFieldVisualize/waveview2.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.5/src/wassncplot/__init.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.5/src/wassncplot/__main__.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.5/src/wassncplot/wassncplot.py
--rw-rw-r--   0 fibe      (1000) fibe      (1000)    13287 2024-04-12 21:49:57.000000 wassncplot-2.5/src/wassncplot/wassncplot2.py
-drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-12 21:50:42.788569 wassncplot-2.5/src/wassncplot.egg-info/
--rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/PKG-INFO
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/SOURCES.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/dependency_links.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/entry_points.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/requires.txt
--rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-12 21:50:42.000000 wassncplot-2.5/src/wassncplot.egg-info/top_level.txt
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-16 12:39:45.723531 wassncplot-2.5.1/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     4808 2024-04-08 09:41:38.000000 wassncplot-2.5.1/README.md
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     1214 2022-09-21 13:02:46.000000 wassncplot-2.5.1/pyproject.toml
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       38 2024-04-16 12:39:45.723531 wassncplot-2.5.1/setup.cfg
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.719531 wassncplot-2.5.1/src/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot/
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        0 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/__init__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     8284 2024-04-08 09:41:38.000000 wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/waveview2.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       32 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/__init.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       91 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/__main__.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)     6750 2022-09-01 10:26:19.000000 wassncplot-2.5.1/src/wassncplot/wassncplot.py
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)    13861 2024-04-16 12:31:34.000000 wassncplot-2.5.1/src/wassncplot/wassncplot2.py
+drwxrwxr-x   0 fibe      (1000) fibe      (1000)        0 2024-04-16 12:39:45.723531 wassncplot-2.5.1/src/wassncplot.egg-info/
+-rw-r--r--   0 fibe      (1000) fibe      (1000)     5533 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/PKG-INFO
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      458 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)        1 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       70 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/entry_points.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)      107 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/requires.txt
+-rw-rw-r--   0 fibe      (1000) fibe      (1000)       11 2024-04-16 12:39:45.000000 wassncplot-2.5.1/src/wassncplot.egg-info/top_level.txt
```

### Comparing `wassncplot-2.5/PKG-INFO` & `wassncplot-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.5.0
+Version: 2.5.1
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wassncplot-2.5/README.md` & `wassncplot-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5/pyproject.toml` & `wassncplot-2.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5/src/wassncplot/WaveFieldVisualize/waveview2.py` & `wassncplot-2.5.1/src/wassncplot/WaveFieldVisualize/waveview2.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5/src/wassncplot/wassncplot.py` & `wassncplot-2.5.1/src/wassncplot/wassncplot.py`

 * *Files identical despite different names*

### Comparing `wassncplot-2.5/src/wassncplot/wassncplot2.py` & `wassncplot-2.5.1/src/wassncplot/wassncplot2.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from .WaveFieldVisualize.waveview2 import WaveView
 from tqdm import tqdm
 import sys
 import os
 import argparse
 import glob
 import scipy.io
-from scipy.interpolate import LinearNDInterpolator#, CloughTocher2DInterpolator
+from scipy.interpolate import LinearNDInterpolator, griddata
 
 
-VERSION="2.5.0"
+VERSION="2.5.1"
 
 
 
 def wassncplot_main():
 
     print(" wassncplot v.", VERSION )
     print("=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-\nCopyright (C) Filippo Bergamasco 2024 \n")
@@ -73,14 +73,15 @@
         stereo_baseline = rootgrp["scale"][0]
 
     print("Stereo baseline: ",stereo_baseline, " (use -b option to change)")
     XX = np.array( rootgrp["X_grid"] )/1000.0
     YY = np.array( rootgrp["Y_grid"] )/1000.0
     ZZ = rootgrp["Z"]
 
+    Iw, Ih = rootgrp["meta"].image_width, rootgrp["meta"].image_height
 
     P0plane = None
     P1plane = None
     stereo_image_index = 0
 
     if "P0plane" in rootgrp["meta"].variables:
         P0plane = np.array( rootgrp["meta"]["P0plane"] )
@@ -89,17 +90,24 @@
 
     if "stereo_image_index" in rootgrp["meta"].ncattrs():
         stereo_image_index = rootgrp["meta"].stereo_image_index
 
     print("Rendering frames from camera %d"%stereo_image_index )
     PPlane = P0plane if stereo_image_index == 0 else P1plane
 
+    toNorm = np.array( [[ 2.0/Iw, 0     , -1, 0],
+                        [ 0     , 2.0/Ih, -1, 0],
+                        [ 0,      0,       1, 0],
+                        [ 0,      0,       0, 1]], dtype=float )
+    toNormI = np.linalg.inv(toNorm)
+    Pcam = toNormI @ PPlane 
+
+
     nframes = ZZ.shape[0]
 
-    Iw, Ih = rootgrp["meta"].image_width, rootgrp["meta"].image_height
 
     if args.zmin is None:
         try:
             args.zmin = rootgrp["meta"].zmin
         except:
             print("zmin not specified from command line and not found in NC file, aborting.")
             sys.exit(-1)
@@ -241,28 +249,34 @@
             img[(img.shape[0]-dark_area_h):,:,:] *= 2
 
             texth = 1.5/2048*img.shape[0]
             cv.putText( img, "%s Frame %d"%(args.text_prefix,image_idx), (5,img.shape[0]-5), cv.FONT_HERSHEY_DUPLEX, texth, color=(255,255,255))
 
 
         if draw_marker:
-            def _drawmarker( img, marker_x, marker_y, marker_radius ):
-                aux = np.arange(5,dtype=float)/5.0*np.pi*2
+            def _drawmarker( img, marker_x, marker_y, marker_radius, XX, YY, ZZ, Pcam ):
+                aux = np.arange(50,dtype=float)/50.0*np.pi*2
                 p3d = np.vstack([np.cos(aux)*marker_radius + marker_x, np.sin(aux)*marker_radius + marker_y, aux*0, aux*0+1])
-                toNorm = np.array( [[ 2.0/I0.shape[1], 0     , -1, 0],
-                                    [ 0     , 2.0/I0.shape[0], -1, 0],
-                                    [ 0,      0,       1, 0],
-                                    [ 0,      0,       0, 1]], dtype=float )
-                toNormI = np.linalg.inv(toNorm)
-                p2d = toNormI @ PPlane @ p3d
+
+                XXl = np.expand_dims( XX.flatten(), axis= 1 )
+                YYl = np.expand_dims( YY.flatten(), axis= 1 )
+                points = np.concatenate( [XXl,YYl], axis=-1 )
+                p3d[2,:] = griddata( points, ZZ.flatten(), (p3d[0,:], p3d[1,:]), method='nearest')
+
+                p2d = Pcam @ p3d
                 p2d = p2d[:2,:] / p2d[2,:]
-                ell = cv.fitEllipse( p2d.T.astype(np.float32) )
-                cv.ellipse( img, ell, (0,0,0), 9, cv.LINE_AA )
-                cv.ellipse( img, ell, (255,255,255), 5, cv.LINE_AA )
-            _drawmarker( img, marker_x=markervals[0], marker_y=markervals[1], marker_radius=markervals[2] )
+
+                pline = np.expand_dims(p2d.T, axis=1 )
+
+                cv.polylines( img, [pline.astype(int)], isClosed=True, color=(0,0,0), thickness=9, lineType=cv.LINE_AA )
+                cv.polylines( img, [pline.astype(int)], isClosed=True, color=(255,255,255), thickness=5, lineType=cv.LINE_AA )
+                #ell = cv.fitEllipse( p2d.T.astype(np.float32) )
+                #cv.ellipse( img, ell, (0,0,0), 9, cv.LINE_AA )
+                #cv.ellipse( img, ell, (255,255,255), 5, cv.LINE_AA )
+            _drawmarker( img, marker_x=markervals[0], marker_y=markervals[1], marker_radius=markervals[2], XX=XX, YY=YY, ZZ=ZZ_data, Pcam=Pcam )
             del _drawmarker
 
         cv.imwrite('%s/%08d_grid.png'%(outdir,image_idx), img )
 
         if output_image_size is None:
             output_image_size = (img.shape[1],img.shape[0])
```

### Comparing `wassncplot-2.5/src/wassncplot.egg-info/PKG-INFO` & `wassncplot-2.5.1/src/wassncplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassncplot
-Version: 2.5.0
+Version: 2.5.1
 Summary: WASSncplot is a small tool to plot NetCDF 3D data generated with WASS on top of the original image files.
 Author: Filippo Bergamasco
 Author-email: filippo.bergamasco@unive.it
 License: GPL3
 Project-URL: repository, https://github.com/fbergama/wassncplot
 Keywords: WASS
 Classifier: Programming Language :: Python :: 3
```

