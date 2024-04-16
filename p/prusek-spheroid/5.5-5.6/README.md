# Comparing `tmp/prusek_spheroid-5.5.tar.gz` & `tmp/prusek_spheroid-5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusek_spheroid-5.5.tar", last modified: Mon Apr 15 17:00:16 2024, max compression
+gzip compressed data, was "prusek_spheroid-5.6.tar", last modified: Mon Apr 15 17:21:05 2024, max compression
```

## Comparing `prusek_spheroid-5.5.tar` & `prusek_spheroid-5.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.194156 prusek_spheroid-5.5/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 17:00:16.193865 prusek_spheroid-5.5/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)     9738 2024-04-12 06:53:12.000000 prusek_spheroid-5.5/README.md
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.192698 prusek_spheroid-5.5/prusek_spheroid/
--rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.5/prusek_spheroid/ContoursClassGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    51985 2024-04-15 16:54:02.000000 prusek_spheroid-5.5/prusek_spheroid/GUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.5/prusek_spheroid/GradientDescentGUI.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.5/prusek_spheroid/characteristic_functions.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.5/prusek_spheroid/conversion.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     7196 2024-04-15 16:59:57.000000 prusek_spheroid-5.5/prusek_spheroid/file_management.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.5/prusek_spheroid/image_processing.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.5/prusek_spheroid/merge_directories.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.5/prusek_spheroid/methods.py
--rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.5/prusek_spheroid/metrics.py
--rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.5/prusek_spheroid/selection_dialog.py
-drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:00:16.193635 prusek_spheroid-5.5/prusek_spheroid.egg-info/
--rw-r--r--   0 michalprusek   (501) staff       (20)    10310 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/PKG-INFO
--rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/SOURCES.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/dependency_links.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/requires.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 17:00:16.000000 prusek_spheroid-5.5/prusek_spheroid.egg-info/top_level.txt
--rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 17:00:16.194205 prusek_spheroid-5.5/setup.cfg
--rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 17:00:11.000000 prusek_spheroid-5.5/setup.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:21:05.305924 prusek_spheroid-5.6/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-15 17:21:05.305615 prusek_spheroid-5.6/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)     9873 2024-04-15 17:20:52.000000 prusek_spheroid-5.6/README.md
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:21:05.304084 prusek_spheroid-5.6/prusek_spheroid/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    19014 2024-04-12 11:59:24.000000 prusek_spheroid-5.6/prusek_spheroid/ContoursClassGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    51961 2024-04-15 17:16:23.000000 prusek_spheroid-5.6/prusek_spheroid/GUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)    12586 2024-04-10 14:43:59.000000 prusek_spheroid-5.6/prusek_spheroid/GradientDescentGUI.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4491 2024-01-27 10:12:42.000000 prusek_spheroid-5.6/prusek_spheroid/characteristic_functions.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4675 2024-04-04 17:10:48.000000 prusek_spheroid-5.6/prusek_spheroid/conversion.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     7172 2024-04-15 17:16:23.000000 prusek_spheroid-5.6/prusek_spheroid/file_management.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     5604 2024-04-07 11:37:32.000000 prusek_spheroid-5.6/prusek_spheroid/image_processing.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     2579 2024-04-06 17:55:28.000000 prusek_spheroid-5.6/prusek_spheroid/merge_directories.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     3644 2024-04-06 18:09:39.000000 prusek_spheroid-5.6/prusek_spheroid/methods.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)      571 2024-04-02 12:34:56.000000 prusek_spheroid-5.6/prusek_spheroid/metrics.py
+-rw-r--r--   0 michalprusek   (501) staff       (20)     4779 2024-04-04 17:35:30.000000 prusek_spheroid-5.6/prusek_spheroid/selection_dialog.py
+drwxr-xr-x   0 michalprusek   (501) staff       (20)        0 2024-04-15 17:21:05.305385 prusek_spheroid-5.6/prusek_spheroid.egg-info/
+-rw-r--r--   0 michalprusek   (501) staff       (20)    10445 2024-04-15 17:21:05.000000 prusek_spheroid-5.6/prusek_spheroid.egg-info/PKG-INFO
+-rw-r--r--   0 michalprusek   (501) staff       (20)      581 2024-04-15 17:21:05.000000 prusek_spheroid-5.6/prusek_spheroid.egg-info/SOURCES.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)        1 2024-04-15 17:21:05.000000 prusek_spheroid-5.6/prusek_spheroid.egg-info/dependency_links.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)      127 2024-04-15 17:21:05.000000 prusek_spheroid-5.6/prusek_spheroid.egg-info/requires.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       16 2024-04-15 17:21:05.000000 prusek_spheroid-5.6/prusek_spheroid.egg-info/top_level.txt
+-rw-r--r--   0 michalprusek   (501) staff       (20)       38 2024-04-15 17:21:05.305978 prusek_spheroid-5.6/setup.cfg
+-rw-r--r--   0 michalprusek   (501) staff       (20)      769 2024-04-15 17:16:39.000000 prusek_spheroid-5.6/setup.py
```

### Comparing `prusek_spheroid-5.5/PKG-INFO` & `prusek_spheroid-5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.5
+Version: 5.6
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -81,14 +81,16 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
+**Important**: When using Prusek-Spheroid on Windows, folder names that are part of the addresses in your project must be unaccented.
+
 1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files. 
 
 **Important**: When downloading COCO 1.0 annotations from CVAT, it is necessary to check the "save with images" box to add the "images" folder to the resulting downloaded ZIP file in addition to the "annotations" folder.
 
 **Important**: Supported image formats are **PNG**, **JPG**, **JPEG**, **BMP**, **TIFF**, **TIF**
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
```

### Comparing `prusek_spheroid-5.5/README.md` & `prusek_spheroid-5.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
+**Important**: When using Prusek-Spheroid on Windows, folder names that are part of the addresses in your project must be unaccented.
+
 1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files. 
 
 **Important**: When downloading COCO 1.0 annotations from CVAT, it is necessary to check the "save with images" box to add the "images" folder to the resulting downloaded ZIP file in addition to the "annotations" folder.
 
 **Important**: Supported image formats are **PNG**, **JPG**, **JPEG**, **BMP**, **TIFF**, **TIF**
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
```

### Comparing `prusek_spheroid-5.5/prusek_spheroid/ContoursClassGUI.py` & `prusek_spheroid-5.6/prusek_spheroid/ContoursClassGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/GUI.py` & `prusek_spheroid-5.6/prusek_spheroid/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import tkinter as tk
 from tkinter import filedialog
 from tkinter import messagebox
 from prusek_spheroid import GradientDescentGUI as g
 from prusek_spheroid import ContoursClassGUI as F
 import threading
 import time
```

### Comparing `prusek_spheroid-5.5/prusek_spheroid/GradientDescentGUI.py` & `prusek_spheroid-5.6/prusek_spheroid/GradientDescentGUI.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/characteristic_functions.py` & `prusek_spheroid-5.6/prusek_spheroid/characteristic_functions.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/conversion.py` & `prusek_spheroid-5.6/prusek_spheroid/conversion.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/file_management.py` & `prusek_spheroid-5.6/prusek_spheroid/file_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import shutil
 import cv2 as cv
 import numpy as np
 import json as js
 from tkinter import messagebox
 import zipfile
 import os
```

### Comparing `prusek_spheroid-5.5/prusek_spheroid/image_processing.py` & `prusek_spheroid-5.6/prusek_spheroid/image_processing.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/merge_directories.py` & `prusek_spheroid-5.6/prusek_spheroid/merge_directories.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/methods.py` & `prusek_spheroid-5.6/prusek_spheroid/methods.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/metrics.py` & `prusek_spheroid-5.6/prusek_spheroid/metrics.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid/selection_dialog.py` & `prusek_spheroid-5.6/prusek_spheroid/selection_dialog.py`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/prusek_spheroid.egg-info/PKG-INFO` & `prusek_spheroid-5.6/prusek_spheroid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusek_spheroid
-Version: 5.5
+Version: 5.6
 Summary: Spheroid segmentation package
 Home-page: https://github.com/michalprusek/prusek-spheroid
 Author: Michal Prusek
 Author-email: prusemic@cvut.cz
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -81,14 +81,16 @@
 
 Prusek-Spheroid is a sophisticated Python package equipped with a user-friendly graphical interface (GUI) that facilitates image segmentation and optimization tasks. This guide provides an overview of the GUI functionalities and how to use them effectively. The whole program is based on the knowledge of segmentations of several (approximately 15 to 20) spheroids. Based on these segmentations, the program learns to segment the remaining spheroid images in the dataset (project). So far the only possible formats in which the segmentations can be loaded are the COCO 1.0 format or loading masks and corresponding images. This is the format supported by the CVAT (Computer Vision Annotation Tool) platform.
 
 ### Using the Spheroid Segmentation GUI
 
 The Prusek-Spheroid GUI is designed to be intuitive, providing a range of functionalities for effective image segmentation. Here’s a detailed overview of the key elements:
 
+**Important**: When using Prusek-Spheroid on Windows, folder names that are part of the addresses in your project must be unaccented.
+
 1. **Input File and Folder Selection**: These two tabs are used for selecting and loading the annotations from CVAT in COCO 1.0 format (or loading masks and their corresponding images) and directory where your dataset images for segmentation are stored. You can easily navigate and choose the required folders and zip file (in COCO 1.0 format from downloaded from CVAT) that contain your image files. 
 
 **Important**: When downloading COCO 1.0 annotations from CVAT, it is necessary to check the "save with images" box to add the "images" folder to the resulting downloaded ZIP file in addition to the "annotations" folder.
 
 **Important**: Supported image formats are **PNG**, **JPG**, **JPEG**, **BMP**, **TIFF**, **TIF**
 
 2. **Output Folder Selection**: After processing, the results will be saved in the selected output folder. This feature allows you to specify where you want the segmented images and other outputs to be stored. If selected, the properties of the contours are also saved in the resulting folder as an excel file. Furthermore, the JSON file with the optimal parameters is also saved in the selected output folder in the "IoU" subfolder.
```

### Comparing `prusek_spheroid-5.5/prusek_spheroid.egg-info/SOURCES.txt` & `prusek_spheroid-5.6/prusek_spheroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prusek_spheroid-5.5/setup.py` & `prusek_spheroid-5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="prusek_spheroid",
-    version="5.5",
+    version="5.6",
     description="Spheroid segmentation package",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Michal Prusek",
     author_email="prusemic@cvut.cz",
     url="https://github.com/michalprusek/prusek-spheroid",
     packages=["prusek_spheroid"],
```

