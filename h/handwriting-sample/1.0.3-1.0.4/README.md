# Comparing `tmp/handwriting-sample-1.0.3.tar.gz` & `tmp/handwriting-sample-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handwriting-sample-1.0.3.tar", last modified: Fri Nov  3 21:40:50 2023, max compression
+gzip compressed data, was "handwriting-sample-1.0.4.tar", last modified: Mon Apr 15 23:29:42 2024, max compression
```

## Comparing `handwriting-sample-1.0.3.tar` & `handwriting-sample-1.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.638106 handwriting-sample-1.0.3/
--rw-r--r--   0 jano       (501) staff       (20)     1091 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/LICENSE
--rw-r--r--   0 jano       (501) staff       (20)       25 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/MANIFEST.in
--rw-r--r--   0 jano       (501) staff       (20)    15841 2023-11-03 21:40:50.637853 handwriting-sample-1.0.3/PKG-INFO
--rw-r--r--   0 jano       (501) staff       (20)    15046 2023-11-03 20:50:35.000000 handwriting-sample-1.0.3/README.md
--rw-r--r--   0 jano       (501) staff       (20)       38 2023-11-03 21:40:50.638143 handwriting-sample-1.0.3/setup.cfg
--rw-r--r--   0 jano       (501) staff       (20)     1322 2023-11-03 21:37:22.000000 handwriting-sample-1.0.3/setup.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.630395 handwriting-sample-1.0.3/src/
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.632509 handwriting-sample-1.0.3/src/handwriting_sample/
--rw-r--r--   0 jano       (501) staff       (20)      103 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/__init__.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.634316 handwriting-sample-1.0.3/src/handwriting_sample/base/
--rw-r--r--   0 jano       (501) staff       (20)       83 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/base/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)     1202 2023-11-03 21:10:42.000000 handwriting-sample-1.0.3/src/handwriting_sample/base/containers.py
--rw-r--r--   0 jano       (501) staff       (20)      894 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/base/utils.py
--rw-r--r--   0 jano       (501) staff       (20)        1 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)    24530 2023-11-03 21:25:23.000000 handwriting-sample-1.0.3/src/handwriting_sample/interface.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.635139 handwriting-sample-1.0.3/src/handwriting_sample/reader/
--rw-r--r--   0 jano       (501) staff       (20)      122 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/reader/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)     1110 2023-11-03 15:58:30.000000 handwriting-sample-1.0.3/src/handwriting_sample/reader/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)     3895 2023-11-03 19:02:08.000000 handwriting-sample-1.0.3/src/handwriting_sample/reader/interface.py
--rw-r--r--   0 jano       (501) staff       (20)    10234 2023-11-03 21:13:02.000000 handwriting-sample-1.0.3/src/handwriting_sample/reader/readers.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.635735 handwriting-sample-1.0.3/src/handwriting_sample/transformer/
--rw-r--r--   0 jano       (501) staff       (20)      138 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/transformer/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)     1083 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/transformer/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)    17534 2023-11-03 20:27:39.000000 handwriting-sample-1.0.3/src/handwriting_sample/transformer/interface.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.636369 handwriting-sample-1.0.3/src/handwriting_sample/validator/
--rw-r--r--   0 jano       (501) staff       (20)      132 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/validator/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)      797 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/validator/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)     4726 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/validator/interface.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.636808 handwriting-sample-1.0.3/src/handwriting_sample/visualizer/
--rw-r--r--   0 jano       (501) staff       (20)      134 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/visualizer/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)        0 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/visualizer/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)    11252 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/visualizer/interface.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.637583 handwriting-sample-1.0.3/src/handwriting_sample/writer/
--rw-r--r--   0 jano       (501) staff       (20)      123 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/writer/__init__.py
--rw-r--r--   0 jano       (501) staff       (20)        0 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/writer/exceptions.py
--rw-r--r--   0 jano       (501) staff       (20)     5621 2023-11-03 19:09:54.000000 handwriting-sample-1.0.3/src/handwriting_sample/writer/interface.py
--rw-r--r--   0 jano       (501) staff       (20)     1285 2023-10-26 12:27:05.000000 handwriting-sample-1.0.3/src/handwriting_sample/writer/writers.py
-drwxr-xr-x   0 jano       (501) staff       (20)        0 2023-11-03 21:40:50.633758 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/
--rw-r--r--   0 jano       (501) staff       (20)    15841 2023-11-03 21:40:50.000000 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/PKG-INFO
--rw-r--r--   0 jano       (501) staff       (20)     1257 2023-11-03 21:40:50.000000 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/SOURCES.txt
--rw-r--r--   0 jano       (501) staff       (20)        1 2023-11-03 21:40:50.000000 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/dependency_links.txt
--rw-r--r--   0 jano       (501) staff       (20)       24 2023-11-03 21:40:50.000000 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/requires.txt
--rw-r--r--   0 jano       (501) staff       (20)       19 2023-11-03 21:40:50.000000 handwriting-sample-1.0.3/src/handwriting_sample.egg-info/top_level.txt
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.674314 handwriting-sample-1.0.4/
+-rw-r--r--   0 jano       (501) staff       (20)     1091 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/LICENSE
+-rw-r--r--   0 jano       (501) staff       (20)       25 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/MANIFEST.in
+-rw-r--r--   0 jano       (501) staff       (20)    15841 2024-04-15 23:29:42.673980 handwriting-sample-1.0.4/PKG-INFO
+-rw-r--r--   0 jano       (501) staff       (20)    15046 2023-11-03 20:50:35.000000 handwriting-sample-1.0.4/README.md
+-rw-r--r--   0 jano       (501) staff       (20)       38 2024-04-15 23:29:42.674361 handwriting-sample-1.0.4/setup.cfg
+-rw-r--r--   0 jano       (501) staff       (20)     1322 2024-04-15 23:28:49.000000 handwriting-sample-1.0.4/setup.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.665963 handwriting-sample-1.0.4/src/
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.667839 handwriting-sample-1.0.4/src/handwriting_sample/
+-rw-r--r--   0 jano       (501) staff       (20)      103 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/__init__.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.669622 handwriting-sample-1.0.4/src/handwriting_sample/base/
+-rw-r--r--   0 jano       (501) staff       (20)       83 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/base/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)     1202 2023-11-03 21:10:42.000000 handwriting-sample-1.0.4/src/handwriting_sample/base/containers.py
+-rw-r--r--   0 jano       (501) staff       (20)      894 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/base/utils.py
+-rw-r--r--   0 jano       (501) staff       (20)        1 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)    24530 2023-11-03 21:25:23.000000 handwriting-sample-1.0.4/src/handwriting_sample/interface.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.670621 handwriting-sample-1.0.4/src/handwriting_sample/reader/
+-rw-r--r--   0 jano       (501) staff       (20)      122 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/reader/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)     1110 2023-11-03 15:58:30.000000 handwriting-sample-1.0.4/src/handwriting_sample/reader/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)     3895 2023-11-03 19:02:08.000000 handwriting-sample-1.0.4/src/handwriting_sample/reader/interface.py
+-rw-r--r--   0 jano       (501) staff       (20)    11159 2024-04-15 23:21:42.000000 handwriting-sample-1.0.4/src/handwriting_sample/reader/readers.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.671330 handwriting-sample-1.0.4/src/handwriting_sample/transformer/
+-rw-r--r--   0 jano       (501) staff       (20)      138 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/transformer/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)     1083 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/transformer/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)    17534 2023-11-03 20:27:39.000000 handwriting-sample-1.0.4/src/handwriting_sample/transformer/interface.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.672299 handwriting-sample-1.0.4/src/handwriting_sample/validator/
+-rw-r--r--   0 jano       (501) staff       (20)      132 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/validator/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)      797 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/validator/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)     4726 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/validator/interface.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.672845 handwriting-sample-1.0.4/src/handwriting_sample/visualizer/
+-rw-r--r--   0 jano       (501) staff       (20)      134 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/visualizer/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)        0 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/visualizer/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)    11252 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/visualizer/interface.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.673736 handwriting-sample-1.0.4/src/handwriting_sample/writer/
+-rw-r--r--   0 jano       (501) staff       (20)      123 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/writer/__init__.py
+-rw-r--r--   0 jano       (501) staff       (20)        0 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/writer/exceptions.py
+-rw-r--r--   0 jano       (501) staff       (20)     5621 2023-11-03 19:09:54.000000 handwriting-sample-1.0.4/src/handwriting_sample/writer/interface.py
+-rw-r--r--   0 jano       (501) staff       (20)     1285 2023-10-26 12:27:05.000000 handwriting-sample-1.0.4/src/handwriting_sample/writer/writers.py
+drwxr-xr-x   0 jano       (501) staff       (20)        0 2024-04-15 23:29:42.669084 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/
+-rw-r--r--   0 jano       (501) staff       (20)    15841 2024-04-15 23:29:42.000000 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/PKG-INFO
+-rw-r--r--   0 jano       (501) staff       (20)     1257 2024-04-15 23:29:42.000000 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/SOURCES.txt
+-rw-r--r--   0 jano       (501) staff       (20)        1 2024-04-15 23:29:42.000000 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/dependency_links.txt
+-rw-r--r--   0 jano       (501) staff       (20)       24 2024-04-15 23:29:42.000000 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/requires.txt
+-rw-r--r--   0 jano       (501) staff       (20)       19 2024-04-15 23:29:42.000000 handwriting-sample-1.0.4/src/handwriting_sample.egg-info/top_level.txt
```

### Comparing `handwriting-sample-1.0.3/LICENSE` & `handwriting-sample-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/PKG-INFO` & `handwriting-sample-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handwriting-sample
-Version: 1.0.3
+Version: 1.0.4
 Summary: Handwriting sample
 Home-page: https://github.com/BDALab/handwriting-sample
 Author: Brain Diseases Analysis Laboratory
 Author-email: mucha@vut.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `handwriting-sample-1.0.3/README.md` & `handwriting-sample-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/setup.py` & `handwriting-sample-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "pandas",
     "matplotlib"
 ]
 
 # Prepare the setup
 setup(
     name="handwriting-sample",
-    version="1.0.3",
+    version="1.0.4",
     description="Handwriting sample",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BDALab/handwriting-sample",
     author="Brain Diseases Analysis Laboratory",
     author_email="mucha@vut.cz",
     packages=packages,
```

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/base/containers.py` & `handwriting-sample-1.0.4/src/handwriting_sample/base/containers.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/base/utils.py` & `handwriting-sample-1.0.4/src/handwriting_sample/base/utils.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/reader/exceptions.py` & `handwriting-sample-1.0.4/src/handwriting_sample/reader/exceptions.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/reader/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/reader/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/reader/readers.py` & `handwriting-sample-1.0.4/src/handwriting_sample/reader/readers.py`

 * *Files 4% similar despite different names*

```diff
@@ -193,14 +193,16 @@
 
     @classmethod
     def _transform_html_data_to_sample_data(cls,
                                             html_data,
                                             transform_x_y_to_mm=True,
                                             transform_time_to_seconds=True,
                                             transform_tilt_xy_to_azimuth_and_tilt=True,
+                                            revert_y_axis=True,
+                                            transform_pressure=True,
                                             **kwargs):
         """Transforms HTML data to sample data"""
 
         allowed_kwargs = ["time_conversion",
                           "tablet_pixel_resolution",
                           "tablet_mm_dimensions",]
 
@@ -253,14 +255,32 @@
             else:
                 # Default PX to MM
                 px_to_mm = HandwritingSampleTransformer.PX_TO_MM
 
             html_data[cls.HTML_AXIS_X] = [x * px_to_mm for x in html_data.get(cls.HTML_AXIS_X)]
             html_data[cls.HTML_AXIS_Y] = [y * px_to_mm for y in html_data.get(cls.HTML_AXIS_Y)]
 
+        # Revert Y axis
+        if revert_y_axis:
+            # Get max Y value form kwarg, if not set use default
+            max_y_value_mm = kwargs.get("max_y_value_mm", None)
+            if not max_y_value_mm:
+                max_y_value_mm = HandwritingSampleTransformer.DEFAULT_MM_DIMENSIONS[1]
+
+            ax_data = html_data[cls.HTML_AXIS_Y]
+            html_data[cls.HTML_AXIS_Y] = HandwritingSampleTransformer.revert_axis(ax_data, max_y_value_mm)
+
+        # Transform pressure
+        if transform_pressure:
+            pressure_levels = kwargs.get("pressure_levels", None)
+            if not pressure_levels:
+                pressure_levels = HandwritingSampleTransformer.PRESSURE_LEVELS
+
+            html_data[cls.HTML_PRESSURE] = html_data[cls.HTML_PRESSURE] * pressure_levels
+
         # Transform data for Handwriting Sample
         sample_data = {
             "x": html_data.get(cls.HTML_AXIS_X),
             "y": html_data.get(cls.HTML_AXIS_Y),
             "time": html_data.get(cls.HTML_TIME),
             "pen_status": html_data.get(cls.HTML_BUTTONS),
             "azimuth": azimuth,
```

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/transformer/exceptions.py` & `handwriting-sample-1.0.4/src/handwriting_sample/transformer/exceptions.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/transformer/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/transformer/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/validator/exceptions.py` & `handwriting-sample-1.0.4/src/handwriting_sample/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/validator/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/validator/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/visualizer/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/visualizer/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/writer/interface.py` & `handwriting-sample-1.0.4/src/handwriting_sample/writer/interface.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample/writer/writers.py` & `handwriting-sample-1.0.4/src/handwriting_sample/writer/writers.py`

 * *Files identical despite different names*

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample.egg-info/PKG-INFO` & `handwriting-sample-1.0.4/src/handwriting_sample.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: handwriting-sample
-Version: 1.0.3
+Version: 1.0.4
 Summary: Handwriting sample
 Home-page: https://github.com/BDALab/handwriting-sample
 Author: Brain Diseases Analysis Laboratory
 Author-email: mucha@vut.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `handwriting-sample-1.0.3/src/handwriting_sample.egg-info/SOURCES.txt` & `handwriting-sample-1.0.4/src/handwriting_sample.egg-info/SOURCES.txt`

 * *Files identical despite different names*

