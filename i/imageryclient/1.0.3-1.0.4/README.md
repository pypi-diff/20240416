# Comparing `tmp/imageryclient-1.0.3.tar.gz` & `tmp/imageryclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imageryclient-1.0.3.tar", last modified: Thu Jun 29 22:21:36 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `imageryclient-1.0.3.tar` & `imageryclient-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,9 @@
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.686398 imageryclient-1.0.3/
--rw-r--r--   0 caseysm    (501) staff       (20)     1079 2022-11-16 18:21:56.000000 imageryclient-1.0.3/LICENSE
--rw-r--r--   0 caseysm    (501) staff       (20)       49 2022-11-16 18:21:56.000000 imageryclient-1.0.3/MANIFEST.in
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-06-29 22:21:36.686074 imageryclient-1.0.3/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)    16014 2023-05-08 17:45:33.000000 imageryclient-1.0.3/README.md
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.684172 imageryclient-1.0.3/imageryclient/
--rw-r--r--   0 caseysm    (501) staff       (20)      133 2023-06-29 22:21:23.000000 imageryclient-1.0.3/imageryclient/__init__.py
--rw-r--r--   0 caseysm    (501) staff       (20)    11089 2022-11-29 01:10:22.000000 imageryclient-1.0.3/imageryclient/composite.py
--rw-r--r--   0 caseysm    (501) staff       (20)    40224 2023-06-29 22:19:16.000000 imageryclient-1.0.3/imageryclient/imagery.py
--rw-r--r--   0 caseysm    (501) staff       (20)     6579 2023-06-29 22:20:49.000000 imageryclient-1.0.3/imageryclient/utils.py
-drwxr-xr-x   0 caseysm    (501) staff       (20)        0 2023-06-29 22:21:36.685469 imageryclient-1.0.3/imageryclient.egg-info/
--rw-r--r--   0 caseysm    (501) staff       (20)     1554 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/PKG-INFO
--rw-r--r--   0 caseysm    (501) staff       (20)      356 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/SOURCES.txt
--rw-r--r--   0 caseysm    (501) staff       (20)        1 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/dependency_links.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       81 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/requires.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       14 2023-06-29 22:21:36.000000 imageryclient-1.0.3/imageryclient.egg-info/top_level.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       82 2022-11-28 07:21:09.000000 imageryclient-1.0.3/requirements.txt
--rw-r--r--   0 caseysm    (501) staff       (20)       38 2023-06-29 22:21:36.686484 imageryclient-1.0.3/setup.cfg
--rw-r--r--   0 caseysm    (501) staff       (20)     1166 2022-11-16 18:21:56.000000 imageryclient-1.0.3/setup.py
--rw-r--r--   0 caseysm    (501) staff       (20)     1254 2022-11-16 18:21:56.000000 imageryclient-1.0.3/short_readme.md
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 imageryclient-1.0.4/imageryclient/__init__.py
+-rw-r--r--   0        0        0    11087 2020-02-02 00:00:00.000000 imageryclient-1.0.4/imageryclient/composite.py
+-rw-r--r--   0        0        0    40205 2020-02-02 00:00:00.000000 imageryclient-1.0.4/imageryclient/imagery.py
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 imageryclient-1.0.4/imageryclient/utils.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 imageryclient-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 imageryclient-1.0.4/LICENSE
+-rw-r--r--   0        0        0    16018 2020-02-02 00:00:00.000000 imageryclient-1.0.4/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 imageryclient-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 imageryclient-1.0.4/PKG-INFO
```

### Comparing `imageryclient-1.0.3/LICENSE` & `imageryclient-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imageryclient-1.0.3/README.md` & `imageryclient-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 An optional `dim` argument will perform the slicing on axes other than the z-axis, although anisotropy in voxel resolution will not be accounted for.
 
 ```python
 ctr = [5019, 8677, 1211]
 width = 100
 z_slices = 3
 
-bounds_3d = ic.bounds_from_center(ctr, delx=width, dely=width, delz=z_slices)
+bounds_3d = ic.bounds_from_center(ctr, width=width, height=width, depth=z_slices)
 
 image, segs = img_client.image_and_segmentation_cutout(bounds_3d, split_segmentations=True)
 
 overlays = ic.composite_overlay(segs, imagery=image, alpha=0.3, width=3,
                                 merge_outline=False, side='in')
 
 overlays[0]
```

### Comparing `imageryclient-1.0.3/imageryclient/composite.py` & `imageryclient-1.0.4/imageryclient/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
                       l=DEFAULT_L,
                       s=DEFAULT_S,
                       ):
     """Make a colored composite overlay for a 3d mask from an iterable of masks.
 
     Parameters
     ----------
-    masks : list-like or dict
+    segs: list-like or dict
         Iterable of masked images of the same size. If a dict, colors must be a dict as well.
     colors : list-like, dict, or None
         Iterable of RGB colors of the same size as masks. If a dict, masks must also be a dict and colors
         must have all keys in masks. If None, uses `discrete_colors` to generate colors.
     alpha : float, optional
         Alpha value for the overlay
     imagery : PIL.Image.Image or None, optional
```

### Comparing `imageryclient-1.0.3/imageryclient/imagery.py` & `imageryclient-1.0.4/imageryclient/imagery.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         2x3 array of lower and upper bounds (in that order).
     """
     xl = ctr - np.array([width // 2, height // 2, depth // 2])
     xh = xl + np.array([width, height, depth])
     return np.array([xl, xh])
 
 
-
 def save_image_slices(
     filename_prefix,
     filename_suffix,
     img,
     slice_axis,
     image_type,
     verbose=False,
@@ -69,40 +68,33 @@
 class ImageryClient(object):
     """Tool to help download imagery and segmentation data.
 
     Can either take explicit cloudvolume paths for imagery and segmentation or use the Info Service to look up the right paths.
 
     Parameters
     ----------
+    client : caveclient.CAVEclient or None, optional
+        A pre-initialized CAVEclient to use for configuration and authentication.
+        If used, image source, segmentation source, and resolution come from the info service values.
+    resolution : array-like or 'image' or 'segmentation', optional
+        Sets the voxel resolution that bounds will be entered in, by default 'image', which is the mip 0 resolution of the imagery.
+        Note that if a client is used to set the sources, the resolution will be set to the client default.
+    segmentation : bool, optional
+        If False, no segmentation cloudvolume is initialized. By default True
+    imagery : bool, optional
+        If False, no imagery cloudvolume is initialized. By default True
     image_source : str, optional
         CloudVolume path to an imagery source, by default None
     segmentation_source : str, optional
         CloudVolume path to a segmentation source, by default None
-    datastack_name : str, optional
-        Datastack name to lookup information for in the InfoService, by default None
-    server_address : str, optional
-        Address of an InfoService host, by default None. If none, uses defaults in
-        the CAVEclient.
-    base_resolution : array-like or 'image' or 'segmentation', optional
-        Sets the voxel resolution that bounds will be entered in, by default 'image'.
-        Literal resolutions will be followed, while "image" or "segmentation" use the
-        mip 0 values of the associated cloudvolumes.
-    table_name : str, optional
-        Name of the chunkedgraph table (if used), by default None
     image_mip : int, optional
         Default mip level to use for imagery lookups, by default 0. Note that the same mip
         level for imagery and segmentation can correspond to different voxel resolutions.
     segmentation_mip : int, optional
         Default mip level to use for segmentation lookups, by default 0.
-    segmentation : bool, optional
-        If False, no segmentation cloudvolume is initialized. By default True
-    imagery : bool, optional
-        If False, no imagery cloudvolume is initialized. By default True
-    framework_client : caveclient.CAVEclient, optional
-        A pre-initialized Framework client to be used instead of initializing a new one.
     auth_token : str or None, optional
         Auth token to use for cloudvolume. If None, uses the default values from the CAVEclient. Default is None.
     timestamp : datetime.datetime or None,
         Fixed timestamp to use for segmentation lookups. If None, defaults to the present time
         when each function is run. Default is None.
     """
 
@@ -115,15 +107,14 @@
         image_source=None,
         segmentation_source=None,
         image_mip=None,
         segmentation_mip=None,
         auth_token=None,
         timestamp=None,
     ):
-
         self._image_source = image_source
         self._segmentation_source = segmentation_source
 
         self._auth_token = None
         if auth_token is not None:
             self._auth_token = auth_token
 
@@ -152,49 +143,59 @@
             self._image_source = client.info.image_source()
         if self._segmentation_source is None and self._use_segmentation:
             self._segmentation_source = client.info.segmentation_source()
         if self._resolution is None:
             self._resolution = client.info.viewer_resolution()
 
     def _configure_mip_levels(self, image_mip, segmentation_mip):
-        if image_mip is None:
+        if self._use_imagery is False:
+            self._base_imagery_mip = -1
+        elif image_mip is None:
             self._base_imagery_mip = utils._get_lowest_nonplaceholder(self.image_cv)
         else:
             self._base_imagery_mip = image_mip
-        if segmentation_mip is None:
-            self._base_segmentation_mip = utils._get_lowest_nonplaceholder(self.segmentation_cv)        
+
+        if self._use_segmentation is False:
+            self._base_segmentation_mip = -1
+        elif segmentation_mip is None:
+            self._base_segmentation_mip = utils._get_lowest_nonplaceholder(
+                self.segmentation_cv
+            )
         else:
             self._base_segmentation_mip = segmentation_mip
 
     def _configure_resolution(self, resolution):
         if resolution is None:
             resolution = "image"
-        
+
         if isinstance(resolution, str):
             if resolution in ["image", "segmentation"]:
                 if resolution == "image":
                     if self._use_imagery is None:
                         raise ValueError(
                             "Cannot set resolution from imagery if not being used"
                         )
-                    self._resolution = np.array(self.image_cv.mip_resolution(self._base_imagery_mip))
+                    self._resolution = np.array(
+                        self.image_cv.mip_resolution(self._base_imagery_mip)
+                    )
                 elif resolution == "segmentation":
                     if self._use_segmentation is None:
                         raise ValueError(
                             "Cannot set resolution from segmentation if not being used"
                         )
-                    self._resolution = np.array(self.segmentation_cv.mip_resolution(self._base_segmentation_mip))
+                    self._resolution = np.array(
+                        self.segmentation_cv.mip_resolution(self._base_segmentation_mip)
+                    )
             else:
                 raise ValueError(
                     'Base resolution must be set by the client, array-like, "image" or "segmentation"'
                 )
         else:
             self._resolution = np.array(resolution)
 
-
     @property
     def token(self):
         return self._auth_token
 
     @property
     def timestamp(self):
         if self._timestamp is None:
@@ -281,25 +282,25 @@
             ]
 
     def image_bbox_size_from_dimensions(self, image_size, mip=None, resolution=None):
         """Get the bbox_size equivalent for an imagery cutout with specified pixel dimensions
 
         Parameters
         ----------
-            image_size: list-like
-                Image size in pixels (2-element) or voxels (3-element)
-            mip: int or None, optional
-                Mip for which the image would be computed. Defaults to None, which uses the client default.
-            resolution: list-like or None, optional.
-                Resolution to use for the bbox_size. Defaults to None, or the client defauls.
+        image_size: list-like
+            Image size in pixels (2-element) or voxels (3-element)
+        mip: int or None, optional
+            Mip for which the image would be computed. Defaults to None, which uses the client default.
+        resolution: list-like or None, optional.
+            Resolution to use for the bbox_size. Defaults to None, or the client defauls.
 
         Returns
         -------
-            tuple:
-                Argument for bbox_size that would give the desired pixel dimensions.
+        tuple:
+            Argument for bbox_size that would give the desired pixel dimensions.
         """
         if mip is None:
             mip = self._base_imagery_mip
         if resolution is None:
             resolution = self._resolution
         return self._compute_dimensions_from_image_size(
             image_size, self.image_cv.mip_resolution(mip), resolution
@@ -308,25 +309,25 @@
     def segmentation_bbox_size_from_dimensions(
         self, image_size, mip=None, resolution=None
     ):
         """Get the bbox_size equivalent for an segmentation cutout with specified pixel dimensions
 
         Parameters
         ----------
-            image_size: list-like
-                Image size in pixels (2-element) or voxels (3-element)
-            mip: int or None, optional
-                Mip for which the image would be computed. Defaults to None, which uses the client default.
-            resolution: list-like or None, optional.
-                Resolution to use for the bbox_size. Defaults to None, or the client defauls.
+        image_size: list-like
+            Image size in pixels (2-element) or voxels (3-element)
+        mip: int or None, optional
+            Mip for which the image would be computed. Defaults to None, which uses the client default.
+        resolution: list-like or None, optional.
+            Resolution to use for the bbox_size. Defaults to None, or the client defauls.
 
         Returns
         -------
-            tuple:
-                Argument for bbox_size that would give the desired pixel dimensions.
+        tuple:
+            Argument for bbox_size that would give the desired pixel dimensions.
         """
 
         if mip is None:
             mip = self._base_segmentation_mip
         if resolution is None:
             resolution = self._resolution
         return self._compute_dimensions_from_image_size(
@@ -447,15 +448,15 @@
         timestamp : datetime or None, optional
             Timestamp to use for dynamic segmentation data
         scale_to_bounds : bool or None, optional
             If True, rescales image to the same size as the bounds. Default is None, which rescales if mip is not set but otherwise does not.
         convert_to_int64 : bool, optional
             If True, converts segmentation data to int64 from uint64 if it is safe to do so. Default is True.
             If not safe, raises a warning and does not convert from uint64.
-            
+
         Returns
         -------
         numpy.ndarray
             Array whose elements correspond to the root id (or, if root_ids=None, the supervoxel id) at each voxel.
         """
         if self.segmentation_cv is None:
             return np.array([])
@@ -505,15 +506,17 @@
                     )
                 )
             )
         if convert_to_int64:
             if utils.safe_to_convert_uint64(seg):
                 seg = seg.astype(np.int64)
             else:
-                raise Warning('Could not convert to int64 because values are too large. Returning as uint64.')
+                raise Warning(
+                    "Could not convert to int64 because values are too large. Returning as uint64."
+                )
 
         if scale_to_bounds:
             return utils.rescale_to_bounds(
                 seg,
                 self._compute_bounds(bounds, bbox_size),  # downloading changes the bbox
             )
         else:
@@ -585,15 +588,14 @@
         include_null_root=False,
         bbox_size=None,
         resolution=None,
         timestamp=None,
         scale_to_bounds=None,
         convert_to_int64=True,
     ):
-
         """Download aligned and scaled imagery and segmentation data at a given resolution.
 
         Parameters
         ----------
         bounds : 2x3 list of ints
             A list of the lower and upper bound point for the cutout. The units are voxels in the resolution set by the
             base_resolution parameter.
```

### Comparing `imageryclient-1.0.3/imageryclient/utils.py` & `imageryclient-1.0.4/imageryclient/utils.py`

 * *Files identical despite different names*

