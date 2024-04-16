# Comparing `tmp/bigstream-1.2.9.tar.gz` & `tmp/bigstream-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigstream-1.2.9.tar", last modified: Wed Jan 31 16:33:36 2024, max compression
+gzip compressed data, was "bigstream-1.3.0.tar", last modified: Tue Apr 16 14:40:05 2024, max compression
```

## Comparing `bigstream-1.2.9.tar` & `bigstream-1.3.0.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-01-31 16:33:36.141940 bigstream-1.2.9/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1518 2023-10-02 19:28:02.000000 bigstream-1.2.9/LICENSE.md
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      264 2024-01-31 16:33:36.140651 bigstream-1.2.9/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.2.9/README.md
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-01-31 16:33:36.116768 bigstream-1.2.9/bigstream/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.2.9/bigstream/__init__.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    43711 2024-01-24 16:41:16.000000 bigstream-1.2.9/bigstream/align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9265 2024-01-16 21:48:49.000000 bigstream-1.2.9/bigstream/application_pipelines.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7599 2023-11-08 19:06:20.000000 bigstream-1.2.9/bigstream/configure_irm.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     5482 2024-01-16 21:48:49.000000 bigstream-1.2.9/bigstream/features.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6554 2024-01-22 19:55:56.000000 bigstream-1.2.9/bigstream/level_set.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    10153 2023-11-08 19:06:20.000000 bigstream-1.2.9/bigstream/metrics.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    25408 2024-01-04 22:07:14.000000 bigstream-1.2.9/bigstream/motion_correct.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    24504 2024-01-31 16:31:54.000000 bigstream-1.2.9/bigstream/piecewise_align.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    17674 2023-11-08 19:06:20.000000 bigstream-1.2.9/bigstream/piecewise_transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16188 2023-11-08 19:06:20.000000 bigstream-1.2.9/bigstream/stitch.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    15427 2024-01-23 21:57:41.000000 bigstream-1.2.9/bigstream/transform.py
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22844 2024-01-17 20:23:43.000000 bigstream-1.2.9/bigstream/utility.py
-drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-01-31 16:33:36.135985 bigstream-1.2.9/bigstream.egg-info/
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      264 2024-01-31 16:33:35.000000 bigstream-1.2.9/bigstream.egg-info/PKG-INFO
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      516 2024-01-31 16:33:35.000000 bigstream-1.2.9/bigstream.egg-info/SOURCES.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-01-31 16:33:35.000000 bigstream-1.2.9/bigstream.egg-info/dependency_links.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      287 2024-01-31 16:33:35.000000 bigstream-1.2.9/bigstream.egg-info/requires.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2024-01-31 16:33:35.000000 bigstream-1.2.9/bigstream.egg-info/top_level.txt
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-01-31 16:33:36.143316 bigstream-1.2.9/setup.cfg
--rw-r--r--   0 fleishmang (61373) scicomp  (93098)      859 2024-01-31 16:33:05.000000 bigstream-1.2.9/setup.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.925942 bigstream-1.3.0/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     1518 2023-10-02 19:28:02.000000 bigstream-1.3.0/LICENSE.md
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-04-16 14:40:05.924454 bigstream-1.3.0/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     8731 2023-07-11 16:34:08.000000 bigstream-1.3.0/README.md
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.899900 bigstream-1.3.0/bigstream/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        5 2023-07-11 16:34:08.000000 bigstream-1.3.0/bigstream/__init__.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    46332 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     9265 2024-01-16 21:48:49.000000 bigstream-1.3.0/bigstream/application_pipelines.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7793 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/configure_irm.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    21545 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6148 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_io_utility.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    22766 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/distributed_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     7403 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/features.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6665 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/io_utility.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)     6554 2024-01-22 19:55:56.000000 bigstream-1.3.0/bigstream/level_set.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    10153 2023-11-08 19:06:20.000000 bigstream-1.3.0/bigstream/metrics.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    25553 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/motion_correct.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    24297 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/piecewise_align.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    19357 2024-04-11 20:49:31.000000 bigstream-1.3.0/bigstream/piecewise_transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16188 2023-11-08 19:06:20.000000 bigstream-1.3.0/bigstream/stitch.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    18807 2024-04-11 20:49:47.000000 bigstream-1.3.0/bigstream/transform.py
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)    16649 2024-04-10 16:12:30.000000 bigstream-1.3.0/bigstream/utility.py
+drwxr-xr-x   0 fleishmang (61373) scicomp  (93098)        0 2024-04-16 14:40:05.918426 bigstream-1.3.0/bigstream.egg-info/
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      270 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/PKG-INFO
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      642 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/SOURCES.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)        1 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/dependency_links.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      275 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/requires.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       10 2024-04-16 14:40:05.000000 bigstream-1.3.0/bigstream.egg-info/top_level.txt
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)       38 2024-04-16 14:40:05.927498 bigstream-1.3.0/setup.cfg
+-rw-r--r--   0 fleishmang (61373) scicomp  (93098)      854 2024-04-16 14:39:31.000000 bigstream-1.3.0/setup.py
```

### Comparing `bigstream-1.2.9/LICENSE.md` & `bigstream-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/README.md` & `bigstream-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/bigstream/align.py` & `bigstream-1.3.0/bigstream/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import sys
 import numpy as np
 import SimpleITK as sitk
 import bigstream.utility as ut
+import time
+
 from bigstream.configure_irm import configure_irm
-from bigstream.transform import apply_transform, compose_transform_list
+from bigstream.transform import apply_transform, compose_transform_list, compress_transform_list
 from bigstream.metrics import patch_mutual_information
 from bigstream import features
 import cv2
 
 
 def apply_alignment_spacing(
     fix,
@@ -63,18 +65,22 @@
     # ensure spacings are floating point
     fix_spacing = fix_spacing.astype(np.float64)
     mov_spacing = mov_spacing.astype(np.float64)
 
     # get mask spacings
     fix_mask_spacing = None
     if fix_mask is not None:
-        fix_mask_spacing = ut.relative_spacing(fix_mask, fix, fix_spacing)
+        fix_mask_spacing = ut.relative_spacing(fix_mask.shape,
+                                               fix.shape,
+                                               fix_spacing)
     mov_mask_spacing = None
     if mov_mask is not None:
-        mov_mask_spacing = ut.relative_spacing(mov_mask, mov, mov_spacing)
+        mov_mask_spacing = ut.relative_spacing(mov_mask.shape,
+                                               mov.shape,
+                                               mov_spacing)
 
     # skip sample
     if alignment_spacing:
         fix, fix_spacing = ut.skip_sample(fix, fix_spacing, alignment_spacing)
         mov, mov_spacing = ut.skip_sample(mov, mov_spacing, alignment_spacing)
         if fix_mask is not None:
             fix_mask, fix_mask_spacing = ut.skip_sample(
@@ -188,15 +194,17 @@
     2. The tuple of transform origins
     """
 
     spacings = []
     for transform in transforms:
         spacing = fix_spacing
         if len(transform.shape) not in [1, 2]:
-            spacing = ut.relative_spacing(transform, fix, fix_spacing)
+            spacing = ut.relative_spacing(transform.shape, 
+                                          fix.shape,
+                                          fix_spacing)
         spacings.append(spacing)
     spacings = tuple(spacings)
     origins = (fix_origin,)*len(transforms)
     return (spacings, origins)
 
 
 def feature_point_ransac_affine_align(
@@ -206,20 +214,23 @@
     blob_sizes,
     alignment_spacing=None,
     num_sigma_max=15,
     cc_radius=12,
     nspots=5000,
     match_threshold=0.7,
     max_spot_match_distance=None,
+    point_matches_threshold=50,
     align_threshold=2.0,
     diagonal_constraint=0.25,
     fix_spot_detection_kwargs={},
     mov_spot_detection_kwargs={},
     fix_spots=None,
+    fix_spots_count_threshold=100,
     mov_spots=None,
+    mov_spots_count_threshold=100,
     fix_mask=None,
     mov_mask=None,
     fix_origin=None,
     mov_origin=None,
     static_transform_list=[],
     default=None,
     **kwargs,
@@ -281,14 +292,17 @@
         consider them corresponding points
 
     max_spot_match_distance : scalar float (default: None)
         The maximum distance a fix and mov spot can be before alignment
         to still be considered matching spots; in microns. This helps
         prevent false positive correspondences.
 
+    point_matches_threshold : scalar int (default: 50)
+        Minimum number of matching points for a valid alignment
+
     align_threshold : scalar float (default: 2.0)
         The maximum distance two points can be to be considered aligned
         by the affine transform; in microns.
 
     diagonal_constraint : scalar float (default: 0.25)
         Diagonal entries of the affine matrix cannot be lower than
         1 - diagonal_contraint or higher than 1 + diagonal_contraint. 
@@ -300,17 +314,27 @@
 
     mov_spot_detection_kwargs : dict (default {})
         Arguments passed to bigstream.features.blob_detection for moving image
 
     fix_spots : nd-array Nx3 (default: None)
         Skip the spot detection for the fixed image and provide your own spot coordinate
 
+    fix_spots_count_threshold : scalar int (default: 100)
+        Minimum number of fixed spots that need to exist for a valid alignment.
+        Note that many times in order to have a better alignment it is better to tweak
+        threshold and/or threshold_rel in fix_spot_detection_kwargs then to lower this value
+
     mov_spots : nd-array Nx3 (default: None)
         Skip the spot detection for the moving image and provide your own spot coordinate
 
+    mov_spots_count_threshold : scalar int (default: 100)
+        Minimum number of fixed spots that need to exist for a valid alignment.
+        Note that many times in order to have a better alignment it is better to tweak
+        threshold and/or threshold_rel in mov_spot_detection_kwargs then to lower this value
+
     fix_mask : binary nd-array (default: None)
         Spots from fixed image can only be found in the foreground of this mask
 
     mov_mask : binary nd-array (default: None)
         Spots from moving image can only be found in the foreground of this mask
 
     fix_origin : 1d array (default: all zeros)
@@ -374,95 +398,115 @@
     mov_spacing = X[5]
     fix_mask_spacing = X[6]
     mov_mask_spacing = X[7]
 
     # get fix spots
     num_sigma = int(min(blob_sizes[1] - blob_sizes[0], num_sigma_max))
     assert num_sigma > 0, 'num_sigma must be greater than 0, make sure blob_sizes[1] > blob_sizes[0]'
-    print('computing fixed spots', flush=True)
+    print(f'{time.ctime(time.time())} computing fixed spots', flush=True)
     if fix_spots is None:
         fix_kwargs = {
             'num_sigma':num_sigma,
             'exclude_border':cc_radius,
-            'mask':fix_mask,
         }
         fix_kwargs = {**fix_kwargs, **fix_spot_detection_kwargs}
+        print(f'{time.ctime(time.time())} fixed spots detection using',
+              fix_kwargs, flush=True)
         fix_spots = features.blob_detection(
             fix, blob_sizes[0], blob_sizes[1],
+            mask=fix_mask,
             **fix_kwargs,
         )
-    print(f'found {len(fix_spots)} fixed spots')
-    if len(fix_spots) < 100:
-        print('insufficient fixed spots found, returning default', flush=True)
+    print(f'{time.ctime(time.time())} found {len(fix_spots)} fixed spots',
+          flush=True)
+    if len(fix_spots) < fix_spots_count_threshold:
+        print(f'{time.ctime(time.time())}',
+              'insufficient fixed spots found, returning default',
+              flush=True)
         return default
 
     # get mov spots
-    print('computing moving spots', flush=True)
+    print(f'{time.ctime(time.time())} computing moving spots', flush=True)
     if mov_spots is None:
         mov_kwargs = {
             'num_sigma':num_sigma,
             'exclude_border':cc_radius,
-            'mask':mov_mask,
         }
         mov_kwargs = {**mov_kwargs, **mov_spot_detection_kwargs}
+        print(f'{time.ctime(time.time())} moving spots detection using',
+              mov_kwargs, flush=True)
         mov_spots = features.blob_detection(
             mov, blob_sizes[0], blob_sizes[1],
+            mask=mov_mask,
             **mov_kwargs,
         )
-    print(f'found {len(mov_spots)} moving spots')
-    if len(mov_spots) < 100:
-        print('insufficient moving spots found, returning default', flush=True)
+
+    print(f'{time.ctime(time.time())} found {len(mov_spots)} moving spots',
+          flush=True)
+    if len(mov_spots) < mov_spots_count_threshold:
+        print(f'{time.ctime(time.time())}',
+              'insufficient moving spots found, returning default',
+              flush=True)
         return default
 
     # sort
-    print('sorting spots', flush=True)
+    print(f'{time.ctime(time.time())} sorting spots', flush=True)
     sort_idx = np.argsort(fix_spots[:, 3])[::-1]
     fix_spots = fix_spots[sort_idx, :3][:nspots]
     sort_idx = np.argsort(mov_spots[:, 3])[::-1]
     mov_spots = mov_spots[sort_idx, :3][:nspots]
 
     # get contexts
-    print('extracting contexts', flush=True)
+    print(f'{time.ctime(time.time())} extracting contexts', flush=True)
     fix_spot_contexts = features.get_contexts(fix, fix_spots, cc_radius)
     mov_spot_contexts = features.get_contexts(mov, mov_spots, cc_radius)
 
     # get pairwise correlations
-    print('computing pairwise correlations', flush=True)
+    print(f'{time.ctime(time.time())} computing pairwise correlations',
+          flush=True)
     correlations = features.pairwise_correlation(
         fix_spot_contexts, mov_spot_contexts,
     )
 
     # convert to physical units
     fix_spots = fix_spots * fix_spacing
     mov_spots = mov_spots * mov_spacing
 
     # get matching points
     fix_spots, mov_spots = features.match_points(
         fix_spots, mov_spots,
         correlations, match_threshold,
         max_distance=max_spot_match_distance,
     )
-    print(f'found {len(fix_spots)} matched spot pairs')
-    if len(fix_spots) < 50 or len(mov_spots) < 50:
-        print('insufficient spot matches found, returning default', flush=True)
+    print(f'{time.ctime(time.time())} {len(fix_spots)} - {len(mov_spots)} matched spots',
+          flush=True)
+    if len(fix_spots) < point_matches_threshold or len(mov_spots) < point_matches_threshold:
+        print(f'{time.ctime(time.time())}',
+              'insufficient point matches found, returning default',
+              flush=True)
         return default
 
     # align
-    # TODO: this is a hard 3D constraint, check opencv for a 2D version
-    print('aligning', flush=True)
-    r, Aff, inline = cv2.estimateAffine3D(
+    print(f'{time.ctime(time.time())}',
+          'Found enough spots to estimate the affine',
+          'fix:', len(fix_spots), ',',
+          'moving:', len(mov_spots),
+          flush=True)
+    _, Aff, _ = cv2.estimateAffine3D(
         fix_spots, mov_spots,
         ransacThreshold=align_threshold,
         confidence=0.999,
         **kwargs,
     )
 
     # ensure affine is sensible
     if np.any( np.abs(np.diag(Aff) - 1) > diagonal_constraint ):
-        print("Degenerate affine produced, returning default", flush=True)
+        print(f'{time.ctime(time.time())}',
+              'Degenerate affine produced, returning default',
+              flush=True)
         return default
 
     # augment matrix and return
     affine = np.eye(fix.ndim + 1)
     affine[:fix.ndim, :] = Aff
     return affine
 
@@ -714,15 +758,15 @@
     # score all random affines
     current_best_score = WORST_POSSIBLE_SCORE
     scores = np.empty(random_iterations + 1, dtype=np.float64)
     for iii, ppp in enumerate(params):
         scores[iii] = score_affine(ut.physical_parameters_to_affine_matrix_3d(ppp, center))
         if print_running_improvements and scores[iii] < current_best_score:
                 current_best_score = scores[iii]
-                print(iii, ': ', current_best_score, '\n', ppp)
+                print(f'{time.ctime(time.time())}',iii, ': ', current_best_score, '\n', ppp)
     sys.stdout.flush()
 
     # return top results
     partition_indx = np.argpartition(scores, nreturn)[:nreturn]
     params, scores = params[partition_indx], scores[partition_indx]
     return [ut.physical_parameters_to_affine_matrix_3d(p, center) for p in params[np.argsort(scores)]]
 
@@ -888,27 +932,35 @@
 
     # execute alignment, for any exceptions return default
     try:
         initial_metric_value = irm.MetricEvaluate(fix, mov)
         irm.Execute(fix, mov)
         final_metric_value = irm.MetricEvaluate(fix, mov)
     except Exception as e:
-        print("Registration failed due to ITK exception:\n", e)
-        print("Returning default", flush=True)
+        print(f'{time.ctime(time.time())}',
+              'Registration failed due to ITK exception:\n', e,
+              flush=True)
+        print(f'{time.ctime(time.time())} Returning default',
+              flush=True)
         return default
 
     # if registration improved metric return result
     # otherwise return default
     if final_metric_value < initial_metric_value:
-        print("Registration succeeded", flush=True)
+        print(f'{time.ctime(time.time())} Registration succeeded',
+              flush=True)
         return ut.affine_transform_to_matrix(transform)
     else:
-        print("Optimization failed to improve metric")
-        print(f"METRIC VALUES initial: {initial_metric_value} final: {final_metric_value}")
-        print("Returning default", flush=True)
+        print(f'{time.ctime(time.time())} Optimization failed to improve metric',
+              flush=True)
+        print(f'{time.ctime(time.time())}',
+              f'METRIC VALUES initial: {initial_metric_value} final: {final_metric_value}',
+              flush=True)
+        print(f'{time.ctime(time.time())} Returning default',
+              flush=True)
         return default
 
 
 def deformable_align(
     fix,
     mov,
     fix_spacing,
@@ -1074,33 +1126,41 @@
 
     # execute alignment, for any exceptions return default
     try:
         initial_metric_value = irm.MetricEvaluate(fix, mov)
         irm.Execute(fix, mov)
         final_metric_value = irm.MetricEvaluate(fix, mov)
     except Exception as e:
-        print("Registration failed due to ITK exception:\n", e)
-        print("Returning default", flush=True)
+        print(f'{time.ctime(time.time())}',
+              'Registration failed due to ITK exception:\n', e,
+              flush=True)
+        print(f'{time.ctime(time.time())} Returning default',
+              flush=True)
         return default
 
     # if registration improved metric return result
     # otherwise return default
     if final_metric_value < initial_metric_value:
         params = np.concatenate((transform.GetFixedParameters(), transform.GetParameters()))
         field = ut.bspline_to_displacement_field(
             transform, initial_fix_shape,
             spacing=initial_fix_spacing, origin=fix_origin,
             direction=np.eye(fix.GetDimension()),
         )
-        print("Registration succeeded", flush=True)
+        print(f'{time.ctime(time.time())} Registration succeeded',
+              flush=True)
         return params, field
     else:
-        print("Optimization failed to improve metric")
-        print(f"METRIC VALUES initial: {initial_metric_value} final: {final_metric_value}")
-        print("Returning default", flush=True)
+        print(f'{time.ctime(time.time())} Optimization failed to improve metric',
+              flush=True)
+        print(f'{time.ctime(time.time())}',
+              f'METRIC VALUES initial: {initial_metric_value} final: {final_metric_value}',
+              flush=True)
+        print(f'{time.ctime(time.time())} Returning default',
+              flush=True)
         return default
 
 
 def alignment_pipeline(
     fix,
     mov,
     fix_spacing,
@@ -1208,23 +1268,21 @@
              'rigid': lambda **c: affine_align(*a, **{**b, **c}, rigid=True),
              'affine':lambda **c: affine_align(*a, **{**b, **c}),
              'deform':lambda **c: deformable_align(*a, **{**b, **c})[1],}
 
     # loop over steps
     new_transforms = []
     for alignment, arguments in steps:
+        print(f'{time.ctime(time.time())} Run', alignment, arguments,
+              flush=True)
         arguments = {**kwargs, **arguments}
         arguments['static_transform_list'] = static_transform_list + new_transforms
         new_transforms.append(align[alignment](**arguments))
 
     # return in the requested format
     if return_format == 'independent':
         return new_transforms
     elif return_format == 'compressed':
-        shapes = np.array([x.shape for x in new_transforms], dtype=object)
-        changes = np.where(shapes[:-1] != shapes[1:])[0] + 1
-        changes = [0,] + list(changes) + [len(new_transforms),]
-        F = lambda a, b: compose_transform_list(new_transforms[a:b], fix_spacing)
-        return [F(a, b) for a, b in zip(changes[:-1], changes[1:])]
+        return compress_transform_list(new_transforms, [fix_spacing,]*len(new_transforms))
     elif return_format == 'flatten':
         return compose_transform_list(new_transforms, fix_spacing)
```

### Comparing `bigstream-1.2.9/bigstream/application_pipelines.py` & `bigstream-1.3.0/bigstream/application_pipelines.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/bigstream/configure_irm.py` & `bigstream-1.3.0/bigstream/configure_irm.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,19 +129,25 @@
     irm : itk::simple::ImageRegistrationMethod object
         The configured ImageRegistrationMethod object. Simply needs
         images and a transform type to be ready for optimization.
     """
 
     # identify number of physical cores available
     ncores = ut.get_number_of_cores()
+    if 'ITK_THREADS' in os.environ:
+        nthreads = int(os.environ["ITK_THREADS"])
+    elif 'NO_HYPERTHREADING' in os.environ:
+        nthreads = ncores
+    else:
+        nthreads = 2*ncores
 
     # initialize IRM object, be completely sure nthreads is set
-    sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(2*ncores)
+    sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(nthreads)
     irm = sitk.ImageRegistrationMethod()
-    irm.SetNumberOfThreads(2*ncores)
+    irm.SetNumberOfThreads(nthreads)
 
     # set interpolator
     irm.SetInterpolator(interpolator_switch[interpolator])
 
     # metric switch
     metric_switch = {
         'ANC':irm.SetMetricAsANTSNeighborhoodCorrelation,
```

### Comparing `bigstream-1.2.9/bigstream/features.py` & `bigstream-1.3.0/bigstream/features.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import numpy as np
+import time
+
 from fishspot.filter import white_tophat, apply_foreground_mask
-from fishspot.detect import detect_spots_log
-from scipy.stats.mstats import winsorize
 from scipy.spatial import cKDTree
+from scipy.stats.mstats import winsorize
+from skimage.feature import blob_dog, blob_log
 
 
 def blob_detection(
     image,
     min_blob_radius,
     max_blob_radius,
+    num_sigma=5,
     winsorize_limits=None,
     background_subtract=False,
+    blob_method='log',
     mask=None,
     **kwargs,
 ):
     """
     Find discrete blobs in an image
 
     Parameters
@@ -36,26 +40,68 @@
     Returns
     -------
     blob_coordinates_and_intensities : nd-array Nx4
         The first three columns of the array are the coordinates of the
         detected blobs. The last column is the image intensity at the
         detected coordinate location.
     """
-
     processed_image = np.copy(image)
-    if winsorize_limits is not None:
-        processed_image = winsorize(processed_image, limits=winsorize_limits)
+    start_time = time.time()
+
+    # ensure iterable radii
+    if not isinstance(min_blob_radius, (tuple, list, np.ndarray)):
+        min_blob_radius = (min_blob_radius,)*image.ndim
+    if not isinstance(max_blob_radius, (tuple, list, np.ndarray)):
+        max_blob_radius = (max_blob_radius,)*image.ndim
+
+    blob_detect_method = None
+    if blob_method == 'dog':
+        # difference of gaussian
+        blob_detect_method = blob_dog
+    else:
+        # laplacian of gaussian
+        blob_detect_method = blob_log
+        kwargs['num_sigma'] = num_sigma
+
+    # set given arguments
+    kwargs['min_sigma'] = np.array(min_blob_radius) / np.sqrt(image.ndim)
+    kwargs['max_sigma'] = np.array(max_blob_radius) / np.sqrt(image.ndim)
+
+    # set additional defaults
+    if 'threshold' not in kwargs or kwargs['threshold'] is None:
+        kwargs['threshold'] = None
+        kwargs['threshold_rel'] = 0.1
+
+    print(f'{time.ctime(time.time())}',
+          f'Start spot detection ({min_blob_radius}, {max_blob_radius})',
+          kwargs,
+          flush=True)
+    if winsorize_limits:
+        processed_image = winsorize(processed_image, limits=winsorize_limits,
+                                    inplace=True)
+        done_winsorize_time = time.time()
+        print(f'{time.ctime(time.time())}',
+              f'Winsorization completed in {done_winsorize_time-start_time}s',
+              flush=True)
     if background_subtract:
         processed_image = white_tophat(processed_image, max_blob_radius)
-    spots = detect_spots_log(
+        done_tophat_time = time.time()
+        print(f'{time.ctime(time.time())}',
+              f'White top hat completed in {done_tophat_time-start_time}s',
+              flush=True)
+
+    spots = blob_detect_method(
         processed_image,
-        min_blob_radius,
-        max_blob_radius,
         **kwargs,
     ).astype(int)
+    done_spots_time = time.time()
+    print(f'{time.ctime(time.time())}',
+          f'Spot detection ({min_blob_radius}, {max_blob_radius})',
+          f'completed in {done_spots_time-start_time}s',
+          flush=True)
     if mask is not None: spots = apply_foreground_mask(spots, mask)
     intensities = image[ tuple(spots[:, iii] for iii in range(image.ndim)) ]
     return np.hstack((spots[:, :image.ndim], intensities[..., None]))
 
 
 def get_contexts(image, coords, radius):
     """
@@ -84,21 +130,27 @@
         contexts.append(image[crop])
     return contexts    
 
 
 def _stats(arr):
     """
     """
-
-    # compute mean and standard deviation along columns
-    arr = arr.astype(np.float64)
-    means = np.mean(arr, axis=1)
-    sqr_means = np.mean(np.square(arr), axis=1)
-    stddevs = np.sqrt( sqr_means - np.square(means) )
-    return means, stddevs
+    try:
+        # compute mean and standard deviation along columns
+        arr = arr.astype(np.float64)
+        means = np.mean(arr, axis=1)
+        sqr_means = np.mean(np.square(arr), axis=1)
+        stddevs = np.sqrt( sqr_means - np.square(means) )
+        return means, stddevs
+    except Exception as e:
+        print(f'{time.ctime(time.time())}',
+              'Stats exception for array of shape',
+              arr.shape, e,
+              flush=True)
+        raise e
 
 
 def pairwise_correlation(A, B):
     """
     Pearson correlation coefficient of all neighborhoods in A to all neighborhoods in B
 
     Parameters
```

### Comparing `bigstream-1.2.9/bigstream/level_set.py` & `bigstream-1.3.0/bigstream/level_set.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/bigstream/metrics.py` & `bigstream-1.3.0/bigstream/metrics.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/bigstream/motion_correct.py` & `bigstream-1.3.0/bigstream/motion_correct.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,15 @@
         Temporary files may be created during alignment. The temporary files will be
         in their own folder within the `temporary_directory`. The default is the
         current directory. Temporary files are removed if the function completes
         successfully.
 
     write_path : string (default: None)
         If not None, the final array of transforms will be written to disk as a zarr
-        array at this path. If None then this array is returned in memroy. Only use
+        array at this path. If None then this array is returned in memory. Only use
         this if transforms are deformation and if the resultant set of transforms
         is too large to fit in memory. 
 
     kwargs : any additional arguments
         Passed to alignment_pipeline. Control the nature of alignments through these arguments
 
     Returns
@@ -421,15 +421,14 @@
     for iii, transform in enumerate(transforms[1:]):
         new_transforms[iii+1] = compose_transforms(
             transform, new_transforms[iii], spacing, spacing,
         )
     return new_transforms
         
 
-
 # TODO: VERY OLD - UPDATE TO TAKE ZARR INPUTS AND BE
 #    CONSISTENT WITH motion_correct FUNCTION
 def deformable_motion_correct(
     fix, frames,
     fix_spacing, frames_spacing,
     time_stride=1,
     sigma=7,
@@ -559,15 +558,15 @@
         d = json.load(f)
     return np.array([d[str(i)] for i in range(len(d))])
 
 
 @cluster
 def resample_frames(
     fix,
-    mov_zarr,
+    mov,
     fix_spacing,
     mov_spacing,
     transforms,
     write_path,
     mask=None,
     time_stride=1,
     interpolator='1',
@@ -581,18 +580,17 @@
     Resample a 4D dataset using a set of motion correction transforms
 
     Parameters
     ----------
     fix : numpy.ndarray
         The reference image. Frames will be resampled onto this voxel grid.
 
-    mov_zarr : zarr.Array
-        The moving image frames. This should be a 4D zarr Array object that is
-        only lazy loaded, e.g. not in memory. The time axis should be the first
-        axis.
+    mov : numpy.ndarray or zarr.Array
+        The moving image frames. This should be a 3D or 4D. The time axis should be
+        the first axis.
 
     fix_spacing : 1d array
         the voxel spacing of the fixed image in micrometers
 
     mov_spacing : 1d array
         The voxel spacing of the moving images in micrometers
 
@@ -646,19 +644,24 @@
 
     # format and depost mask in location accessible to all workers
     temporary_directory = tempfile.TemporaryDirectory(
         prefix='.', dir=os.getcwd(),
     )
     np.save(temporary_directory.name + '/fix.npy', fix)
     if mask is not None:
-        mask_sh, mov_sh = mask.shape, mov_zarr.shape[1:]
+        mask_sh, mov_sh = mask.shape, mov.shape[1:]
         if mask_sh != mov_sh:
             mask = zoom(mask, np.array(mov_sh) / mask_sh, order=0)
         np.save(temporary_directory.name + '/mask.npy', mask)
 
+    # save moving image frames as zarr array
+    zarr_blocks = (1,) + mov.shape[1:]
+    mov_zarr_path = temporary_directory.name + '/mov.zarr'
+    mov_zarr = ut.numpy_to_zarr(mov, zarr_blocks, mov_zarr_path)
+
     # save transforms as zarr array
     zarr_blocks = (1,) + transforms.shape[1:]
     transforms_zarr_path = temporary_directory.name + '/transforms.zarr'
     transforms_zarr = ut.numpy_to_zarr(transforms, zarr_blocks, transforms_zarr_path)
 
     # save initial deforms to location accessible to all workers
     new_list = []
```

### Comparing `bigstream-1.2.9/bigstream/piecewise_align.py` & `bigstream-1.3.0/bigstream/piecewise_align.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,15 @@
 
     Parameters
     ----------
     fix : ndarray
         the fixed image
 
     mov : ndarray
-        the moving image; `fix.shape` must equal `mov.shape`
-        I.e. typically piecewise affine alignment is done after
-        a global affine alignment wherein the moving image has
-        been resampled onto the fixed image voxel grid.
+        the moving image
 
     fix_spacing : 1d array
         The spacing in physical units (e.g. mm or um) between voxels
         of the fixed image.
         Length must equal `fix.ndim`
 
     mov_spacing : 1d array
@@ -253,15 +250,15 @@
         for transform in static_transform_list[::-1]:
             if len(transform.shape) == 2:
                 mov_block_coords_phys = apply_transform_to_coordinates(
                     mov_block_coords_phys, [transform,],
                 )
                 transform = ut.change_affine_matrix_origin(transform, fix_block_coords_phys[0])
             else:
-                spacing = ut.relative_spacing(transform, fix_zarr, fix_spacing)
+                spacing = ut.relative_spacing(transform.shape, fix_zarr.shape, fix_spacing)
                 ratio = np.array(transform.shape[:-1]) / fix_zarr.shape
                 start = np.round( ratio * fix_block_coords[0] ).astype(int)
                 stop = np.round( ratio * (fix_block_coords[-1] + 1) ).astype(int)
                 transform_slices = tuple(slice(a, b) for a, b in zip(start, stop))
                 transform = transform[transform_slices]
                 origin = spacing * start
                 mov_block_coords_phys = apply_transform_to_coordinates(
```

### Comparing `bigstream-1.2.9/bigstream/piecewise_transform.py` & `bigstream-1.3.0/bigstream/piecewise_transform.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from itertools import product
 import bigstream.utility as ut
 import os, tempfile
 from ClusterWrap.decorator import cluster
 import dask.array as da
 import zarr
 import bigstream.transform as bs_transform
+from dask.distributed import as_completed
 
 
 @cluster
 def distributed_apply_transform(
     fix_zarr, mov_zarr,
     fix_spacing, mov_spacing,
     transform_list,
@@ -113,14 +114,15 @@
 
     # get overlap and number of blocks
     blocksize = np.array(blocksize)
     overlap = np.round(blocksize * overlap).astype(int)  # NOTE: default overlap too big?
     nblocks = np.ceil(np.array(fix_zarr.shape) / blocksize).astype(int)
 
     # store block coordinates in a dask array
+    # TODO: remove use of dask array
     block_coords = np.empty(nblocks, dtype=tuple)
     for (i, j, k) in np.ndindex(*nblocks):
         start = blocksize * (i, j, k) - overlap
         stop = start + blocksize + 2 * overlap
         start = np.maximum(0, start)
         stop = np.minimum(fix_zarr.shape, stop)
         block_coords[i, j, k] = tuple(slice(x, y) for x, y in zip(start, stop))
@@ -287,29 +289,29 @@
     temporary_directory = temporary_directory or os.getcwd()
     temporary_directory = tempfile.TemporaryDirectory(
         prefix='.', dir=temporary_directory,
     )
 
     # ensure all deforms are zarr
     new_list = []
-    zarr_blocks = (128,)*3 + (3,)  # TODO: generalize
+    zarr_blocks = (128,)*3 + (3,)
     for iii, transform in enumerate(transform_list):
-        if transform.shape != (4, 4):
+        if not len(transform.shape) in [1, 2]:
             zarr_path = temporary_directory.name + f'/deform{iii}.zarr'
             transform = ut.numpy_to_zarr(transform, zarr_blocks, zarr_path)
         new_list.append(transform)
     transform_list = new_list
 
     # determine partitions of coordinates
     origin = np.min(coordinates, axis=0)
     nblocks = np.max(coordinates, axis=0) - origin
     nblocks = np.ceil(nblocks / partition_size).astype(int)
     partitions, indices = [], []
-    for (i, j, k) in np.ndindex(*nblocks):
-        lower_bound = origin + partition_size * np.array((i, j, k))
+    for index in np.ndindex(*nblocks):
+        lower_bound = origin + partition_size * np.array(index)
         upper_bound = lower_bound + partition_size
         not_too_low = np.all(coordinates >= lower_bound, axis=1)
         not_too_high = np.all(coordinates < upper_bound, axis=1)
         part_indices = np.nonzero( not_too_low * not_too_high )[0]
         if part_indices.size != 0:
             partitions.append(coordinates[part_indices])
             indices.append(part_indices)
@@ -318,18 +320,20 @@
     def transform_partition(coordinates, transform_list):
 
         # read relevant region of transform
         a = np.min(coordinates, axis=0)
         b = np.max(coordinates, axis=0)
         new_list = []
         for iii, transform in enumerate(transform_list):
-            if transform.shape != (4, 4):
+            if not len(transform.shape) in [1, 2]:
                 spacing = transform_spacing
                 if isinstance(spacing, tuple): spacing = spacing[iii]
                 start = np.floor(a / spacing).astype(int)
+                last_index = np.array(transform.shape[:-1]) - 1
+                start = np.minimum(last_index, start)
                 stop = np.ceil(b / spacing).astype(int) + 1
                 crop = tuple(slice(x, y) for x, y in zip(start, stop))
                 transform = transform[crop]
             new_list.append(transform)
         transform_list = new_list
 
         # apply transforms
@@ -348,42 +352,45 @@
     results = np.empty_like(permuted)
     results[indices] = permuted
     return results
 
 
 @cluster
 def distributed_invert_displacement_vector_field(
-    field_zarr,
+    field,
     spacing,
     blocksize,
-    write_path,
+    write_path=None,
     step=0.5,
     iterations=10,
     sqrt_order=2,
     sqrt_step=0.5,
     sqrt_iterations=5,
     cluster=None,
     cluster_kwargs={},
+    temporary_directory=None,
 ):
     """
     Numerically find the inverse of a larger-than-memory displacement vector field
 
     Parameters
     ----------
-    field_zarr : zarr array
+    field : array like, can be zarr or numpy array
         The displacement vector field to invert
 
     spacing : 1d-array
         The physical voxel spacing of the displacement field
 
     blocksize : iterable
         The shape of blocks in voxels
 
     write_path : string (default: None)
-        Location on disk to write the resampled data as a zarr array
+        Location on disk to write the inverted displacement field
+        If None, then the inverted transform is returned in memory
+        to the client process (make sure you have enough RAM if you do this!)
 
     step : float (default: 0.5)
         The step size used for each iteration of the stationary point algorithm
 
     iterations : scalar int (default: 10)
         The number of stationary point iterations to find inverse. More
         iterations gives a more accurate inverse but takes more time.
@@ -405,42 +412,70 @@
     cluster_kwargs : dict (default: {})
         Arguments passed to ClusterWrap.cluster
         If working with an LSF cluster, this will be
         ClusterWrap.janelia_lsf_cluster. If on a workstation
         this will be ClusterWrap.local_cluster.
         This is how distribution parameters are specified.
 
+    temporary_directory : string (default: None)
+        Temporary files may be created during inversion. The temporary files will be
+        in their own folder within the `temporary_directory`. The default is the
+        current directory. Temporary files are removed if the function completes
+        successfully.
+
     Returns
     -------
     inverse_field : zarr array
         The numerical inverse of the given displacement vector field as a zarr array.
     """
 
+    # ensure input field is zarr
+    temporary_directory = tempfile.TemporaryDirectory(
+        prefix='.', dir=temporary_directory or os.getcwd(),
+    )
+    zarr_blocks = tuple(blocksize) + (field.shape[-1],)
+    field_zarr_path = temporary_directory.name + '/field.zarr'
+    field_zarr = ut.numpy_to_zarr(field, zarr_blocks, field_zarr_path)
+
+    # create output array
+    if write_path:
+        output_zarr = ut.create_zarr(
+            write_path,
+            field_zarr.shape,
+            zarr_blocks,
+            field_zarr.dtype,
+        )
+
     # get overlap and number of blocks
     blocksize = np.array(blocksize)
     overlap = np.round(blocksize * 0.25).astype(int)
     nblocks = np.ceil(np.array(field_zarr.shape[:-1]) / blocksize).astype(int)
 
-    # TODO: eliminate use of dask array
-    # store block coordinates in a dask array
-    block_coords = np.empty(nblocks, dtype=tuple)
+    # determine block coordinates
+    block_coords = []
+    block_coords_overlaps = []
     for (i, j, k) in np.ndindex(*nblocks):
-        start = blocksize * (i, j, k) - overlap
-        stop = start + blocksize + 2 * overlap
-        start = np.maximum(0, start)
+        start = blocksize * (i, j, k)
+        stop = start + blocksize
+        start_ol = start - overlap
+        stop_ol = stop + overlap
+
+        start_ol = np.maximum(0, start_ol)
         stop = np.minimum(field_zarr.shape[:-1], stop)
-        coords = tuple(slice(x, y) for x, y in zip(start, stop))
-        block_coords[i, j, k] = coords
-    block_coords = da.from_array(block_coords, chunks=(1,)*block_coords.ndim)
+        stop_ol = np.minimum(field_zarr.shape[:-1], stop_ol)
 
+        coords = tuple(slice(x, y) for x, y in zip(start, stop))
+        coords_ol = tuple(slice(x, y) for x, y in zip(start_ol, stop_ol))
+        block_coords.append(coords)
+        block_coords_overlaps.append(coords_ol)
 
-    def invert_block(slices):
+    # the function to run on every block
+    def invert_block(slices, slices_overlaps):
 
-        slices = slices.item()
-        field = field_zarr[slices]
+        field = field_zarr[slices_overlaps]
         inverse = bs_transform.invert_displacement_vector_field(
             field,
             spacing,
             step=step,
             iterations=iterations,
             sqrt_order=sqrt_order,
             sqrt_step=sqrt_step,
@@ -448,38 +483,44 @@
         )
 
         # crop out overlap
         for axis in range(inverse.ndim - 1):
 
             # left side
             slc = [slice(None),]*(inverse.ndim - 1)
-            if slices[axis].start != 0:
+            if slices_overlaps[axis].start != 0:
                 slc[axis] = slice(overlap[axis], None)
                 inverse = inverse[tuple(slc)]
 
             # right side
             slc = [slice(None),]*(inverse.ndim - 1)
             if inverse.shape[axis] > blocksize[axis]:
                 slc[axis] = slice(None, blocksize[axis])
                 inverse = inverse[tuple(slc)]
 
-        # return result
-        return inverse
+        # handle output
+        if not write_path:
+            return inverse
+        else:
+            output_zarr[slices] = inverse
+            return True
 
-    # invert all blocks
-    inverse = da.map_blocks(
+    # submit all blocks
+    futures = cluster.client.map(
         invert_block,
         block_coords,
-        dtype=field_zarr.dtype,
-        new_axis=[3,],
-        chunks=tuple(blocksize) + (3,),
+        block_coords_overlaps,
     )
 
-    # crop to original size
-    inverse = inverse[tuple(slice(0, s) for s in field_zarr.shape[:-1])]
-
-    # compute result, write to zarr array
-    da.to_zarr(inverse, write_path)
-
-    # return reference to result
-    return zarr.open(write_path, 'r+')
+    # reconstruct output if necessary
+    if not write_path:
+        future_keys = [f.key for f in futures]
+        inverse = np.zeros_like(field)
+        for batch in as_completed(futures, with_results=True).batches():
+            for future, result in batch:
+                iii = future_keys.index(future.key)
+                inverse[block_coords[iii]] = result
+        return inverse
+    else:
+        all_written = np.all(cluster.client.gather(futures))
+        return output_zarr
```

### Comparing `bigstream-1.2.9/bigstream/stitch.py` & `bigstream-1.3.0/bigstream/stitch.py`

 * *Files identical despite different names*

### Comparing `bigstream-1.2.9/bigstream/transform.py` & `bigstream-1.3.0/bigstream/transform.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     transform_list,
     transform_spacing=None,
     transform_origin=None,
     fix_origin=None,
     mov_origin=None,
     interpolator='1',
     extrapolate_with_nn=False,
+    compress_transforms=False,
 ):
     """
     Resample moving image onto fixed image through a list
     of transforms.
 
     Parameters
     ----------
@@ -70,28 +71,49 @@
         See bigstream.configure_irm.configure_irm documentation for options
 
     extrapolate_with_nn : Bool (default: False)
         If true extrapolations are done with Nearest Neighbors. Use if warping
         segmentation/multi-label data. Also prevents edge effects from padding
         when warping image data.
 
+    compress_transforms : Bool (default: False)
+        If False, all transforms are independently added to the composite transform
+        before it is applied to the moving image. If True, we compose all neighboring
+        transforms of similar type in the transform list before applying. For example,
+        with this transform list, [affine1, affine2, deform1, deform2, affine3] and
+        compress_transform_list == False, the composite transform will include all five
+        transforms as indpendent objects. Especially when more than one deformation is
+        applied, this can sometimes result in interpolation artifacts on the edges of
+        images. With compress_transform_list == True, the given list would compress to
+        [composed_affine, composed_deform, affine3]. This reduces the likelihood of
+        edge artifacts, but is also slower.
+
     Returns
     -------
     warped image : ndarray
         The moving image warped through transform_list and resampled onto the
         fixed image grid.
     """
 
     # set global number of threads
     ncores = ut.get_number_of_cores()
     sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(2*ncores)
 
-    # construct transform
+    # format transform spacing
     fix_spacing = np.array(fix_spacing)
     if transform_spacing is None: transform_spacing = fix_spacing
+    if not isinstance(transform_spacing, tuple):
+        transform_spacing = (transform_spacing,) * len(transform_list)
+
+    # construct transform
+    if compress_transforms:
+        transform_list, transform_spacing = compress_transform_list(
+            transform_list, list(transform_spacing),
+        )
+        transform_spacing = tuple(transform_spacing)
     transform = ut.transform_list_to_composite_transform(
         transform_list, transform_spacing, transform_origin,
     )
 
     # set up resampler object
     resampler = sitk.ResampleImageFilter()
     resampler.SetNumberOfThreads(2*ncores)
@@ -340,22 +362,63 @@
         transform = compose_transforms(
             transforms.pop(), transform,
             spacings.pop(), transform_spacing,
         )
     return transform
 
 
+def compress_transform_list(transforms, spacings):
+    """
+    Separately compose all neighboring transforms of the same type
+    For example, [affine1, affine2, deform1, deform2, affine3, deform3]
+    becomes [composed_affine, composed_deform, affine3, deform3]
+
+    Parameters
+    ----------
+    transforms : list
+        Elements of list must be either 3x3 or 4x4 affine matrices or displacement
+        vector fields
+
+    spacings : list of 1d-arrays
+        The voxel spacing of all transforms in the list
+        Ignored for affine transforms (just put in a dummy value)
+
+    Returns
+    -------
+    compressed_transform_list : list of nd-arrays
+        A list of transforms where all neighboring transforms of the same type
+        are composed
+    compressed_spacings_list : list of 1d-arrays
+        A list of spacings for the transforms in compressed_transform_list
+    """
+
+    if len(transforms) == 2:
+        dims = [len(x.shape) for x in transforms]
+        if dims[0] == dims[1]:
+            transforms = [compose_transform_list(transforms, spacings),]
+            spacings = [spacings[1],]
+    if len(transforms) > 2:
+        dims = np.array([len(x.shape) for x in transforms])
+        changes = np.where(dims[:-1] != dims[1:])[0] + 1
+        changes = [0,] + list(changes) + [len(transforms),]
+        F = lambda a, b: compose_transform_list(transforms[a:b], spacings[a:b])
+        transforms = [F(a, b) for a, b in zip(changes[:-1], changes[1:])]
+        spacings = [spacings[x-1] for x in changes[1:]]
+    return transforms, spacings
+
+
 def invert_displacement_vector_field(
     field,
     spacing,
     step=0.5,
     iterations=10,
     sqrt_order=2,
     sqrt_step=0.5,
     sqrt_iterations=5,
+    verbose=True,
 ):
     """
     Numerically find the inverse of a displacement vector field.
 
     Parameters
     ----------
     field : nd-array
@@ -376,34 +439,43 @@
 
     sqrt_step : float (default: 0.5)
         The step size used for each iteration of the composition square root gradient descent
 
     sqrt_iterations : scalar int (default: 5)
         The number of iterations to find the field composition square root
 
+    verbose : bool (default: True)
+        Whether or not to print optimization feedback to standard output
+
     Returns
     -------
     inverse_field : nd-array
         The numerical inverse of the given displacement vector field.
         field(inverse_field) should be nearly zeros everywhere.
         inverse_field(field) should be nearly zeros everywhere.
         If precision is not high enough, look at iterations,
         order, and sqrt_iterations.
     """
 
     # initialize inverse as negative root
     root = _displacement_field_composition_nth_square_root(
         field, spacing, sqrt_order, sqrt_step, sqrt_iterations,
+        verbose=verbose,
     )
     inv = - np.copy(root)
 
     # iterate to invert
+    if verbose: print('INVERTING ROOT')
     for i in range(iterations):
         residual = compose_transforms(root, inv, spacing, spacing)
         inv -= step * residual
+        if verbose:
+            residual_magnitude = np.linalg.norm(residual)
+            print(f'FITTING INVERSE  -  Iteration: {i} --> Residual: {residual_magnitude}')
+    if verbose: print('', flush=True)
 
     # square-compose inv order times
     for i in range(sqrt_order):
         inv = compose_transforms(inv, inv, spacing, spacing)
 
     # return result
     return inv
@@ -411,48 +483,53 @@
 
 def _displacement_field_composition_nth_square_root(
     field,
     spacing,
     order,
     step,
     iterations,
+    verbose=True,
 ):
     """
     """
 
     # initialize with given field
     root = np.copy(field)
 
     # iterate taking square roots
     for i in range(order):
+        if verbose: print(f'FINDING ROOT ORDER {i}')
         root = _displacement_field_composition_square_root(
-            root, spacing, step, iterations,
+            root, spacing, step, iterations, verbose=verbose,
         )
 
     # return result
     return root
 
 
 def _displacement_field_composition_square_root(
     field,
     spacing,
     step,
     iterations,
+    verbose=True,
 ):
     """
     """
 
     # container to hold root
     root = 0.5 * field
 
     # iterate
     for i in range(iterations):
         residual = (field - compose_transforms(root, root, spacing, spacing))
-        gradient = np.einsum('...ij,...j', displacement_field_jacobian(root, spacing), residual) + residual
-        root += step * gradient
+        root += step * residual
+        if verbose:
+            residual_magnitude = np.linalg.norm(residual)
+            print(f'FITTING ROOT  -  Iteration: {i} --> Residual: {residual_magnitude}')
 
     # return result
     return root
 
 
 def displacement_field_jacobian(field, spacing):
     """
@@ -473,9 +550,7 @@
 
 def displacement_field_jacobian_determinant(field, spacing):
     """
     """
 
     jacobian = displacement_field_jacobian(field, spacing)
     return np.linalg.det(jacobian)
-
-
```

### Comparing `bigstream-1.2.9/bigstream.egg-info/SOURCES.txt` & `bigstream-1.3.0/bigstream.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 LICENSE.md
 README.md
 setup.py
 bigstream/__init__.py
 bigstream/align.py
 bigstream/application_pipelines.py
 bigstream/configure_irm.py
+bigstream/distributed_align.py
+bigstream/distributed_io_utility.py
+bigstream/distributed_transform.py
 bigstream/features.py
+bigstream/io_utility.py
 bigstream/level_set.py
 bigstream/metrics.py
 bigstream/motion_correct.py
 bigstream/piecewise_align.py
 bigstream/piecewise_transform.py
 bigstream/stitch.py
 bigstream/transform.py
```

### Comparing `bigstream-1.2.9/setup.py` & `bigstream-1.3.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import setuptools
 
 setuptools.setup(
     name="bigstream",
-    version="1.2.9",
+    version="1.3.0",
     author="Greg M. Fleishman",
     author_email="greg.nli10me@gmail.com",
     description="Tools for distributed alignment of massive images",
-    url="https://github.com/GFleishman/bigstream",
-    license="MIT",
+    url="https://github.com/JaneliaScicomp/bigstream",
+    license="BSD-3",
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=[
         'numpy>=1.20.3',
         'scipy>=1.9.1',
         'opencv-python>=4.5.5.64',
-        'bokeh>=2.4.3',
-        'dask>=2022.9.1',
-        'dask[array]>=2022.9.1',
-        'dask[delayed]>=2022.9.1',
-        'dask[distributed]>=2022.9.1',
+        'bokeh>=2.4.3,<3',
+        'dask>=2023.10.1',
+        'distributed>=2023.10.1',
         'ClusterWrap>=0.3.0',
         'zarr>=2.12.0',
         'h5py>=3.8.0',
         'numcodecs>=0.9.1',
         'fishspot>=0.2.3',
         'SimpleITK>=2.2.0',
         'tifffile>=2022.10.10',
-        'morphsnakes>=2.0.0'
+        'morphsnakes>=2.0.0',
+        'pynrrd>=1.0.0',
+        'scikit-image>=0.20.0',
     ]
 )
```

