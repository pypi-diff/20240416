# Comparing `tmp/blending_toolkit-1.0.0b6.tar.gz` & `tmp/blending_toolkit-1.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blending_toolkit-1.0.0b6.tar", max compression
+gzip compressed data, was "blending_toolkit-1.0.0b7.tar", max compression
```

## Comparing `blending_toolkit-1.0.0b6.tar` & `blending_toolkit-1.0.0b7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1178 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/LICENSE
--rw-r--r--   0        0        0     4721 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/README.md
--rw-r--r--   0        0        0      601 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/btk/__init__.py
--rw-r--r--   0        0        0    18209 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/btk/blend_batch.py
--rw-r--r--   0        0        0     2480 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/btk/blend_generator.py
--rw-r--r--   0        0        0     5623 2024-02-22 20:13:15.800614 blending_toolkit-1.0.0b6/btk/catalog.py
--rw-r--r--   0        0        0    25191 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/deblend.py
--rw-r--r--   0        0        0    25288 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/draw_blends.py
--rw-r--r--   0        0        0    13796 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/match.py
--rw-r--r--   0        0        0     5404 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/measure.py
--rw-r--r--   0        0        0      139 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/__init__.py
--rw-r--r--   0        0        0     1449 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/base.py
--rw-r--r--   0        0        0     2171 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/detection.py
--rw-r--r--   0        0        0     2417 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/reconstruction.py
--rw-r--r--   0        0        0     1314 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/segmentation.py
--rw-r--r--   0        0        0     4680 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/metrics/utils.py
--rw-r--r--   0        0        0     2568 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/multiprocess.py
--rw-r--r--   0        0        0     1191 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/plotting.py
--rw-r--r--   0        0        0    24704 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/sampling_functions.py
--rw-r--r--   0        0        0     9341 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/survey.py
--rw-r--r--   0        0        0      889 2024-02-22 20:13:15.804614 blending_toolkit-1.0.0b6/btk/utils.py
--rw-r--r--   0        0        0     2372 2024-02-22 20:13:36.580609 blending_toolkit-1.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     5980 1970-01-01 00:00:00.000000 blending_toolkit-1.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1178 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/LICENSE
+-rw-r--r--   0        0        0     4721 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/README.md
+-rw-r--r--   0        0        0      601 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/__init__.py
+-rw-r--r--   0        0        0    17521 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/blend_batch.py
+-rw-r--r--   0        0        0     2480 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/blend_generator.py
+-rw-r--r--   0        0        0     5623 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/catalog.py
+-rw-r--r--   0        0        0    26203 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/deblend.py
+-rw-r--r--   0        0        0    25983 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/draw_blends.py
+-rw-r--r--   0        0        0    13914 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/match.py
+-rw-r--r--   0        0        0     5398 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/measure.py
+-rw-r--r--   0        0        0      139 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/__init__.py
+-rw-r--r--   0        0        0     1449 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/base.py
+-rw-r--r--   0        0        0     2171 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/detection.py
+-rw-r--r--   0        0        0     2417 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/reconstruction.py
+-rw-r--r--   0        0        0     1314 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/segmentation.py
+-rw-r--r--   0        0        0     4704 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/metrics/utils.py
+-rw-r--r--   0        0        0     2588 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/multiprocess.py
+-rw-r--r--   0        0        0     1191 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/plotting.py
+-rw-r--r--   0        0        0    24700 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/sampling_functions.py
+-rw-r--r--   0        0        0     9325 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/survey.py
+-rw-r--r--   0        0        0      889 2024-04-16 16:10:02.864935 blending_toolkit-1.0.0b7/btk/utils.py
+-rw-r--r--   0        0        0     4193 2024-04-16 16:10:29.041516 blending_toolkit-1.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0     5974 1970-01-01 00:00:00.000000 blending_toolkit-1.0.0b7/PKG-INFO
```

### Comparing `blending_toolkit-1.0.0b6/LICENSE` & `blending_toolkit-1.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/README.md` & `blending_toolkit-1.0.0b7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 ```
 
 ## Installation
 
 BTK is pip installable, with the following command:
 
 ```bash
-pip install blending-toolkit==1.0.0b6
+pip install blending-toolkit==1.0.0b7
 ```
 
 In case of any issues and for details of required packages, please see the more detailed installation instructions [here](https://lsstdesc.org/BlendingToolKit/install.html).
 
 ## Contributing
 
 Everyone can contribute to this project, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) document for details.
```

### Comparing `blending_toolkit-1.0.0b6/btk/__init__.py` & `blending_toolkit-1.0.0b7/btk/__init__.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/blend_batch.py` & `blending_toolkit-1.0.0b7/btk/blend_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         n_bands = len(self.survey.available_filters)
         b1, c1, ps11, ps12 = self.blend_images.shape
         b2, n, c2, ps21, ps22 = self.isolated_images.shape
         assert b1 == b2 == len(self.catalog_list) == self.batch_size
         assert c1 == c2 == n_bands
         assert n == self.max_n_sources
         assert ps11 == ps12 == ps21 == ps22 == self._get_image_size()
-        assert self.isolated_images.min() >= 0
 
     def _get_image_size(self) -> int:
         """Returns the size of the stamps in pixels."""
         pixel_scale = self.survey.pixel_scale.to_value("arcsec")
         return int(self.stamp_size / pixel_scale)
 
     def _get_wcs(self):
@@ -211,20 +210,20 @@
         self.catalog = self._validate_catalog(self.catalog)
         self.segmentation = self._validate_segmentation(self.segmentation)
         self.deblended_images = self._validate_deblended_images(self.deblended_images)
 
     def _validate_catalog(self, catalog: Table):
         if not ("ra" in catalog.colnames and "dec" in catalog.colnames):
             raise ValueError(
-                "The output catalog of at least one of your measurement functions does"
+                "The output catalog of at least one of your deblenders does"
                 "not contain the mandatory 'ra' and 'dec' columns"
             )
         if not len(catalog) <= self.max_n_sources:
             raise ValueError(
-                "The predicted catalog of at least one of your deblended images "
+                "The detection catalog of at least one of your deblended images "
                 "contains more sources than the maximum number of sources specified."
             )
         return catalog
 
     def _validate_segmentation(self, segmentation):
         if segmentation is not None:
             if self.image_size is None or self.n_bands is None:
@@ -254,19 +253,15 @@
                 self.image_size,
             )
             if deblended_images.shape != deblended_shape:
                 raise ValueError(
                     "The predicted deblended_images of at least one of your deblended images "
                     f"has the wrong shape. It should be {deblended_shape}."
                 )
-            if deblended_images.min() < 0:
-                raise ValueError(
-                    "The predicted deblended_images of at least one of your "
-                    "deblended images has negative values which is unphysical."
-                )
+
         return deblended_images
 
     def __repr__(self):
         """Return string representation of class."""
         string = (
             f"DeblendExample(max_n_sources = {self.max_n_sources}, "
             f"n_bands = {self.n_bands}, "
@@ -321,15 +316,15 @@
             if not ("ra" in catalog.colnames and "dec" in catalog.colnames):
                 raise ValueError(
                     "The output catalog of at least one of your measurement functions does"
                     "not contain the mandatory 'ra' and 'dec' columns"
                 )
             if not len(catalog) <= self.max_n_sources:
                 raise ValueError(
-                    "The predicted catalog of at least one of your deblended images "
+                    "The detections catalog of at least one of your deblended images "
                     "contains more sources than the maximum number of sources specified."
                 )
         return catalog_list
 
     def _validate_segmentation(self, segmentation: Optional[np.ndarray] = None) -> np.ndarray:
         if segmentation is not None:
             if self.image_size is None:
@@ -355,19 +350,14 @@
                 self.batch_size,
                 self.max_n_sources,
                 self.n_bands,
                 self.image_size,
                 self.image_size,
             )
 
-            if deblended_images.min() < 0:
-                raise ValueError(
-                    "The predicted deblended_images of at least one of your "
-                    "deblended images has negative values which is unphysical."
-                )
         return deblended_images
 
     def __repr__(self) -> str:
         """Return string representation of class."""
         string = (
             f"DeblendBatch(batch_size = {self.batch_size}, "
             f"max_n_sources = {self.max_n_sources} "
@@ -428,24 +418,18 @@
         with h5py.File(fpath, "r") as f:
             # load catalog with astropy hdf5 functions
             catalog_list = []
             for ii in range(f.attrs["batch_size"]):
                 catalog_list.append(read_table_hdf5(f, path=f"catalog_list/{ii}"))
 
             # load segmentation
-            if "segmentation" in f.keys():
-                segmentation = f["segmentation"][:]
-            else:
-                segmentation = None
+            segmentation = f["segmentation"][:] if "segmentation" in f.keys() else None
 
             # load deblended images
-            if "deblended_images" in f.keys():
-                deblended_images = f["deblended_images"][:]
-            else:
-                deblended_images = None
+            deblended_images = f["deblended_images"][:] if "deblended_images" in f.keys() else None
 
             # load general info about blend
             batch_size = f.attrs["batch_size"]
             max_n_sources = f.attrs["max_n_sources"]
             image_size = f.attrs["image_size"]
             n_bands = f.attrs["n_bands"]
```

### Comparing `blending_toolkit-1.0.0b6/btk/blend_generator.py` & `blending_toolkit-1.0.0b7/btk/blend_generator.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/catalog.py` & `blending_toolkit-1.0.0b7/btk/catalog.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/deblend.py` & `blending_toolkit-1.0.0b7/btk/deblend.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,20 @@
 from astropy import units
 from astropy.coordinates import SkyCoord
 from astropy.table import Table
 from galcheat.utilities import mean_sky_level
 from numpy.linalg import LinAlgError
 from skimage.feature import peak_local_max
 
-from btk.blend_batch import BlendBatch, DeblendBatch, DeblendExample, MultiResolutionBlendBatch
+from btk.blend_batch import (
+    BlendBatch,
+    DeblendBatch,
+    DeblendExample,
+    MultiResolutionBlendBatch,
+)
 from btk.draw_blends import DrawBlendsGenerator
 from btk.multiprocess import multiprocess
 
 
 class Deblender(ABC):
     """Abstract base class containing the measure class for BTK.
 
@@ -35,14 +40,16 @@
 
     def __call__(self, blend_batch: BlendBatch, njobs: int = 1, **kwargs) -> DeblendBatch:
         """Calls the (user-implemented) `deblend` method along with validation of the input.
 
         Args:
             ii: The index of the example in the batch.
             blend_batch: Instance of `BlendBatch` class.
+            njobs: Number of processes to use.
+            kwargs: Additional arguments to pass to deblender call.
 
         Returns:
             Instance of `DeblendedExample` class.
         """
         if not isinstance(blend_batch, BlendBatch):
             raise TypeError(
                 f"Got type '{type(blend_batch)}', but expected an object of a BlendBatch class."
@@ -68,15 +75,16 @@
 
         Overwrite this function if you perform measurments on the batch.
         The default fucntionality is to use multiprocessing to speed up
         the iteration over all examples in the batch.
 
         Args:
             blend_batch: Instance of `BlendBatch` class
-            njobs: Number of njobs to paralelize across
+            njobs: Number of jobs to paralelize across
+            kwargs: Additional keyword arguments to pass to each deblend call.
 
         Returns:
             Instance of `DeblendedBatch` class
         """
         args_iter = ((ii, blend_batch) for ii in range(blend_batch.batch_size))
         kwargs_iter = repeat(kwargs)
         output = multiprocess(self.deblend, args_iter, kwargs_iter, njobs=njobs)
@@ -122,14 +130,15 @@
         self, ii: int, mr_batch: MultiResolutionBlendBatch, njobs: int = 1
     ) -> DeblendBatch:
         """Calls the (user-implemented) deblend method along with validation of the input.
 
         Args:
             ii: The index of the example in the batch.
             mr_batch: Instance of `MultiResolutionBlendBatch` class
+            njobs: Number of processes to use.
 
         Returns:
             Instance of `DeblendedExample` class
         """
         if not isinstance(mr_batch, MultiResolutionBlendBatch):
             raise TypeError(
                 f"Got type'{type(mr_batch)}', but expected a MultiResolutionBlendBatch object."
@@ -172,53 +181,50 @@
         return cls.__name__
 
 
 class PeakLocalMax(Deblender):
     """This class detects centroids with `skimage.feature.peak_local_max`.
 
     The function performs detection and deblending of the sources based on the provided
-    band index. If use_mean feature is used, then the measurement function is using
+    band index. If use_mean feature is used, then the Deblender will use
     the average of all the bands.
     """
 
     def __init__(
         self,
         max_n_sources: int,
         threshold_scale: int = 5,
         min_distance: int = 2,
         use_mean: bool = False,
         use_band: Optional[int] = None,
     ) -> None:
-        """Initializes measurement class. Exactly one of 'use_mean' or 'use_band' must be specified.
+        """Initializes Deblender class. Exactly one of 'use_mean' or 'use_band' must be specified.
 
         Args:
             max_n_sources: See parent class.
             threshold_scale: Minimum intensity of peaks.
             min_distance: Minimum distance in pixels between two peaks.
-            use_mean: Flag to use the band average for the measurement.
-            use_band: Integer index of the band to use for the measurement.
+            use_mean: Flag to use the band average for deblending.
+            use_band: Integer index of the band to use for deblending
         """
         super().__init__(max_n_sources)
         self.min_distance = min_distance
         self.threshold_scale = threshold_scale
 
         if use_band is None and not use_mean:
             raise ValueError("Either set 'use_mean=True' OR indicate a 'use_band' index")
         if use_band is not None and use_mean:
             raise ValueError("Only one of the parameters 'use_band' and 'use_mean' has to be set")
         self.use_mean = use_mean
         self.use_band = use_band
 
     def deblend(self, ii: int, blend_batch: BlendBatch) -> DeblendExample:
-        """Performs measurement on the ii-th example from the batch."""
+        """Performs deblending on the ii-th example from the batch."""
         blend_image = blend_batch.blend_images[ii]
-        if self.use_mean:
-            image = np.mean(blend_image, axis=0)
-        else:
-            image = blend_image[self.use_band]
+        image = np.mean(blend_image, axis=0) if self.use_mean else blend_image[self.use_band]
 
         # compute threshold value
         threshold = self.threshold_scale * np.std(image)
 
         # calculate coordinates
         coordinates = peak_local_max(image, min_distance=self.min_distance, threshold_abs=threshold)
         x, y = coordinates[:, 1], coordinates[:, 0]
@@ -230,14 +236,20 @@
         dec *= 3600
 
         # wrap in catalog
         catalog = Table()
         catalog["ra"], catalog["dec"] = ra, dec
         catalog["x_peak"], catalog["y_peak"] = x, y
 
+        if len(catalog) > self.max_n_sources:
+            raise ValueError(
+                "`PeakLocalMax` detected more sources than `max_n_sources`. Consider increasing"
+                "`threshold_scale` or `max_n_sources`."
+            )
+
         return DeblendExample(self.max_n_sources, catalog)
 
 
 class SepSingleBand(Deblender):
     """Return detection, segmentation and deblending information running SEP on a single band.
 
     The function performs detection and deblending of the sources based on the provided
@@ -251,51 +263,58 @@
         self,
         max_n_sources: int,
         thresh: float = 1.5,
         min_area: int = 5,
         use_mean: bool = False,
         use_band: Optional[int] = None,
     ) -> None:
-        """Initializes measurement class. Exactly one of 'use_mean' or 'use_band' must be specified.
+        """Initializes Deblender class. Exactly one of 'use_mean' or 'use_band' must be specified.
 
         Args:
             max_n_sources: See parent class.
             thresh: Threshold pixel value for detection use in `sep.extract`. This is
                 interpreted as a relative threshold: the absolute threshold at pixel (j, i)
                 will be `thresh * err[j, i]` where `err` is set to the global rms of
                 the background measured by SEP.
             min_area: Minimum number of pixels required for an object. Default is 5.
-            use_mean: Flag to use the band average for the measurement
-            use_band: Integer index of the band to use for the measurement
+            use_mean: Flag to use the band average for deblending.
+            use_band: Integer index of the band to use for deblending.
         """
         super().__init__(max_n_sources)
         if use_band is None and not use_mean:
             raise ValueError("Either set 'use_mean=True' OR indicate a 'use_band' index")
         if use_band is not None and use_mean:
             raise ValueError("Only one of the parameters 'use_band' and 'use_mean' has to be set")
         self.use_mean = use_mean
         self.use_band = use_band
         self.thresh = thresh
         self.min_area = min_area
 
     def deblend(self, ii: int, blend_batch: BlendBatch) -> DeblendExample:
-        """Performs measurement on the i-th example from the batch."""
+        """Performs deblending on the i-th example from the batch."""
         # get a 1-channel input for sep
         blend_image = blend_batch.blend_images[ii]
-        if self.use_mean:
-            image = np.mean(blend_image, axis=0)
-        else:
-            image = blend_image[self.use_band]
+        image = np.mean(blend_image, axis=0) if self.use_mean else blend_image[self.use_band]
 
         # run source extractor
         bkg = sep.Background(image)
         catalog, segmentation = sep.extract(
-            image, self.thresh, err=bkg.globalrms, segmentation_map=True, minarea=self.min_area
+            image,
+            self.thresh,
+            err=bkg.globalrms,
+            segmentation_map=True,
+            minarea=self.min_area,
         )
 
+        if len(catalog) > self.max_n_sources:
+            raise ValueError(
+                "SEP predicted more sources than `max_n_sources`. Consider increasing `thresh`"
+                " or `max_n_sources`."
+            )
+
         segmentation_exp = np.zeros((self.max_n_sources, *image.shape), dtype=bool)
         deblended_images = np.zeros((self.max_n_sources, *image.shape), dtype=image.dtype)
         n_objects = len(catalog)
         for jj in range(n_objects):
             seg_i = segmentation == jj + 1
             segmentation_exp[jj] = seg_i
             deblended_images[jj] = image * seg_i.astype(image.dtype)
@@ -328,36 +347,42 @@
     to a running list of detected coordinates. In order to avoid repeating detections,
     we run a KD-Tree algorithm to calculate the angular distance between each new
     coordinate and its closest neighbour. Then we discard those new coordinates that
     were closer than `matching_threshold` to any one of already detected coordinates.
     """
 
     def __init__(self, max_n_sources: int, matching_threshold: float = 1.0, thresh: float = 1.5):
-        """Initialize the SepMultiband measurement function.
+        """Initialize the SepMultiband Deblender.
 
         Args:
             max_n_sources: See parent class.
             matching_threshold: Threshold value for match detections that are close (arcsecs).
             thresh: See `SepSingleBand` class.
         """
         super().__init__(max_n_sources)
         self.matching_threshold = matching_threshold
         self.thresh = thresh
 
     def deblend(self, ii: int, blend_batch: BlendBatch) -> DeblendExample:
-        """Performs measurement on the ii-th example from the batch."""
+        """Performs deblending on the ii-th example from the batch."""
         # run source extractor on the first band
         wcs = blend_batch.wcs
         image = blend_batch.blend_images[ii]
         bkg = sep.Background(image[0])
         catalog = sep.extract(image[0], self.thresh, err=bkg.globalrms, segmentation_map=False)
         ra_coordinates, dec_coordinates = wcs.pixel_to_world_values(catalog["x"], catalog["y"])
         ra_coordinates *= 3600
         dec_coordinates *= 3600
 
+        if len(catalog) > self.max_n_sources:
+            raise ValueError(
+                "SEP predicted more sources than `max_n_sources`. Consider increasing `thresh`"
+                " or `max_n_sources`."
+            )
+
         # iterate over remaining bands and match predictions using KdTree
         for band in range(1, image.shape[0]):
             # run source extractor
             band_image = image[band]
             bkg = sep.Background(band_image)
             catalog = sep.extract(
                 band_image, self.thresh, err=bkg.globalrms, segmentation_map=False
@@ -376,18 +401,24 @@
             if len(c1) > 0 and len(c2) > 0:
                 # runs KD-tree to get distances to the closest neighbours
                 _, distance2d, _ = c1.match_to_catalog_sky(c2)
                 distance2d = distance2d.arcsec
 
                 # add new predictions, masking those that are closer than threshold
                 ra_coordinates = np.concatenate(
-                    [ra_coordinates, ra_detections[distance2d > self.matching_threshold]]
+                    [
+                        ra_coordinates,
+                        ra_detections[distance2d > self.matching_threshold],
+                    ]
                 )
                 dec_coordinates = np.concatenate(
-                    [dec_coordinates, dec_detections[distance2d > self.matching_threshold]]
+                    [
+                        dec_coordinates,
+                        dec_detections[distance2d > self.matching_threshold],
+                    ]
                 )
             else:
                 ra_coordinates = np.concatenate([ra_coordinates, ra_detections])
                 dec_coordinates = np.concatenate([dec_coordinates, dec_detections])
 
         # Wrap in the astropy table
         catalog = Table()
@@ -432,20 +463,20 @@
         self.max_iter = max_iter
         self.max_components = max_components
         self.min_snr = min_snr
 
     def deblend(
         self, ii: int, blend_batch: BlendBatch, reference_catalogs: Table = None
     ) -> DeblendExample:
-        """Performs measurement on the ii-th example from the batch.
+        """Performs deblending on the ii-th example from the batch.
 
         Args:
             ii: The index of the example in the batch.
             blend_batch: Instance of `BlendBatch` class.
-            reference_catalog: Reference catalog to use for deblending. If None, the
+            reference_catalogs: Reference catalog to use for deblending. If None, the
                 truth catalog is used.
 
         Returns:
             Instance of `DeblendedExample` class.
         """
         import scarlet  # pylint: disable=import-outside-toplevel
 
@@ -539,22 +570,22 @@
     def __init__(
         self,
         deblenders: Union[List[Deblender], Deblender],
         draw_blend_generator: DrawBlendsGenerator,
         njobs: int = 1,
         verbose: bool = False,
     ):
-        """Initialize measurement generator.
+        """Initialize deblender generator.
 
         Args:
             deblenders: Deblender or a list of Deblender that will be used on the
                             outputs of the draw_blend_generator.
             draw_blend_generator: Instance of subclasses of `DrawBlendsGenerator`.
             njobs: The number of parallel processes to run [Default: 1].
-            verbose: Whether to print information about measurement.
+            verbose: Whether to print information about deblending.
         """
         self.deblenders = self._validate_deblenders(deblenders)
         self.deblender_names = self._get_unique_deblender_names()
         self.draw_blend_generator = draw_blend_generator
         self.njobs = njobs
 
         self.batch_size = self.draw_blend_generator.batch_size
@@ -598,15 +629,15 @@
         for ii, name in enumerate(deblender_names):
             if name in names_counts:
                 deblender_names[ii] += f"_{names_counts[name]}"
                 names_counts[name] += 1
         return deblender_names
 
     def __next__(self) -> Tuple[BlendBatch, Dict[str, DeblendBatch]]:
-        """Return measurement results on a single batch from the draw_blend_generator.
+        """Return deblending results on a single batch from the draw_blend_generator.
 
         Returns:
             blend_batch: draw_blend_generator output from its `__next__` method.
             deblended_output (dict): Dictionary with keys being the name of each
                 measure function passed in, and each value its corresponding `MeasuredBatch`.
         """
         blend_batch = next(self.draw_blend_generator)
```

### Comparing `blending_toolkit-1.0.0b6/btk/draw_blends.py` & `blending_toolkit-1.0.0b7/btk/draw_blends.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from astropy.table import Column, Table
 from astropy.wcs import WCS
 from galcheat.utilities import mag2counts, mean_sky_level
 from tqdm.auto import tqdm
 
 from btk.blend_batch import BlendBatch, MultiResolutionBlendBatch
 from btk.blend_generator import BlendGenerator
-from btk.catalog import Catalog
+from btk.catalog import Catalog, CosmosCatalog
 from btk.multiprocess import get_current_process, multiprocess
 from btk.sampling_functions import SamplingFunction
 from btk.survey import Filter, Survey, make_wcs
 from btk.utils import DEFAULT_SEED
 
 MAX_SEED_INT = 1_000_000_000
 
@@ -124,16 +124,15 @@
         )
         components.append(bulge)
 
     if agn_flux > 0:
         agn = galsim.Gaussian(flux=agn_flux, sigma=1e-8)
         components.append(agn)
 
-    profile = galsim.Add(components)
-    return profile
+    return galsim.Add(components)
 
 
 class DrawBlendsGenerator(ABC):
     """Class that generates images of blends and individual isolated objects in batches.
 
     Batch is divided into 'mini-batches' of size `batch_size//njobs` and
     each mini-batch analyzed separately. The results are then combined to output a
@@ -428,17 +427,15 @@
         slen = int(self.stamp_size / survey.pixel_scale.to_value("arcsec"))
 
         iso_image = np.zeros((self.max_number, slen, slen))
         blend_image = galsim.Image(np.zeros((slen, slen)))
 
         for ii, entry in enumerate(blend_catalog):
             single_image = self.render_single(entry, filt, psf, survey)
-            if single_image is None:
-                iso_image[ii] = np.zeros(single_image)
-            else:
+            if single_image is not None:
                 iso_image[ii] = single_image.array
                 blend_image += single_image
 
         # add noise.
         if self.add_noise in ("galaxy", "all"):
             if self.verbose:
                 print("Galaxy noise added to blend image")
@@ -517,27 +514,28 @@
 class CosmosGenerator(DrawBlendsGenerator):
     """Subclass of DrawBlendsGenerator for drawing galaxies from the COSMOS catalog."""
 
     compatible_catalogs = ("CosmosCatalog",)
 
     def __init__(
         self,
-        catalog: Catalog,
+        catalog: CosmosCatalog,
         sampling_function: SamplingFunction,
         surveys: List[Survey],
         batch_size: int = 8,
         stamp_size: float = 24.0,
         njobs: int = 1,
         verbose: bool = False,
         add_noise: str = "all",
         seed: int = DEFAULT_SEED,
         use_bar: bool = False,
         apply_shear: bool = False,
         augment_data: bool = False,
         gal_type: str = "real",
+        noise_pad_size: float = 0,
     ):
         """Initializes the CosmosGenerator class. See parent class for most attributes.
 
         Args:
             catalog: See parent class.
             sampling_function: See parent class.
             surveys: See parent class.
@@ -548,14 +546,20 @@
             add_noise: See parent class.
             seed: See parent class.
             use_bar: See parent class.
             apply_shear: See parent class.
             augment_data: See parent class.
             gal_type: string to specify the type of galaxy simulations.
                             Either "real" (default) or "parametric".
+            noise_pad_size: For realistic galaxies, the size of region to pad with noise for
+                            each individual galaxy before forming the blend. This is the argument
+                            to the `COSMOSCatalog.makeGalaxy` function inside `galsim`. In BTK, we
+                            add noise after the blend is produced according to the `sky_level`,
+                            so the default for this argument is 0, as otherwise, noise would
+                            be added to the image twice.
         """
         super().__init__(
             catalog,
             sampling_function,
             surveys,
             batch_size,
             stamp_size,
@@ -569,39 +573,42 @@
         )
 
         if gal_type not in ("real", "parametric"):
             raise ValueError(
                 f"gal_type must be either 'real' or 'parametric', but you provided {gal_type}"
             )
         self.gal_type = gal_type
+        self.noise_pad_size = noise_pad_size
 
     def _check_compatibility(self, survey: Survey) -> None:
         if type(self.catalog).__name__ not in self.compatible_catalogs:
             raise ValueError(
                 f"The catalog provided is of the wrong type. The types of "
                 f"catalogs available for the {type(self).__name__} are {self.compatible_catalogs}"
             )
-        for band in survey.available_filters:
-            if f"{survey.name}_{band}" not in self.catalog.table.keys():
-                raise ValueError(
-                    f"The {band} filter of the survey {survey.name} "
-                    f"has no associated magnitude in the given catalog."
-                )
 
     def render_single(self, entry: Table, filt: Filter, psf: galsim.GSObject, survey: Survey):
         """Returns the Galsim Image of an isolated galaxy."""
-        galsim_catalog = self.catalog.get_galsim_catalog()
+        galsim_catalog: galsim.COSMOSCatalog = self.catalog.get_galsim_catalog()
+
+        # we optionally check if additional entres if of the form `f'{survey_name}_{filter_name}`
+        # were added to the catalog in which case we use that (assuming it's an AB magnitude).
+        # otherwise we simply use the COSMOS magnitudes which AB magnitudes so we can apply
+        # the standard approach to converting to fluxes.
+        if f"{survey.name}_{filt.name}" in entry.colnames:
+            gal_mag = entry[f"{survey.name}_{filt.name}"]
+        else:
+            gal_mag = entry["MAG"]
 
-        # get galaxy flux
-        mag_name = f"{survey.name}_{filt.name}"
-        gal_mag = entry[mag_name]
         gal_flux = mag2counts(gal_mag, survey, filt).to_value("electron")
 
         index = entry["btk_index"]
-        gal = galsim_catalog.makeGalaxy(index, gal_type=self.gal_type, noise_pad_size=0)
+        gal = galsim_catalog.makeGalaxy(
+            index, gal_type=self.gal_type, noise_pad_size=self.noise_pad_size
+        )
         gal = gal.withFlux(gal_flux)
         gal = gal.rotate(galsim.Angle(entry["btk_rotation"], unit=galsim.degrees))
         if self.apply_shear:
             if "g1" in entry.keys() and "g2" in entry.keys():
                 gal = gal.shear(g1=entry["g1"], g2=entry["g2"])
             else:
                 raise KeyError("g1 and g2 not found in blend list.")
```

### Comparing `blending_toolkit-1.0.0b6/btk/match.py` & `blending_toolkit-1.0.0b7/btk/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
     """Match based on pixel coordinates using Hungarian matching algorithm."""
 
     def __init__(self, pixel_max_sep=5.0, **kwargs) -> None:
         """Initialize matching class.
 
         Args:
             pixel_max_sep: the maximum separation in pixels to be considered a match
+            kwargs: Additional arguments for parent class.
         """
         super().__init__(**kwargs)
         self.distance_function = pixel_l2_distance_matrix
         self.max_sep = pixel_max_sep
 
     def match_catalogs(self, truth_catalog: Table, predicted_catalog: Table) -> np.ndarray:
         """Performs Hungarian matching algorithm on pixel coordinates from catalogs.
@@ -232,14 +233,15 @@
     """Match based on closest neighbour in the sky."""
 
     def __init__(self, arcsec_max_sep=2.0, **kwargs) -> None:
         """Initialize matching class.
 
         Args:
             arcsec_max_sep: the maximum separation in arcsec to be considered a match
+            kwargs: Additional arguments for parent class.
         """
         super().__init__(**kwargs)
         self.max_sep = arcsec_max_sep
 
     def preprocess_catalog(self, catalog: Table) -> Tuple[np.ndarray, np.ndarray]:
         """Extract ra, dec coordinates out of catalogs."""
         if "ra" not in catalog.colnames or "dec" not in catalog.colnames:
```

### Comparing `blending_toolkit-1.0.0b6/btk/measure.py` & `blending_toolkit-1.0.0b7/btk/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 def get_ksb_ellipticity(
     images: np.ndarray, psf: GSObject, pixel_scale: float, verbose=False
 ) -> np.ndarray:
     """Return ellipticities of both true and detected galaxies, assuming they are matched."""
     # psf is assumed to be the same for the entire batch and correspond to selected band.
-    assert len(images.shape) == 4  # (batch_size, max_n_sources, H, W)
+    assert images.ndim == 4  # (batch_size, max_n_sources, H, W)
     batch_size, max_n_sources, _, _ = images.shape
     ellipticities = np.zeros((batch_size, max_n_sources, 2))
     for ii in range(batch_size):
         for jj in range(max_n_sources):
             if np.sum(images[ii, jj]) > 0:
                 ellipticities[ii, jj] = _get_single_ksb_ellipticity(
                     images[ii, jj], psf, pixel_scale, verbose=verbose
```

### Comparing `blending_toolkit-1.0.0b6/btk/metrics/base.py` & `blending_toolkit-1.0.0b7/btk/metrics/base.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/metrics/detection.py` & `blending_toolkit-1.0.0b7/btk/metrics/detection.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/metrics/reconstruction.py` & `blending_toolkit-1.0.0b7/btk/metrics/reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
             n_sources2 = np.sum(iso_images2[ii].sum(axis=(-1, -2)) > 0).astype(int)
             n_sources = min(n_sources1, n_sources2)  # just in case
             if n_sources > 0:
                 images1 = iso_images1[ii, :n_sources]
                 images2 = iso_images2[ii, :n_sources]
                 mets = metric_func(images1, images2)
                 assert mets.shape == (n_sources,)
-                for ii in range(n_sources):
-                    results.append(mets[ii])
+                for jj in range(n_sources):
+                    results.append(mets[jj])
 
         return np.array(results)
 
     def _get_data(self, iso_images1: np.ndarray, iso_images2: np.ndarray) -> Dict[str, np.ndarray]:
         """Compute reconstruction metric based on isolated or deblended images."""
```

### Comparing `blending_toolkit-1.0.0b6/btk/metrics/segmentation.py` & `blending_toolkit-1.0.0b7/btk/metrics/segmentation.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/metrics/utils.py` & `blending_toolkit-1.0.0b7/btk/metrics/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     is_on = isolated_images.sum(axis=(-1, -2)) > 0
     is_on = is_on[:, :, None, None].repeat(h, axis=2).repeat(w, axis=3)
     seg = isolated_images > sigma_noise * err
     assert is_on.shape == seg.shape
     return np.where(is_on, seg, np.nan)
 
 
-def mse(image1: np.ndarray, image2: np.ndarray) -> np.ndarray:
+def mse(images1: np.ndarray, images2: np.ndarray) -> np.ndarray:
     """Computes mean-squared-error (MSE) between two images.
 
     Args:
         images1: Array of shape `*HW` containing `*` images each of
                         size `*HW`.
         images2: Array of shape `*HW` containing `*` images each of
                         size `*HW`.
 
     Returns:
         Returns MSE between each corresponding iamge as an array of shape `*`.
     """
-    return np.sqrt(np.power((image1 - image2), 2).mean(axis=(-1, -2)))
+    return np.sqrt(np.power((images1 - images2), 2).mean(axis=(-1, -2)))
 
 
 def iou(seg1: np.ndarray, seg2: np.ndarray) -> np.ndarray:
     """Calculates intersection-over-union (IoU) given two semgentation arrays.
 
     The segmentation arrays should each have values of 1 or 0s only.
 
@@ -61,38 +61,38 @@
     seg1 = seg1.astype(bool)
     seg2 = seg1.astype(bool)
     i = np.logical_and(seg1, seg2).sum(axis=(-1, -2))
     u = np.logical_or(seg1, seg2).sum(axis=(-1, -2))
     return i / u
 
 
-def psnr(image1: np.ndarray, image2: np.ndarray) -> np.ndarray:
+def psnr(images1: np.ndarray, images2: np.ndarray) -> np.ndarray:
     """Compute peak-signal-to-noise-ratio from skimage.
 
     Args:
         images1: Array of shape `NHW` containing `N` images each of
                 size `NHW`.
         images2: Array of shape `NHW` containing `N` images each of
                 size `NHW`.
 
     Returns:
         Returns PSNR between each corresponding iamge as an array of shape `N`.
     """
-    n, h, w = image1.shape
-    assert image1.min() >= 0 and image2.min() >= 0
-    assert (n, h, w) == image2.shape
+    n, h, w = images1.shape
+    assert images1.min() >= 0 and images2.min() >= 0
+    assert (n, h, w) == images2.shape
     psnr_ = np.zeros(n)
     for ii in range(n):
-        im1 = image1[ii] / image1[ii].max()
-        im2 = image2[ii] / image2[ii].max()
+        im1 = images1[ii] / images1[ii].max()
+        im2 = images2[ii] / images2[ii].max()
         psnr_[ii] = peak_signal_noise_ratio(im1, im2, data_range=1)
     return psnr_
 
 
-def struct_sim(image1: np.ndarray, image2: np.ndarray, **kwargs) -> np.ndarray:
+def struct_sim(images1: np.ndarray, images2: np.ndarray, **kwargs) -> np.ndarray:
     """Compute structural similarity index from skimage.
 
     By default, we normalize the images to be between 0 and 1. So that the
     `data_range` is 1.
 
     Args:
         images1: Array of shape `NHW` containing `N` images each of
@@ -102,21 +102,21 @@
         kwargs: Keyword arguments to be passed in to `peak_signal_noise_ratio` function
                 within `skimage.metrics`.
 
     Returns:
         Returns structural similarity index between each corresponding iamge as
         an array of shape `N`.
     """
-    assert image1.min() >= 0 and image2.min() >= 0
-    n, h, w = image1.shape
-    assert (n, h, w) == image2.shape
+    assert images1.min() >= 0 and images2.min() >= 0
+    n, h, w = images1.shape
+    assert (n, h, w) == images2.shape
     ssim = np.zeros(n)
     for ii in range(n):
-        im1 = image1[ii] / image1[ii].max()
-        im2 = image2[ii] / image2[ii].max()
+        im1 = images1[ii] / images1[ii].max()
+        im2 = images2[ii] / images2[ii].max()
         ssim[ii] = structural_similarity(im1, im2, data_range=1, **kwargs)
     return ssim
 
 
 def effmat(tp: np.ndarray, t: np.ndarray) -> np.ndarray:
     """Returns efficiency matrices based on number of matched truth and predicted galaxies."""
     n = len(t)  # batch size
```

### Comparing `blending_toolkit-1.0.0b6/btk/multiprocess.py` & `blending_toolkit-1.0.0b7/btk/multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tools for multiprocessing in BTK."""
 
 import multiprocessing as mp
 from itertools import repeat, starmap
-from typing import Callable, Iterable
+from typing import Callable, Iterable, Optional
 
 
 def _apply_args_and_kwargs(func: Callable, args, kwargs):
     return func(*args, **kwargs)
 
 
 def _pool_starmap_with_kwargs(pool, func: Callable, args_iter: Iterable, kwargs_iter: Iterable):
@@ -25,15 +25,15 @@
         return "main"
     return mp.current_process().ident
 
 
 def multiprocess(
     func: Callable,
     args_iter: Iterable,
-    kwargs_iter: Iterable = None,
+    kwargs_iter: Optional[Iterable] = None,
     njobs: int = 1,
     verbose: bool = False,
 ):
     """Sole function that implements multiprocessing across mini-batches/batches for BTK.
 
     Args:
         func: Function to run in parallel on each positional arguments returned by
```

### Comparing `blending_toolkit-1.0.0b6/btk/plotting.py` & `blending_toolkit-1.0.0b7/btk/plotting.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/btk/sampling_functions.py` & `blending_toolkit-1.0.0b7/btk/sampling_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             max_mag: Maximum magnitude allowed in samples.
             mag_name: Name of the magnitude column in the catalog.
         """
         super().__init__(max_number=max_number, min_number=min_number, seed=seed)
         self.stamp_size = stamp_size
         self.min_mag, self.max_mag = min_mag, max_mag
         self.mag_name = mag_name
-        self.max_shift = self.stamp_size / 2 if not max_shift else max_shift
+        self.max_shift = max_shift if max_shift else self.stamp_size / 2
 
         # only within area where sources are allowed
         self.exp_count = density * (self.max_shift * 2 / 60) ** 2
 
     def __call__(self, table: Table) -> Table:
         """Applies default sampling to catalog.
```

### Comparing `blending_toolkit-1.0.0b6/btk/survey.py` & `blending_toolkit-1.0.0b7/btk/survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     @classmethod
     def from_galcheat_filter(cls, galcheat_filter: galcheat.filter.Filter):
         """Return the corresponding BTK Filter from the Galcheat Filter."""
         return cls(**vars(galcheat_filter))
 
 
 def get_surveys(
-    names: Union[str, List[str]], psf_func: Callable = None
+    names: Union[str, List[str]], psf_func: Optional[Callable] = None
 ) -> Union[Survey, List[Survey]]:
     """Return specified surveys from galcheat extended to contain PSF information.
 
     This function currently returns a list of `Survey` instances if `names` is a list with more
     than one element. If `names` is a str or a singleton list then we return a single `Survey`.
 
     Args:
@@ -201,20 +201,19 @@
     if len(psf_files) > 1:
         psf_file = rd.choice(psf_files)
     elif len(psf_files) == 1:
         psf_file = psf_files[0]
     else:
         raise RuntimeError(f"No psf files found in '{psf_dir}'.")
     psf_array = fits.getdata(psf_dir + "/" + psf_file)
-    psf_model = galsim.InterpolatedImage(
+
+    return galsim.InterpolatedImage(
         galsim.Image(psf_array), scale=survey.pixel_scale.to_value("arcsec")
     ).withFlux(1.0)
 
-    return psf_model
-
 
 def make_wcs(
     pixel_scale: float,
     shape: Tuple[int, int],
     projection: str = "TAN",
     center_pix: Optional[Tuple[int, int]] = None,
     center_sky: Optional[Tuple[int, int]] = None,
```

### Comparing `blending_toolkit-1.0.0b6/btk/utils.py` & `blending_toolkit-1.0.0b7/btk/utils.py`

 * *Files identical despite different names*

### Comparing `blending_toolkit-1.0.0b6/PKG-INFO` & `blending_toolkit-1.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blending_toolkit
-Version: 1.0.0b6
+Version: 1.0.0b7
 Summary: Blending ToolKit
 Home-page: https://lsstdesc.org/BlendingToolKit/index.html
 License: MIT
 Keywords: cosmology,galaxies,blending,lsst,simulation
 Author: Ismael Mendoza
 Author-email: imendoza@umich.edu
 Requires-Python: >=3.8.1,<3.12
@@ -18,15 +18,15 @@
 Requires-Dist: astropy (>=5.1)
 Requires-Dist: fast3tree (>=0.4.1,<0.5.0)
 Requires-Dist: galcheat (>=1.0.0,<2.0.0)
 Requires-Dist: galsim (>=2.4.9)
 Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: numpy (>=1.22)
-Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
+Requires-Dist: ruff (>=0.3.2,<0.4.0)
 Requires-Dist: scikit-image (>=0.20.0)
 Requires-Dist: scipy (>=1.9.1)
 Requires-Dist: sep (>=1.2.1)
 Requires-Dist: tqdm (>=4.65.0)
 Project-URL: Bug Tracker, https://github.com/LSSTDESC/BlendingToolKit/issues
 Project-URL: Repository, https://github.com/LSSTDESC/BlendingToolKit
 Description-Content-Type: text/markdown
@@ -115,15 +115,15 @@
 ```
 
 ## Installation
 
 BTK is pip installable, with the following command:
 
 ```bash
-pip install blending-toolkit==1.0.0b6
+pip install blending-toolkit==1.0.0b7
 ```
 
 In case of any issues and for details of required packages, please see the more detailed installation instructions [here](https://lsstdesc.org/BlendingToolKit/install.html).
 
 ## Contributing
 
 Everyone can contribute to this project, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) document for details.
```

