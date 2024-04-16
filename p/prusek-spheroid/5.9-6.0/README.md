# Comparing `tmp/prusek_spheroid-5.9.tar.gz` & `tmp/prusek_spheroid-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.9.tar", last modified: Tue Apr 16 09:38:53 2024, max compression
+gzip compressed data, was "prusek_spheroid-6.0.tar", last modified: Tue Apr 16 09:42:59 2024, max compression
```

## Comparing `prusek_spheroid-5.9.tar` & `prusek_spheroid-6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:38:53.615189 prusek_spheroid-5.9/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:38:53.614858 prusek_spheroid-5.9/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-5.9/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:38:53.613433 prusek_spheroid-5.9/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19347 2024-04-16 09:37:57.000000 prusek_spheroid-5.9/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-5.9/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.9/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.9/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.9/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-5.9/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.9/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.9/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.9/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.9/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.9/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:38:53.614637 prusek_spheroid-5.9/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:38:53.000000 prusek_spheroid-5.9/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-16 09:38:53.000000 prusek_spheroid-5.9/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-16 09:38:53.000000 prusek_spheroid-5.9/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-16 09:38:53.000000 prusek_spheroid-5.9/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-16 09:38:53.000000 prusek_spheroid-5.9/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-16 09:38:53.615238 prusek_spheroid-5.9/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-16 09:38:50.000000 prusek_spheroid-5.9/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.459338 prusek_spheroid-6.0/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:42:59.459020 prusek_spheroid-6.0/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-6.0/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.457719 prusek_spheroid-6.0/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    18855 2024-04-16 09:42:50.000000 prusek_spheroid-6.0/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-6.0/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-6.0/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-6.0/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-6.0/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-6.0/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-6.0/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-6.0/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-6.0/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-6.0/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-6.0/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-16 09:42:59.458806 prusek_spheroid-6.0/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-16 09:42:59.000000 prusek_spheroid-6.0/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-16 09:42:59.459389 prusek_spheroid-6.0/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-16 09:42:55.000000 prusek_spheroid-6.0/setup.py
```

### Comparing `prusek_spheroid-5.9/PKG-INFO` & `prusek_spheroid-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.9
+Version: 6.0
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.9/README.md` & `prusek_spheroid-6.0/README.md`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-6.0/prusek_spheroid/ContoursClassGUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,38 +39,32 @@
         self.detect_corrupted = detect_corrupted
         self.create_json = create_json
         self.calculate_properties = calculate_properties
         self.f = function
         self.progress_window = progress_window
         self.min_area = self.parameters["min_area"]
 
-        current_dir = os.path.dirname(os.path.abspath(__file__)).replace('\\\\', '\\')
+        current_dir = os.path.dirname(os.path.abspath(__file__))
         try:
 
             model_path = os.path.join(current_dir, 'gradient_boosting_classifier.joblib')
             scaler_path = os.path.join(current_dir, 'scaler.joblib')
 
             # Normalize the paths to ensure they are correct
+            print(f"pred1: {model_path}")
             model_path = os.path.normpath(model_path)
+            print(f"pred2: {model_path}")
+            model_path = model_path.replace("\\\\", "\\")
+            print(f'pred3: {model_path}')
             scaler_path = os.path.normpath(scaler_path)
             # Load the model and scaler
             self.model = joblib.load(model_path)
             self.scaler = joblib.load(scaler_path)
         except Exception as e:
             print(f"Loading from primary location failed: {e}")
-            print("Attempting to load from alternate location...")
-            # Attempt to load the model and scaler from the alternate location
-            # Load the model and scaler
-            model_path = os.path.join(current_dir, 'prusek_spheroid', 'gradient_boosting_classifier.joblib')
-            scaler_path = os.path.join(current_dir, 'prusek_spheroid', 'scaler.joblib')
-            # Normalize the paths to ensure they are correct
-            model_path = os.path.normpath(model_path)
-            scaler_path = os.path.normpath(scaler_path)
-            self.model = joblib.load(model_path)
-            self.scaler = joblib.load(scaler_path)
 
         fm.create_directory(os.path.dirname(self.output_json_path), delete=True)
         fm.create_directory(self.output_images_path, delete=True)
         fm.create_directory(os.path.join(self.output_segmented_path, "masks"), delete=True)
         fm.create_directory(os.path.join(self.output_segmented_path, "results"), delete=True)
 
     def evaluate(self, contour):
```

### Comparing `prusek_spheroid-5.9/prusek_spheroid/GUI.py` & `prusek_spheroid-6.0/prusek_spheroid/GUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-6.0/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-6.0/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/conversion.py` & `prusek_spheroid-6.0/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/file_management.py` & `prusek_spheroid-6.0/prusek_spheroid/file_management.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/image_processing.py` & `prusek_spheroid-6.0/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/merge_directories.py` & `prusek_spheroid-6.0/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/methods.py` & `prusek_spheroid-6.0/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/metrics.py` & `prusek_spheroid-6.0/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-6.0/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-6.0/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.9
+Version: 6.0
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `prusek_spheroid-5.9/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-6.0/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.9/setup.py` & `prusek_spheroid-6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.9",
+    version="6.0",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

