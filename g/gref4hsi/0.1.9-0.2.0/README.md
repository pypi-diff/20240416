# Comparing `tmp/gref4hsi-0.1.9.tar.gz` & `tmp/gref4hsi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gref4hsi-0.1.9.tar", last modified: Mon Apr 15 08:13:05 2024, max compression
+gzip compressed data, was "gref4hsi-0.2.0.tar", last modified: Tue Apr 16 07:31:00 2024, max compression
```

## Comparing `gref4hsi-0.1.9.tar` & `gref4hsi-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13807 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/LICENCE.MD
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       79 2024-03-12 08:17:47.000000 gref4hsi-0.1.9/MANIFEST.in
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    18091 2024-04-15 08:03:32.000000 gref4hsi-0.1.9/README.md
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.373281 gref4hsi-0.1.9/gref4hsi/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      205 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/__init__.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.373281 gref4hsi-0.1.9/gref4hsi/scripts/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/scripts/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    36833 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/coregistration.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     7844 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/georeference.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9507 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/scripts/orthorectification.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi/tests/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/tests/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1616 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_hi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    10686 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_specim.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8213 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/tests/test_main_uhi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3000 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3684 2024-03-07 14:11:10.000000 gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi/utils/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.1.9/gref4hsi/utils/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1587 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/colours.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3143 2024-03-13 12:06:06.000000 gref4hsi-0.1.9/gref4hsi/utils/config_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    51438 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/geometry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    44610 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/gis_tools.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    22622 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8706 2024-03-15 10:24:09.000000 gref4hsi-0.1.9/gref4hsi/utils/photogrammetry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    23551 2024-03-14 09:13:50.000000 gref4hsi-0.1.9/gref4hsi/utils/radiometry.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25630 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/specim_parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    27489 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/uhi_parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9874 2024-04-15 08:00:02.000000 gref4hsi-0.1.9/gref4hsi/utils/visualize.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/gref4hsi.egg-info/
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      935 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/SOURCES.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        1 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/dependency_links.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      188 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/requires.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        9 2024-04-15 08:13:05.000000 gref4hsi-0.1.9/gref4hsi.egg-info/top_level.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      106 2024-03-12 08:17:47.000000 gref4hsi-0.1.9/pyproject.toml
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       38 2024-04-15 08:13:05.377281 gref4hsi-0.1.9/setup.cfg
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1567 2024-04-15 08:08:25.000000 gref4hsi-0.1.9/setup.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.926560 gref4hsi-0.2.0/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13807 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/LICENCE.MD
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       79 2024-03-12 08:17:47.000000 gref4hsi-0.2.0/MANIFEST.in
+-rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-16 07:31:00.926560 gref4hsi-0.2.0/PKG-INFO
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    18091 2024-04-16 05:06:29.000000 gref4hsi-0.2.0/README.md
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.922560 gref4hsi-0.2.0/gref4hsi/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      205 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/gref4hsi/__init__.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.922560 gref4hsi-0.2.0/gref4hsi/scripts/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/gref4hsi/scripts/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    39307 2024-04-16 05:06:29.000000 gref4hsi-0.2.0/gref4hsi/scripts/coregistration.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     7802 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/scripts/georeference.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9507 2024-04-16 05:03:47.000000 gref4hsi-0.2.0/gref4hsi/scripts/orthorectification.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.922560 gref4hsi-0.2.0/gref4hsi/tests/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/gref4hsi/tests/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1616 2024-04-16 05:03:47.000000 gref4hsi-0.2.0/gref4hsi/tests/test_main_hi.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    10816 2024-04-16 05:06:29.000000 gref4hsi-0.2.0/gref4hsi/tests/test_main_specim.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8210 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/tests/test_main_uhi.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3000 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/gref4hsi/tests/test_multi_ray_trace.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3684 2024-03-07 14:11:10.000000 gref4hsi-0.2.0/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.922560 gref4hsi-0.2.0/gref4hsi/utils/
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.0/gref4hsi/utils/__init__.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1588 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/utils/colours.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3143 2024-03-13 12:06:06.000000 gref4hsi-0.2.0/gref4hsi/utils/config_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    52059 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/utils/geometry_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    44611 2024-04-16 05:21:04.000000 gref4hsi-0.2.0/gref4hsi/utils/gis_tools.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    22603 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/utils/parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8706 2024-03-15 10:24:09.000000 gref4hsi-0.2.0/gref4hsi/utils/photogrammetry_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    23551 2024-03-14 09:13:50.000000 gref4hsi-0.2.0/gref4hsi/utils/radiometry.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25630 2024-04-16 05:03:47.000000 gref4hsi-0.2.0/gref4hsi/utils/specim_parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    33111 2024-04-16 06:58:50.000000 gref4hsi-0.2.0/gref4hsi/utils/uhi_parsing_utils.py
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9874 2024-04-16 05:03:47.000000 gref4hsi-0.2.0/gref4hsi/utils/visualize.py
+drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 07:31:00.922560 gref4hsi-0.2.0/gref4hsi.egg-info/
+-rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-16 07:31:00.000000 gref4hsi-0.2.0/gref4hsi.egg-info/PKG-INFO
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      935 2024-04-16 07:31:00.000000 gref4hsi-0.2.0/gref4hsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        1 2024-04-16 07:31:00.000000 gref4hsi-0.2.0/gref4hsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      188 2024-04-16 07:31:00.000000 gref4hsi-0.2.0/gref4hsi.egg-info/requires.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        9 2024-04-16 07:31:00.000000 gref4hsi-0.2.0/gref4hsi.egg-info/top_level.txt
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      106 2024-03-12 08:17:47.000000 gref4hsi-0.2.0/pyproject.toml
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       38 2024-04-16 07:31:00.926560 gref4hsi-0.2.0/setup.cfg
+-rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1567 2024-04-16 07:08:53.000000 gref4hsi-0.2.0/setup.py
```

### Comparing `gref4hsi-0.1.9/LICENCE.MD` & `gref4hsi-0.2.0/LICENCE.MD`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/PKG-INFO` & `gref4hsi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gref4hsi
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gref4hsi-0.1.9/README.md` & `gref4hsi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/scripts/coregistration.py` & `gref4hsi-0.2.0/gref4hsi/scripts/coregistration.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from gref4hsi.utils.gis_tools import GeoSpatialAbstractionHSI
 from gref4hsi.utils.parsing_utils import Hyperspectral
 import gref4hsi.utils.geometry_utils as geom_utils
 from gref4hsi.utils.geometry_utils import CalibHSI, GeoPose
 
 from scipy.spatial.transform import Rotation as RotLib
 from scipy.optimize import least_squares
-from scipy.interpolate import interp1d
+from scipy.interpolate import interp1d, RBFInterpolator
 import pandas as pd
 from scipy.sparse import lil_matrix
 
 
 
 def numerical_jacobian(fun, param, eps=1e-6, **kwargs):
   """
@@ -55,24 +55,31 @@
     :type method: str, optional
     :return: _description_
     :rtype: _type_
     """
     # One simple option is to use Scipy's sortiment of interpolation options. The sparsity pattern should be included somehow..
     if method in ['nearest', 'linear', 'slinear', 'quadratic', 'cubic']:
         return interp1d(time_from, value, kind=method)(time_to)
+    elif method in ['gaussian']:
+        # Use sigma as the difference between two neighboring time nodes
+        sigma = time_from[1]-time_from[0]
+        eps**2 = np.sqrt(0.5*1/(sigma**2))
+        # sigma = 1/(sqrt(2)eps)
+        #https://docs.scipy.org/doc/scipy/reference/generated/scipy.interpolate.Rbf.html
+        return RBFInterpolator(time_from.reshape((-1,1)), value, kernel='gaussian', epsilon = eps)(np.array(time_to).reshape((-1,1)))
     
 
 def compose_pose_errors(param_pose_tot, time_nodes, unix_time_features, rot_body_ned, rot_ned_ecef, pos_body, time_interpolation_method):
     """Takes a (6*n_node) vector of errors, interpolates and composes (adds) them to the pose from the navigation data"""
     n_features = len(unix_time_features)
 
     # Interpolate to the right time
     err_interpolated = interpolate_time_nodes(time_nodes, 
                                               param_pose_tot,
-                                             time_to = unix_time_features, 
+                                              time_to = unix_time_features, 
                                               method=time_interpolation_method).transpose()
 
     # The errors in the interpolated form
     param_err_pos = err_interpolated[:, 0:3]
     param_err_eul_ZYX = np.vstack((err_interpolated[:, 3:4].flatten(), 
                                         np.zeros(n_features),
                                         np.zeros(n_features))).transpose()
@@ -129,15 +136,16 @@
                       'cx': param_vec_total[3],
                       'f': param_vec_total[4],
                       'k1': param_vec_total[5],
                       'k2': param_vec_total[6],
                       'k3': param_vec_total[7],
                       'tx': param_vec_total[8],
                       'ty': param_vec_total[9],
-                      'tz': param_vec_total[10]}
+                      'tz': param_vec_total[10],
+                      'width': -1} # Must be set elsewhere
         
         return calib_dict
     else:
         # If data is to be returned as vector
         return param_vec_total
 
 
@@ -347,35 +355,39 @@
     return feature_mask
 
 
 def calculate_cam_and_pose_from_param(h5_filename, param, features_df, param0, is_variab_param_intr, is_variab_param_extr, time_nodes, time_interpolation_method, h5_paths):
 
     # Seems wize to return
     # Return in a dictionary allowing for simple dumping to XML file (exept width)
-    if is_variab_param_intr.sum() != 0:
-        # Only compute if one or more parameters have been calibrated
+    if is_variab_param_intr.sum() > 0:
         calib_param_intr = calculate_intrinsic_param(is_variab_param_intr, param, param0, as_calib_obj = True)
+    else:
+        # Make identifiable that this has not been calibrated
+        calib_param_intr = None
 
 
-    if time_nodes is None:
+    # Read the original poses and time stamps from h5
+        
+    position_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name=h5_paths['h5_folder_position_ecef'])
+    # Extract the ecef orientations for each frame
+    quaternion_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name=h5_paths['h5_folder_quaternion_ecef'])
+    # Extract the timestamps for each frame
+    time_pose = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name=h5_paths['h5_folder_time_pose'])
+    
+    
+
+    if time_nodes is not None:
 
         # Calculate the pose vector
         param_pose_tot = calculate_pose_param(is_variab_param_extr, is_variab_param_intr, param)
 
-        # Read the original poses and time stamps from h5
-        
-        position_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                        dataset_name=h5_paths['h5_folder_position_ecef'])
-        # Extract the ecef orientations for each frame
-        quaternion_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                        dataset_name=h5_paths['h5_folder_quaternion_ecef'])
-        # Extract the timestamps for each frame
-        time_pose = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                        dataset_name=h5_paths['h5_folder_quaternion_ecef'])
-        
         # Minor code block for decomposing orientation into BODY-NED and NED-ECEF rotations
         rot_body = RotLib.from_quat(quaternion_ecef)
         geo_pose = GeoPose(timestamps=time_pose, 
                             rot_obj=rot_body, 
                             rot_ref='ECEF', 
                             pos=position_ecef, 
                             pos_epsg=4978)
@@ -387,16 +399,22 @@
                         time_nodes, 
                         time_pose, 
                         rot_body_ned, 
                         rot_ned_ecef, 
                         position_ecef, 
                         time_interpolation_method)
         
+        quaternion_body_ecef_corrected = rot_body_ecef_corrected.as_quat()
+    else:
+        # If no corrections should be applied, set to none for identifiability
+        pos_body_corrected = None
+        rot_body_ecef_corrected = None
+        
     
-    return calib_param_intr, pos_body_corrected, rot_body_ecef_corrected.as_quat()
+    return calib_param_intr, pos_body_corrected, quaternion_body_ecef_corrected
 
 
     
     
 
 
     
@@ -428,14 +446,18 @@
     # Create a temporary folder for resampled reference orthomosaics and DEMs
     ref_resampled_gis_path = config['Absolute Paths']['ref_ortho_reshaped']
     if not os.path.exists(ref_resampled_gis_path):
         os.mkdir(ref_resampled_gis_path)
 
 
     ref_gcp_path = config['Absolute Paths']['ref_gcp_path']
+
+    # Location for the calibrated Cal file:calib_file_coreg
+    calib_file_coreg = config['Absolute Paths']['calib_file_coreg']
+
     
 
     # The necessary data from the H5 file for getting the positions and orientations.
         
     # Position is stored here in the H5 file
     h5_folder_position_ecef = config['HDF.processed_nav']['position_ecef']
 
@@ -449,15 +471,15 @@
     h5_folder_quaternion_ecef_coreg = config['HDF.coregistration']['quaternion_ecef']
 
     # Timestamps here
     h5_folder_time_pose = config['HDF.processed_nav']['timestamp']
 
     h5_paths = {'h5_folder_position_ecef': h5_folder_position_ecef,
                 'h5_folder_quaternion_ecef': h5_folder_quaternion_ecef,
-                'h5_folder_time_pose': h5_folder_quaternion_ecef, 
+                'h5_folder_time_pose': h5_folder_time_pose, 
                 'h5_folder_position_ecef_coreg': h5_folder_position_ecef_coreg,
                 'h5_folder_quaternion_ecef_coreg': h5_folder_quaternion_ecef_coreg}
 
     
 
     print("\n################ Coregistering: ################")
 
@@ -624,15 +646,15 @@
                           'calibrate_k1': False,
                           'calibrate_k2': True,
                           'calibrate_k3': True}
         
         calibrate_per_transect = True
         estimate_time_varying = True
         time_node_spacing = 10 # s. If spacing 10 and transect lasts for 53 s will attempt to divide into largest integer leaving
-        time_interpolation_method = 'linear'
+        time_interpolation_method = 'gaussian'
 
         # Select which time varying degrees of freedom to estimate errors for
         calibrate_dict_extr = {'calibrate_pos_x': True,
                           'calibrate_pos_y': True,
                           'calibrate_pos_z': True,
                           'calibrate_roll': False,
                           'calibrate_pitch': False,
@@ -712,43 +734,53 @@
                     'is_variab_param_intr': is_variab_param_intr,
                     'time_nodes': None,
                     'is_variab_param_extr': is_variab_param_extr,
                     'time_interpolation_method': time_interpolation_method}
 
         # The sometimes natural think to do
         if calibrate_per_transect:
-            # Number of transects is found form data frame
+            # Number of transects is found from data frame
             n_transects = 1 + (df_gcp_filtered['file_count'].max() - df_gcp_filtered['file_count'].min())
             
             # Iterate through transects
             for i in range(int(n_transects)):
                 df_current = df_gcp_filtered[df_gcp_filtered['file_count'] == i]
                 
                 # Update the feature info
                 kwargs['features_df'] = df_current
 
                 n_features = df_current.shape[0]
 
+                # Read out the file name corresponding to file index i
+                h5_filename = df_current['h5_filename'].iloc[0]
+
                 if estimate_time_varying:
-                    times_samples = df_current['unix_time']
-                    transect_duration_sec = times_samples.max() - times_samples.min()
+                    ## The time range is defined by the transect time:
+                    #times_samples = df_current['unix_time']
+
+                    # Extract the timestamps for each frame
+                    time_pose = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                                    dataset_name=h5_folder_time_pose)
+
+
+                    transect_duration_sec = time_pose.max() - time_pose.min()
                     number_of_nodes = int(np.floor(transect_duration_sec/time_node_spacing)) + 1
 
                     # The time varying parameters are in total the number of dofs times number of nodes
                     param0_time_varying = np.zeros(n_adjustable_dofs*number_of_nodes)
 
                     # The time-varying parameters are stacked after the intrinsic parameters.
                     # This vector only holds parameters that will be adjusted
                     param0_variab_tot = np.concatenate((param0_variab, 
                                                         param0_time_varying), axis=0)
 
                     # Calculate the number of nodes. It divides the transect into equal intervals, 
                     # meaning that the intervals can be somewhat different at least for a small number of them.
-                    time_nodes = np.linspace(start=times_samples.min(), 
-                                        stop = times_samples.max(), 
+                    time_nodes = np.linspace(start=time_pose.min(), 
+                                        stop = time_pose.max(), 
                                         num = number_of_nodes)
                     # Update optimization kwarg
                     kwargs['time_nodes'] = time_nodes
                     
                     # Calculate the Jacobian for finding and exploiting sparsity
                     J = numerical_jacobian(fun = objective_fun_reprojection_error, param = param0_variab_tot, **kwargs)
 
@@ -793,18 +825,43 @@
                 print(f'Number of nodes was {number_of_nodes}')
                 print(f'Number of features was {n_features}')
                 print('')
                 
 
                 # TODO: the parameters should be injected into h5-file
 
-                h5_filename = df_current['h5_filename'][0]
+                
                 param_optimized = res.x
                 camera_model_dict_updated, position_updated, quaternion_updated = calculate_cam_and_pose_from_param(h5_filename, param_optimized, **kwargs, h5_paths=h5_paths)
 
+
+                # Now the data has been computed and can be written to h5:
+                if position_updated is None:
+                    pass
+                else:
+                    Hyperspectral.add_dataset(data=position_updated, 
+                                              name = h5_folder_position_ecef_coreg,
+                                              h5_filename=h5_filename)
+                if position_updated is None:
+                    pass
+                else:
+                    Hyperspectral.add_dataset(data = quaternion_updated, 
+                                              name = h5_folder_quaternion_ecef_coreg,
+                                              h5_filename = h5_filename)
+                if camera_model_dict_updated is None:
+                    pass
+                else:
+                    # Width is not a parameter and is inherited from the original file
+                    camera_model_dict_updated['width'] = cal_obj_prior['width']
+
+                    CalibHSI(file_name_cal_xml= calib_file_coreg, 
+                             mode = 'w',
+                             param_dict = camera_model_dict_updated)
+                    
+
         else:
             
             n_features = df_gcp_filtered.shape[0]
 
             res_pre_optim = objective_fun_reprojection_error(param0_variab, df_gcp_filtered, param0, is_variab_param_intr)
             median_error_x = np.median(np.abs(res_pre_optim[0:n_features]))
             median_error_y = np.median(np.abs(res_pre_optim[n_features:2*n_features]))
```

### Comparing `gref4hsi-0.1.9/gref4hsi/scripts/georeference.py` & `gref4hsi-0.2.0/gref4hsi/scripts/georeference.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         pos = pos_ref_ecef # Reference positions in ECEF
         rot_obj = RotLib.from_quat(quat_ref_ecef) # Reference orientations wrt ECEF
         
         ray_directions_local = intrinsic_geometry_dict['ray_directions_local']
         translation_ref_hsi = intrinsic_geometry_dict['translation_ref_hsi']
         rot_hsi_ref_obj = intrinsic_geometry_dict['rot_hsi_ref_obj']
 
-        hsi_geometry = CameraGeometry(pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True, use_absolute_position=True)
+        hsi_geometry = CameraGeometry(pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True)
         
         
         hsi_geometry.intrinsicTransformHSI(translation_ref_hsi=translation_ref_hsi, rot_hsi_ref_obj = rot_hsi_ref_obj)
 
         hsi_geometry.defineRayDirections(dir_local = ray_directions_local)
 
         return hsi_geometry
@@ -130,15 +130,15 @@
         path_tide = config['Absolute Paths']['tide_path']
     except Exception as e:
         path_tide = 'Undefined'
     
     # Maximal allowed ray length
     max_ray_length = float(config['General']['max_ray_length'])
 
-    mesh = pv.read(path_mesh)
+    mesh = pv.read(path_mesh,)
 
     
     print("\n################ Georeferencing: ################")
     files = sorted(os.listdir(dir_r))
     n_files= len(sorted(os.listdir(dir_r)))
     file_count = 0
     for filename in files:
@@ -150,15 +150,15 @@
             # Path to hierarchical file
             path_hdf = dir_r + filename
 
             # Read h5 file
             hyp = Hyperspectral(path_hdf, config)
 
             # Using the cal file, we can define lever arm, boresight and local ray geometry (in dictionary)
-            intrinsic_geometry_dict = cal_file_to_rays(filename_cal=hsi_cal_xml, config=config)
+            intrinsic_geometry_dict = cal_file_to_rays(filename_cal=hsi_cal_xml)
 
             
             # Define the rays in ECEF for each frame. 
             hsi_geometry = define_hsi_ray_geometry(pos_ref_ecef = hyp.pos_ref, 
                                     quat_ref_ecef = hyp.quat_ref, 
                                     time_pose = hyp.pose_time,
                                     intrinsic_geometry_dict = intrinsic_geometry_dict)
```

### Comparing `gref4hsi-0.1.9/gref4hsi/scripts/orthorectification.py` & `gref4hsi-0.2.0/gref4hsi/scripts/orthorectification.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/tests/test_main_hi.py` & `gref4hsi-0.2.0/gref4hsi/tests/test_main_hi.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/tests/test_main_specim.py` & `gref4hsi-0.2.0/gref4hsi/tests/test_main_specim.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,24 +131,26 @@
                     'Absolute Paths': {
                         'geoid_path' : GEOID_PATH,
                         #'geoid_path' : 'data/world/geoids/egm08_25.gtx',
                         'dem_path' : DEM_PATH,
                         'orthomosaic_reference_folder' : os.path.join(specim_mission_folder, "orthomosaic"),
                         'ref_ortho_reshaped' : os.path.join(DATA_DIR, "Intermediate", "RefOrthoResampled"),
                         'ref_gcp_path' : os.path.join(DATA_DIR, "Intermediate", "gcp.csv"),
+                        'calib_file_coreg' : os.path.join(DATA_DIR, "Output", "HSI_coreg.xml"),
                         # (above) The georeferencing allows processing using norwegian geoid NN2000 and worldwide EGM2008. Also, use of seafloor terrain models are supported. '
                         # At the moment refractive ray tracing is not implemented, but it could be relatively easy by first ray tracing with geoid+tide, 
                         # and then ray tracing from water
                         #'tide_path' : 'D:/HyperspectralDataAll/HI/2022-08-31-060000-Remoy-Specim/Input/tidevann_nn2000_NMA.txt'
                         },
+                    
                     # If coregistration is done, then the data must be stored after processing somewhere
                     'HDF.coregistration': {
-                        'position_ecef': 'processed/coreg/position_ecef',
-                        'quaternion_ecef' : 'processed/coreg/quaternion_ecef'
-                    }
+                            'position_ecef': 'processed/coreg/position_ecef',
+                            'quaternion_ecef' : 'processed/coreg/quaternion_ecef'
+                        }
                     
     }
 
     if TERRAIN_TYPE == 'geoid':
         custom_config['Absolute Paths']['geoid_path'] = GEOID_PATH
         #'geoid_path' : 'data/world/geoids/egm08_25.gtx'
     elif TERRAIN_TYPE == 'dem_file':
@@ -181,15 +183,15 @@
         visualize.show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame='ENU')"""
 
     # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
     #georeference.main(config_file_mission)
 
     #orthorectification.main(config_file_mission)
 
-    coregistration.main(config_file_mission, mode='compare')
+    #coregistration.main(config_file_mission, mode='compare')
 
     coregistration.main(config_file_mission, mode='calibrate')
 
 
 if __name__ == "__main__":
     # Select a recording folder on drive
     specim_mission_folder = os.path.join(base_fp, r"Specim/Missions/2022-08-31-Remøy/remoy_202208310800_ntnu_hyperspectral_74m")
```

### Comparing `gref4hsi-0.1.9/gref4hsi/tests/test_main_uhi.py` & `gref4hsi-0.2.0/gref4hsi/tests/test_main_uhi.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,59 +9,60 @@
 if os.name == 'nt':
     # Windows OS
     base_fp = 'D:'
     home = 'C:/Users/haavasl'
 elif os.name == 'posix':
     # This Unix-like systems inl. Mac and Linux
     base_fp = '/media/haavasl/Expansion'
-    home = 'C:/Users/haavasl'
+    home = '/home/haavasl'
+
 
 # Use this if working with the github repo to do quick changes to the module
 module_path = os.path.join(home, 'VsCodeProjects/gref4hsi/')
 if module_path not in sys.path:
     sys.path.append(module_path)
 
 from gref4hsi.utils import parsing_utils, uhi_parsing_utils
 from gref4hsi.scripts import georeference, orthorectification
 from gref4hsi.utils import visualize
 from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths, customize_config
 
 
-DATA_DIR = os.path.join(base_fp, "HyperspectralDataAll/UHI/2020-07-01-14-40-15-ArcticSeaIce-Ben-Lange/")
+DATA_DIR = os.path.join(base_fp, "HyperspectralDataAll/UHI/2020-07-01-14-34-57-ArcticSeaIce-Ben-Lange/")
 
 # The configuration file stores the settings for georeferencing
 config_file_mission = os.path.join(DATA_DIR, 'configuration.ini')
 
 
 config_path_template = os.path.join(home, 'VsCodeProjects/gref4hsi/data/config_examples/configuration_uhi.ini')
 
 # Copies the template to config_file_mission and sets up the necessary directories
 prepend_data_dir_to_relative_paths(config_path=config_path_template, DATA_DIR=DATA_DIR)
 
 # Non-default settings
 custom_config = {'General':
                     {'mission_dir': DATA_DIR,
                     'model_export_type': 'dem_file', # Infer seafloor structure from altimeter recordings
-                    'max_ray_length': 20,
+                    'max_ray_length': 5,
                     'lab_cal_dir': os.path.join(base_fp, 'HyperspectralDataAll/UHI/Lab_Calibration_Data/NP')}, # Max distance in meters from UHI to seafloor
 
                 'Coordinate Reference Systems': 
                     {'proj_epsg' : 3395, # The projected CRS for orthorectified data (an arctic CRS)
                     'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
                     'dem_epsg' : 3395, # (Optional) If you have a DEM this can be used
                     'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
 
                 'Relative Paths':
                     {'dem_folder': 'Input/GIS/'}, # Using altimeter, we generate one DEM per transect chunk
                 
                 'Absolute Paths':
-                    {'geoid_path': os.path.join(home, 'VsCodeProjects\gref4hsi\data\world\geoids\egm08_25.gtx')}, # Using altimeter, we generate one DEM per transect chunk
+                    {'geoid_path': os.path.join(home, "VsCodeProjects/gref4hsi/data/world/geoids/egm08_25.gtx")}, # Using altimeter, we generate one DEM per transect chunk
 
                 'Orthorectification':
-                    {'resample_rgb_only': False, # Good choice for speed
+                    {'resample_rgb_only': True, # Good choice for speed
                     'resolutionhyperspectralmosaic': 0.01, # 1 cm
                     'raster_transform_method': 'north_east'},
                 
                 'HDF.raw_nav': {'altitude': 'raw/nav/altitude',
                     'rotation_reference_type' : 'eul_ZYX', # The vehicles orientations are used as Yaw, Pitch, Roll
                     'is_global_rot' : False, # The vehicles orientations are used as Yaw, Pitch, Roll
                     'eul_is_degrees' : True},
@@ -84,36 +85,36 @@
 
 # Customizes the config file
 customize_config(config_path=config_file_mission, dict_custom=custom_config)
 
 # Settings specific to the pre-processing of UHI data. At present they are hardcoded, but they could be integrated 
 SettingsPreprocess = namedtuple('SettingsPreprocessing', ['dtype_datacube', 
                                                             'rotation_matrix_hsi_to_body',
-                                                            'translation_hsi_to_body',
+                                                            'translation_body_to_hsi',
                                                             'rotation_matrix_alt_to_body',
                                                             'translation_alt_to_body',
                                                             'config_file_name',
                                                             'time_offset_sec',
                                                             'lon_lat_alt_origin',
                                                             'resolution_dem',
                                                             'agisoft_process'])
 
 config_uhi_preprocess = SettingsPreprocess(dtype_datacube = np.float32,
                             # The fill value for empty cells (select values not occcuring in cube or ancillary data)
                             rotation_matrix_hsi_to_body = np.array([[0, 1, 0],
                                                                     [1, 0, 0],
                                                                     [0, 0, -1]]),
                             # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
-                            translation_hsi_to_body = np.array([0, 0, 0]),
+                            translation_body_to_hsi = np.array([0, 0, 0]),
                             rotation_matrix_alt_to_body = np.array([[0, 1, 0],
                                                                     [1, 0, 0],
                                                                     [0, 0, -1]]),
                             # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
                             translation_alt_to_body = np.array([0.5, 0, 0]),
-                            time_offset_sec =  0,
+                            time_offset_sec =  22,
                             # Ben's tick s1 starts at 1593614097.992003 -> 22 s delay
                             # Ben's tick s2 starts at 1593614414.995001 -> 0 s delay
 
                             lon_lat_alt_origin =  np.array([1, 1, 0]),
                             # The beast sets up a fake coordinate system at 1 deg lon/lat.
                             config_file_name = 'configuration.ini',
                             resolution_dem = 0.2, # The resolution of the Altimeter-based DEM
```

### Comparing `gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace.py` & `gref4hsi-0.2.0/gref4hsi/tests/test_multi_ray_trace.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py` & `gref4hsi-0.2.0/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/colours.py` & `gref4hsi-0.2.0/gref4hsi/utils/colours.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import numpy as np
+
 import cv2 as cv
 
 class Image():
     def __init__(self, array):
         """Takes in an image array with nxmx3 of type uint8"""
         self.image_array = array
```

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/config_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/geometry_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/geometry_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             # Update xml_dict['calibration'] with values from param_dict
             for key, value in param_dict.items():
                 xml_dict['calibration'][key] = value
             with open(file_name_cal_xml, 'w') as fd:
                 fd.write(xmltodict.unparse(xml_dict))
 
 class CameraGeometry():
-    def __init__(self, pos, rot, time, is_interpolated = False, use_absolute_position = False):
+    def __init__(self, pos, rot, time, is_interpolated = False):
         
         self.position_nav = pos
         self.rotation_nav = rot
 
         self.time = time
         self.IsLocal = False
         self.decoupled = True
@@ -280,14 +280,20 @@
 
         normals = mesh.cell_normals[cells,:]
 
         slit_image_number = np.floor(rays / m).astype(np.int32)
 
         pixel_number = rays % m
 
+        n_points = np.size(points)
+        n_rays = np.size(self.points_ecef_crs)
+        if n_points != n_rays:
+            print(f'The number of hits {n_points} is lower than total number of rays {n_rays}')
+
+
         # Assign normals
         self.points_ecef_crs[slit_image_number, pixel_number] = points
 
         self.normals_ecef_crs[slit_image_number, pixel_number] = normals
 
         self.camera_to_seabed_ECEF = self.points_ecef_crs - start.reshape((n, m, 3))
 
@@ -818,15 +824,15 @@
         hsi_to_feature_local[i, :] /= hsi_to_feature_local[i, 2]
     
     return hsi_to_feature_local
 
 
 
 
-def interpolate_poses(timestamp_from, pos_from, rot_from, timestamps_to, extrapolate = True, use_absolute_position = True):
+def interpolate_poses(timestamp_from, pos_from, rot_from, timestamps_to, extrapolate = True):
     """
 
     :param timestamp_from:
     Original timestamps
     :param pos_from: numpy array (n,3)
     Original positions
     :param rot_from: Rotation-object (n rotations)
@@ -856,16 +862,15 @@
     min_ind = 0
     max_ind = timestamps_to.size
 
 
     # Setting use_absolute_position to True means that position calculations are done with absolute
     referenceGeometry = CameraGeometry(pos=pos_from,
                                rot=rot_from,
-                               time=timestamp_from,
-                               use_absolute_position=use_absolute_position)
+                               time=timestamp_from)
 
     # We exploit a method from the camera object
     referenceGeometry.interpolate(time_hsi=timestamps_to,
                           minIndRGB=min_ind,
                           maxIndRGB=max_ind,
                           extrapolate=extrapolate)
 
@@ -1194,15 +1199,23 @@
                     for y in range(ds.RasterYSize):
                         for x in range(ds.RasterXSize):
                             if mask[y, x]:
                                 x_coord = x_origin + x * x_resolution
                                 y_coord = y_origin + y * y_resolution
                                 xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
             else:
-                print('*.xyz already exists')
+                print('*.xyz already exists, overwriting')
+                with open(output_xyz, 'w') as xyz_file:
+                    # Write data to the XYZ file using the mask and calculated coordinates
+                    for y in range(ds.RasterYSize):
+                        for x in range(ds.RasterXSize):
+                            if mask[y, x]:
+                                x_coord = x_origin + x * x_resolution
+                                y_coord = y_origin + y * y_resolution
+                                xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
             # Clean up
             ds = None
             band = None
     
 
     points = np.loadtxt(output_xyz)
 
@@ -1236,14 +1249,16 @@
 
     (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=x_proj, yy=y_proj, zz=h_proj)
 
     mesh.points[:, 0] = x_ecef.reshape(-1)
     mesh.points[:, 1] = y_ecef.reshape(-1)
     mesh.points[:, 2] = z_ecef.reshape(-1)
 
+   
+
     # Save mesh
     mesh.save(model_path)
 
 def crop_geoid_to_pose(path_dem, config, geoid_path = 'data/world/geoids/egm08_25.gtx'):
     # The desired CRS for the model must be same as positions, orientations
     epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
```

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/gis_tools.py` & `gref4hsi-0.2.0/gref4hsi/utils/gis_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
         (east, north, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
 
         self.points_proj[:,:,0] = east.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
         self.points_proj[:, :, 1] = north.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
         self.points_proj[:, :, 2] = hei.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
 
+
         
 
 
     def footprint_to_shape_file(self, footprint_dir):
         """Uses the georeferenced data points (in projected form) to describe the footprint as a shape file
 
         :param footprint_dir: Where to put the shape files describing the footprint
```

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/parsing_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/parsing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,16 +418,15 @@
 
             timestamp_hsi = hyp.dataCubeTimeStamps.reshape(-1)
 
             # Compute interpolated absolute positions positions and orientation:
             position_interpolated, quaternion_interpolated = interpolate_poses(timestamp_from=timestamps_imu,
                                                              pos_from=position_ref,
                                                              rot_from=rot_obj,
-                                                             timestamps_to=timestamp_hsi,
-                                                             use_absolute_position = True)
+                                                             timestamps_to=timestamp_hsi)
 
             # If the original orientations are with respect to (North-East-Down) NED
             if not is_global_rot:
                 rot_ref = 'NED'
             else:
                 rot_ref = 'ECEF'
 
@@ -438,16 +437,18 @@
             pos_epsg_export = config['Coordinate Reference Systems']['geocsc_epsg_export']
 
             # The interpolated rotation-object
             rot_interpolated = RotLib.from_quat(quaternion_interpolated)
 
             # For simple geo-pose for changing between formats.
             geo_pose_ref = GeoPose(timestamps=timestamp_hsi,
-                                   rot_obj= rot_interpolated, rot_ref=rot_ref,
-                                   pos = position_interpolated, pos_epsg=pos_epsg_orig)
+                                   rot_obj= rot_interpolated, 
+                                   rot_ref=rot_ref,
+                                   pos = position_interpolated, 
+                                   pos_epsg=pos_epsg_orig)
 
             # Convert position to the epsg used for the 3D model
             geo_pose_ref.compute_geocentric_position(epsg_geocsc=pos_epsg_export)
 
 
             # Calculate the geodetic position using the WGS-84 (for conversion of orientations)
             epsg_wgs84 = 4326
```

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/photogrammetry_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/photogrammetry_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/radiometry.py` & `gref4hsi-0.2.0/gref4hsi/utils/radiometry.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/specim_parsing_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/specim_parsing_utils.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/uhi_parsing_utils.py` & `gref4hsi-0.2.0/gref4hsi/utils/uhi_parsing_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -230,57 +230,77 @@
     FOV_FILE_PATH = glob.glob(search_path_fov)[0]
 
     fov_arr = np.array(pd.read_csv(FOV_FILE_PATH)['View_Angle_Deg'])
     param_dict = Specim.fov_2_param(fov = fov_arr)
 
     return param_dict
 
-def set_camera_model(config, config_file_path, config_uhi, model_type, binning_spatial):
-    LAB_CAL_DIR = config['General']['lab_cal_dir'] # Where the fov file is
+def set_camera_model(config, config_file_path, config_uhi, model_type, binning_spatial, fov_arr = None):
+    """_summary_
 
-    if model_type == 'cal_dir':
+    :param config: _description_
+    :type config: _type_
+    :param config_file_path: _description_
+    :type config_file_path: _type_
+    :param config_uhi: _description_
+    :type config_uhi: _type_
+    :param model_type: ['cal_txt', 'embedded']
+    :type model_type: str
+    :param binning_spatial: _description_
+    :type binning_spatial: _type_
+    :param fov_arr: _description_, defaults to None
+    :type fov_arr: _type_, optional
+    """
+    if model_type == 'cal_txt':
+        # Assumes a csv file with column "View_Angle_Deg" holding the view angles
+        LAB_CAL_DIR = config['General']['lab_cal_dir'] # Where the fov file is
         param_dict = read_fov_file_to_param(LAB_CAL_DIR=LAB_CAL_DIR, binning_spatial=binning_spatial)
-        # User set rotation matrix
-        R_hsi_body = config_uhi.rotation_matrix_hsi_to_body
+    elif model_type == 'embedded':
+        # Use supplied fov_array
+        param_dict = Specim.fov_2_param(fov = fov_arr)
+    else:
+        pass
 
-        r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
 
-        # Euler angle representation (any other would do too)
-        param_dict['rz'] = r_zyx[0]
-        param_dict['ry'] = r_zyx[1]
-        param_dict['rx'] = r_zyx[2]
-
-        # Vector from origin of HSI to body origin, expressed in body
-        # User set
-        t_hsi_body = config_uhi.translation_hsi_to_body
-        param_dict['tz'] = t_hsi_body[0]
-        param_dict['ty'] = t_hsi_body[1]
-        param_dict['tz'] = t_hsi_body[2]
-        
-        file_name_xml = 'HSI_' + str(binning_spatial) + 'b.xml'
-        CAMERA_CALIB_XML_DIR = config['Absolute Paths']['calib_folder']
-        xml_cal_write_path = CAMERA_CALIB_XML_DIR + file_name_xml
 
-        CalibHSI(file_name_cal_xml= xml_cal_write_path,  
-                        mode = 'w', 
-                        param_dict = param_dict)
 
+    # User set rotation matrix
+    R_hsi_body = config_uhi.rotation_matrix_hsi_to_body
 
-        # Set value in config file and update:
-        config.set('Relative Paths', 'hsi_calib_path', value = 'Input/Calib/' + file_name_xml)
+    r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
 
-        with open(config_file_path, 'w') as configfile:
-                config.write(configfile)
+    # Euler angle representation (any other would do too)
+    param_dict['rz'] = r_zyx[0]
+    param_dict['ry'] = r_zyx[1]
+    param_dict['rx'] = r_zyx[2]
 
+    # Vector from origin of body to HSI
+    t_hsi_body = config_uhi.translation_body_to_hsi
+    param_dict['tz'] = t_hsi_body[0]
+    param_dict['ty'] = t_hsi_body[1]
+    param_dict['tz'] = t_hsi_body[2]
 
-    elif model_type == 'embedded':
-        print('Should make support for this')
-        pass
-    else:
-        pass
+    # Define where to write calibrated data
+    file_name_xml = 'HSI_' + str(binning_spatial) + 'b.xml'
+    CAMERA_CALIB_XML_DIR = config['Absolute Paths']['calib_folder']
+    xml_cal_write_path = CAMERA_CALIB_XML_DIR + file_name_xml
+
+
+    CalibHSI(file_name_cal_xml= xml_cal_write_path,  
+                        mode = 'w', 
+                        param_dict = param_dict)
+    
+    
+
+
+    # Set value in config file and update:
+    config.set('Relative Paths', 'hsi_calib_path', value = 'Input/Calib/' + file_name_xml)
+
+    with open(config_file_path, 'w') as configfile:
+            config.write(configfile)
 
 
     
 
 def read_nav_from_mat(mat_filename):
     """Function for reading mat data from the beast format into a NAV object"""
     mat_contents = {}
@@ -467,16 +487,34 @@
     # Still the points are given in a form of NED
 
     # NED is no frame for GIS, but an OK frame for certain vector operations.
     # The above linearization is only accurate for small surveys such as those in UHI
 
     return points_altimeter_transect
 
-def write_point_cloud_to_dem(points, config, resolution_dem, lon0, lat0, h0, method='nearest', smooth_DEM=True):
-    
+def point_cloud_to_dem(points, config, resolution_dem, lon0, lat0, h0, method='nearest', smooth_DEM=True):
+    """Converts the sparse point cloud of altimeter data into a digital elevation model.
+
+    :param points: _description_
+    :type points: _type_
+    :param config: _description_
+    :type config: _type_
+    :param resolution_dem: _description_
+    :type resolution_dem: _type_
+    :param lon0: _description_
+    :type lon0: _type_
+    :param lat0: _description_
+    :type lat0: _type_
+    :param h0: _description_
+    :type h0: _type_
+    :param method: _description_, defaults to 'nearest'
+    :type method: str, optional
+    :param smooth_DEM: _description_, defaults to True
+    :type smooth_DEM: bool, optional
+    """
     # The name of the digital elevation model
     output_dem_path = config['Absolute Paths']['dem_path']
 
     # The padding (ensuring that all rays hit the model)
     pad_xy = float(config['General']['max_ray_length'])
 
     x_coords = points[:,0]
@@ -506,15 +544,15 @@
     crs_84 = CRS.from_epsg(epsg_wgs84)
     crs_dem = CRS.from_epsg(dem_epsg)
     transformer = Transformer.from_crs(crs_84, crs_dem)
 
     # Transform extent
     (x, y, z) = transformer.transform(xx=lat_ext, yy=lon_ext, zz=h_ext)
 
-    if crs_dem.is_geocentric:
+    if crs_dem.is_geographic:
 
         res_x = resolution_dem*(x.max() - x.min())/(x_max - x_min)
         res_y = resolution_dem*(y.max() - y.min())/(y_max - y_min)
         transform = Affine(a = res_y,
                         b = 0,
                         c = y.min(),
                         d = 0,
@@ -569,22 +607,24 @@
         num_threads=0)
 
         grid_z = idw.reshape(grid_x.shape)
 
 
     if smooth_DEM == True:
         from scipy import ndimage
+        # Smooths by 4 pixel units
         sigma_x = 4
         sigma_y = 4
         grid_z = ndimage.gaussian_filter(grid_z, sigma=(sigma_y, sigma_x))
+        
 
     
-
+    # Writes to a file
     with rasterio.open(output_dem_path, 'w', driver='GTiff', height=grid_z.shape[0],
-                    width=grid_z.shape[1], count=1, dtype='float32', crs='EPSG:' + str(dem_epsg),
+                    width=grid_z.shape[1], count=1, dtype='float64', crs='EPSG:' + str(dem_epsg),
                     transform=transform) as dst:
         dst.write(grid_z, 1)
 
 
 
 
 def uhi_beast(config, config_uhi):
@@ -645,15 +685,15 @@
         if h5_index == 0:
             # Camera model is set once, assuming same spatial binning throughout
             binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
             # Sets camera model with user specified boresight ...
             set_camera_model(config=config, 
                              config_file_path = config_file_path, 
                              config_uhi=config_uhi, 
-                             model_type = 'cal_dir', 
+                             model_type = 'cal_txt', 
                              binning_spatial = binning_spatial)
 
         true_time_hsi = hyp.hsi_frames_timestamp - time_offset
 
         # Interpolate nav to roll time, IMU time (considered nav timestamp)
 
         ## write nav data to h5 file
@@ -699,19 +739,139 @@
     if config_uhi.agisoft_process:
         agisoft_object.load_photos_and_reference()
 
 
 
 
 
-    write_point_cloud_to_dem(point_cloud_altimeter_total, 
+    point_cloud_to_dem(point_cloud_altimeter_total, 
                                  config, 
                                  resolution_dem = config_uhi.resolution_dem, 
                                  lon0=lon0, 
                                  lat0=lat0, 
                                  h0=alt0)
 
 
+
+
+def uhi_dbe(config, config_uhi):
+    """Preparing data for the UHI-2x blueye edition (almost copy of beast)
+
+    :param config: _description_
+    :type config: _type_
+    :param config_uhi: _description_
+    :type config_uhi: _type_
+    """
+    MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
+    
+
+    # For writing
+    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
+
+    SPATIAL_PIXELS = 1936 # Same for almost all UHI
+    
+
+    INPUT_DIR = MISSION_PATH + 'Input/'
+
+    h5_folder = config['Absolute Paths']['h5_folder']
+    H5_PATTERN = '*.h5'
+
+    MAT_DIR = INPUT_DIR
+    MAT_PATTERN = '*.mat'
+
+    # Locate mat file with nav data 
+    search_path_mat = os.path.normpath(os.path.join(MAT_DIR, MAT_PATTERN))
+    MAT_FILE_PATHS = glob.glob(search_path_mat)
+    MAT_PATH = MAT_FILE_PATHS[0] # Assuming there is only one
+
+
+    # TODO: replace with how you read in data from DVL/H5 folders
+    nav = read_nav_from_mat(mat_filename=MAT_PATH)
+
+    
+
+    # Search the h5 folder (these are the files to iterate)
+    search_path_h5 = os.path.normpath(os.path.join(h5_folder, H5_PATTERN))
+    H5_FILE_PATHS = glob.glob(search_path_h5)
+
+    number_of_h5_files = len(H5_FILE_PATHS)
+
+    h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
+            'fov': config['HDF.calibration']['fov'],
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
+            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
+            }
+    
+    time_offset = config_uhi.time_offset_sec
+    lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
+
+    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
+    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
+    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
+    # Should interface towards ODM as well
+
+    for h5_index in range(number_of_h5_files):
+        H5_FILE_PATH = H5_FILE_PATHS[h5_index]
+
+        # Read the specified entries
+        hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
+
+        if h5_index == 0:
+            # Camera model is set once, assuming same spatial binning throughout
+            binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
+            
+            # Extract from the hyperspectral object
+            fov_arr = hyp.fov
+
+            # Sets camera model with user specified boresight ...
+            set_camera_model(config=config, 
+                             config_file_path = config_file_path, 
+                             config_uhi=config_uhi, 
+                             model_type = 'embedded', 
+                             binning_spatial = binning_spatial,
+                             fov_arr=fov_arr)
+
+        true_time_hsi = hyp.hsi_frames_timestamp - time_offset
+
+        # Interpolate nav to roll time, IMU time (considered nav timestamp)
+
+        ## write nav data to h5 file
+        write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH)
+        
+        # Build a point cloud
+        point_cloud_altimeter = altimeter_data_to_point_cloud(nav = nav, 
+                                                              config_uhi=config_uhi, 
+                                                              true_time_hsi = true_time_hsi, 
+                                                              lon0=lon0, 
+                                                              lat0=lat0, 
+                                                              h0=alt0)
+        if h5_index == 0:
+            point_cloud_altimeter_total = point_cloud_altimeter
+        else:
+            point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
         
         
+        
+        print(H5_FILE_PATH)
+    
+    # Use the total point cloud to make a DEM
+    
+
+    if config_uhi.agisoft_process:
+        agisoft_object.load_photos_and_reference()
+
+
+
+
+
+    point_cloud_to_dem(point_cloud_altimeter_total, 
+                                 config, 
+                                 resolution_dem = config_uhi.resolution_dem, 
+                                 lon0=lon0, 
+                                 lat0=lat0, 
+                                 h0=alt0)
+
+
```

### Comparing `gref4hsi-0.1.9/gref4hsi/utils/visualize.py` & `gref4hsi-0.2.0/gref4hsi/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/gref4hsi.egg-info/PKG-INFO` & `gref4hsi-0.2.0/gref4hsi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gref4hsi
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
 Home-page: https://github.com/havardlovas/gref4hsi
 Author: Haavard Snefjellaa Loevaas
 Author-email: havard.s.lovas@ntnu.no
 License: EUPL-1.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gref4hsi-0.1.9/gref4hsi.egg-info/SOURCES.txt` & `gref4hsi-0.2.0/gref4hsi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gref4hsi-0.1.9/setup.py` & `gref4hsi-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
     name='gref4hsi',
-    version='0.1.9',    
+    version='0.2.0',    
     description='A Python package for for georeferencing and orthorectifying hyperspectral imagery',
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type = "text/markdown",
     url='https://github.com/havardlovas/gref4hsi',
     author='Haavard Snefjellaa Loevaas',
     author_email='havard.s.lovas@ntnu.no',
     license='EUPL-1.2',
```

