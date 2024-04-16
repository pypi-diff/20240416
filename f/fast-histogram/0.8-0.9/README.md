# Comparing `tmp/fast-histogram-0.8.tar.gz` & `tmp/fast-histogram-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmppvdprbuw/tmpf43sjm53/fast-histogram-0.8.tar", last modified: Tue Jan  7 17:08:11 2020, max compression
+gzip compressed data, was "/tmp/tmpa4lualsk/tmp8eom5y7a/fast-histogram-0.9.tar", last modified: Sun May 24 20:52:50 2020, max compression
```

## Comparing `fast-histogram-0.8.tar` & `fast-histogram-0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:11.000000 fast-histogram-0.8/
--rw-r--r--   0 vsts      (1001) docker     (117)      791 2020-01-07 17:08:00.000000 fast-histogram-0.8/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (117)     1322 2020-01-07 17:08:00.000000 fast-histogram-0.8/CHANGES.rst
--rw-r--r--   0 vsts      (1001) docker     (117)     1299 2020-01-07 17:08:00.000000 fast-histogram-0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (117)       78 2020-01-07 17:08:00.000000 fast-histogram-0.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (117)     7852 2020-01-07 17:08:11.000000 fast-histogram-0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)     6262 2020-01-07 17:08:00.000000 fast-histogram-0.8/README.rst
--rw-r--r--   0 vsts      (1001) docker     (117)     1508 2020-01-07 17:08:00.000000 fast-histogram-0.8/azure-pipelines.yml
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:11.000000 fast-histogram-0.8/comparison/
--rw-r--r--   0 vsts      (1001) docker     (117)      244 2020-01-07 17:08:00.000000 fast-histogram-0.8/comparison/README.rst
--rw-r--r--   0 vsts      (1001) docker     (117)     2569 2020-01-07 17:08:00.000000 fast-histogram-0.8/comparison/benchmark.py
--rw-r--r--   0 vsts      (1001) docker     (117)      761 2020-01-07 17:08:00.000000 fast-histogram-0.8/comparison/plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:11.000000 fast-histogram-0.8/fast_histogram/
--rw-r--r--   0 vsts      (1001) docker     (117)       69 2020-01-07 17:08:00.000000 fast-histogram-0.8/fast_histogram/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)    18431 2020-01-07 17:08:00.000000 fast-histogram-0.8/fast_histogram/_histogram_core.c
--rw-r--r--   0 vsts      (1001) docker     (117)     3213 2020-01-07 17:08:00.000000 fast-histogram-0.8/fast_histogram/histogram.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:11.000000 fast-histogram-0.8/fast_histogram/tests/
--rw-r--r--   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:00.000000 fast-histogram-0.8/fast_histogram/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (117)     6478 2020-01-07 17:08:00.000000 fast-histogram-0.8/fast_histogram/tests/test_histogram.py
--rw-r--r--   0 vsts      (1001) docker     (117)      114 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (117)        0 2020-01-07 17:08:11.000000 fast-histogram-0.8/fast_histogram.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (117)     7852 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (117)      613 2020-01-07 17:08:11.000000 fast-histogram-0.8/fast_histogram.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (117)        1 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (117)       50 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (117)       15 2020-01-07 17:08:09.000000 fast-histogram-0.8/fast_histogram.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (117)      170 2020-01-07 17:08:00.000000 fast-histogram-0.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (117)      492 2020-01-07 17:08:11.000000 fast-histogram-0.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (117)      428 2020-01-07 17:08:00.000000 fast-histogram-0.8/setup.py
--rw-r--r--   0 vsts      (1001) docker     (117)    26102 2020-01-07 17:08:00.000000 fast-histogram-0.8/speedup_compared.png
--rw-r--r--   0 vsts      (1001) docker     (117)      893 2020-01-07 17:08:00.000000 fast-histogram-0.8/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:50.000000 fast-histogram-0.9/
+-rw-r--r--   0 vsts      (1001) docker     (118)      791 2020-05-24 20:52:36.000000 fast-histogram-0.9/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (118)     1550 2020-05-24 20:52:36.000000 fast-histogram-0.9/CHANGES.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     1299 2020-05-24 20:52:36.000000 fast-histogram-0.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (118)       78 2020-05-24 20:52:36.000000 fast-histogram-0.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (118)     7852 2020-05-24 20:52:50.000000 fast-histogram-0.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)     6262 2020-05-24 20:52:36.000000 fast-histogram-0.9/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     1508 2020-05-24 20:52:36.000000 fast-histogram-0.9/azure-pipelines.yml
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:50.000000 fast-histogram-0.9/comparison/
+-rw-r--r--   0 vsts      (1001) docker     (118)      244 2020-05-24 20:52:36.000000 fast-histogram-0.9/comparison/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (118)     2569 2020-05-24 20:52:36.000000 fast-histogram-0.9/comparison/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      761 2020-05-24 20:52:36.000000 fast-histogram-0.9/comparison/plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:50.000000 fast-histogram-0.9/fast_histogram/
+-rw-r--r--   0 vsts      (1001) docker     (118)       69 2020-05-24 20:52:36.000000 fast-histogram-0.9/fast_histogram/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    18595 2020-05-24 20:52:36.000000 fast-histogram-0.9/fast_histogram/_histogram_core.c
+-rw-r--r--   0 vsts      (1001) docker     (118)     3213 2020-05-24 20:52:36.000000 fast-histogram-0.9/fast_histogram/histogram.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:50.000000 fast-histogram-0.9/fast_histogram/tests/
+-rw-r--r--   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:36.000000 fast-histogram-0.9/fast_histogram/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (118)     7720 2020-05-24 20:52:36.000000 fast-histogram-0.9/fast_histogram/tests/test_histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (118)      114 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram/version.py
+drwxr-xr-x   0 vsts      (1001) docker     (118)        0 2020-05-24 20:52:50.000000 fast-histogram-0.9/fast_histogram.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (118)     7852 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (118)      613 2020-05-24 20:52:50.000000 fast-histogram-0.9/fast_histogram.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)        1 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (118)       50 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)       15 2020-05-24 20:52:49.000000 fast-histogram-0.9/fast_histogram.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (118)      170 2020-05-24 20:52:36.000000 fast-histogram-0.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (118)      492 2020-05-24 20:52:50.000000 fast-histogram-0.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (118)      428 2020-05-24 20:52:36.000000 fast-histogram-0.9/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (118)    26102 2020-05-24 20:52:36.000000 fast-histogram-0.9/speedup_compared.png
+-rw-r--r--   0 vsts      (1001) docker     (118)      893 2020-05-24 20:52:36.000000 fast-histogram-0.9/tox.ini
```

### Comparing `fast-histogram-0.8/.gitignore` & `fast-histogram-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/CHANGES.rst` & `fast-histogram-0.9/CHANGES.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+0.9 (2020-05-24)
+----------------
+
+- Fixed a bug that caused incorrect results in the weighted
+  1-d histogram and the weighted and unweighted 2-d histogram
+  functions if using arrays with different layouts in memory.
+  [#52]
+
 0.8 (2020-01-07)
 ----------------
 
 - Fixed compatibility of test suite with latest version of the
   hypothesis package. [#40]
 
 0.7 (2019-01-09)
```

### Comparing `fast-histogram-0.8/LICENSE` & `fast-histogram-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/PKG-INFO` & `fast-histogram-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-histogram
-Version: 0.8
+Version: 0.9
 Summary: Fast simple 1D and 2D histograms
 Home-page: https://github.com/astrofrog/fast-histogram
 Author: Thomas Robitaille
 Author-email: thomas.robitaille@gmail.com
 License: BSD
 Description: |Azure Status| |asv|
```

### Comparing `fast-histogram-0.8/README.rst` & `fast-histogram-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/azure-pipelines.yml` & `fast-histogram-0.9/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/comparison/benchmark.py` & `fast-histogram-0.9/comparison/benchmark.py`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/comparison/plot.py` & `fast-histogram-0.9/comparison/plot.py`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/fast_histogram/_histogram_core.c` & `fast-histogram-0.9/fast_histogram/_histogram_core.c`

 * *Files 2% similar despite different names*

```diff
@@ -298,31 +298,32 @@
   count = (double *)PyArray_DATA(count_array);
 
   Py_BEGIN_ALLOW_THREADS
 
   do {
 
     /* Get the inner loop data/stride/count values */
-    npy_intp stride = *strideptr;
+    npy_intp stride0 = strideptr[0];
+    npy_intp stride1 = strideptr[1];
     npy_intp size = *innersizeptr;
 
     /* This is a typical inner loop for NPY_ITER_EXTERNAL_LOOP */
     while (size--) {
 
       tx = *(double *)dataptr[0];
       ty = *(double *)dataptr[1];
 
       if (tx >= xmin && tx < xmax && ty >= ymin && ty < ymax) {
         ix = (tx - xmin) * normx * fnx;
         iy = (ty - ymin) * normy * fny;
         count[iy + ny * ix] += 1.;
       }
 
-      dataptr[0] += stride;
-      dataptr[1] += stride;
+      dataptr[0] += stride0;
+      dataptr[1] += stride1;
     }
 
   } while (iternext(iter));
 
   Py_END_ALLOW_THREADS
 
   NpyIter_Deallocate(iter);
@@ -447,30 +448,31 @@
   count = (double *)PyArray_DATA(count_array);
 
   Py_BEGIN_ALLOW_THREADS
 
   do {
 
     /* Get the inner loop data/stride/count values */
-    npy_intp stride = *strideptr;
+    npy_intp stride0 = strideptr[0];
+    npy_intp stride1 = strideptr[1];
     npy_intp size = *innersizeptr;
 
     /* This is a typical inner loop for NPY_ITER_EXTERNAL_LOOP */
     while (size--) {
 
       tx = *(double *)dataptr[0];
       tw = *(double *)dataptr[1];
 
       if (tx >= xmin && tx < xmax) {
         ix = (tx - xmin) * normx * fnx;
         count[ix] += tw;
       }
 
-      dataptr[0] += stride;
-      dataptr[1] += stride;
+      dataptr[0] += stride0;
+      dataptr[1] += stride1;
     }
 
   } while (iternext(iter));
 
   Py_END_ALLOW_THREADS
 
   NpyIter_Deallocate(iter);
@@ -606,15 +608,17 @@
   count = (double *)PyArray_DATA(count_array);
 
   Py_BEGIN_ALLOW_THREADS
 
   do {
 
     /* Get the inner loop data/stride/count values */
-    npy_intp stride = *strideptr;
+    npy_intp stride0 = strideptr[0];
+    npy_intp stride1 = strideptr[1];
+    npy_intp stride2 = strideptr[2];
     npy_intp size = *innersizeptr;
 
     /* This is a typical inner loop for NPY_ITER_EXTERNAL_LOOP */
     while (size--) {
 
       tx = *(double *)dataptr[0];
       ty = *(double *)dataptr[1];
@@ -622,17 +626,17 @@
 
       if (tx >= xmin && tx < xmax && ty >= ymin && ty < ymax) {
         ix = (tx - xmin) * normx * fnx;
         iy = (ty - ymin) * normy * fny;
         count[iy + ny * ix] += tw;
       }
 
-      dataptr[0] += stride;
-      dataptr[1] += stride;
-      dataptr[2] += stride;
+      dataptr[0] += stride0;
+      dataptr[1] += stride1;
+      dataptr[2] += stride2;
     }
 
   } while (iternext(iter));
 
   Py_END_ALLOW_THREADS
 
   NpyIter_Deallocate(iter);
```

### Comparing `fast-histogram-0.8/fast_histogram/histogram.py` & `fast-histogram-0.9/fast_histogram/histogram.py`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/fast_histogram/tests/test_histogram.py` & `fast-histogram-0.9/fast_histogram/tests/test_histogram.py`

 * *Files 13% similar despite different names*

```diff
@@ -197,7 +197,36 @@
         histogram1d([1, 2, 3], bins=edges, range=(0, 10))
     assert exc.value.args[0] == 'bins should be an integer'
 
     with pytest.raises(TypeError) as exc:
         histogram2d([1, 2, 3], [1, 2 ,3], bins=[edges, edges],
                     range=[(0, 10), (0, 10)])
     assert exc.value.args[0] == 'bins should be an iterable of two integers'
+
+
+def test_mixed_strides():
+
+    # Make sure all functions work properly when passed arrays with mismatched
+    # strides.
+
+    x = np.random.random((30, 20, 40, 50))[:, 10, :, 20]
+    y = np.random.random((30, 40, 50))[:, :, 10]
+    z = np.random.random((30, 10, 5, 80, 90))[:, 5, 2, ::2, 22]
+
+    assert x.shape == y.shape and x.shape == z.shape
+    assert x.strides != y.strides and y.strides != z.strides and z.strides != x.strides
+
+    result_1 = histogram1d(x, bins=10, range=(0, 1))
+    result_2, _ = np.histogram(x, bins=10, range=(0, 1))
+    np.testing.assert_equal(result_1, result_2)
+
+    result_3 = histogram1d(x, weights=y, bins=10, range=(0, 1))
+    result_4, _ = np.histogram(x, weights=y, bins=10, range=(0, 1))
+    np.testing.assert_equal(result_3, result_4)
+
+    result_5 = histogram2d(x, y, bins=(10, 10), range=[(0, 1), (0, 1)])
+    result_6, _, _ = np.histogram2d(x.ravel(), y.ravel(), bins=(10, 10), range=[(0, 1), (0, 1)])
+    np.testing.assert_equal(result_5, result_6)
+
+    result_7 = histogram2d(x, y, weights=z, bins=(10, 10), range=[(0, 1), (0, 1)])
+    result_8, _, _ = np.histogram2d(x.ravel(), y.ravel(), weights=z.ravel(), bins=(10, 10), range=[(0, 1), (0, 1)])
+    np.testing.assert_equal(result_7, result_8)
```

### Comparing `fast-histogram-0.8/fast_histogram.egg-info/PKG-INFO` & `fast-histogram-0.9/fast_histogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-histogram
-Version: 0.8
+Version: 0.9
 Summary: Fast simple 1D and 2D histograms
 Home-page: https://github.com/astrofrog/fast-histogram
 Author: Thomas Robitaille
 Author-email: thomas.robitaille@gmail.com
 License: BSD
 Description: |Azure Status| |asv|
```

### Comparing `fast-histogram-0.8/fast_histogram.egg-info/SOURCES.txt` & `fast-histogram-0.9/fast_histogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/speedup_compared.png` & `fast-histogram-0.9/speedup_compared.png`

 * *Files identical despite different names*

### Comparing `fast-histogram-0.8/tox.ini` & `fast-histogram-0.9/tox.ini`

 * *Files identical despite different names*

