# Comparing `tmp/lkcom-0.5.3.tar.gz` & `tmp/lkcom-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkcom-0.5.3.tar", last modified: Tue Mar  5 10:31:34 2024, max compression
+gzip compressed data, was "lkcom-0.5.4.tar", last modified: Tue Apr 16 13:05:56 2024, max compression
```

## Comparing `lkcom-0.5.3.tar` & `lkcom-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 10:31:34.901710 lkcom-0.5.3/
--rw-rw-rw-   0        0        0      897 2024-03-05 10:31:34.899710 lkcom-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-05 10:31:34.882711 lkcom-0.5.3/lkcom/
--rw-rw-rw-   0        0        0      188 2024-03-05 10:31:00.000000 lkcom-0.5.3/lkcom/__init__.py
--rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.5.3/lkcom/cfgparse.py
--rw-rw-rw-   0        0        0    35878 2024-01-08 15:02:59.000000 lkcom-0.5.3/lkcom/dataio.py
--rw-rw-rw-   0        0        0    18170 2023-11-30 15:43:56.000000 lkcom-0.5.3/lkcom/image.py
--rw-rw-rw-   0        0        0    57876 2024-03-05 10:19:05.000000 lkcom-0.5.3/lkcom/plot.py
--rw-rw-rw-   0        0        0     4783 2023-12-12 07:46:12.000000 lkcom-0.5.3/lkcom/standard_func.py
--rw-rw-rw-   0        0        0    26770 2023-12-12 07:55:58.000000 lkcom-0.5.3/lkcom/string.py
--rw-rw-rw-   0        0        0    35143 2024-01-02 14:34:51.000000 lkcom-0.5.3/lkcom/util.py
-drwxrwxrwx   0        0        0        0 2024-03-05 10:31:34.898711 lkcom-0.5.3/lkcom.egg-info/
--rw-rw-rw-   0        0        0      897 2024-03-05 10:31:34.000000 lkcom-0.5.3/lkcom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-03-05 10:31:34.000000 lkcom-0.5.3/lkcom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 10:31:34.000000 lkcom-0.5.3/lkcom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-03-05 10:31:34.000000 lkcom-0.5.3/lkcom.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-05 10:31:34.000000 lkcom-0.5.3/lkcom.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-05 10:31:34.901710 lkcom-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:56.220362 lkcom-0.5.4/
+-rw-rw-rw-   0        0        0      897 2024-04-16 13:05:56.219363 lkcom-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2021-11-15 10:30:15.000000 lkcom-0.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:56.208365 lkcom-0.5.4/lkcom/
+-rw-rw-rw-   0        0        0      188 2024-04-16 13:03:55.000000 lkcom-0.5.4/lkcom/__init__.py
+-rw-rw-rw-   0        0        0     3183 2023-03-01 07:58:13.000000 lkcom-0.5.4/lkcom/cfgparse.py
+-rw-rw-rw-   0        0        0    35878 2024-01-08 15:02:59.000000 lkcom-0.5.4/lkcom/dataio.py
+-rw-rw-rw-   0        0        0    18170 2023-11-30 15:43:56.000000 lkcom-0.5.4/lkcom/image.py
+-rw-rw-rw-   0        0        0    58679 2024-04-16 10:59:39.000000 lkcom-0.5.4/lkcom/plot.py
+-rw-rw-rw-   0        0        0     4783 2023-12-12 07:46:12.000000 lkcom-0.5.4/lkcom/standard_func.py
+-rw-rw-rw-   0        0        0    26770 2023-12-12 07:55:58.000000 lkcom-0.5.4/lkcom/string.py
+-rw-rw-rw-   0        0        0    35331 2024-03-19 08:02:01.000000 lkcom-0.5.4/lkcom/util.py
+drwxrwxrwx   0        0        0        0 2024-04-16 13:05:56.218366 lkcom-0.5.4/lkcom.egg-info/
+-rw-rw-rw-   0        0        0      897 2024-04-16 13:05:56.000000 lkcom-0.5.4/lkcom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-04-16 13:05:56.000000 lkcom-0.5.4/lkcom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 13:05:56.000000 lkcom-0.5.4/lkcom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-16 13:05:56.000000 lkcom-0.5.4/lkcom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 13:05:56.000000 lkcom-0.5.4/lkcom.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 13:05:56.221363 lkcom-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1327 2022-12-15 15:01:50.000000 lkcom-0.5.4/setup.py
```

### Comparing `lkcom-0.5.3/PKG-INFO` & `lkcom-0.5.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.5.3/lkcom/cfgparse.py` & `lkcom-0.5.4/lkcom/cfgparse.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.5.3/lkcom/dataio.py` & `lkcom-0.5.4/lkcom/dataio.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.5.3/lkcom/image.py` & `lkcom-0.5.4/lkcom/image.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.5.3/lkcom/plot.py` & `lkcom-0.5.4/lkcom/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,15 @@
 
 def imshow_ex(
         img, ax=None,
         vmin=None, vmax=None, vrng_algorithm='minmax', min_vspan=None,
         vrng_symmetric=False,
         auto_vrng_percentile_min=0, auto_vrng_percentile_max=99.5,
         bad_color=no_signal_color, logscale=False, cmap='viridis',
-        with_hist=True, hist_color=None,
+        with_hist=True, hist_color=None, show_full_hist=False,
         title_str=None, is_angle=False,
         export_img=False,
         img_file_name='image.png',
         **kwargs):
     """Show an image with a histogram and colorbar.
 
     TODO: ShowImage says it does the same, integrate the two.
@@ -555,22 +555,38 @@
 
     img_bb = ax.get_position().bounds
     img_x = img_bb[0]
     img_y = img_bb[1]
     img_w = img_bb[2]
     img_h = img_bb[3]
 
+
     if with_hist:
         hist_bb = (img_bb[0], img_bb[1] - img_h*0.11, img_bb[2], img_h*0.1)
         plt.axes(hist_bb)
 
         bins = np.linspace(vmin, vmax, 50)
 
+        if show_full_hist:
+            # Show the full histrogram using the same bin step. This makes it
+            # easy to see how much of the data range is the image actually
+            # showing. This doesn't work with current colormap display though.
+            print("WARNING: show_full_hist is an experimental feature, the histogram x limits and the image colorbar are now out-of-sync")
+            img_min = np.nanmin(img)
+            img_max = np.nanmax(img)
+            plt.hist(img.flatten(), bins=np.arange(img_min, img_max, np.mean(np.diff(bins))), log=True, orientation="vertical", color='gray')
         plt.hist(img.flatten(), bins=bins, log=True, orientation="vertical", color=hist_color)
-        plt.xlim([vmin, vmax])
+
+        if show_full_hist:
+            add_x_marker(vmin)
+            add_x_marker(vmax)
+            plt.xlim([img_min, img_max])
+        else:
+            plt.xlim([vmin, vmax])
+
         hide_axes()
 
     cbar_bb = np.array(cbar_ax.get_position().bounds)
     cbar_bb[0] = img_x
     cbar_bb[1] = img_y - cbar_bb[3] - img_h*0.02
     cbar_bb[2] = img_w
```

### Comparing `lkcom-0.5.3/lkcom/standard_func.py` & `lkcom-0.5.4/lkcom/standard_func.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.5.3/lkcom/string.py` & `lkcom-0.5.4/lkcom/string.py`

 * *Files identical despite different names*

### Comparing `lkcom-0.5.3/lkcom/util.py` & `lkcom-0.5.4/lkcom/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 Copyright 2015-2023 Lukas Kontenis
 Contact: dse.ssd@gmail.com
 """
 import os
 import sys
 import time
+import datetime
 
 import numpy as np
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.pyplot import get_cmap
 
 
 class MultiPrinter(object):
@@ -291,15 +292,18 @@
 
     if isarray(val):
         return [find_closest(arr, val1) for val1 in val]
     else:
         if val is None:
             return None
         else:
-            return np.nanargmin((arr-val)**2)
+            if isinstance(val, datetime.datetime):
+                return np.nanargmin(np.array([delta.total_seconds() for delta in arr-val])**2)
+            else:
+                return np.nanargmin((arr-val)**2)
 
 
 def interp(xval, xarr, yarr):
     """1D interpolation for increasing or decreasing xarr."""
     if (np.diff(xarr) > 0).all():
         return np.interp(xval, xarr, yarr)
     elif (np.diff(xarr) < 0).all():
```

### Comparing `lkcom-0.5.3/lkcom.egg-info/PKG-INFO` & `lkcom-0.5.4/lkcom.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkcom
-Version: 0.5.3
+Version: 0.5.4
 Summary: A Python library of useful routines.
 Home-page: https://bitbucket.org/lukaskontenis/lkcom/
 Author: Lukas Kontenis
 Author-email: dse.ssd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lkcom-0.5.3/setup.py` & `lkcom-0.5.4/setup.py`

 * *Files identical despite different names*

