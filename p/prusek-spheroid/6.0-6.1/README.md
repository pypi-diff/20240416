# Comparing `tmp/prusek_spheroid-6.0.tar.gz` & `tmp/prusek_spheroid-6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-6.0.tar", last modified: Tue Apr 16 09:42:59 2024, max compression
+gzip compressed data, was "prusek_spheroid-6.1.tar", last modified: Tue Apr 16 09:56:05 2024, max compression
```

## Comparing `prusek_spheroid-6.0.tar` & `prusek_spheroid-6.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.459338 prusek_spheroid-6.0/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:42:59.459020 prusek_spheroid-6.0/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-6.0/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.457719 prusek_spheroid-6.0/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    18855 2024-04-16 09:42:50.000000 prusek_spheroid-6.0/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-6.0/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-6.0/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-6.0/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-6.0/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-6.0/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-6.0/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-6.0/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-6.0/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-6.0/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-6.0/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.458806 prusek_spheroid-6.0/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-16 09:42:59.459389 prusek_spheroid-6.0/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-16 09:42:55.000000 prusek_spheroid-6.0/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:56:05.226139 prusek_spheroid-6.1/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:56:05.225909 prusek_spheroid-6.1/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-6.1/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:56:05.224461 prusek_spheroid-6.1/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    18599 2024-04-16 09:54:39.000000 prusek_spheroid-6.1/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-6.1/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-6.1/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-6.1/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-6.1/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-6.1/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-6.1/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-6.1/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-6.1/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-6.1/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-6.1/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:56:05.225691 prusek_spheroid-6.1/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:56:05.000000 prusek_spheroid-6.1/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-16 09:56:05.000000 prusek_spheroid-6.1/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-16 09:56:05.000000 prusek_spheroid-6.1/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-16 09:56:05.000000 prusek_spheroid-6.1/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-16 09:56:05.000000 prusek_spheroid-6.1/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-16 09:56:05.226184 prusek_spheroid-6.1/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-16 09:55:39.000000 prusek_spheroid-6.1/setup.py
```

### Comparing `prusek_spheroid-6.0/PKG-INFO` & `prusek_spheroid-6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 6.0
+Version: 6.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-6.0/README.md` & `prusek_spheroid-6.1/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-6.1/prusek_spheroid/ContoursClassGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,21 +45,14 @@
 
         current_dir = os.path.dirname(os.path.abspath(__file__))
         try:
 
             model_path = os.path.join(current_dir, 'gradient_boosting_classifier.joblib')
             scaler_path = os.path.join(current_dir, 'scaler.joblib')
 
-            # Normalize the paths to ensure they are correct
-            print(f"pred1: {model_path}")
-            model_path = os.path.normpath(model_path)
-            print(f"pred2: {model_path}")
-            model_path = model_path.replace("\\\\", "\\")
-            print(f'pred3: {model_path}')
-            scaler_path = os.path.normpath(scaler_path)
             # Load the model and scaler
             self.model = joblib.load(model_path)
             self.scaler = joblib.load(scaler_path)
         except Exception as e:
             print(f"Loading from primary location failed: {e}")
 
         fm.create_directory(os.path.dirname(self.output_json_path), delete=True)
@@ -134,14 +127,15 @@
                             img_with):
                         print(
                             f"FAILED to save image: {os.path.join(self.output_segmented_path, 'results', filename.replace('.bmp', '.png'))}")
 
                 else:
                     img_without = img.copy()
                     mask_without = np.zeros_like(img_gray)
+                    mask_with = np.zeros_like(img_gray)
 
                     for contour in outer_contours:
                         contour = np.array(contour, dtype=np.int32)
                         cv.fillPoly(mask_without, [contour], 255)
 
                     if self.contours_state == "all" or self.contours_state == "select":
                         inner_mask = np.zeros_like(img_gray)
@@ -157,15 +151,16 @@
                         # Subtract intersection from the outer contours mask
                         mask_with = mask_without - intersection
 
                         for contour in inner_contours:
                             cv.drawContours(img_with, [contour], -1, (255, 0, 0), 2)
 
                     for index, contour in enumerate(outer_contours):
-                        contour_budding = self.evaluate(contour)
+                        if self.model:
+                            contour_budding = self.evaluate(contour)
 
                         if not contour_budding == "no_split":
                             color = (0, 255, 0)
                         else:
                             color = (0, 0, 255)
 
                         if self.contours_state == "all":
```

### Comparing `prusek_spheroid-6.0/prusek_spheroid/GUI.py` & `prusek_spheroid-6.1/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-6.1/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-6.1/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/conversion.py` & `prusek_spheroid-6.1/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/file_management.py` & `prusek_spheroid-6.1/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/image_processing.py` & `prusek_spheroid-6.1/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/merge_directories.py` & `prusek_spheroid-6.1/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/methods.py` & `prusek_spheroid-6.1/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/metrics.py` & `prusek_spheroid-6.1/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-6.1/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-6.1/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 6.0
+Version: 6.1
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-6.0/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-6.1/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-6.0/setup.py` & `prusek_spheroid-6.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="6.0",
+    version="6.1",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

