# Comparing `tmp/gref4hsi-0.1.5.tar.gz` & `tmp/gref4hsi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gref4hsi-0.1.5.tar", last modified: Tue Mar 12 10:12:27 2024, max compression
+gzip compressed data, was "gref4hsi-0.1.9.tar", last modified: Mon Apr 15 08:13:05 2024, max compression
```

## Comparing `gref4hsi-0.1.5.tar` & `gref4hsi-0.1.9.tar`

### file list

```diff
@@ -1,46 +1,40 @@
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13807 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/LICENCE.MD
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       79 2024-03-12 08:17:47.000000 gref4hsi-0.1.5/MANIFEST.in
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)     2547 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1144 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/README.md
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      205 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/__init__.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi/notebooks/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1388 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/notebooks/elevation_chart.png
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    15172 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/notebooks/kartverket_api.ipynb
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    29456 2024-03-12 10:09:50.000000 gref4hsi-0.1.5/gref4hsi/notebooks/specim_preprocessing.ipynb
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       97 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/notebooks/test_terrain.xml
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    28650 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/notebooks/test_tide.xml
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25225 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/notebooks/uhi_beast.ipynb
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi/scripts/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/scripts/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1587 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/scripts/colours.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8148 2024-03-12 09:09:01.000000 gref4hsi-0.1.5/gref4hsi/scripts/georeference.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9835 2024-03-12 09:09:49.000000 gref4hsi-0.1.5/gref4hsi/scripts/orthorectification.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    23230 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/scripts/radiometry.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    10284 2024-03-12 09:30:11.000000 gref4hsi-0.1.5/gref4hsi/scripts/visualize.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi/tests/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/tests/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1609 2024-03-12 10:08:55.000000 gref4hsi-0.1.5/gref4hsi/tests/test_main_hi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    11037 2024-03-12 10:08:55.000000 gref4hsi-0.1.5/gref4hsi/tests/test_main_specim.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     7676 2024-03-12 10:08:55.000000 gref4hsi-0.1.5/gref4hsi/tests/test_main_uhi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3000 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/tests/test_multi_ray_trace.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3684 2024-03-07 14:11:10.000000 gref4hsi-0.1.5/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi/utils/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/utils/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3059 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/utils/config_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    50018 2024-03-12 09:12:10.000000 gref4hsi-0.1.5/gref4hsi/utils/geometry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    40676 2024-03-12 09:13:46.000000 gref4hsi-0.1.5/gref4hsi/utils/gis_tools.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    36588 2024-03-12 09:14:36.000000 gref4hsi-0.1.5/gref4hsi/utils/parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8728 2024-03-07 12:34:03.000000 gref4hsi-0.1.5/gref4hsi/utils/photogrammetry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25619 2024-03-12 10:11:02.000000 gref4hsi-0.1.5/gref4hsi/utils/specim_parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    27250 2024-03-12 10:08:55.000000 gref4hsi-0.1.5/gref4hsi/utils/uhi_parsing_utils.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/gref4hsi.egg-info/
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)     2547 2024-03-12 10:12:27.000000 gref4hsi-0.1.5/gref4hsi.egg-info/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1135 2024-03-12 10:12:27.000000 gref4hsi-0.1.5/gref4hsi.egg-info/SOURCES.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        1 2024-03-12 10:12:27.000000 gref4hsi-0.1.5/gref4hsi.egg-info/dependency_links.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      188 2024-03-12 10:12:27.000000 gref4hsi-0.1.5/gref4hsi.egg-info/requires.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        9 2024-03-12 10:12:27.000000 gref4hsi-0.1.5/gref4hsi.egg-info/top_level.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      106 2024-03-12 08:17:47.000000 gref4hsi-0.1.5/pyproject.toml
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       38 2024-03-12 10:12:27.475982 gref4hsi-0.1.5/setup.cfg
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1567 2024-03-12 10:11:57.000000 gref4hsi-0.1.5/setup.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13807 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/LICENCE.MD
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       79 2024-03-12 08:17:47.000000 gref4hsi-0.1.9/MANIFEST.in
+-rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/PKG-INFO
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    18091 2024-04-15 08:03:32.000000 gref4hsi-0.1.9/README.md
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.373281 gref4hsi-0.1.9/gref4hsi/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      205 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/__init__.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.373281 gref4hsi-0.1.9/gref4hsi/scripts/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/scripts/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    36833 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/coregistration.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     7844 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/georeference.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9507 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/orthorectification.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi/tests/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/tests/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1616 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_hi.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    10686 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_specim.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8213 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_uhi.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3000 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3684 2024-03-07 14:11:10.000000 gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi/utils/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/utils/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1587 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/colours.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3143 2024-03-13 12:06:06.000000 gref4hsi-0.1.9/gref4hsi/utils/config_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    51438 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/geometry_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    44610 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/gis_tools.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    22622 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8706 2024-03-15 10:24:09.000000 gref4hsi-0.1.9/gref4hsi/utils/photogrammetry_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    23551 2024-03-14 09:13:50.000000 gref4hsi-0.1.9/gref4hsi/utils/radiometry.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25630 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/specim_parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    27489 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/uhi_parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9874 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/visualize.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi.egg-info/
+-rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/PKG-INFO
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      935 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        1 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      188 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/requires.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        9 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/top_level.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      106 2024-03-12 08:17:47.000000 gref4hsi-0.1.9/pyproject.toml
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       38 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/setup.cfg
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1567 2024-04-15 08:08:25.000000 gref4hsi-0.1.9/setup.py
```

### Comparing `gref4hsi-0.1.5/LICENCE.MD` & `gref4hsi-0.1.9/LICENCE.MD`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.5/gref4hsi/scripts/colours.py` & `gref4hsi-0.1.9/gref4hsi/utils/colours.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.5/gref4hsi/scripts/georeference.py` & `gref4hsi-0.1.9/gref4hsi/scripts/georeference.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import numpy as np
 import pyvista as pv
 import h5py
 
 # Lib resources:
 from gref4hsi.utils.geometry_utils import CameraGeometry, CalibHSI
 from gref4hsi.utils.parsing_utils import Hyperspectral
-from gref4hsi.scripts import visualize
+from gref4hsi.utils import visualize
 
 
-def cal_file_to_rays(filename_cal, config):
+def cal_file_to_rays(filename_cal):
         # See paper by Sun, Bo, et al. "Calibration of line-scan cameras for precision measurement." Applied optics 55.25 (2016): 6836-6843.
         # Loads line camera parameters for the hyperspectral imager from an xml file.
 
         # Certain imagers deliver geometry "per pixel". This can be resolved by fitting model parameters.
-        calHSI = CalibHSI(file_name_cal_xml=filename_cal, config = config)
+        calHSI = CalibHSI(file_name_cal_xml=filename_cal)
         f = calHSI.f
         u_c = calHSI.cx
 
         # Radial distortion parameters
         k1 = calHSI.k1
         k2 = calHSI.k2
 
@@ -62,46 +62,36 @@
         p_dir[:, 0] = x_norm
         p_dir[:, 2] = 1
 
         rot_hsi_ref_eul = np.array([rot_z, rot_y, rot_x])
 
         rot_hsi_ref_obj = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False)
 
-        try:
-            lever_arm_unit = config['General']['lever_arm_unit']
-        except:
-             # Defaults to meter if not set
-             lever_arm_unit = 'm'
-
-        # Handle legacy
-        if lever_arm_unit == 'mm':
-            translation_ref_hsi = np.array([trans_x, trans_y, trans_z]) / 1000 # These are millimetres
-        elif lever_arm_unit == 'm':
-            translation_ref_hsi = np.array([trans_x, trans_y, trans_z])
+        translation_ref_hsi = np.array([trans_x, trans_y, trans_z])
 
         intrinsic_geometry_dict = {'translation_ref_hsi': translation_ref_hsi,
                                    'rot_hsi_ref_obj': rot_hsi_ref_obj,
                                    'ray_directions_local': p_dir}
         
         # Notably, one could compress the information by expressing the ray directions in the body frame
 
         return intrinsic_geometry_dict
 
-def define_hsi_ray_geometry(pos_ref_ecef, quat_ref_ecef, time_pose, pos0, intrinsic_geometry_dict):
+def define_hsi_ray_geometry(pos_ref_ecef, quat_ref_ecef, time_pose, intrinsic_geometry_dict):
         """Instantiate a camera geometry object from the h5 pose data"""
 
 
-        pos = pos_ref_ecef # Reference positions in ECEF offset by pos0
+        pos = pos_ref_ecef # Reference positions in ECEF
         rot_obj = RotLib.from_quat(quat_ref_ecef) # Reference orientations wrt ECEF
         
         ray_directions_local = intrinsic_geometry_dict['ray_directions_local']
         translation_ref_hsi = intrinsic_geometry_dict['translation_ref_hsi']
         rot_hsi_ref_obj = intrinsic_geometry_dict['rot_hsi_ref_obj']
 
-        hsi_geometry = CameraGeometry(pos0=pos0, pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True, use_absolute_position=True)
+        hsi_geometry = CameraGeometry(pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True, use_absolute_position=True)
         
         
         hsi_geometry.intrinsicTransformHSI(translation_ref_hsi=translation_ref_hsi, rot_hsi_ref_obj = rot_hsi_ref_obj)
 
         hsi_geometry.defineRayDirections(dir_local = ray_directions_local)
 
         return hsi_geometry
@@ -142,67 +132,74 @@
         path_tide = 'Undefined'
     
     # Maximal allowed ray length
     max_ray_length = float(config['General']['max_ray_length'])
 
     mesh = pv.read(path_mesh)
 
-    print('Georeferencing Images')
-
-    for filename in sorted(os.listdir(dir_r)):
+    
+    print("\n################ Georeferencing: ################")
+    files = sorted(os.listdir(dir_r))
+    n_files= len(sorted(os.listdir(dir_r)))
+    file_count = 0
+    for filename in files:
         if filename.endswith('h5') or filename.endswith('hdf'):
+
+            progress_perc = 100*file_count/n_files
+            print(f"Georeferencing file {file_count+1}/{n_files}, progress is {progress_perc} %")
+
             # Path to hierarchical file
             path_hdf = dir_r + filename
 
             # Read h5 file
             hyp = Hyperspectral(path_hdf, config)
 
             # Using the cal file, we can define lever arm, boresight and local ray geometry (in dictionary)
             intrinsic_geometry_dict = cal_file_to_rays(filename_cal=hsi_cal_xml, config=config)
 
             
-            # Define the rays in ECEF for each frame. Note that if there is no position offset, pos0 is a 1x3 of zeros
+            # Define the rays in ECEF for each frame. 
             hsi_geometry = define_hsi_ray_geometry(pos_ref_ecef = hyp.pos_ref, 
                                     quat_ref_ecef = hyp.quat_ref, 
-                                    time_pose = hyp.pose_time, 
-                                    pos0 = hyp.pos0, 
+                                    time_pose = hyp.pose_time,
                                     intrinsic_geometry_dict = intrinsic_geometry_dict)
 
             
-            hsi_geometry.intersectWithMesh(mesh = mesh, max_ray_length=max_ray_length)
+            hsi_geometry.intersect_with_mesh(mesh = mesh, max_ray_length=max_ray_length)
             
             # Computes the view angles in the local NED. Computationally intensive as local NED is defined for each intersection
             hsi_geometry.compute_view_directions_local_tangent_plane()
 
             # Computes the sun angles in the local NED. Computationally intensive as local NED is defined for each intersection
             hsi_geometry.compute_sun_angles_local_tangent_plane()
 
             hsi_geometry.compute_tide_level(path_tide, tide_format = 'NMA')
 
-            hsi_geometry.compute_elevation_mean_sealevel(source_epsg=config['Coordinate Reference Systems']['geocsc_epsg_export'], geoid_path=config['Absolute Paths']['geoid_path'])
+            hsi_geometry.compute_elevation_mean_sealevel(source_epsg = config['Coordinate Reference Systems']['geocsc_epsg_export'], 
+                                                         geoid_path = config['Absolute Paths']['geoid_path'])
             
             write_intersection_geometry_2_h5_file(hsi_geometry=hsi_geometry, config = config, h5_filename=path_hdf)
 
-            print('Writing Point Cloud')
-            hsi_geometry.writeRGBPointCloud(config = config, hyp = hyp, transect_string = filename.split('.')[0])
+            hsi_geometry.write_rgb_point_cloud(config = config, hyp = hyp, transect_string = filename.split('.')[0])
 
             if viz:
                  visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, 
                                                      config=config, 
                                                      transect_string = filename.split('.')[0])
 
-            print('Intersection geometry written to:\n {0}'.format(filename))
+            
 
 
             
             
 
             #from scripts import visualize
             #visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, config=config, transect_string = filename.split('.')[0])
 
+        file_count+=1
```

### Comparing `gref4hsi-0.1.5/gref4hsi/scripts/orthorectification.py` & `gref4hsi-0.1.9/gref4hsi/scripts/orthorectification.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,29 +51,20 @@
         h5_folder_wavelength_widths = 'undefined'
 
     # The necessary data (a dictionary) from H5 file for resampling ancillary data (uses the same grid as datacube)
     anc_dict = config['Georeferencing']
 
     # Settings having to do with coordinate reference systems, described below
     SettingsCRS = namedtuple('SettingsOrthorectification', ['epsg_geocsc', 
-                                                              'epsg_proj', 
-                                                              'off_x', 
-                                                              'off_y', 
-                                                              'off_z'])
+                                                              'epsg_proj'])
     
     config_crs = SettingsCRS(epsg_geocsc=int(config['Coordinate Reference Systems']['geocsc_epsg_export']),
                              # The epsg code of the geocentric coordinate system (ECEF)
                              epsg_proj=int(config['Coordinate Reference Systems']['proj_epsg']),
                              # The epsg code of the projected coordinate system (e.g. UTM 32 has epsg 32632 for wgs 84 ellipsoid)
-                             off_x = float(config['General']['offset_x']),
-                             # The geocentric offset along x
-                             off_y = float(config['General']['offset_y']),
-                             # The geocentric offset along y
-                             off_z = float(config['General']['offset_z'])
-                             # The geocentric offset along z
                              )
 
     # Settings associated with orthorectification of datacube
     SettingsOrtho = namedtuple('SettingsOrthorectification', ['ground_resolution', 
                                                                             'wl_red', 
                                                                             'wl_green', 
                                                                             'wl_blue',
@@ -114,18 +105,23 @@
                               # Brand and model
                               interleave = config['Orthorectification']['interleave']
                               # ENVI interleave: either 'bsq', 'bip' or 'bil', see:
                               # https://envi.geoscene.cn/help/Subsystems/envi/Content/ExploreImagery/ENVIImageFiles.htm
                               )
 
 
-    print('Orthorectifying Images')
-
-    for filename in sorted(os.listdir(h5_folder)):
+    print("\n################ Orthorectifying: ################")
+    files = sorted(os.listdir(h5_folder))
+    n_files= len(sorted(os.listdir(h5_folder)))
+    file_count = 0
+    for filename in files:
         if filename.endswith('h5') or filename.endswith('hdf'):
+
+            progress_perc = 100*file_count/n_files
+            print(f"Orthorectifying file {file_count+1}/{n_files}, progress is {progress_perc} %")
             # Path to hierarchical file
             h5_filename = h5_folder + filename
 
             # Read the 3D point cloud, radiance cube 
             # Extract the point cloud
             point_cloud_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
                                                          dataset_name=h5_folder_point_cloud_ecef)
@@ -168,12 +164,13 @@
 
             # The ancilliary data is read from h5 files and converted into a datacube
             if eval(config['Orthorectification']['resample_ancillary']): 
                 gisHSI.resample_ancillary(h5_filename=h5_filename, 
                                         anc_dict = anc_dict, 
                                         anc_dir = anc_dir,
                                         interleave=config_ortho.interleave)
-
+        
+        file_count+=1
 if __name__ == '__main__':
     args = sys.argv[1:]
     iniPath = args[0]
     main(iniPath)
```

### Comparing `gref4hsi-0.1.5/gref4hsi/scripts/radiometry.py` & `gref4hsi-0.1.9/gref4hsi/utils/radiometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import pandas as pd
 from scipy.interpolate import interp1d
 from scipy.special import expi
 from scipy.special import erf
 from scipy.special import erfi
 from scipy.optimize import fsolve
+import matplotlib.pyplot as plt
 
 def fresnel(theta_i, n_i, n_t, is_transmittance, method):
     # This is used for computing the transmittance at the interfaces
     # First Snells:
     if method == 1:
         theta_t = np.arcsin((n_i / n_t)*np.sin(theta_i))
 
@@ -41,26 +42,25 @@
     else:
         return R_F
 
 
 
 
 def solid_angle_ratio(theta_w, n_w):
-    theta_a = np.arcsin((n_w / 1) * np.sin(theta_w)) # Snells law with n_a = 1
+    """Computes the in-air angle corresponding to an in-water angle using Snell's law"""
+    n_a = 1 # Approximate n_a = 1
+    theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w)) # Snells law
+    return theta_a
 
 def immersion_factor(theta_w, n_w, n_g, pixel_nr):
+    """Calculates the immersion factor for imager with planar glass port in underwater hyperspectral imaging"""
     n_a = 1
 
     theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w))
 
-    import matplotlib.pyplot as plt
-
-    #plt.hist(theta_w.reshape(-1))
-    #plt.show()
-
     t_ag = fresnel(theta_i=theta_a, n_i = n_a, n_t = n_g, is_transmittance=1, method=1)
 
     t_wg = fresnel(theta_i=theta_w, n_i=n_w, n_t=n_g, is_transmittance=1, method=1)
 
     I_f_LU = ((n_w**2)/(n_a**2) ) * (t_ag/t_wg)
 
     I_f = I_f_LU[pixel_nr.reshape(-1), :]
@@ -95,23 +95,18 @@
     Intensity = I_0*np.exp(-0.5*z**2)
 
     Intensity_Spectral = np.multiply(Intensity.reshape((-1, 1)), I_hat.reshape((1, -1)))
 
     return Intensity/I_0, Intensity_Spectral
 
 def compute_gamma(dir, normals):
+    """Compute the angle between a normal vector and an incoming ray"""
     dot_prod = np.einsum('ij, ij -> i', normals, -dir)
     len_vec = np.linalg.norm(dir, axis = 1) * np.linalg.norm(normals, axis = 1)
     gamma = np.arccos(dot_prod/len_vec)
-
-    gamma[gamma > 80*np.pi/180] = 80*np.pi/180
-
-    #import matplotlib.pyplot as plt
-    #plt.hist(gamma * 180 / np.pi, 50)
-    #plt.show()
     return gamma.reshape((-1, 1))
 
 def compute_n_g(wlen):
     n_g = 1.4424 + (7.1661/(wlen - 144.170))
     return n_g
 
 def compute_n_w(wlen, method):
@@ -164,16 +159,14 @@
 
     # Compute psi for all t by m cells. Check that angles are on the right side of 90 deg
 
     dot_prod = np.einsum('jk, ijk -> ij', d_pix, r_si_b)
     len_vec = np.linalg.norm(d_pix, axis=1) * np.linalg.norm(r_si_b, axis=2)
     psi = np.pi - np.arccos(dot_prod / len_vec)
 
-
-
     beta_p_interp = fournier_forand(B_p)  # Assumed constant backscatter fraction across wl. Is a log-log interpolator
 
     beta_p = np.exp( beta_p_interp(np.log(psi)) ).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # Due to the interpolation in log-log domain. t by m
 
     beta_w = compute_beta_w(psi).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # t by m
 
     beta_tot = (1/b)*(b_p*beta_p + b_w*beta_w) # t by m by k
@@ -201,25 +194,27 @@
 
 
 
 
 
 
 def compute_light_source_integral(sigma):
-    # Computes the relation between spectral radiant flux P [W] and peak intensity I_0 [W/sr]
+    """Computes the relation between spectral radiant flux P [W] and peak intensity I_0 [W/sr] for a directionally gaussian beam
+    with sigma standard decviation"""
     constant = np.exp(-0.5 * sigma ** 2) * sigma
 
     term1 = -0.626657j * erf(0 + 0.707107j * sigma)
     term2 = 0.626657j * erf(1.11072 / sigma + 0.707107j * sigma)
     term3 = -0.626657 * erfi((0.707107 * (sigma ** 2 + 1.5708j)) / sigma)
     term4 = 0.626657 * erfi(0.707107 * sigma + 0j)
 
     return np.real(constant * (term1 + term2 + term3 + term4))*2*np.pi
 
 def fournier_forand(B_p):
+    """Calculates the phase function values for a given backscatter fraction"""
 
     # Partition data into equal 100 bins from 10 degrees to 100:
     logPsi = np.linspace(np.log(10*np.pi/180), np.log(180*np.pi/180), 100)
     psi = np.exp(logPsi)
     # Convert B_p to FF parameters
     mu, n = compute_FF_params(B_p)
     #
@@ -270,16 +265,16 @@
 
     B_p = 1 - num/den
 
     return B_p_true - B_p
 
 
 
-
 def compute_beta_w(psi):
+    """The scattering phase function of pure water"""
     # Psi is an array of scattering angles
     # Analytical Formula from Ocean Optics p. 180
     return 0.0608*(1 + 0.925*(np.cos(psi))**2)
```

### Comparing `gref4hsi-0.1.5/gref4hsi/scripts/visualize.py` & `gref4hsi-0.1.9/gref4hsi/utils/visualize.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,25 +23,20 @@
     try:
         texture_path = config['Absolute Paths']['tex_path']
     except KeyError:
         texture_path = None
         
     pose_path = config['Absolute Paths']['pose_path']
 
-    # Offsets used for plotting
-    offset_x = float(config['General']['offset_x'])
-    offset_y = float(config['General']['offset_y'])
-    offset_z = float(config['General']['offset_z'])
-
 
     pose = pd.read_csv(
         pose_path, sep=',',
         header=0)
 
-    points_cam_ecef = np.concatenate( (pose[" X"].values.reshape((-1,1)) - offset_x, pose[" Y"].values.reshape((-1,1)) - offset_y, pose[" Z"].values.reshape((-1,1)) - offset_z), axis = 1)
+    points_cam_ecef = np.concatenate( (pose[" X"].values.reshape((-1,1)), pose[" Y"].values.reshape((-1,1)), pose[" Z"].values.reshape((-1,1))), axis = 1)
     use_local = False
     if use_local == True:
         eul_cam = np.concatenate((pose[" Yaw"].values.reshape((-1, 1)),
                                   pose[" Pitch"].values.reshape((-1, 1)),
                                   pose[" Roll"].values.reshape((-1, 1))), axis=1)
     else:
         eul_cam = np.concatenate( (pose[" RotZ"].values.reshape((-1,1)), pose[" RotY"].values.reshape((-1,1)), pose[" RotX"].values.reshape((-1,1))), axis = 1)
@@ -49,71 +44,64 @@
 
     R_body_to_ecef = Rotation.from_euler("ZYX", eul_cam, degrees=True)
     
 
     # Read the mesh
     mesh = pv.read(mesh_path)
     if ref_frame == 'NED':
-        x = offset_x
-        y = offset_y
-        z = offset_z
+        x = np.mean(points_mesh_ecef[:,0])
+        y = np.mean(points_mesh_ecef[:,1])
+        z = np.mean(points_mesh_ecef[:,2])
         
         lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
         R_ecef_to_ned = Rotation.from_matrix(rotation_matrix_ecef2ned(lon=lon0, lat=lat0))
 
         R_body_to_ned = R_ecef_to_ned*R_body_to_ecef
         rotMats = R_body_to_ned.as_matrix()
 
         points_mesh_ecef = mesh.points
 
         # Next part is to make a NED
-        x_cam, y_cam, z_cam = pm.ecef2ned(x = points_cam_ecef[:,0] + x, y = points_cam_ecef[:,1] + y, z = points_cam_ecef[:,2] + z, lon0=lon0, lat0=lat0, h0=hei0)
+        x_cam, y_cam, z_cam = pm.ecef2ned(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
 
         points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
 
-        x_mesh, y_mesh, z_mesh = pm.ecef2ned(x = points_mesh_ecef[:,0] + x, y = points_mesh_ecef[:,1] + y, z = points_mesh_ecef[:,2] + z, lon0=lon0, lat0=lat0, h0=hei0)
+        x_mesh, y_mesh, z_mesh = pm.ecef2ned(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
 
         points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
 
         mesh.points = points_mesh
 
 
     elif ref_frame == 'ENU':
-        x = offset_x
-        y = offset_y
-        z = offset_z
         lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
         R_ecef_to_enu = Rotation.from_matrix(rotation_matrix_ecef2enu(lon=lon0, lat=lat0))
 
         R_body_to_enu = R_ecef_to_enu*R_body_to_ecef
         rotMats = R_body_to_enu.as_matrix()
 
         points_mesh_ecef = mesh.points
 
         # Next part is to make a NED
-        x_cam, y_cam, z_cam = pm.ecef2enu(x = points_cam_ecef[:,0] + x, y = points_cam_ecef[:,1] + y, z = points_cam_ecef[:,2] + z, lon0=lon0, lat0=lat0, h0=hei0)
+        x_cam, y_cam, z_cam = pm.ecef2enu(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
 
         points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
 
-        x_mesh, y_mesh, z_mesh = pm.ecef2enu(x = points_mesh_ecef[:,0] + x, y = points_mesh_ecef[:,1] + y, z = points_mesh_ecef[:,2] + z, lon0=lon0, lat0=lat0, h0=hei0)
+        x_mesh, y_mesh, z_mesh = pm.ecef2enu(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
 
         points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
         mesh.points = points_mesh
     
     else:
         rotMats = R_body_to_ecef.as_matrix()
         points_cam = points_cam_ecef
 
 
     
 
-    #cam_rot = Rotation.from_euler("ZYX", np.array([0, 0, 0]), degrees=True).as_matrix()
-
-    # Compose the two
-    #rotMats = rotMats*cam_rot
     p = BackgroundPlotter(window_size=(600, 400))
     
     if show_mesh:
         if texture_path != None:
             tex = pv.read_texture(texture_path)
             p.add_mesh(mesh, texture=tex)
         else:
```

### Comparing `gref4hsi-0.1.5/gref4hsi/tests/test_main_hi.py` & `gref4hsi-0.1.9/gref4hsi/tests/test_main_hi.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import os
 
 # Local resources
 from scripts import georeference
 from scripts import orthorectification
 from utils import parsing_utils
-from scripts import visualize
+from gref4hsi.utils import visualize
 from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths
 
 """
 This script is meant to be used for testing the processing pipeline of airborne HI data.
 """ 
 DATA_DIR = 'D:/HyperspectralDataAll/HI/2022-05-27-053505-NyAlesund-Flight8/'
 config_file = DATA_DIR + 'configuration.ini'
```

### Comparing `gref4hsi-0.1.5/gref4hsi/tests/test_main_specim.py` & `gref4hsi-0.1.9/gref4hsi/tests/test_main_specim.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,138 +1,114 @@
 # Standard python library
 import configparser
 import sys
 import os
 import argparse
 from collections import namedtuple
 import pathlib
+import yaml
 
-# This is very hard coded, but not necessary if Python does not know where to look
-module_path = '/home/haavasl/VsCodeProjects/gref4hsi/gref4hsi/'
+if os.name == 'nt':
+    # Windows OS
+    base_fp = 'D:'
+    home = 'C:/Users/haavasl'
+elif os.name == 'posix':
+    # This Unix-like systems inl. Mac and fLinux
+    base_fp = '/media/haavasl/Expansion'
+    home = '/home/haavasl'
+
+# Use this if working with the github repo to do quick changes to the module
+module_path = os.path.join(home, 'VsCodeProjects/gref4hsi/')
 if module_path not in sys.path:
     sys.path.append(module_path)
 
 # Local resources
-from scripts import georeference
-from scripts import orthorectification
-from utils import parsing_utils, specim_parsing_utils
-from scripts import visualize
+from gref4hsi.scripts import georeference
+from gref4hsi.scripts import orthorectification
+from gref4hsi.scripts import coregistration
+from gref4hsi.utils import parsing_utils, specim_parsing_utils
+from gref4hsi.utils import visualize
 from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths, customize_config
 
 
 import numpy as np
+
 """
 This script is meant to be used for testing the processing pipeline of airborne HI data from the Specim AFX10 instrument.
 """
 
+# Make it simple to swap when working a bit on windows and a bit on Linux
 
 
 
-def main():
-    # Set up argparse
-    parser = argparse.ArgumentParser('georeference and rectify images')
-
-    parser.add_argument('-s', '--specim_mission_folder',
-                        type=str, 
-                        default= r"/media/haavasl/Expansion/Specim/Missions/2024-02-19-Sletvik/slettvik_hopavaagen_202402191253_ntnu_hyperspectral_74m/",
-                        help='folder storing the hyperspectral data for the specific mission')
-
-    parser.add_argument('-e', '--epsg_code', 
-                        default=25832, 
-                        type=int,
-                        help='Coordinate Reference System EPSG code (e.g. 25832 for UTM 32)')
-
-    parser.add_argument('-r', '--resolution_orthomosaic', 
-                        type=float,
-                        default=1, 
-                        help='Resolution of the final processed orthomosaic in meters')
-
-    parser.add_argument('-cal_dir', '--calibration_directory', 
-                        type=str,
-                        default="/media/haavasl/Expansion/Specim/Lab_Calibrations", 
-                        help='Directory holding all spectral/radiometric/geometric calibrations for all binning values' )
-
-    parser.add_argument('-c', '--config_file_yaml', 
-                        default="",
-                        help='File that contains the configuration \
-                            parameters for the processing. \
-                            If nothing, one is generated from template.\
-                            can simply be one that was used for another mission.')
-
-    parser.add_argument('-t', '--terrain_type', 
-                        default="geoid", type=str,
-                        help ='If terrain DEM is known, select "dem_file", and if not select "geoid".')
-
-    parser.add_argument('-geoid', '--geoid_path', 
-                        default="/media/haavasl/Expansion/Specim/Missions/2024-02-19-Sletvik/slettvik_hopavaagen_202402191253_ntnu_hyperspectral_74m/geoids/no_kv_HREF2018A_NN2000_EUREF89.tif", 
-                        type=str,
-                        help='If terrain DEM is not available.')
-
-    parser.add_argument('-d', '--dem_path', 
-                        default="/media/haavasl/Expansion/Specim/Missions/2024-02-19-Sletvik/slettvik_hopavaagen_202402191253_ntnu_hyperspectral_74m/dem/dem.tif", 
-                        type=str,
-                        help='A digital terrain model, if available. If none, the geoid will be used.')
-
-    parser.add_argument('-v', '--enable_visualize', 
-                        default=False, 
-                        type = bool,
-                        help='Visualize vehicle track and terrain model')
-
-
-    args = parser.parse_args()
-
+def main(config_yaml, specim_mission_folder, geoid_path, config_template_path, lab_calibration_path):
+    # Read flight-specific yaml file
+    with open(config_yaml, 'r') as file:  
+        config_data = yaml.safe_load(file)
+    
+    
     # assigning the arguments to variables for simple backwards compatibility
-    SPECIM_MISSION_FOLDER = args.specim_mission_folder
-    EPSG_CODE = args.epsg_code
-    RESOLUTION_ORTHOMOSAIC = args.resolution_orthomosaic
-    CALIBRATION_DIRECTORY = args.calibration_directory
-    CONFIG_FILE = args.config_file_yaml
-    ENABLE_VISUALIZE = args.enable_visualize
-    TERRAIN_TYPE = args.terrain_type
-    DEM_PATH = args.dem_path
-    GEOID_PATH = args.geoid_path
+    SPECIM_MISSION_FOLDER = specim_mission_folder
+    EPSG_CODE = config_data['mission_epsg']
+    RESOLUTION_ORTHOMOSAIC = config_data['resolution_orthomosaic']
+    CALIBRATION_DIRECTORY = lab_calibration_path
+    
+    
+    dem_fold = os.path.join(specim_mission_folder, "dem")
+
+    if not os.path.exists(dem_fold):
+        print('DEM folder does not exist so Geoid is used as terrain instead')
+        TERRAIN_TYPE = "geoid"
+    else:
+        if not os.listdir(dem_fold):
+            #print(f"The folder '{dem_fold}' is empty so Geoid is used as terrain instead.")
+            TERRAIN_TYPE = "geoid"
+        else:
+            # If there is a folder and it is not empty
+            # Find the only file that is there
+            files = [f for f in os.listdir(dem_fold) if f not in ('.', '..')]
+            DEM_PATH = os.path.join(dem_fold, files[0])
+            #print(f"The file '{DEM_PATH}' is used as terrain.")
+            TERRAIN_TYPE = "dem_file"
+            
+    
+    
+    GEOID_PATH = geoid_path
 
     # Settings associated with preprocessing of data from Specim Proprietary data to pipeline-compatible data
     SettingsPreprocess = namedtuple('SettingsPreprocessing', ['dtype_datacube', 
                                                                             'lines_per_chunk', 
                                                                             'specim_raw_mission_dir',
                                                                             'cal_dir',
                                                                             'reformatted_missions_dir',
                                                                             'rotation_matrix_hsi_to_body',
                                                                             'translation_body_to_hsi',
                                                                             'config_file_name'])
 
     config_specim_preprocess = SettingsPreprocess(dtype_datacube = np.float32, # The data type for the datacube
-                                lines_per_chunk= 2000,  # Raw datacube is chunked into this many lines. GB_per_chunk = lines_per_chunk*n_pixels*n_bands*4 bytes
+                                lines_per_chunk= 8000,  # Raw datacube is chunked into this many lines. GB_per_chunk = lines_per_chunk*n_pixels*n_bands*4 bytes
                                 specim_raw_mission_dir = SPECIM_MISSION_FOLDER, # Folder containing several mission
                                 cal_dir = CALIBRATION_DIRECTORY,  # Calibration directory holding all calibrations at all binning levels
-                                reformatted_missions_dir = SPECIM_MISSION_FOLDER + 'processed/', # The fill value for empty cells (select values not occcuring in cube or ancillary data)
+                                reformatted_missions_dir = os.path.join(SPECIM_MISSION_FOLDER, 'processed'), # The fill value for empty cells (select values not occcuring in cube or ancillary data)
                                 rotation_matrix_hsi_to_body = np.array([[0, 1, 0],
                                                                         [-1, 0, 0],
                                                                         [0, 0, 1]]), # Rotation matrix R rotating so that vec_body = R*vec_hsi.
                                 translation_body_to_hsi = np.array([0, 0, 0]), # Translation t so that vec_body_to_object = vec_hsi_to_object + t
                                 # For large files, RAM issues could be a concern. For rectified files exeeding this size, data is written chunk-wize to a memory map.
                                 config_file_name = 'configuration.ini')
 
 
 
     # Where to place the config
     DATA_DIR = config_specim_preprocess.reformatted_missions_dir
-    config_file_mission = DATA_DIR + 'configuration.ini'
-
-
-    # Read config from a template (relative path):
-    if CONFIG_FILE != "":
-        config_path_template = CONFIG_FILE
-    else:
-        config_path_template = '/home/haavasl/VsCodeProjects/gref4hsi/data/config_examples/configuration_specim.ini'
+    config_file_mission = os.path.join(DATA_DIR, 'configuration.ini')
 
 
     # Set the data directory for the mission, and create empty folder structure
-    prepend_data_dir_to_relative_paths(config_path=config_path_template, DATA_DIR=DATA_DIR)
+    prepend_data_dir_to_relative_paths(config_path=config_template_path, DATA_DIR=DATA_DIR)
 
     # Non-default settings
     custom_config = {'General':
                         {'mission_dir': DATA_DIR,
                         'model_export_type': TERRAIN_TYPE, # Ray trace onto geoid
                         'max_ray_length': 200}, # Max distance in meters from spectral imager to seafloor. Specim does not fly higher
 
@@ -140,32 +116,39 @@
                         {'proj_epsg' : EPSG_CODE, # The projected CRS UTM 32, common on mainland norway
                         'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
                         'dem_epsg' : EPSG_CODE, # (Optional) If you have a DEM this can be used
                         'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
 
                     'Orthorectification':
                         {'resample_rgb_only': True, # True can be good choice for speed during DEV
+                         'resample_ancillary': True,
                         'resolutionhyperspectralmosaic': RESOLUTION_ORTHOMOSAIC, # Resolution in m
                         'raster_transform_method': 'north_east'}, # North-east oriented rasters.
                     
                     'HDF.raw_nav': {
                         'rotation_reference_type' : 'eul_ZYX', # The vehicle orientations are given in Yaw, Pitch, Roll from the NAV system
                         'is_global_rot' : False, # The vehicles orientations from NAV system are Yaw, Pitch, Roll
                         'eul_is_degrees' : True}, # And given in degrees
                     'Absolute Paths': {
                         'geoid_path' : GEOID_PATH,
                         #'geoid_path' : 'data/world/geoids/egm08_25.gtx',
                         'dem_path' : DEM_PATH,
+                        'orthomosaic_reference_folder' : os.path.join(specim_mission_folder, "orthomosaic"),
+                        'ref_ortho_reshaped' : os.path.join(DATA_DIR, "Intermediate", "RefOrthoResampled"),
+                        'ref_gcp_path' : os.path.join(DATA_DIR, "Intermediate", "gcp.csv"),
                         # (above) The georeferencing allows processing using norwegian geoid NN2000 and worldwide EGM2008. Also, use of seafloor terrain models are supported. '
                         # At the moment refractive ray tracing is not implemented, but it could be relatively easy by first ray tracing with geoid+tide, 
                         # and then ray tracing from water
                         #'tide_path' : 'D:/HyperspectralDataAll/HI/2022-08-31-060000-Remoy-Specim/Input/tidevann_nn2000_NMA.txt'
-                        }
-                        # Tide data can be downloaded from https://www.kartverket.no/til-sjos/se-havniva
-                        # Preferably it is downloaded with reference "NN2000" to agree with DEM
+                        },
+                    # If coregistration is done, then the data must be stored after processing somewhere
+                    'HDF.coregistration': {
+                        'position_ecef': 'processed/coreg/position_ecef',
+                        'quaternion_ecef' : 'processed/coreg/quaternion_ecef'
+                    }
                     
     }
 
     if TERRAIN_TYPE == 'geoid':
         custom_config['Absolute Paths']['geoid_path'] = GEOID_PATH
         #'geoid_path' : 'data/world/geoids/egm08_25.gtx'
     elif TERRAIN_TYPE == 'dem_file':
@@ -184,24 +167,38 @@
     """specim_parsing_utils.main(config=config,
                               config_specim=config_specim_preprocess)"""
     
     # Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
     config = parsing_utils.export_pose(config_file_mission)
     
     # Exports model
-    parsing_utils.export_model(config_file_mission)
+    """parsing_utils.export_model(config_file_mission)"""
 
     # Commenting out the georeference step is fine if it has been done
 
     
     ## Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
-    if ENABLE_VISUALIZE:
-        visualize.show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame='ENU')
+    """if ENABLE_VISUALIZE:
+        visualize.show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame='ENU')"""
 
     # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
     #georeference.main(config_file_mission)
 
-    orthorectification.main(config_file_mission)
+    #orthorectification.main(config_file_mission)
+
+    coregistration.main(config_file_mission, mode='compare')
+
+    coregistration.main(config_file_mission, mode='calibrate')
 
 
 if __name__ == "__main__":
-    main()
+    # Select a recording folder on drive
+    specim_mission_folder = os.path.join(base_fp, r"Specim/Missions/2022-08-31-Remøy/remoy_202208310800_ntnu_hyperspectral_74m")
+    
+    # Globally accessible files:
+    geoid_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/world/geoids/egm08_25.gtx")
+    config_template_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/config_examples/configuration_specim.ini")
+    lab_calibration_path = os.path.join(base_fp, "Specim/Lab_Calibrations")
+    
+    # The configuration file
+    config_yaml = os.path.join(specim_mission_folder, "config.seabee.yaml")
+    main(str(config_yaml), str(specim_mission_folder), geoid_path, config_template_path, lab_calibration_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gref4hsi-0.1.5/gref4hsi/tests/test_main_uhi.py` & `gref4hsi-0.1.9/gref4hsi/tests/test_main_uhi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,93 @@
 from collections import namedtuple
 import configparser
 import os
+import sys
 
 import numpy as np
 
-from utils import parsing_utils, uhi_parsing_utils
-from scripts import georeference, orthorectification
-from scripts import visualize
+# Detect OS and set FPs
+if os.name == 'nt':
+    # Windows OS
+    base_fp = 'D:'
+    home = 'C:/Users/haavasl'
+elif os.name == 'posix':
+    # This Unix-like systems inl. Mac and Linux
+    base_fp = '/media/haavasl/Expansion'
+    home = 'C:/Users/haavasl'
+
+# Use this if working with the github repo to do quick changes to the module
+module_path = os.path.join(home, 'VsCodeProjects/gref4hsi/')
+if module_path not in sys.path:
+    sys.path.append(module_path)
+
+from gref4hsi.utils import parsing_utils, uhi_parsing_utils
+from gref4hsi.scripts import georeference, orthorectification
+from gref4hsi.utils import visualize
 from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths, customize_config
 
 
-DATA_DIR = "D:/HyperspectralDataAll/UHI/2020-07-01-14-34-57-ArcticSeaIce-Ben-Lange/"
+DATA_DIR = os.path.join(base_fp, "HyperspectralDataAll/UHI/2020-07-01-14-40-15-ArcticSeaIce-Ben-Lange/")
 
 # The configuration file stores the settings for georeferencing
-config_file_mission = DATA_DIR + 'configuration.ini'
+config_file_mission = os.path.join(DATA_DIR, 'configuration.ini')
 
 
+config_path_template = os.path.join(home, 'VsCodeProjects/gref4hsi/data/config_examples/configuration_uhi.ini')
 
-# If the user has set a config file already, then that one can be used
-if os.path.exists(config_file_mission):
-    # Set the data directory for the mission, and create empty folder structure
-    prepend_data_dir_to_relative_paths(config_path=config_file_mission, DATA_DIR=DATA_DIR)
-else:
-    # Read config from a template (relative path):
-    config_path_template = 'data/config_examples/configuration_uhi.ini'
-
-    # Copies the template to config_file_mission and sets up the necessary directories
-    prepend_data_dir_to_relative_paths(config_path=config_path_template, DATA_DIR=DATA_DIR)
-
-    # Non-default settings
-    custom_config = {'General':
-                        {'mission_dir': DATA_DIR,
-                        'model_export_type': 'dem_file', # Infer seafloor structure from altimeter recordings
-                        'max_ray_length': 5,
-                        'lab_cal_dir': 'D:/HyperspectralDataAll/UHI/Lab_Calibration_Data/NP/'}, # Max distance in meters from UHI to seafloor
-
-                    'Coordinate Reference Systems': 
-                        {'proj_epsg' : 3395, # The projected CRS for orthorectified data (an arctic CRS)
-                        'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
-                        'dem_epsg' : 3395, # (Optional) If you have a DEM this can be used
-                        'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
-
-                    'Relative Paths':
-                        {'dem_folder': 'Input/GIS/'}, # Using altimeter, we generate one DEM per transect chunk
-
-                    'Orthorectification':
-                        {'resample_rgb_only': True, # Good choice for speed
-                        'resolutionhyperspectralmosaic': 0.1, # 1 cm
-                        'raster_transform_method': 'north_east'},
-                    
-                    'HDF.raw_nav': {'altitude': 'raw/nav/altitude',
-                        'rotation_reference_type' : 'eul_ZYX', # The vehicles orientations are used as Yaw, Pitch, Roll
-                        'is_global_rot' : False, # The vehicles orientations are used as Yaw, Pitch, Roll
-                        'eul_is_degrees' : True},
-
-                    'HDF.calibration': {'band2wavelength' : 'processed/radiance/calibration/spectral/band2Wavelength',
-                                    'darkframe' : 'processed/radiance/calibration/radiometric/darkFrame',
-                                    'radiometricframe' : 'processed/radiance/calibration/radiometric/radiometricFrame',
-                                    'fov' : 'processed/radiance/calibration/geometric/fieldOfView'},
-                    
-                    # Where to find the standard data for the cube. Note that is_calibrated implies whether data is already in correct format
-                    'HDF.hyperspectral': {'datacube' : 'processed/radiance/dataCube',
-                                        'exposuretime' : 'processed/radiance/exposureTime',
-                                        'timestamp' : 'processed/radiance/timestamp',
-                                        'is_calibrated' : True},
-
-                    'HDF.rgb' :{'rgb_frames' : 'rawdata/rgb/rgbFrames',
-                                'rgb_frames_timestamp' : 'rawdata/rgb/timestamp'}
-                    
-    }
+# Copies the template to config_file_mission and sets up the necessary directories
+prepend_data_dir_to_relative_paths(config_path=config_path_template, DATA_DIR=DATA_DIR)
 
-    # Customizes the config file
-    customize_config(config_path=config_file_mission, dict_custom=custom_config)
+# Non-default settings
+custom_config = {'General':
+                    {'mission_dir': DATA_DIR,
+                    'model_export_type': 'dem_file', # Infer seafloor structure from altimeter recordings
+                    'max_ray_length': 20,
+                    'lab_cal_dir': os.path.join(base_fp, 'HyperspectralDataAll/UHI/Lab_Calibration_Data/NP')}, # Max distance in meters from UHI to seafloor
+
+                'Coordinate Reference Systems': 
+                    {'proj_epsg' : 3395, # The projected CRS for orthorectified data (an arctic CRS)
+                    'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
+                    'dem_epsg' : 3395, # (Optional) If you have a DEM this can be used
+                    'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
+
+                'Relative Paths':
+                    {'dem_folder': 'Input/GIS/'}, # Using altimeter, we generate one DEM per transect chunk
+                
+                'Absolute Paths':
+                    {'geoid_path': os.path.join(home, 'VsCodeProjects\gref4hsi\data\world\geoids\egm08_25.gtx')}, # Using altimeter, we generate one DEM per transect chunk
+
+                'Orthorectification':
+                    {'resample_rgb_only': False, # Good choice for speed
+                    'resolutionhyperspectralmosaic': 0.01, # 1 cm
+                    'raster_transform_method': 'north_east'},
+                
+                'HDF.raw_nav': {'altitude': 'raw/nav/altitude',
+                    'rotation_reference_type' : 'eul_ZYX', # The vehicles orientations are used as Yaw, Pitch, Roll
+                    'is_global_rot' : False, # The vehicles orientations are used as Yaw, Pitch, Roll
+                    'eul_is_degrees' : True},
+
+                'HDF.calibration': {'band2wavelength' : 'processed/radiance/calibration/spectral/band2Wavelength',
+                                'darkframe' : 'processed/radiance/calibration/radiometric/darkFrame',
+                                'radiometricframe' : 'processed/radiance/calibration/radiometric/radiometricFrame',
+                                'fov' : 'processed/radiance/calibration/geometric/fieldOfView'},
+                
+                # Where to find the standard data for the cube. Note that is_calibrated implies whether data is already in correct format
+                'HDF.hyperspectral': {'datacube' : 'processed/radiance/dataCube',
+                                    'exposuretime' : 'processed/radiance/exposureTime',
+                                    'timestamp' : 'processed/radiance/timestamp',
+                                    'is_calibrated' : True},
+
+                'HDF.rgb' :{'rgb_frames' : 'rawdata/rgb/rgbFrames',
+                            'rgb_frames_timestamp' : 'rawdata/rgb/timestamp'}
+                
+}
+
+# Customizes the config file
+customize_config(config_path=config_file_mission, dict_custom=custom_config)
 
 # Settings specific to the pre-processing of UHI data. At present they are hardcoded, but they could be integrated 
 SettingsPreprocess = namedtuple('SettingsPreprocessing', ['dtype_datacube', 
                                                             'rotation_matrix_hsi_to_body',
                                                             'translation_hsi_to_body',
                                                             'rotation_matrix_alt_to_body',
                                                             'translation_alt_to_body',
@@ -93,25 +105,28 @@
                             # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
                             translation_hsi_to_body = np.array([0, 0, 0]),
                             rotation_matrix_alt_to_body = np.array([[0, 1, 0],
                                                                     [1, 0, 0],
                                                                     [0, 0, -1]]),
                             # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
                             translation_alt_to_body = np.array([0.5, 0, 0]),
-                            time_offset_sec =  23,
+                            time_offset_sec =  0,
+                            # Ben's tick s1 starts at 1593614097.992003 -> 22 s delay
+                            # Ben's tick s2 starts at 1593614414.995001 -> 0 s delay
+
                             lon_lat_alt_origin =  np.array([1, 1, 0]),
                             # The beast sets up a fake coordinate system at 1 deg lon/lat.
                             config_file_name = 'configuration.ini',
-                            resolution_dem = 0.2,
-                            agisoft_process  = False)
+                            resolution_dem = 0.2, # The resolution of the Altimeter-based DEM
+                            agisoft_process  = False) # This is an option for photogrammetry-based processing in the case you have imagery
+
 
 
 
 
-# TODO: update config.ini automatically with paths for simple reproducability
 """config = configparser.ConfigParser()
 config.read(config_file)"""
 
 def main():
 
     # The config stores all relevant configurations
     config = configparser.ConfigParser()
@@ -126,15 +141,15 @@
 
     config.read(config_file_mission)
     
     # Exports model
     parsing_utils.export_model(config_file_mission)
 
     # Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
-    visualize.show_mesh_camera(config)
+    #visualize.show_mesh_camera(config)
 
     # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
     georeference.main(config_file_mission, viz=False)
 
     orthorectification.main(config_file_mission)
     # Alternatively mode = 'calibrate'
     # georeference.main(config_file, mode='calibrate', is_calibrated=True)
```

### Comparing `gref4hsi-0.1.5/gref4hsi/tests/test_multi_ray_trace.py` & `gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.5/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py` & `gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/config_utils.py` & `gref4hsi-0.1.9/gref4hsi/utils/config_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,43 +29,48 @@
     if 'Absolute Paths' not in config:
         # Create a new section for 'Absolute Paths'
         config.add_section('Absolute Paths')
 
     # Iterate through the key-value pairs in 'Relative Paths'
     for key, relative_path in config['Relative Paths'].items():
         # Copy the key-value pair to 'Absolute Paths' section
-        absolute_path = DATA_DIR + relative_path
+        absolute_path = os.path.join(DATA_DIR, relative_path)
         config.set('Absolute Paths', key, absolute_path)
 
         # Only directories end with separators
         is_dir = (len(absolute_path.split('.'))==1)
 
         # Only create directories if path is a valid directory
         if mkdirs and is_dir:
             # If it exists, do nothing
             if os.path.exists(absolute_path):
                 pass
             else:
                 os.makedirs(absolute_path, exist_ok=True)
 
     # Save the updated configuration to the file
-    with open(DATA_DIR + 'configuration.ini', 'w') as configfile:
+    
+    config_path_write = os.path.join(DATA_DIR, 'configuration.ini')
+    
+    with open(config_path_write, 'w') as configfile:
         config.write(configfile)
 
 def customize_config(config_path, dict_custom):
     """Allows changing dictionary-specified entries of the config to custom values
 
     :param config_path: path to config file for read and write
     :type config_path: str
     :param dict_custom: dictionary of custom options for processing.
     :type dict_custom: nested dictionary. Dictionary of sections which are dictionaries
     """
     config = configparser.ConfigParser()
     config.read(config_path)
 
+    
+
     # dict_custom like config is a two-level nested dictionary
     for key_section, section_dict in dict_custom.items():
         # Iterate through each section, and assign custom values 
         for key_sub_section, value_custom in section_dict.items():
             try:
                 config.set(key_section, key_sub_section, str(value_custom))
             except configparser.NoSectionError:
```

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/geometry_utils.py` & `gref4hsi-0.1.9/gref4hsi/utils/geometry_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Third party
 import numpy as np
+import numpy.matlib
 from osgeo import gdal, osr
 import rasterio
 from scipy.spatial.transform import Rotation as RotLib
 from scipy.spatial.transform import Slerp
-from scipy.interpolate import interp1d
 import open3d as o3d
 import xmltodict
 from pyproj import CRS, Transformer
 import pymap3d as pm
 import ephem
 import pandas as pd
 from scipy.interpolate import interp1d
@@ -22,15 +22,15 @@
 import os
 import time
 from datetime import datetime
 from dateutil import parser
 
 # A file were we define geometry and geometric transforms
 class CalibHSI:
-    def __init__(self, file_name_cal_xml, config, mode = 'r', param_dict = None):
+    def __init__(self, file_name_cal_xml, mode = 'r', param_dict = None):
         """
         :param file_name_cal_xml: str
         File name of calibration file for line camera model
         :param config: config
         global configuration object.
         :param mode: str
         open file for reading (for general use) or writing (post calibration)
@@ -76,24 +76,17 @@
             # Update xml_dict['calibration'] with values from param_dict
             for key, value in param_dict.items():
                 xml_dict['calibration'][key] = value
             with open(file_name_cal_xml, 'w') as fd:
                 fd.write(xmltodict.unparse(xml_dict))
 
 class CameraGeometry():
-    def __init__(self, pos0, pos, rot, time, is_interpolated = False, use_absolute_position = False):
-        self.pos0 = pos0
-
-        if use_absolute_position:
-            self.position_nav = pos
-        else:
-            self.position_nav = pos - np.transpose(pos0) # Camera pos
-
-
-
+    def __init__(self, pos, rot, time, is_interpolated = False, use_absolute_position = False):
+        
+        self.position_nav = pos
         self.rotation_nav = rot
 
         self.time = time
         self.IsLocal = False
         self.decoupled = True
 
         if is_interpolated:
@@ -230,15 +223,15 @@
         n = self.position_ecef.shape[0]
         m = dir_local.shape[0]
 
         self.rayDirectionsGlobal = np.zeros((n, m, 3))
 
         for i in range(n):
             self.rayDirectionsGlobal[i, :, :] = self.rotation_hsi[i].apply(dir_local)
-    def intersectWithMesh(self, mesh, max_ray_length):
+    def intersect_with_mesh(self, mesh, max_ray_length):
         """Intersects the rays of the camera with the 3D triangular mesh
 
         :param mesh: A mesh object read via the pyvista library
         :type mesh: Pyvista mesh
         :param max_ray_length: The upper bound length of the camera rays (it is determined )
         :type max_ray_length: _type_
         """
@@ -250,15 +243,15 @@
         self.normals_ecef_crs = np.zeros((n, m, 3), dtype=np.float64)
 
         # Duplicate multiple camera centres
         start = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
 
         dir = (self.rayDirectionsGlobal * max_ray_length).reshape((-1,3))
 
-        print('Starting Ray Tracing')
+        
         
         start_time = time.time()
 
 
         
         try:
             # This will only work if exact Python version is rigght and you have PyEmbree
@@ -281,16 +274,14 @@
                                                                 ray_directions=dir, 
                                                                 multiple_hits=False,
                                                                 return_locations=True)
 
 
         stop_time = time.time()
 
-        print('Ray traced {0} rays on a mesh with {1} cells in {2} seconds'.format(dir.shape[0], mesh.cell_normals.shape[0], stop_time - start_time))
-
         normals = mesh.cell_normals[cells,:]
 
         slit_image_number = np.floor(rays / m).astype(np.int32)
 
         pixel_number = rays % m
 
         # Assign normals
@@ -313,15 +304,15 @@
 
             # Calculate surface normals of intersected triangles (for artificial illumination)
             self.normals_hsi_crs[i,:,:] = (self.rotation_hsi[i].inv()).apply(self.normals_ecef_crs[i, :, :])
 
             # Calculate a depth map (the z-component, 1D scanline)
             self.depth_map[i, :] = self.points_hsi_crs[i, :, 2]/self.rayDirectionsLocal[:, 2]
 
-        print('Finished ray tracing')
+        
 
         self.unix_time_grid = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), self.time.reshape((-1,1)))
         self.unix_time = self.unix_time_grid.reshape((-1, 1)) # Vector-form
         self.pixel_nr_grid = np.matlib.repmat(np.arange(m), n, 1)
         self.frame_nr_grid = np.matlib.repmat(np.arange(n).reshape(-1,1), 1, m)
 
         
@@ -338,18 +329,14 @@
         """
 
         # Solves equation lam^2 *(d_hat'B*d_hat) + lam * 2*(p0' * B* dir_hat) + (p0' *B* p0)= 1
         a = np.transpose(dir_hat).dot(B.dot(dir_hat))
         b = 2*np.transpose(p0).dot(B.dot(dir_hat))
         c = np.transpose(p0).dot(B.dot(p0)) - 1
 
-        print(a)
-        print(b)
-        print(c)
-
         p = np.zeros(3)
         p[0] = a
         p[1] = b
         p[2] = c
 
         lam = np.roots(p)
 
@@ -405,25 +392,25 @@
         m = self.rayDirectionsGlobal.shape[1]
 
         self.seabed_to_camera_NED = np.zeros(self.camera_to_seabed_ECEF.shape)
         self.normals_ned_crs = np.zeros(self.normals_ecef_crs.shape)
         self.theta_v = np.zeros((n, m))
         self.phi_v = np.zeros((n, m))
 
-        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1)) + self.pos0[0]
-        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1)) + self.pos0[1]
-        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1)) + self.pos0[2]
+        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
+        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1))
+        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
         
         lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
 
         start = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
 
-        x_hsi = start[:, 0].reshape((-1,1)) + self.pos0[0]
-        y_hsi = start[:, 1].reshape((-1,1)) + self.pos0[1]
-        z_hsi = start[:, 2].reshape((-1,1)) + self.pos0[2]
+        x_hsi = start[:, 0].reshape((-1,1))
+        y_hsi = start[:, 1].reshape((-1,1))
+        z_hsi = start[:, 2].reshape((-1,1))
 
         # Compute vectors from seabed intersections to HSI in NED
         NED = pm.ecef2ned(x= x_hsi, y= y_hsi, z=z_hsi, lat0 = lats, lon0=lons, h0 = alts)
 
         self.seabed_to_camera_NED = np.hstack((NED[0], NED[1], NED[2])).reshape((n, m, 3))
 
         # For remote sensing with a sun-lit seafloor:
@@ -447,17 +434,17 @@
             
 
 
     def compute_sun_angles_local_tangent_plane(self):
         n = self.rayDirectionsGlobal.shape[0]
         m = self.rayDirectionsGlobal.shape[1]
 
-        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1)) + self.pos0[0]
-        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1)) + self.pos0[1]
-        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1)) + self.pos0[2]
+        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
+        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1)) 
+        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
 
         lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
 
         self.lats = lats
         self.lons = lons
         self.alts = alts
 
@@ -469,17 +456,17 @@
 
         
 
     def compute_elevation_mean_sealevel(self, source_epsg, geoid_path = 'data/world/geoids/egm08_25.gtx'):
         n = self.rayDirectionsGlobal.shape[0]
         m = self.rayDirectionsGlobal.shape[1]
 
-        x_ecef = self.position_ecef[:, 0].reshape((-1,1)) + self.pos0[0]
-        y_ecef = self.position_ecef[:, 1].reshape((-1,1)) + self.pos0[1]
-        z_ecef = self.position_ecef[:, 2].reshape((-1,1)) + self.pos0[2]
+        x_ecef = self.position_ecef[:, 0].reshape((-1,1))
+        y_ecef = self.position_ecef[:, 1].reshape((-1,1))
+        z_ecef = self.position_ecef[:, 2].reshape((-1,1))
 
         #lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
 
         
 
         alts_msl = CameraGeometry.elevation_msl(x_ecef, y_ecef, z_ecef, source_epsg=source_epsg, geoid_path = geoid_path)
         
@@ -555,23 +542,23 @@
                     tide_timestamp = df_tide['UnixTime']
                     
                     hsi_tide_interp = interp1d(x = tide_timestamp, y= tide_height_NN2000)(x = self.time)
 
                     # Make into gridded form:
                     self.hsi_tide_gridded = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), hsi_tide_interp.reshape((-1,1)))
                 except:
-                    print('No tide file was found!!')
+                    #print('No tide file was found!!')
                     self.hsi_tide_gridded = constant_height*np.ones((n, m, 1))
 
 
 
             else: # A Good place to write parsers for other formats
                 TypeError
         
-    def writeRGBPointCloud(self, config, hyp, transect_string, extrapolate = True, minInd = None, maxInd = None):
+    def write_rgb_point_cloud(self, config, hyp, transect_string, extrapolate = True, minInd = None, maxInd = None):
         wl_red = float(config['General']['red_wave_length'])
         wl_green = float(config['General']['green_wave_length'])
         wl_blue = float(config['General']['blue_wave_length'])
         dir_point_cloud = config['Absolute Paths']['rgb_point_cloud_folder']
 
         wavelength_nm = np.array([wl_red, wl_green, wl_blue])
 
@@ -602,15 +589,15 @@
         self.config = config
         self.type = type
         self.HSIPositionFeature = [] # Function of feature line
         self.HSIRotationFeature = [] #
         self.isfirst = True
 
     def load_cam_calibration(self, filename_cal, config):
-        calHSI = CalibHSI(file_name_cal_xml=filename_cal, config = config)  # Generates a calibration object
+        calHSI = CalibHSI(file_name_cal_xml=filename_cal)  # Generates a calibration object
         self.f = calHSI.f
         self.v_c = calHSI.cx
         self.k1 = calHSI.k1
         self.k2 = calHSI.k2
         self.k3 = calHSI.k3
 
         self.trans_x = calHSI.tx
@@ -725,47 +712,15 @@
 
         # Compose the values to rot0
         rot_tot = delta_rot_interp * rot_Q_00
 
 
         return rot_tot
 
-    def computeDirections(self, param):
-        self.rot_x = param[0]  # Pitch relative to cam (Equivalent to cam defining NED and uhi BODY)
-        self.rot_y = param[1]*0  # Roll relative to cam
-        self.rot_z = param[2]  # Yaw relative to cam
-        self.v_c = param[3]
-        self.f = param[4]
-        self.k1 = param[5]*0
-        self.k2 = param[6]
-        self.k3 = param[7]
-
-
-        #self.v_c = 455.414296
-        #self.f = 9.55160147e+02
-        #self.k1 = 0
-        #self.k2 = 3.22199561e+02
-        #self.k3 = -7.36445822e+01
-        #self.rot_x = 1.41822029e-03
-        #self.rot_z = -3.77072811e-03
-        # Define camera model array for 960 pixels and 480. 1 is subtracted when.
-        # Pixel ranges from -0.5
-        # How to compensate for binning?
-
-        self.v = self.pixel*self.binning + 0.5*(self.binning + 1)
-
-        # Express uhi ray directions in uhi frame using line-camera model
-        x_norm_lin = (self.v - self.v_c) / self.f
-
-        x_norm_nonlin = -(self.k1 * ((self.v - self.v_c) / 1000) ** 5 + \
-                          self.k2 * ((self.v - self.v_c) / 1000) ** 3 + \
-                          self.k3 * ((self.v - self.v_c) / 1000) ** 2) / self.f
-
-        self.x_norm = x_norm_lin + x_norm_nonlin
-
+    
     # At the time of updated parameters
     def reprojectFeaturesHSI(self):
         rot_hsi_rgb = np.array([self.rot_z, self.rot_y, self.rot_x]) * 180 / np.pi
 
         self.rotation_hsi_rgb = RotLib.from_euler('ZYX', rot_hsi_rgb, degrees=True)
 
         self.rotation_hsi = self.rotationRGB * self.rotation_hsi_rgb # Composing rotations.
@@ -780,15 +735,98 @@
                 self.HSIToFeaturesGlobal[i, :])
 
             self.HSIToFeaturesLocal[i, :] /= self.HSIToFeaturesLocal[i, 2]
 
 
 
 
-def interpolate_poses(timestamp_from, pos_from, pos0, rot_from, timestamps_to, extrapolate = True, use_absolute_position = True):
+def compute_camera_rays_from_parameters(pixel_nr, cx, f, k1, k2, k3):
+    """_summary_
+
+    :param pixel_nr: _description_
+    :type pixel_nr: _type_
+    :param rot_x: _description_
+    :type rot_x: _type_
+    :param rot_y: _description_
+    :type rot_y: _type_
+    :param rot_z: _description_
+    :type rot_z: _type_
+    :param cx: _description_
+    :type cx: _type_
+    :param f: _description_
+    :type f: _type_
+    :param k1: _description_
+    :type k1: _type_
+    :param k2: _description_
+    :type k2: _type_
+    :param k3: _description_
+    :type k3: _type_
+    :return: _description_
+    :rtype: _type_
+    """
+
+    u = pixel_nr + 1
+
+    # Express uhi ray directions in uhi frame using line-camera model
+    x_norm_lin = (u - cx) / f
+
+    x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                        k2 * ((u - cx) / 1000) ** 3 + \
+                        k3 * ((u - cx) / 1000) ** 2) / f
+
+    x_norm = x_norm_lin + x_norm_nonlin
+
+    return x_norm
+
+
+def reproject_world_points_to_hsi_plane(trans_hsi_body, rot_hsi_body, pos_body, rot_body, points_world):
+    """Reprojects world points to local image plane coordinates (x_h, y_h, 1)
+
+    :param trans_hsi_body: lever arm from body center to hsi focal point
+    :type trans_hsi_body: _type_
+    :param rot_hsi_body: boresight rotation 
+    :type rot_hsi_body: Scipy rotation object
+    :param pos_body: The earth fixed earth centered position of the vehicle body centre
+    :type pos_body: _type_
+    :param rot_body: The rotation of the body in ECEF
+    :type rot_body: Scipy rotation object
+    :param points_world: World points in ECEF
+    :type points_world: _type_
+    :return: The reprojection coordinates
+    :rtype: ndarray(n, 3)
+    """
+
+    
+
+    # We compose the hypothesized boresight (rot_hsi_body) an lever arm (trans_hsi_body) to get the hypothesized position/orientation
+    # of the hyperspectral imager
+    rotation_hsi = rot_body * rot_hsi_body
+    position_hsi = pos_body + rot_body.apply(trans_hsi_body)
+
+    # Given the positions, the hsi-point vector can be expressed in ECEF
+    hsi_to_feature_global = points_world - position_hsi
+
+    # Number of features to iterate
+    n = hsi_to_feature_global.shape[0]
+
+    # We can now express the hsi-point vector in the HSI frame and normalize by the z component to find the image plane projection
+    hsi_to_feature_local = np.zeros(hsi_to_feature_global.shape)
+    for i in range(n):
+        # The vector expressed in HSI frame
+        hsi_to_feature_local[i, :] = (rotation_hsi[i].inv()).apply(hsi_to_feature_global[i, :])
+
+        # The vector normalized to lie on the virtual plane
+        hsi_to_feature_local[i, :] /= hsi_to_feature_local[i, 2]
+    
+    return hsi_to_feature_local
+
+
+
+
+def interpolate_poses(timestamp_from, pos_from, rot_from, timestamps_to, extrapolate = True, use_absolute_position = True):
     """
 
     :param timestamp_from:
     Original timestamps
     :param pos_from: numpy array (n,3)
     Original positions
     :param rot_from: Rotation-object (n rotations)
@@ -816,16 +854,15 @@
     """
 
     min_ind = 0
     max_ind = timestamps_to.size
 
 
     # Setting use_absolute_position to True means that position calculations are done with absolute
-    referenceGeometry = CameraGeometry(pos0=pos0,
-                               pos=pos_from,
+    referenceGeometry = CameraGeometry(pos=pos_from,
                                rot=rot_from,
                                time=timestamp_from,
                                use_absolute_position=use_absolute_position)
 
     # We exploit a method from the camera object
     referenceGeometry.interpolate(time_hsi=timestamps_to,
                           minIndRGB=min_ind,
@@ -863,24 +900,14 @@
 
 
 
 
 
 
 
-class MeshGeometry():
-    def __init__(self, config):
-        mesh_path = config['General']['model_path']
-        texture_path = config['General']['tex_path']
-        offset_x = float(config['General']['offset_x'])
-        offset_y = float(config['General']['offset_y'])
-        offset_z = float(config['General']['offset_z'])
-        self.pos0 = np.array([offset_x, offset_y, offset_z]).reshape([-1, 1])
-
-
 
 def rotation_matrix_ecef2ned(lon, lat):
     """
     Computes the rotation matrix R from earth-fixed-earth centered (ECEF) to north-east-down (NED).
     :param lat: float in range [-90, 90]
     The latitude in degrees
     :param lon: float in range [-180, 180]
@@ -940,15 +967,21 @@
         self.epsg = pos_epsg
 
 
         self.lat = None
         self.lon = None
         self.hei = None
 
-    def compute_geodetic_position(self, epsg_geod):
+        self.compute_geodetic_position()
+        self.compute_geocentric_orientation()
+        self.compute_ned_orientation()
+        self.compute_ned_2_ecef()
+
+
+    def compute_geodetic_position(self, epsg_geod = 4326):
         """
             Function for transforming positions to latitude longitude height
             :param epsg_geod: int
             EPSG code of the transformed geodetic coordinate system
         """
         # If geocentric position has not been defined.
         from_CRS = CRS.from_epsg(self.epsg)
@@ -989,53 +1022,53 @@
         if self.rot_obj_ecef == None:
             # Define rotations from ned to ecef
             if self.lat.any == None:
                 # Needed to encode rotation between NED and ECEF
                 self.compute_geodetic_position()
 
             R_body_2_ned = self.rot_obj_ned
-            R_ned_2_ecef = self.compute_rot_obj_ned_2_ecef()
+            R_ned_2_ecef = self.compute_ned_2_ecef()
             R_body_2_ecef = R_ned_2_ecef*R_body_2_ned
 
             self.rot_obj_ecef = R_body_2_ecef
 
         else:
             pass
 
     def compute_ned_orientation(self):
         if self.rot_obj_ned == None:
             # Define rotations from body to ecef
             R_body_2_ecef = self.rot_obj_ecef
 
             # Define rotation from ecef 2 ned
-            R_ecef_2_ned = self.compute_rot_obj_ned_2_ecef().inv()
+            R_ecef_2_ned = self.compute_ned_2_ecef().inv()
 
             # Compose
             R_body_2_ned = R_ecef_2_ned*R_body_2_ecef
 
             self.rot_obj_ned = R_body_2_ned
 
 
         else:
             pass
 
-    def compute_rot_obj_ned_2_ecef(self):
+    def compute_ned_2_ecef(self):
 
         N = self.lat.shape[0]
         rot_mats_ned_2_ecef = np.zeros((N, 3, 3), dtype=np.float64)
         
         for i in range(N):
             rot_mats_ned_2_ecef[i,:,:] = rot_mat_ned_2_ecef(lat=self.lat[i], lon = self.lon[i])
 
 
-        self.rots_obj_ned_2_ecef = RotLib.from_matrix(rot_mats_ned_2_ecef)
-
-        return self.rots_obj_ned_2_ecef
+        self.rot_obj_ned_2_ecef = RotLib.from_matrix(rot_mats_ned_2_ecef)
 
+        return self.rot_obj_ned_2_ecef
 
+    
 
 
 def rot_mat_ned_2_ecef(lat, lon):
     """
     Computes the rotation matrix R from north-east-down (NED) to earth-fixed-earth centered (ECEF)
     :param lat: float in range [-90, 90]
     The latitude in degrees
@@ -1056,15 +1089,44 @@
     # TODO: add source
     R_ned_ecef = np.array([[-np.cos(l) * np.sin(mu), -np.sin(l), -np.cos(l) * np.cos(mu)],
                            [-np.sin(l) * np.sin(mu), np.cos(l), -np.sin(l) * np.cos(mu)],
                            [np.cos(mu), 0, -np.sin(mu)]])
     return R_ned_ecef
 
 
+def read_raster(filename, out_crs="EPSG:3857", use_z=False):
+    """Read a raster to a ``pyvista.StructuredGrid``.
 
+    This will handle coordinate transformations.
+    """
+    from rasterio import transform
+    import rioxarray
+    # Read in the data
+    data = rioxarray.open_rasterio(filename)
+    values = np.asarray(data)
+    data.rio.nodata
+    nans = values == data.rio.nodata
+    if np.any(nans):
+        # values = np.ma.masked_where(nans, values)
+        values[nans] = np.nan
+    # Make a mesh
+    xx, yy = np.meshgrid(data["x"], data["y"])
+    if use_z and values.shape[0] == 1:
+        # will make z-comp the values in the file
+        zz = values.reshape(xx.shape)
+    else:
+        # or this will make it flat
+        zz = np.zeros_like(xx)
+    mesh = pv.StructuredGrid(xx, yy, zz)
+    pts = mesh.points
+    lon, lat = transform(data.rio.crs, out_crs, pts[:, 0], pts[:, 1])
+    mesh.points[:, 0] = lon
+    mesh.points[:, 1] = lat
+    mesh["data"] = values.reshape(mesh.n_points, -1, order="F")
+    return mesh
 
 def dem_2_mesh(path_dem, model_path, config):
     """
     A function for converting a specified DEM to a 3D mesh model (*.vtk, *.ply or *.stl). 
     Consequently, mesh should be thought of as 2.5D representation.
     In the case 
 
@@ -1111,47 +1173,49 @@
                 is_projected = True
                 config.set('Coordinate Reference Systems', 'dem_epsg', str(epsg_proj))
             elif spatial_reference.IsGeographic():
                 epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 0)
                 proj = ds.GetProjection()
                 is_projected = False
 
-            print(f"DEM projected EPSG Code: {epsg_proj}")
 
             # Automatically set
             
             
             # Get the band's data as a NumPy array
             band_data = band.ReadAsArray()
 
             # Create a mask to identify no-data values
             mask = band_data != no_data_value
 
             # Create and open the output XYZ file for writing if it does not exist:
-            #if not os.path.exists(output_xyz):
-            with open(output_xyz, 'w') as xyz_file:
-                # Write data to the XYZ file using the mask and calculated coordinates
-                for y in range(ds.RasterYSize):
-                    for x in range(ds.RasterXSize):
-                        if mask[y, x]:
-                            x_coord = x_origin + x * x_resolution
-                            y_coord = y_origin + y * y_resolution
-                            xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
+            if not os.path.exists(output_xyz):
+                with open(output_xyz, 'w') as xyz_file:
+                    # Write data to the XYZ file using the mask and calculated coordinates
+                    for y in range(ds.RasterYSize):
+                        for x in range(ds.RasterXSize):
+                            if mask[y, x]:
+                                x_coord = x_origin + x * x_resolution
+                                y_coord = y_origin + y * y_resolution
+                                xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
+            else:
+                print('*.xyz already exists')
             # Clean up
             ds = None
             band = None
     
-    print("DEM-Mesh conversion completed.")
+
     points = np.loadtxt(output_xyz)
 
     # Create a pyvista point cloud object
     cloud = pv.PolyData(points)
-
+    
+    # TODO: Apply patch to avoid crash for triangulation when using big DEM files
     # Generate a mesh from points
-    mesh = cloud.delaunay_2d()
+    mesh = cloud.delaunay_2d(progress_bar=True)
 
     # Transform the mesh points from projected to geocentric ECEF.
     geocsc = CRS.from_epsg(epsg_geocsc)
 
     if epsg_proj == 'EPSG': # If a geographic CRS
         pass
     else:
@@ -1166,28 +1230,19 @@
         y_proj = points_proj[:, 1].reshape((-1, 1))
     else:
         x_proj = points_proj[:, 1].reshape((-1, 1))
         y_proj = points_proj[:, 0].reshape((-1, 1))
     
     h_proj = points_proj[:, 2].reshape((-1, 1))
 
-    (xECEF, yECEF, zECEF) = transformer.transform(xx=x_proj, yy=y_proj, zz=h_proj)
-
-    mesh.points[:, 0] = xECEF.reshape(-1)
-    mesh.points[:, 1] = yECEF.reshape(-1)
-    mesh.points[:, 2] = zECEF.reshape(-1)
-
-    offX = float(config['General']['offset_x'])
-    offY = float(config['General']['offset_y'])
-    offZ = float(config['General']['offset_z'])
-
-    pos0 = np.array([offX, offY, offZ]).reshape((1, -1))
+    (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=x_proj, yy=y_proj, zz=h_proj)
 
-    # Add same offset as position data
-    mesh.points -= pos0
+    mesh.points[:, 0] = x_ecef.reshape(-1)
+    mesh.points[:, 1] = y_ecef.reshape(-1)
+    mesh.points[:, 2] = z_ecef.reshape(-1)
 
     # Save mesh
     mesh.save(model_path)
 
 def crop_geoid_to_pose(path_dem, config, geoid_path = 'data/world/geoids/egm08_25.gtx'):
     # The desired CRS for the model must be same as positions, orientations
     epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
@@ -1307,19 +1362,19 @@
     :return lat_lon_hei: numpy array floats (n,3)
     latitude, longitude ellipsoid height.
     """
     geocsc = CRS.from_epsg(epsg_from)
     geod = CRS.from_epsg(epsg_to)
     transformer = Transformer.from_crs(geocsc, geod)
 
-    xECEF = position_ecef[:, 0].reshape((-1, 1))
-    yECEF = position_ecef[:, 1].reshape((-1, 1))
-    zECEF = position_ecef[:, 2].reshape((-1, 1))
+    x_ecef = position_ecef[:, 0].reshape((-1, 1))
+    y_ecef = position_ecef[:, 1].reshape((-1, 1))
+    z_ecef = position_ecef[:, 2].reshape((-1, 1))
 
-    (lat, lon, hei) = transformer.transform(xx=xECEF, yy=yECEF, zz=zECEF)
+    (lat, lon, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
 
     lat_lon_hei = np.zeros(position_ecef.shape)
     lat_lon_hei[:, 0] = lat.reshape((position_ecef.shape[0], 1))
     lat_lon_hei[:, 1] = lon.reshape((position_ecef.shape[0], 1))
     lat_lon_hei[:, 2] = hei.reshape((position_ecef.shape[0], 1))
 
     return lat_lon_hei
```

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/gis_tools.py` & `gref4hsi-0.1.9/gref4hsi/utils/gis_tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 from rasterio.warp import calculate_default_transform, reproject, Resampling
 from osgeo import gdal, osr
 from shapely.geometry import Polygon, mapping, MultiPoint
 from sklearn.neighbors import NearestNeighbors
 from spectral import envi
 import spectral as sp
 import h5py
+from scipy.spatial.transform import Rotation as RotLib
 
 # Lib modules
-from gref4hsi.scripts.colours import Image as Imcol
+from gref4hsi.utils.colours import Image as Imcol
 
 # ENVI datatype conversion dictionary
 dtype_dict = {1:np.uint8,
              2:np.int16,
              3:np.int32,
              4:np.float32,
              5:np.float64,
@@ -33,22 +34,14 @@
              15:np.uint64}
 
 class GeoSpatialAbstractionHSI():
     def __init__(self, point_cloud, transect_string, config_crs):
         self.name = transect_string
         self.points_geocsc = point_cloud
 
-        self.offX = config_crs.off_x
-        self.offY = config_crs.off_y
-        self.offZ = config_crs.off_z
-
-        if self.offX == -1:
-            print('Offsets have not been set, or they have been overwritten by default value -1')
-            RuntimeError
-
         self.epsg_geocsc = config_crs.epsg_geocsc
         
         self.n_lines = point_cloud.shape[0]
         self.n_pixels = point_cloud.shape[1]
         self.n_bands = point_cloud.shape[1]
 
         # A clean way of doing things would be to define 
@@ -63,21 +56,21 @@
 
         self.points_proj  = np.zeros(self.points_geocsc.shape) # Remains same if it is local
         
         geocsc = CRS.from_epsg(self.epsg_geocsc)
         proj = CRS.from_epsg(self.epsg_proj)
         transformer = Transformer.from_crs(geocsc, proj)
 
-        xECEF = self.points_geocsc[:,:,0].reshape((-1, 1))
-        yECEF = self.points_geocsc[:, :, 1].reshape((-1, 1))
-        zECEF = self.points_geocsc[:, :, 2].reshape((-1, 1))
+        x_ecef = self.points_geocsc[:,:,0].reshape((-1, 1))
+        y_ecef = self.points_geocsc[:, :, 1].reshape((-1, 1))
+        z_ecef = self.points_geocsc[:, :, 2].reshape((-1, 1))
 
         
 
-        (east, north, hei) = transformer.transform(xx=xECEF + self.offX, yy=yECEF + self.offY, zz=zECEF + self.offZ)
+        (east, north, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
 
         self.points_proj[:,:,0] = east.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
         self.points_proj[:, :, 1] = north.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
         self.points_proj[:, :, 2] = hei.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
 
         
 
@@ -126,14 +119,15 @@
         :param rgb_composite_dir: Directory to write data cubes
         :type rgb_composite_dir: string, path
         :param config_ortho: The relevant configurations for orthorectification
         :type config_ortho: Dictionary
         """
 
 
+
         
         n_bands = len(wavelengths)
         #
         n = radiance_cube.shape[0]
         m = radiance_cube.shape[1]
         k = radiance_cube.shape[2] # Number of bands
 
@@ -366,20 +360,20 @@
                     data = f[h5_hierarchy_item_path][()]
 
 
                     if data.ndim == 2:
                         if data.shape[1]  != self.n_pixels:
                             # For data of shape n_lines x j, for example camera positions, reshape to n_lines x n_pixels x j
                             j = data.shape[1]
-                            data = np.einsum('ijk, ik -> ijk', np.ones((self.n_lines, self.n_pixels, j), dtype=np.float32), data)
+                            data = np.einsum('ijk, ik -> ijk', np.ones((self.n_lines, self.n_pixels, j), dtype=np.float64), data)
                         else:
                             # For data with dimension n_lines x n_pixels, add third dimension
                             data = data.reshape((data.shape[0], data.shape[1], 1))
 
-                    data = data.astype(dtype = np.float32)
+                    data = data.astype(dtype = np.float64)
                     
                     # For first layer
                     if band_counter == 0:
                         anc_data_array = data
                     # For other layers, concatenate with existing layers
                     else:
                         anc_data_array = np.concatenate((anc_data_array, data), axis = 2)
@@ -434,119 +428,136 @@
                                                       metadata=metadata_anc,
                                                       interleave=interleave)
 
         
 
     @staticmethod
     def cube_to_raster_grid(coords, raster_transform_method, resolution):
+        """Function that takes projected coordinates (e.g. UTM 32 east and north) of ray intersections and computes an image grid
+
+        :param coords: _description_
+        :type coords: _type_
+        :param raster_transform_method: How the raster grid is calculated. "north_east" is standard and defines a rectangle along north/east. "minimal_rectangle" is memory optimal as it finds the smallest enclosing rectangle that wraps the points.
+        :type raster_transform_method: _type_
+        :param resolution: _description_
+        :type resolution: _type_
+        :return: _description_
+        :rtype: _type_
+        """
+
+
         if raster_transform_method == 'north_east':
-            # Creates the minimal area (and thus memory) rectangle around chunk
+            # Creates the minimal area (and thus memory) rectangle around points
             polygon = MultiPoint(coords).envelope
 
             # extract coordinates
             x, y = polygon.exterior.xy
 
-            idx_ul = 3
-            idx_ur = 2
-            idx_ll = 4
-
             suffix = '_north_east'
             
 
             
         elif raster_transform_method == 'minimal_rectangle':
             
-            # Creates the minimal area (and thus memory) rectangle around chunk
+            # Creates the minimal area (and thus memory) rectangle around points
             polygon = MultiPoint(coords).minimum_rotated_rectangle
 
             # extract coordinates
             x, y = polygon.exterior.xy
 
-            # Increasing indices are against the clock
             
-            # Determine basis vectors from data
-            idx_ul = 3
-            idx_ur = 2
-            idx_ll = 4
 
             suffix = '_rotated'
 
-        # ul means upper left, ll means lower left and so on
+        # Indices increase against the clock
+        # ul means upper left corner of polygon, ll means lower left and so on
+        idx_ul = 3
+        idx_ur = 2
+        idx_ll = 4
+
         x_ul = x[idx_ul]
         y_ul = y[idx_ul]
 
         x_ur = x[idx_ur]
         y_ur = y[idx_ur]
 
         x_ll = x[idx_ll]
         y_ll = y[idx_ll]
 
-        # The vector from upper-left corner aka origin to the upper-right equals lambda*e_basis_x
+        # The vector from the upper-left corner aka origin to the upper-right equals lambda*e_basis_x
         e_basis_x = np.array([x_ur-x_ul, y_ur-y_ul]).reshape((2,1))
         w_transect = np.linalg.norm(e_basis_x)
         e_basis_x /= w_transect
 
         # The y basis vector is the vector to the other edge
         e_basis_y = np.array([x_ll-x_ul, y_ll-y_ul]).reshape((2,1))
         h_transect = np.linalg.norm(e_basis_y)
         e_basis_y /= h_transect
-        e_basis_y *= -1 # Ensuring Right handedness (image storage y direction is o)
+        e_basis_y *= -1 # Ensuring right handedness (image storage y direction is opposite)
 
         R = np.hstack((e_basis_x, e_basis_y)) # 2D rotation matrix by definition
         
-        # Define origin/translation vector
+        # Define origin/translation vector as the upper left corner
         o = np.array([x[idx_ul], y[idx_ul]]).reshape((2))
 
         # Transformation matrix rigid body 2D
         Trb = np.zeros((3,3))
         Trb[0:2,0:2] = R
         Trb[0:2,2] = o
         Trb[2,2] = 1
 
+        # We operate with same resolution in X and Y. Note that for "minimal_rectangle" X, Y are NOT East and North. 
         s_x = resolution
         s_y = resolution
 
         S = np.diag(np.array([s_x, s_y, 1]))
 
-        # Reflection to account for opposite row/up direction
+        # Reflection matrix to account for opposite row/up direction
         Ref = np.diag(np.array([1, -1, 1]))
 
         # The affine transform is then expressed:
         Taff = Trb.dot(S).dot(Ref)
 
         # The metric width and length of the transect can give us the number of pixels
         width = int(np.ceil(w_transect/s_x))
         height = int(np.ceil(h_transect/s_y))
 
-        # Rasterio operates with a conventional affine
+        # Rasterio operates with a conventional affine geotransform
         a, b, c, d, e, f = Taff[0,0], Taff[0,1], Taff[0,2], Taff[1,0], Taff[1,1], Taff[1,2]
-
         transform = rasterio.Affine(a, b, c, d, e, f)
 
-        # Pixel centers reside at half coordinates.
+        # Define local orthographic pixel grid. Pixel centers reside at half coordinates.
         xi, yi = np.meshgrid(np.arange(width) + 0.5, 
                                 np.arange(height) + 0.5)
+        # To get homogeneous vector (not an actual z coordinate)
         zi = np.ones(xi.shape)
 
-        # Form homogeneous vectors
+        # Form homogeneous vectors (allows translation by multiplication)
         x_r = np.vstack((xi.flatten(), yi.flatten(), zi.flatten())).T
 
-        x_p = np.matmul(Taff, x_r.T).T # Map pixels to geographic
+        # Map orthographic pixels to projected system
+        x_p = np.matmul(Taff, x_r.T).T 
 
+        # Make a point vector of grid points to be used in nearest neighbor
         xy = np.vstack((x_p[:,0].flatten(), x_p[:,1].flatten())).T
         
-
-        # Locate nearest neighbors in a radius defined by the resolution
+        # Define NN search tree from intersection points
         tree = NearestNeighbors(radius=resolution).fit(coords)
 
-        # Calculate the nearest neighbors. Here we only use one neighbor, but other approaches could be employed
-        dist, indexes = tree.kneighbors(xy, 1)
+        # Calculate the nearest intersection point (in "coords") for each grid cell ("xy").
+        
+        # Here we only use one neighbor, and indexes is a vector of len(xy) where an element indexes(i)
+        # says that the closest point to xy[i] is coords[indexes[i]]. Since coords is just a flattened/reshaped version of intersection points
+        #, the data cube can be resampled by datacube_flat=datacube.reshape((dim1*dim2, dim3)) and 
+        # geographic_datacube_flat = datacube.reshape((dim1_geo*dim2_geo, dim3)) so that geographic_datacube_flat = datacube_flat[indexes,:]
+        n_neighbors = 1
+        dist, indexes = tree.kneighbors(xy, n_neighbors)
 
-        # We can mask the data by allowing interpolation with a radius of the resolution
-        mask_nn = dist > resolution
+        # We can mask the data by allowing points within a radius of 2x the resolution
+        mask_nn = dist > 2*resolution
         
         return transform, height, width, indexes, suffix, mask_nn
 
     @staticmethod
     def write_datacube_ENVI(memmap_gen_params, nodata, transform, datacube_path, wavelengths, fwhm, metadata, interleave, crs):
         """_summary_
 
@@ -570,36 +581,36 @@
         mx = memmap_gen_params['width']
         k = memmap_gen_params['datacube'].shape[1] # is collapsed datacube
 
         dtype_cube = memmap_gen_params['datacube'].dtype # is collapsed datacube
 
         crs_rasterio = CRS.from_string(crs)
 
-        writer_type = "envi"
+        writer_type = "envi" # Hardcoded
 
         # Make some simple modifications
         data_file_path = datacube_path + '.' + interleave
         header_file_path = datacube_path + '.hdr'
 
+        if os.path.exists(header_file_path):
+            return
+
         # Clean the files generated by rasterio
         def write_band(args):
             band_data, index, dst = args
             dst.write(band_data, index + 1)
 
         
         def write_band_gdal(args):
             band_data, index, dst = args
             dst.GetRasterBand(index + 1).WriteArray(band_data)
         
         if os.path.exists(data_file_path):
             os.remove(data_file_path)
             os.remove(header_file_path)
-        
-        import time
-        start_time = time.time()
 
         if writer_type == "rasterio":
             # Assuming ortho_datacube is a 3D NumPy array with shape (k, nx, mx)
             with rasterio.open(data_file_path, 'w', driver='ENVI', height=nx, width=mx, count=k, crs=crs_rasterio, dtype=dtype_cube, transform=transform, nodata=nodata) as dst:
                 
                 # Create a ThreadPoolExecutor with as many threads as bands
                 with ThreadPoolExecutor(max_workers=k) as executor:
@@ -643,20 +654,20 @@
             # Create ENVI image without using a context manager
             dst = envi.create_image(datacube_path + '.hdr', interleave='bsq', metadata=header, force=True)
 
             mm = dst.open_memmap(writable=True)
 
             GeoSpatialAbstractionHSI.write_datacube_memmap(memmap_array=mm, **memmap_gen_params)
 
-            #mm[:] = ortho_datacube_reshaped
+            
 
 
 
-        dt = time.time() - start_time
-        print(f"The time difference for {writer_type} was {dt} seconds")
+        
+        
         
         header = sp.io.envi.read_envi_header(datacube_path + '.hdr') # Open for extraction
         header.pop('band names')
 
         # Nobody in the history of the world could have come up with a more annoying bug.
         # Apparently, the CRS string is written with white spaces by rasterio/GDAL, wheras it should have none.
         header['coordinate system string'] = '{' + ",".join(header['coordinate system string']) + '}'
@@ -718,82 +729,79 @@
         header.pop('band names') # Remove defaults
 
         for meta_key, value in metadata.items():
             header[meta_key] = value
 
         sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
 
-    def compare_hsi_composite_with_rgb_mosaic(self):
-        self.rgb_ortho_path = self.config['Absolute Paths']['rgb_ortho_path']
-        self.hsi_composite = self.config['Absolute Paths']['rgb_composite_folder'] + self.name + '.tif'
-        self.rgb_ortho_reshaped = self.config['Absolute Paths']['rgbOrthoReshaped'] + self.name + '.tif'
-        self.dem_path = self.config['Absolute Paths']['dem_path']
-        self.dem_reshaped = self.config['Absolute Paths']['demReshaped'] + self.name + '_dem.tif'
-
-        self.resample_rgb_ortho_to_hsi_ortho()
-
-        self.resample_dem_to_hsi_ortho()
-
+    @staticmethod
+    def compare_hsi_composite_with_rgb_mosaic(hsi_composite_path, ref_ortho_reshaped_path):
+        """Compares an HSI orthomosaic """
+        
+        
 
-        raster_rgb = gdal.Open(self.rgb_ortho_reshaped, gdal.GA_Update)
+        
+        # The RGB orthomosaic after reshaping (the reference)
+        raster_rgb = gdal.Open(ref_ortho_reshaped_path, gdal.GA_Update)
         xoff1, a1, b1, yoff1, d1, e1 = raster_rgb.GetGeoTransform()  # This should be equal
         raster_rgb_array = np.array(raster_rgb.ReadAsArray())
         R = raster_rgb_array[0, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
         G = raster_rgb_array[1, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
         B = raster_rgb_array[2, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
         # del raster_array1
         ortho_rgb = np.concatenate((R, G, B), axis=2)
         rgb_image = Imcol(ortho_rgb)
 
-        raster_hsi = gdal.Open(self.hsi_composite)
+        # The HSI composite raster (the match)
+        raster_hsi = gdal.Open(hsi_composite_path)
         raster_hsi_array = np.array(raster_hsi.ReadAsArray())
         xoff2, a2, b2, yoff2, d2, e2 = raster_hsi.GetGeoTransform()
-        self.transform_pixel_projected = raster_hsi.GetGeoTransform()
+        transform_pixel_projected = raster_hsi.GetGeoTransform()
         R = raster_hsi_array[0, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
         G = raster_hsi_array[1, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
         B = raster_hsi_array[2, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
-
         ortho_hsi = np.concatenate((R, G, B), axis=2)
 
+        # Some form of image processing
         max_val = np.percentile(ortho_hsi.reshape(-1), 99)
         ortho_hsi /= max_val
         ortho_hsi[ortho_hsi > 1] = 1
         ortho_hsi = (ortho_hsi * 255).astype(np.uint8)
         ortho_hsi[ortho_hsi == 0] = 255
         hsi_image = Imcol(ortho_hsi)
 
-
-        # Dem
-        self.raster_dem = rasterio.open(self.dem_reshaped)
-
-
         # Adjust Clahe
         hsi_image.clahe_adjustment()
         rgb_image.clahe_adjustment()
 
         hsi_image.to_luma(gamma=False, image_array = hsi_image.clahe_adjusted)
         rgb_image.to_luma(gamma=False, image_array= rgb_image.clahe_adjusted)
 
-        self.compute_sift_difference(hsi_image.luma_array, rgb_image.luma_array)
+        uv_vec_hsi, uv_vec_rgb, diff_AE_pixels = GeoSpatialAbstractionHSI.compute_sift_difference(hsi_image.luma_array, rgb_image.luma_array)
+
 
+        image_resolution = a2
+        diff_AE_meters = diff_AE_pixels*image_resolution
+        return uv_vec_hsi, uv_vec_rgb, diff_AE_meters, transform_pixel_projected
 
 
-    def resample_rgb_ortho_to_hsi_ortho(self):
+    @staticmethod
+    def resample_rgb_ortho_to_hsi_ortho(ref_ortho_path, hsi_composite_path, ref_ortho_reshaped_path):
         """Reproject RGB orthophoto to match the shape and projection of HSI raster.
 
         Parameters
         ----------
         infile : (string) path to input file to reproject
         match : (string) path to raster with desired shape and projection
         outfile : (string) path to output file tif
         """
 
-        infile = self.rgb_ortho_path
-        match = self.hsi_composite
-        outfile = self.rgb_ortho_reshaped
+        infile = ref_ortho_path
+        match = hsi_composite_path
+        outfile = ref_ortho_reshaped_path
         # open input
         with rasterio.open(infile) as src:
             src_transform = src.transform
 
             # open input to match
             with rasterio.open(match) as match:
                 dst_crs = match.crs
@@ -810,41 +818,41 @@
             # set properties for output
             dst_kwargs = src.meta.copy()
             dst_kwargs.update({"crs": dst_crs,
                                "transform": dst_transform,
                                "width": dst_width,
                                "height": dst_height,
                                "nodata": 0})
-            #print("Coregistered to shape:", dst_height, dst_width, '\n Affine', dst_transform)
+            
             # open output
             with rasterio.open(outfile, "w", **dst_kwargs) as dst:
                 # iterate through bands and write using reproject function
                 for i in range(1, src.count + 1):
                     reproject(
                         source=rasterio.band(src, i),
                         destination=rasterio.band(dst, i),
                         src_transform=src.transform,
                         src_crs=src.crs,
                         dst_transform=dst_transform,
                         dst_crs=dst_crs,
                         resampling=Resampling.cubic)
 
-    def resample_dem_to_hsi_ortho(self):
+    def resample_dem_to_hsi_ortho(dem_path, hsi_composite_path, dem_reshaped):
         """Reproject a file to match the shape and projection of existing raster.
 
         Parameters
         ----------
         infile : (string) path to input file to reproject
         match : (string) path to raster with desired shape and projection
         outfile : (string) path to output file tif
         """
 
-        infile = self.dem_path
-        match = self.hsi_composite
-        outfile = self.dem_reshaped
+        infile = dem_path
+        match = hsi_composite_path
+        outfile = dem_reshaped
         # open input
         with rasterio.open(infile) as src:
             src_transform = src.transform
 
             # open input to match
             with rasterio.open(match) as match:
                 dst_crs = match.crs
@@ -875,27 +883,29 @@
                         destination=rasterio.band(dst, i),
                         src_transform=src.transform,
                         src_crs=src.crs,
                         dst_transform=dst_transform,
                         dst_crs=dst_crs,
                         resampling=Resampling.cubic)
 
+    @staticmethod
+    def compute_sift_difference(gray1, gray2):
+        """Simply matches two grayscale images using SIFT"""
 
-    def compute_sift_difference(self, gray1, gray2):
         gray1 = (gray1 - np.min(gray1)) / (np.max(gray1) - np.min(gray1))
         gray2 = (gray2 - np.min(gray2)) / (np.max(gray2) - np.min(gray2))
 
         gray1 = (gray1 * 255).astype(np.uint8)
         gray2 = (gray2 * 255).astype(np.uint8)
 
 
         # Find the keypoints and descriptors with SIFT
         sift = cv.SIFT_create()
         kp2, des2 = sift.detectAndCompute(gray2, None)
-        print('Key points found')
+        
         kp1, des1 = sift.detectAndCompute(gray1, None)
         FLANN_INDEX_KDTREE = 1
         index_params = dict(algorithm=FLANN_INDEX_KDTREE, trees=5)
         search_params = dict(checks=50)
         flann = cv.FlannBasedMatcher(index_params, search_params)
         matches = flann.knnMatch(des1, des2, k=2)
         # store all the good matches as per Lowe's ratio test. We changed 0.8 to 0.85 to get more matches
@@ -920,69 +930,21 @@
             uv_vec_rgb[i,:] = uv2
 
             ## Conversion to global coordinates
             diff_u[i] = uv2[0] - uv1[0]
             diff_v[i] = uv2[1] - uv1[1]
 
         img3 = cv.drawMatches(gray1, kp1, gray2, kp2, good, None, **draw_params)
-        plt.imshow(img3, 'gray')
-        plt.show()
-
-        #print(len(good))
-
-        med_u = np.median(diff_u[np.abs(diff_u) < 10])
-        med_v = np.median(diff_v[np.abs(diff_u) < 10])
-#
-        #print(np.mean(np.abs(diff_u[np.abs(diff_u) < 100])))
-        #print(np.mean(np.abs(diff_v[np.abs(diff_u) < 100])))
-##
-        #print(np.median(np.abs(diff_u[np.abs(diff_u) < 100]  - med_u)))
-        #print(np.median(np.abs(diff_v[np.abs(diff_u) < 100] - med_v)))
-##
-        MAD_u = np.median(np.abs(diff_u[np.abs(diff_u) < 100]  - med_u))
-        MAD_v = np.median(np.abs(diff_v[np.abs(diff_u) < 100] - med_v))
-##
-        #MAD_tot = np.median(np.sqrt((diff_v[np.abs(diff_u) < 100] - med_v)**2 + (diff_u[np.abs(diff_u) < 100] - med_u)**2))
-        # IF the disagreement is more than 100 pixels, omit it
-        diff = np.sqrt(diff_u ** 2 + diff_v ** 2)
-
-        MAE_tot = np.median(diff[diff < 5])
-        print(len(good))
-        print(MAE_tot)
-        self.feature_uv_hsi = uv_vec_hsi[diff < 5, :]
-        self.feature_uv_rgb = uv_vec_rgb[diff < 5, :]
-        print(len(self.feature_uv_rgb))
-#
-        #print(med_u)
-        #print(med_v)
-        #print(MAD_u)
-        #print(MAD_v)
-
-        #plt.imshow(gray1)
-
-
-
-
-
-        #plt.scatter(uv_vec[:,0][np.abs(diff_u) < 100], uv_vec[:,1][np.abs(diff_u) < 100], c = diff_u[np.abs(diff_u) < 100] - np.median(diff_u[np.abs(diff_u) < 100]))
-        #plt.colorbar()
+        #plt.imshow(img3, 'gray')
         #plt.show()
-
-
-        #plt.hist(diff_u[np.abs(diff) < 100], 50)
-        #plt.title('MAD u: ' + str(np.round(MAD_u,2)))
-        #plt.xlim([-100, 100])
-        #plt.show()
-
-        plt.hist(diff[diff < 10]*0.002, 50)
-        #plt.title('MAD v: ' + str(np.round(MAD_v, 2)))
-        #plt.xlim([-100, 100])
-        plt.show()
-        #
-        self.diff = diff
+##
+        # The absolute errors
+        diff_AE = np.sqrt(diff_u ** 2 + diff_v ** 2)
+        
+        return uv_vec_hsi, uv_vec_rgb, diff_AE
 
 
 
     def map_pixels_back_to_datacube(self, w_datacube):
         """The projected formats can be transformed back with four integer transforms and interpolated accordingly"""
         """As a simple strategy we perform bilinear interpolation"""
 
@@ -1015,19 +977,19 @@
             geocsc = CRS.from_epsg(self.epsg_geocsc)
             proj = CRS.from_epsg(self.epsg_proj)
             transformer = Transformer.from_crs(proj, geocsc)
             self.features_points = np.zeros((xp.shape[0], 3))
 
 
 
-            (xECEF, yECEF, zECEF) = transformer.transform(xx=xp, yy=yp, zz=zp)
+            (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
 
-            self.features_points[:, 0] = xECEF - self.offX
-            self.features_points[:, 1] = yECEF - self.offY
-            self.features_points[:, 2] = zECEF - self.offZ
+            self.features_points[:, 0] = x_ecef
+            self.features_points[:, 1] = y_ecef
+            self.features_points[:, 2] = z_ecef
 
 
 
 
         #
 
         self.v_datacube_hsi = np.zeros((v.shape[0], 4))
@@ -1057,14 +1019,128 @@
         self.x1_x_hsi = v - np.floor(v)
         self.y1_y_hsi = u - np.floor(u)
 
         #self.x1_x_rgb = v_rgb - np.floor(v_rgb)
         #self.y1_y_rgb = u_rgb - np.floor(u_rgb)
 
 
+    def compute_reference_points_ecef(uv_vec_ref, transform_pixel_projected, dem_resampled_path, epsg_proj, epsg_geocsc=4978):
+    
+    
+        """Computes ECEF reference points from a features detected on the orthomosaic and the DEM"""
+        x = uv_vec_ref[:, 0]
+        y = uv_vec_ref[:, 1]
+
+        # Sample the terrain raster to get a projected position of data 
+        raster_dem = rasterio.open(dem_resampled_path)
+        xoff, a, b, yoff, d, e = transform_pixel_projected
+
+        # Convert the pixel coordinates into true coordinates (e.g. UTM N/E)
+        xp = a * x + b * y + xoff + 0.5*a 
+        yp = d * x + e * y + yoff + 0.5*e
+        zp = np.zeros(yp.shape)
+        for i in range(xp.shape[0]):
+            temp = [x for x in raster_dem.sample([(xp[i], yp[i])])]
+            zp[i] = float(temp[0])
+
+        # Transform points to true 3D via pyproj
+        geocsc = CRS.from_epsg(epsg_geocsc)
+        proj = CRS.from_epsg(epsg_proj)
+        transformer = Transformer.from_crs(proj, geocsc)
+        ref_points_ecef = np.zeros((xp.shape[0], 3))
+        (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
+
+        ref_points_ecef[:, 0] = x_ecef
+        ref_points_ecef[:, 1] = y_ecef
+        ref_points_ecef[:, 2] = z_ecef
+        
+        return ref_points_ecef
 
+    def compute_position_orientation_features(uv_vec_hsi, pixel_nr_image, unix_time_image, position_ecef, quaternion_ecef, time_pose, nodata):
+        """Returns the positions, orientations and pixel numbers corresponding to the features. 
+        Also computes a feature mask identifying features that are invalid"""
+        rows = uv_vec_hsi[:, 1]
+        cols = uv_vec_hsi[:, 0]
 
+        # Determine mask
+        x0 = np.floor(cols).astype(int)
+        x1 = x0 + 1
+        y0 = np.floor(rows).astype(int)
+        y1 = y0 + 1
 
+        # All 4 neighbors (as used by bilinear interpolation) should be valid data points
+        feature_mask = np.all([pixel_nr_image[y0, x0].reshape(-1) != nodata,
+               pixel_nr_image[y1, x0].reshape(-1) != nodata,
+               pixel_nr_image[y0, x1].reshape(-1) != nodata,
+               pixel_nr_image[y1, x1].reshape(-1) != nodata], axis=0)
 
 
+        pixel_nr_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(pixel_nr_image, x = cols, y = rows)
+        time_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(unix_time_image, x = cols, y = rows)
+
+        pixel_vec_valid = pixel_nr_vec[feature_mask]
+        time_vec_valid = time_vec[feature_mask]
+
+        
+        from scipy.interpolate import interp1d
+        from gref4hsi.utils import geometry_utils as geom
+        
+
+        rotation_ecef = RotLib.from_quat(quaternion_ecef)
+
+        # Interpolates positions linearly and quaterinons by Slerp
+        position_vec, quaternion_vec = geom.interpolate_poses(time_pose, 
+                                            position_ecef, 
+                                            rotation_ecef,  
+                                            timestamps_to=time_vec_valid)
+        
+        return pixel_vec_valid, time_vec_valid, position_vec, quaternion_vec, feature_mask
+        
+
+        
+
+    @staticmethod
+    def feature_matches_to_GCP(features_hsi, features_ref, pixel_nr_raster, time_raster):
+        """Function to establish 2D feature positions u, j in raw cube, as well as true reference positions X, Y, Z
+
+        :param features_hsi: _description_
+        :type features_hsi: _type_
+        :param features_ref: _description_
+        :type features_ref: _type_
+        :param pixel_nr_raster: _description_
+        :type pixel_nr_raster: _type_
+        :param time_raster: _description_
+        :type time_raster: _type_
+        """
+
+        return None
+
+
+    # COPIED from https://stackoverflow.com/questions/12729228/simple-efficient-bilinear-interpolation-of-images-in-numpy-and-python
+    @staticmethod
+    def bilinear_interpolate(im, x, y):
+        
+        x = np.asarray(x)
+        y = np.asarray(y)
+
+        x0 = np.floor(x).astype(int)
+        x1 = x0 + 1
+        y0 = np.floor(y).astype(int)
+        y1 = y0 + 1
+
+        x0 = np.clip(x0, 0, im.shape[1]-1);
+        x1 = np.clip(x1, 0, im.shape[1]-1);
+        y0 = np.clip(y0, 0, im.shape[0]-1);
+        y1 = np.clip(y1, 0, im.shape[0]-1);
+
+        Ia = im[ y0, x0 ]
+        Ib = im[ y1, x0 ]
+        Ic = im[ y0, x1 ]
+        Id = im[ y1, x1 ]
+
+        wa = (x1-x) * (y1-y)
+        wb = (x1-x) * (y-y0)
+        wc = (x-x0) * (y1-y)
+        wd = (x-x0) * (y-y0)
 
+        return wa*Ia + wb*Ib + wc*Ic + wd*Id
```

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/photogrammetry_utils.py` & `gref4hsi-0.1.9/gref4hsi/utils/photogrammetry_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import Metashape as MS
+
 import ntpath
 import h5py
 import pandas as pd
 import numpy as np
 from PIL import Image
 import numpy as np
 from PIL import Image, ImageOps, ExifTags
```

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/specim_parsing_utils.py` & `gref4hsi-0.1.9/gref4hsi/utils/specim_parsing_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,16 +110,15 @@
 
         fov_arr = df_fov.values[:, 1]
 
         param_dict = Specim.fov_2_param(fov = fov_arr)
         
         file_name_calib = self.config['Absolute Paths']['hsi_calib_path']
 
-        CalibHSI(file_name_cal_xml=file_name_calib, 
-                 config = self.config, 
+        CalibHSI(file_name_cal_xml=file_name_calib,
                  mode = 'w', 
                  param_dict = param_dict)
 
     def read_nav_file(self, nav_file_path, date):
         # Convert date string to datetime object
         date_obj = datetime.strptime(date, "%Y-%m-%d")
         # Open file for reading.
@@ -251,15 +250,15 @@
         self.sync_data = sync_data
 
 """Writer for the h5 file format using a dictionary. The user provides h5 hierarchy paths as values and keys are the names given to the attributes of the specim object.
 A similar write process could be applied to metadata."""
 def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
     with h5py.File(h5_filename, 'w', libver='latest') as f:
         for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-            print(attribute_name)
+            #print(attribute_name)
             dset = f.create_dataset(name=h5_hierarchy_item_path, 
                                             data = getattr(specim_object, attribute_name))            
 
 def add_byte_order_to_envi_header(header_file_path, byte_order_value):
     """Function added to remedy lacking byte-order entry in header files of radiometric calibration data
 
     :param header_file_path: _description_
@@ -285,40 +284,43 @@
     with open(header_file_path, 'w') as f:
         f.writelines(header_lines)
 
 
 
 def main(config, config_specim):
     
-    # Every 1000 lines take up 0.85 GB at 8 Byte float. Therefore it could make sense to partition things that are larger than 2000 lines (sub GB for 32 float/4 byte)
-    #dtype = np.float32
-    #transect_chunk_size = 2000 # The number of lines
+    # Script that calibrates data and reforms to h5 file format.
     dtype = config_specim.dtype_datacube
     transect_chunk_size = config_specim.lines_per_chunk
     cal_dir = config_specim.cal_dir
    
     mission_dir = config_specim.specim_raw_mission_dir
 
     mission_name = Path(mission_dir).name
     out_dir = config_specim.reformatted_missions_dir
-    config_file_path = out_dir + config_specim.config_file_name
+    config_file_path = os.path.join(out_dir, config_specim.config_file_name)
 
-    prepend_data_dir_to_relative_paths(config_path=config_file_path, DATA_DIR=out_dir)
+    #prepend_data_dir_to_relative_paths(config_path=config_file_path, DATA_DIR=out_dir)
 
     specim_object = Specim(mission_path=mission_dir, config=config)
 
     # Patterns for searching data cube files
     PATTERN_ENVI = '*.hdr'
-    capture_dir = mission_dir + '/capture/'
+
+    # Expects the captured data to reside in capture subfolder
+    capture_dir = os.path.join(mission_dir, 'capture')
+
+    # Path for searching (avoid explicit )
     search_path_envi = os.path.normpath(os.path.join(capture_dir, PATTERN_ENVI))
     envi_hdr_file_path = glob.glob(search_path_envi)[0]
 
+    # Read out data
     spectral_image_obj = envi.open(envi_hdr_file_path)
 
-    # Read all meta data from raw file 
+    # Read all meta data from header file (currently hard coded, but could be avoided I guess)
     class Metadata:
         pass
 
     metadata_obj = Metadata()
     # Could do this in iteration, but it would need to specify type (I think)
     metadata_obj.autodarkstartline = int(spectral_image_obj.metadata['autodarkstartline'])
     metadata_obj.n_lines = int(spectral_image_obj.metadata['lines'])
@@ -330,15 +332,15 @@
     metadata_obj.file_type = spectral_image_obj.metadata['file type']
     metadata_obj.sensor_type = spectral_image_obj.metadata['sensor type']
     metadata_obj.acquisition_date = spectral_image_obj.metadata['acquisition date']
     metadata_obj.sensorid = spectral_image_obj.metadata['sensorid']
     metadata_obj.interleave = spectral_image_obj.metadata['interleave']
     metadata_obj.data_type = spectral_image_obj.metadata['data type']
     
-    # Derived from knowledge of the sensor (sensor constants)
+    # Derived from knowledge of the sensor (sensor constants that could differ for other sensors)
     metadata_obj.binning_spatial = int(ACTIVE_SENSOR_SPATIAL_PIXELS/metadata_obj.n_pix)
     metadata_obj.binning_spectral = int(ACTIVE_SENSOR_SPECTRAL_PIXELS/metadata_obj.n_bands)
 
     # Allow Specim Methods to access metadata
     specim_object.metadata_obj = metadata_obj 
     # -
 
@@ -409,23 +411,22 @@
 
     camera_calib_xml_dir = config['Absolute Paths']['calib_folder']
 
     file_name_xml = 'HSI_' + str(metadata_obj.binning_spatial) + 'b.xml'
     xml_cal_write_path = camera_calib_xml_dir + file_name_xml
 
     CalibHSI(file_name_cal_xml= xml_cal_write_path, 
-                    config = config, 
                     mode = 'w', 
                     param_dict = param_dict)
 
 
     # Set value in config file:
     config.set('Relative Paths', 'hsi_calib_path', value = xml_cal_write_path)
 
-    config_file_path = out_dir + config_specim.config_file_name
+    
 
     # Write the config object 
     with open(config_file_path, 'w') as configfile:
             config.write(configfile)
     # -
 
     
@@ -437,27 +438,29 @@
     """Extract radiometric frame from dedicated file"""
 
     PATTERN_ENVI_CAL = '*_' +str(metadata_obj.binning_spectral) + 'x' +  str(metadata_obj.binning_spatial) + '.hdr'
 
     search_path_envi_cal = os.path.normpath(os.path.join(cal_dir, PATTERN_ENVI_CAL))
     ENVI_CAL_HDR_FILE_PATH = glob.glob(search_path_envi_cal)[0]
 
+    # For allowing spectral module to read
     RAD_CAL_BYTE_ORDER = 0
 
     add_byte_order_to_envi_header(header_file_path=ENVI_CAL_HDR_FILE_PATH, byte_order_value=RAD_CAL_BYTE_ORDER)
 
     ENVI_CAL_IMAGE_FILE_PATH = ENVI_CAL_HDR_FILE_PATH.split('.')[0] + '.cal' # SPECTRAL does not expect this suffix by default
 
-    # For some reason, the byte order
+    # For some reason, the byte order is needed
     radiometric_image_obj = envi.open(ENVI_CAL_HDR_FILE_PATH, image = ENVI_CAL_IMAGE_FILE_PATH)
 
     cal_n_lines = int(radiometric_image_obj.metadata['lines'])
     cal_n_bands = int(radiometric_image_obj.metadata['bands'])
     cal_n_pix = int(radiometric_image_obj.metadata['samples'])
 
+    # For calibration
     radiometric_frame = radiometric_image_obj[:,:,:].reshape((cal_n_pix, cal_n_bands))
 
     specim_object.radiometric_frame = radiometric_frame
     # -
 
     # The next step is to load the darkframes
 
@@ -474,19 +477,19 @@
 
     # -
 
     # The navigation data is given as messages is a *.nav file. Locate the file and parse it into a suitable format.
 
     # +
     # Extract the starting/stopping lines
-    START_STOP_DIR = mission_dir + '/start_stop_lines'
+    START_STOP_DIR = os.path.join(mission_dir, 'start_stop_lines')
     
     # Allow software to function if start_stop_lines not specified
-    if not os.path.exists(START_STOP_DIR + '/'):
-        os.mkdir(START_STOP_DIR + '/')
+    if not os.path.exists(START_STOP_DIR):
+        os.mkdir(START_STOP_DIR)
         # Chunk according to chunk size
         start_lines = np.arange(start=0,
                                 stop=metadata_obj.autodarkstartline, 
                                 step=transect_chunk_size)
 
         stop_lines = np.arange(start=transect_chunk_size, 
                                stop=metadata_obj.autodarkstartline + transect_chunk_size, 
@@ -496,15 +499,15 @@
 
         # Make dataframe
         start_stop_data = {'line_start' : start_lines,
                            'line_stop' : stop_lines}
         
         df_start_stop = pd.DataFrame(start_stop_data)
 
-        df_start_stop.to_csv(path_or_buf = START_STOP_DIR + '/' + 'start_stop_lines.txt', sep=' ')
+        df_start_stop.to_csv(path_or_buf = os.path.join(START_STOP_DIR, 'start_stop_lines.txt'), sep=' ')
 
 
 
     PATTERN_START_STOP = '*.txt'
     
 
     search_path_lines_start_stop = os.path.normpath(os.path.join(START_STOP_DIR, PATTERN_START_STOP))
@@ -534,39 +537,34 @@
     # +
     
 
 
     df_imu = pd.DataFrame(specim_object.imu_data)
     df_gnss = pd.DataFrame(specim_object.gnss_data)
     df_sync_hsi = pd.DataFrame(specim_object.sync_data)
-    # Define the time stamps of HSI frames
-
-
-    # Let's consider this an interpolation problem. Every new sync means a new fps # frames:
+    
+    # Define the time stamps of HSI frames (special fix for Specim)
     sync_frames = df_sync_hsi['HsiFrameNum']
     sync_times = df_sync_hsi['TimestampAbs']
     hsi_frames = np.arange(metadata_obj.autodarkstartline)
+    hsi_timestamps_total = interp1d(x = sync_frames, y = sync_times, fill_value = 'extrapolate')(x = hsi_frames)
 
 
-    hsi_timestamps_total = interp1d(x = sync_frames, y= sync_times, fill_value = 'extrapolate')(x = hsi_frames)
-
-
-    # Secondly, for ease, let us interpolate position data to imu time (avoids rotational interpolation)
+    # For ease, let us interpolate position data to imu time (allows one timestamp for nav data)
     imu_time = df_imu['TimestampAbs']
 
     # Drop the specified regular clock time (as it is not needed)
     df_gnss = df_gnss.drop(columns=['TimestampClock'])
 
     # Interpolate each column in GNSS data based on 'imu_time'
     interpolated_values = {
         column: np.interp(imu_time, df_gnss['TimestampAbs'], df_gnss[column])
         for column in df_gnss.columns if column != 'TimestampAbs'
     }
 
-
     # Create a new DataFrame with the interpolated values
     df_gnss_interpolated = pd.DataFrame({'time': imu_time, **interpolated_values})
 
     # The position defined in geodetic coordinates
     lat = np.array(df_gnss_interpolated['Lat']).reshape((-1,1))
     lon = np.array(df_gnss_interpolated['Lon']).reshape((-1,1))
     ellipsoid_height = np.array(df_gnss_interpolated['AltMSL'] + df_gnss_interpolated['AltGeoid']).reshape((-1,1))
@@ -575,15 +573,15 @@
     x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
 
     # Lastly, calculate the roll, pitch, yaw
     roll = np.array(df_imu['Roll']).reshape((-1,1))
     pitch = np.array(df_imu['Pitch']).reshape((-1,1))
     yaw = np.array(df_imu['Yaw']).reshape((-1,1))
 
-    # Roll pitch yaw are stacked with in an unintuitive attribute. The euler angles with rotation order ZYX are Yaw Pitch Roll
+    # Roll pitch yaw are stacked in attribute eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
     specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
 
     # Position is stored as ECEF cartesian coordinates (mutually orthogonal axis) instead of spherioid-like lon, lat, alt
     specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
     specim_object.nav_timestamp = imu_time
     specim_object.t_exp_ms = metadata_obj.t_exp_ms
 
@@ -610,15 +608,15 @@
 
     # # Chunking the recording to user defined sizes and writing it to disk
 
     # +
     # Define h5 file name
     h5_folder = config['Absolute Paths']['h5_folder']
 
-    # It is nicer to deal with 4 byte numbers in general
+    # Each line in start_stop defines a transect
     n_transects = df_start_stop.shape[0]
     for transect_number in range(n_transects):
         start_line = df_start_stop['line_start'][transect_number]
         stop_line = df_start_stop['line_stop'][transect_number]
 
         n_chunks = int(np.ceil((stop_line-start_line)/transect_chunk_size))
 
@@ -627,16 +625,15 @@
             chunk_start_idx = start_line + transect_chunk_size*chunk_number
 
             if chunk_number == n_chunks-1:
                 chunk_stop_idx = stop_line
             else:
                 chunk_stop_idx = chunk_start_idx + transect_chunk_size
 
-
-
+            #print(f'Chunk from line {chunk_start_idx} to line {chunk_stop_idx} is being written')
             data_cube = spectral_image_obj[chunk_start_idx:chunk_stop_idx, :, :]
             # Calibration equation
             specim_object.radiance_cube = ( (data_cube - dark_frame)*radiometric_frame/(metadata_obj.t_exp_ms/1000) ).astype(dtype = dtype) # 4 Byte
             specim_object.hsi_timestamps = hsi_timestamps_total[chunk_start_idx:chunk_stop_idx]
 
             # Possible to name files with <PREFIX>_<time_start>_<Transect#>_<Chunk#>.h5
             h5_filename = h5_folder + mission_name + '_transectnr_' + str(int(transect_number)) + '_chunknr_' + str(int(chunk_number)) + '.h5'
```

### Comparing `gref4hsi-0.1.5/gref4hsi/utils/uhi_parsing_utils.py` & `gref4hsi-0.1.9/gref4hsi/utils/uhi_parsing_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 AttributeError
         else:
             self.time = time
             
         self.value = value
     def interpolate(self, time_interp):
         self.time_interp = time_interp
-        self.value_interp = interp1d(x = self.time, y = self.value, kind='linear', fill_value='extrapolate')(x=self.time_interp)
+        self.value_interp = interp1d(x = self.time, y = self.value, kind='nearest', fill_value='extrapolate')(x=self.time_interp)
             
 
 class NAV:
     """Very simple object allowing for setting time-referenced nav data. Entities end up having four attributes:
     time: Original time stamps
     value: Values
     time_interp: Time stamps interpolated (if interpolate has been run)
@@ -256,16 +256,15 @@
         param_dict['ty'] = t_hsi_body[1]
         param_dict['tz'] = t_hsi_body[2]
         
         file_name_xml = 'HSI_' + str(binning_spatial) + 'b.xml'
         CAMERA_CALIB_XML_DIR = config['Absolute Paths']['calib_folder']
         xml_cal_write_path = CAMERA_CALIB_XML_DIR + file_name_xml
 
-        CalibHSI(file_name_cal_xml= xml_cal_write_path, 
-                        config = config, 
+        CalibHSI(file_name_cal_xml= xml_cal_write_path,  
                         mode = 'w', 
                         param_dict = param_dict)
 
 
         # Set value in config file and update:
         config.set('Relative Paths', 'hsi_calib_path', value = 'Input/Calib/' + file_name_xml)
 
@@ -283,14 +282,19 @@
     
 
 def read_nav_from_mat(mat_filename):
     """Function for reading mat data from the beast format into a NAV object"""
     mat_contents = {}
     mat_contents = loadmat(filename=mat_filename)
 
+    m_att = mat_contents['ATTENTION']
+    #m_att['SpotOnTime'][m_att['Note'] == 'UHI s1 start']
+
+    
+
     
     # +
     """Cell defining all nav data of relevance"""
 
     # For ease, read position orientation data into structs
     nav = NAV()
 
@@ -322,15 +326,15 @@
                         value = mat_contents['ALTIMETER']['Altitude']) # Altimeter readings
     
     return nav
 
 def write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH):
     
     # The time stamp used for writing
-    nav_timestamp_rov = nav.roll.time
+    nav_timestamp_rov = nav.yaw.time
 
     # Interpolate nav data to those times
     nav.interpolate(time_interp=nav_timestamp_rov)
 
     lon = nav.lon.value_interp
     lat = nav.lat.value_interp
     h = -nav.pos_z.value_interp # Depth is opposite of height
@@ -584,15 +588,15 @@
 
 
 def uhi_beast(config, config_uhi):
     MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
     
 
     # For writing
-    config_file_path = MISSION_PATH + 'configuration.ini'
+    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
 
     SPATIAL_PIXELS = 1936 # Same for almost all UHI
     
 
     INPUT_DIR = MISSION_PATH + 'Input/'
 
     h5_folder = config['Absolute Paths']['h5_folder']
@@ -616,22 +620,25 @@
 
     number_of_h5_files = len(H5_FILE_PATHS)
 
     h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
             'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
             'fov': config['HDF.calibration']['fov'],
             'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            'rgb_frames' : config['HDF.rgb']['rgb_frames'],
-            'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']}
+            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
+            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
+            }
     
     time_offset = config_uhi.time_offset_sec
     lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
 
-    from gref4hsi.utils.photogrammetry_utils import Photogrammetry
-    agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
+    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
+    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
+    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
+    # Should interface towards ODM as well
 
     for h5_index in range(number_of_h5_files):
         H5_FILE_PATH = H5_FILE_PATHS[h5_index]
 
         # Read the specified entries
         hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
 
@@ -662,29 +669,29 @@
         if h5_index == 0:
             point_cloud_altimeter_total = point_cloud_altimeter
         else:
             point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
         
 
 
-        # If desirable to write to Agisoft type format
+        """# If desirable to write to Agisoft type format
         if config_uhi.agisoft_process:
             nav_rgb = nav
             nav_rgb.interpolate(time_interp=hyp.rgb_timestamp)
 
             # Prepare for SfM/photogrammetry processing
             try:
                 agisoft_object.export_rgb_from_h5(h5_folder=H5_FILE_PATH, 
                                             rgb_image_cube = hyp.rgb_frames, 
                                             nav_rgb = nav_rgb,
                                             rgb_write_dir=config['Absolute Paths']['rgbimagedir'],
                                             pos_acc = np.array([1, 1, 0.05]), 
                                             rot_acc = np.array([1, 1, 5]))
             except:
-                pass # If no RGB data, move forward
+                pass # If no RGB data, move forward"""
         
         
         
         print(H5_FILE_PATH)
     
     # Use the total point cloud to make a DEM
```

### Comparing `gref4hsi-0.1.5/setup.py` & `gref4hsi-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='gref4hsi',
-    version='0.1.5',    
+    version='0.1.9',    
     description='A Python package for for georeferencing and orthorectifying hyperspectral imagery',
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type = "text/markdown",
     url='https://github.com/havardlovas/gref4hsi',
     author='Haavard Snefjellaa Loevaas',
     author_email='havard.s.lovas@ntnu.no',
     license='EUPL-1.2',
```

