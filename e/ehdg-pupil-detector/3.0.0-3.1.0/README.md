# Comparing `tmp/ehdg_pupil_detector-3.0.0.tar.gz` & `tmp/ehdg_pupil_detector-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdg_pupil_detector-3.0.0.tar", last modified: Mon Apr 15 06:14:58 2024, max compression
+gzip compressed data, was "ehdg_pupil_detector-3.1.0.tar", last modified: Tue Apr 16 00:59:05 2024, max compression
```

## Comparing `ehdg_pupil_detector-3.0.0.tar` & `ehdg_pupil_detector-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.770640 ehdg_pupil_detector-3.0.0/
--rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.0.0/LICENSE
--rw-rw-rw-   0        0        0     4046 2024-04-15 06:14:58.769643 ehdg_pupil_detector-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.0.0/README.md
--rw-rw-rw-   0        0        0     1116 2024-04-15 05:50:53.000000 ehdg_pupil_detector-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 06:14:58.770640 ehdg_pupil_detector-3.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.742715 ehdg_pupil_detector-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.748698 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/
--rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/__init__.py
--rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
--rw-rw-rw-   0        0        0    10070 2024-04-15 06:04:26.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/opmtrack.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:14:58.768645 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/
--rw-rw-rw-   0        0        0     4046 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       92 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-15 06:14:58.000000 ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.235954 ehdg_pupil_detector-3.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-11-05 22:14:35.000000 ehdg_pupil_detector-3.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4068 2024-04-16 00:59:05.234956 ehdg_pupil_detector-3.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-11-22 04:05:27.000000 ehdg_pupil_detector-3.1.0/README.md
+-rw-rw-rw-   0        0        0     1148 2024-04-15 23:50:56.000000 ehdg_pupil_detector-3.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 00:59:05.235954 ehdg_pupil_detector-3.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.205057 ehdg_pupil_detector-3.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.212016 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/
+-rw-rw-rw-   0        0        0        0 2023-11-05 22:27:51.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/__init__.py
+-rw-rw-rw-   0        0        0    22389 2024-01-03 22:00:51.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py
+-rw-rw-rw-   0        0        0      260 2024-04-15 01:15:20.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opm_detector_config.json
+-rw-rw-rw-   0        0        0    11954 2024-04-16 00:04:04.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opmtrack.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:59:05.232962 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/
+-rw-rw-rw-   0        0        0     4068 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       98 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-16 00:59:05.000000 ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/top_level.txt
```

### Comparing `ehdg_pupil_detector-3.0.0/LICENSE` & `ehdg_pupil_detector-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.0.0/PKG-INFO` & `ehdg_pupil_detector-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
 Requires-Dist: ehdg_tools
+Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
 pip install ehdg_pupil_detector
```

### Comparing `ehdg_pupil_detector-3.0.0/README.md` & `ehdg_pupil_detector-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.0.0/pyproject.toml` & `ehdg_pupil_detector-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "ehdg_pupil_detector"
-version = "3.0.0"
+version = "3.1.0"
 authors = [
   { name="Zaw Lin Tun", email="zawlintun1511@gmail.com" },
 ]
 description = "Python Library for Pupil Detector of Eye Health Diagnostic Group"
 readme = "README.md"
-dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools"]
+dependencies = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
@@ -18,18 +18,18 @@
 opmtrack = "ehdg_pupil_detector.opmtrack:main"
 
 [project.urls]
 "Homepage" = "https://github.com/jtur044/ehdg_pupil_detector"
 "Bug Tracker" = "https://github.com/jtur044/ehdg_pupil_detector/issues"
 
 [build-system]
-requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools"]
+requires = ["setuptools>=61.0", "opencv-python>=4.8.1.78", "scipy>=1.11.3", "numpy>=1.26.1", "commentjson", "ehdg_tools", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-mypkg = ["*"]
+ehdg_pupil_detector = ["*"]
```

### Comparing `ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py` & `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/ehdg_pupil_detector.py`

 * *Files identical despite different names*

### Comparing `ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector/opmtrack.py` & `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector/opmtrack.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import argparse
 import importlib.metadata
 from importlib.resources import files
 import cv2
 import commentjson
 from ehdg_pupil_detector import ehdg_pupil_detector
 from ehdg_tools.ehdg_buffers import TinyFillBuffer
+import numpy as np
 
 
 # This function is to get built-in config location with new library (from importlib.resources import files)
 def get_config_location(module_name, config_file_name):
     config_dir = files(module_name).joinpath(config_file_name)
     return str(config_dir)
 
@@ -48,29 +49,35 @@
     temp_dict["ellipse_axis_b"] = ellipse_axis_b
     temp_dict["ellipse_angle"] = ellipse_angle
 
     return temp_dict
 
 
 # This function is to redetect with pupil detector by given detector and tiny fill buffer
-def opm_detect(trial_video, output_csv_dir, config_dict, buffer_length_input, direction_input=None):
+def opm_detect(trial_video, out_dir, config_dict, buffer_length_input, direction_input=None):
+    out_folder = os.path.join(out_dir, "opmtrack_result")
+    if not os.path.isdir(out_folder):
+        os.mkdir(out_folder)
+    out_csv_dir = os.path.join(out_folder, "result.csv")
+    out_video_dir = os.path.join(out_folder, "result.mp4")
+
     detector = ehdg_pupil_detector.Detector()
     buffer = TinyFillBuffer(buffer_length_input)
     detector.update_config(config_dict)
     updated_properties = detector.get_config_info()
     print("<Detector Properties>")
     for info in updated_properties:
         print(f"{info} : {updated_properties[info]}")
 
     cap = cv2.VideoCapture(trial_video)
-    frame_rate = cap.get(cv2.CAP_PROP_FPS)
+    frame_rate = int(cap.get(cv2.CAP_PROP_FPS))
     print(f"frame_rate:{frame_rate}")
-    frame_width = cap.get(cv2.CAP_PROP_FRAME_WIDTH)
+    frame_width = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     print(f"frame_width:{frame_width}")
-    frame_height = cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
+    frame_height = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
     print(f"frame_height:{frame_height}")
     frame_count = 0
 
     print("")
     print(f"Detecting {trial_video} with opm detector")
 
     if direction_input is None:
@@ -81,37 +88,55 @@
                                "ellipse_angle"]
     else:
         column_header_array = ["x_value", "y_value", "x_nom", "y_nom",
                                "record_timestamp", "sensor_timestamp",
                                "frame_rate", "direction", "confidence", "diameter",
                                "ellipse_axis_a", "ellipse_axis_b",
                                "ellipse_angle"]
-    with open(output_csv_dir, mode='w', newline="") as destination_file:
+    fourcc = cv2.VideoWriter_fourcc(*'mp4v')
+    v_writer = cv2.VideoWriter(out_video_dir, fourcc, frame_rate, (frame_width, frame_height))
+    with open(out_csv_dir, mode='w', newline="") as destination_file:
         header_names = column_header_array
         csv_writer = csv.DictWriter(destination_file, fieldnames=header_names)
         csv_writer.writeheader()
 
         while cap.isOpened():
             ret, frame = cap.read()
             if ret:
                 frame_count += 1
                 frame_time = frame_count / frame_rate
                 gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)
                 result = detector.detect(gray)
                 d_ts = result["detector_timestamp"]
-                # center_of_pupil = result["center_of_pupil"]
+                center_of_pupil = result["center_of_pupil"]
+                center_of_pupil_x = int(center_of_pupil[0])
+                center_of_pupil_y = int(center_of_pupil[1])
                 reversed_center_of_pupil = result["reversed_center_of_pupil"]
                 x_value = float(reversed_center_of_pupil[0])
                 y_value = float(reversed_center_of_pupil[1])
                 axes_of_pupil = result["axes_of_pupil"]
                 major_axis = float(axes_of_pupil[0])
                 minor_axis = float(axes_of_pupil[1])
                 angle_of_pupil = float(result["angle_of_pupil"])
                 diameter_of_pupil = float(result["average_diameter_of_pupil"])
                 confidence = 0 if x_value <= 0 and y_value <= 0 else 1
+
+                center_of_pupil = (int(center_of_pupil_x), int(center_of_pupil_y))
+                detected_frame = np.copy(frame)
+                if center_of_pupil != (0, 0):
+                    cv2.ellipse(
+                        detected_frame,
+                        center_of_pupil,
+                        (int(major_axis), int(minor_axis)),
+                        int(angle_of_pupil),
+                        0, 360,  # start/end angle for drawing
+                        (0, 0, 255)  # color (BGR): red
+                    )
+                v_writer.write(detected_frame)
+
                 pupil_data = {}
                 pupil_data["x_value"] = x_value
                 pupil_data["y_value"] = y_value
                 pupil_data["major_axis"] = major_axis
                 pupil_data["minor_axis"] = minor_axis
                 pupil_data["angle_of_pupil"] = angle_of_pupil
                 pupil_data["diameter_of_pupil"] = diameter_of_pupil
@@ -127,56 +152,71 @@
                 for return_data in buffer.buffer:
                     if not got_first_data:
                         got_first_data = True
                     else:
                         temp_dict = get_data_dict(return_data, frame_rate, frame_width, frame_height, direction_input)
                         csv_writer.writerow(temp_dict)
                 destination_file.close()
+                print(f"The opmtrack_result folder is created in {out_dir}.")
+                print(f"Result folder dir: {out_folder}.")
+                print(f"Result csv dir: {out_csv_dir}.")
+                print(f"Result video dir: {out_video_dir}.")
                 break
 
 
 def main():
     parser = argparse.ArgumentParser(prog='opmtrack',
                                      description='OKNTRACK package.')
     opmtrack_version = importlib.metadata.version('ehdg_pupil_detector')
     parser.add_argument('--version', action='version', version=opmtrack_version),
     parser.add_argument("-i", dest="input_video", required=False, default=None,
                         metavar="input video")
-    parser.add_argument("-o", dest="output_csv", required=False, default=None,
-                        metavar="output csv directory")
+    parser.add_argument("-o", dest="output_directory", required=False, default=None,
+                        metavar="output directory")
     parser.add_argument("-c", dest="opm_config", required=False, default=None,
                         metavar="opm detector config")
     parser.add_argument("-d", dest="direction_input", required=False, default=None,
                         metavar="direction input")
     parser.add_argument("-bl", dest="buffer_length", required=False, default=None,
                         metavar="buffer length")
 
     args = parser.parse_args()
     input_video = args.input_video
-    output_csv = args.output_csv
+    output_directory = args.output_directory
     opm_config = args.opm_config
     direction_input = args.direction_input
     buffer_length = args.buffer_length
 
     default_buffer_length = 7
 
     if not os.path.isfile(input_video):
-        raise FileExistsError(f"Input video: {input_video} is not valid.")
+        print(f"Input video is invalid.")
+        print(f"Input video: {input_video} is invalid.")
+        return
+
+    if os.path.isfile(output_directory):
+        print(f"Output directory must be directory not file.")
+        print(f"Output directory: {output_directory}.")
+        return
+    else:
+        if not os.path.isdir(output_directory):
+            try:
+                os.mkdir(output_directory)
+            except FileNotFoundError:
+                print(f"Output directory cannot be created.")
+                print(f"Output directory: {output_directory}.")
+                return
 
     if opm_config is None:
-        opm_config_dict = {
-            "min_circular_ratio": 0.9,
-            "max_circular_ratio": 1.9,
-            "ksize_height": 13,
-            "ksize_width": 13,
-            "min_binary_threshold": 20,
-            "max_binary_threshold": 255,
-            "reflection_fill_dilation_index": 25,
-            "reflection_fill_square_dimension": 200
-        }
+        opm_config = get_config_location("ehdg_pupil_detector", "opm_detector_config.json")
+        try:
+            with open(opm_config) as opm_config_info:
+                opm_config_dict = commentjson.load(opm_config_info)
+        except FileNotFoundError:
+            raise FileNotFoundError(f"Error opening built-in opm config file:{opm_config}!")
     else:
         try:
             with open(opm_config) as opm_config_info:
                 opm_config_dict = commentjson.load(opm_config_info)
         except FileNotFoundError:
             raise FileNotFoundError(f"Error opening opm config file:{opm_config}!")
 
@@ -209,10 +249,9 @@
             print(f"There is buffer length input but it is invalid: {buffer_length}.")
             print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
     else:
         buffer_length_to_be_used = default_buffer_length
         print("There is no buffer length input.")
         print(f"OPM detector will be using Tiny Fill Buffer with default length:{buffer_length_to_be_used}.")
 
-    opm_detect(input_video, output_csv, opm_config_dict,
+    opm_detect(input_video, output_directory, opm_config_dict,
                buffer_length_to_be_used, direction_input=direction_to_be_used)
-    print(f"Output csv is created in {output_csv}")
```

### Comparing `ehdg_pupil_detector-3.0.0/src/ehdg_pupil_detector.egg-info/PKG-INFO` & `ehdg_pupil_detector-3.1.0/src/ehdg_pupil_detector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdg_pupil_detector
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python Library for Pupil Detector of Eye Health Diagnostic Group
 Author-email: Zaw Lin Tun <zawlintun1511@gmail.com>
 Project-URL: Homepage, https://github.com/jtur044/ehdg_pupil_detector
 Project-URL: Bug Tracker, https://github.com/jtur044/ehdg_pupil_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,15 @@
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0
 Requires-Dist: opencv-python>=4.8.1.78
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: commentjson
 Requires-Dist: ehdg_tools
+Requires-Dist: numpy
 
 # EYE HEALTH DIAGNOSTIC GROUP'S PUPIL DETECTOR (ehdg_pupil_detector)
 This is the python package libray pupil detector created by eye health diagnostic group.
 
 ## Installtion
 ```
 pip install ehdg_pupil_detector
```

