# Comparing `tmp/mogptk-0.5.1.tar.gz` & `tmp/mogptk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mogptk-0.5.1.tar", last modified: Mon Dec 11 20:27:56 2023, max compression
+gzip compressed data, was "mogptk-0.5.2.tar", last modified: Tue Apr 16 15:42:57 2024, max compression
```

## Comparing `mogptk-0.5.1.tar` & `mogptk-0.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.327190 mogptk-0.5.1/
--rw-r--r--   0 taco      (1000) users      (100)      147 2023-12-11 20:08:53.000000 mogptk-0.5.1/.gitignore
--rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.5.1/LICENSE
--rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.5.1/MANIFEST.in
--rw-r--r--   0 taco      (1000) users      (100)    11267 2023-12-11 20:27:56.327190 mogptk-0.5.1/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)    10679 2023-05-03 14:36:55.000000 mogptk-0.5.1/README.md
--rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.5.1/config.mako
--rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.5.1/head.mako
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.320524 mogptk-0.5.1/mogptk/
--rw-r--r--   0 taco      (1000) users      (100)      401 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)    57502 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/data.py
--rw-r--r--   0 taco      (1000) users      (100)    30577 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/dataset.py
--rw-r--r--   0 taco      (1000) users      (100)     9820 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/documentation.md
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.327190 mogptk-0.5.1/mogptk/gpr/
--rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.5.1/mogptk/gpr/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     2740 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/gpr/config.py
--rw-r--r--   0 taco      (1000) users      (100)    18330 2023-12-11 20:18:13.000000 mogptk-0.5.1/mogptk/gpr/kernel.py
--rw-r--r--   0 taco      (1000) users      (100)    30679 2023-12-11 20:17:55.000000 mogptk-0.5.1/mogptk/gpr/likelihood.py
--rw-r--r--   0 taco      (1000) users      (100)     4714 2023-12-11 20:17:57.000000 mogptk-0.5.1/mogptk/gpr/mean.py
--rw-r--r--   0 taco      (1000) users      (100)    38145 2023-12-11 16:53:38.000000 mogptk-0.5.1/mogptk/gpr/model.py
--rw-r--r--   0 taco      (1000) users      (100)    29726 2023-12-11 20:18:36.000000 mogptk-0.5.1/mogptk/gpr/multioutput.py
--rw-r--r--   0 taco      (1000) users      (100)    12874 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/gpr/parameter.py
--rw-r--r--   0 taco      (1000) users      (100)     1209 2023-03-22 02:14:00.000000 mogptk-0.5.1/mogptk/gpr/plot.py
--rw-r--r--   0 taco      (1000) users      (100)    28808 2023-12-07 23:27:39.000000 mogptk-0.5.1/mogptk/gpr/singleoutput.py
--rw-r--r--   0 taco      (1000) users      (100)     1719 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/gpr/util.py
--rw-r--r--   0 taco      (1000) users      (100)     5755 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/init.py
--rw-r--r--   0 taco      (1000) users      (100)    43453 2023-12-11 16:16:17.000000 mogptk-0.5.1/mogptk/model.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.327190 mogptk-0.5.1/mogptk/models/
--rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.5.1/mogptk/models/__init__.py
--rw-r--r--   0 taco      (1000) users      (100)     4694 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/conv.py
--rw-r--r--   0 taco      (1000) users      (100)     5172 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/csm.py
--rw-r--r--   0 taco      (1000) users      (100)     7223 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/mohsm.py
--rw-r--r--   0 taco      (1000) users      (100)    12145 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/mosm.py
--rw-r--r--   0 taco      (1000) users      (100)     7578 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/sm.py
--rw-r--r--   0 taco      (1000) users      (100)     5606 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/models/sm_lmc.py
--rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.5.1/mogptk/transformer.py
--rw-r--r--   0 taco      (1000) users      (100)    10263 2023-12-10 02:44:05.000000 mogptk-0.5.1/mogptk/util.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.320524 mogptk-0.5.1/mogptk.egg-info/
--rw-r--r--   0 taco      (1000) users      (100)    11267 2023-12-11 20:27:56.000000 mogptk-0.5.1/mogptk.egg-info/PKG-INFO
--rw-r--r--   0 taco      (1000) users      (100)      790 2023-12-11 20:27:56.000000 mogptk-0.5.1/mogptk.egg-info/SOURCES.txt
--rw-r--r--   0 taco      (1000) users      (100)        1 2023-12-11 20:27:56.000000 mogptk-0.5.1/mogptk.egg-info/dependency_links.txt
--rw-r--r--   0 taco      (1000) users      (100)       82 2023-12-11 20:27:56.000000 mogptk-0.5.1/mogptk.egg-info/requires.txt
--rw-r--r--   0 taco      (1000) users      (100)        7 2023-12-11 20:27:56.000000 mogptk-0.5.1/mogptk.egg-info/top_level.txt
--rw-r--r--   0 taco      (1000) users      (100)       79 2023-12-11 20:27:56.330524 mogptk-0.5.1/setup.cfg
--rw-r--r--   0 taco      (1000) users      (100)      959 2023-12-11 20:27:34.000000 mogptk-0.5.1/setup.py
-drwxr-xr-x   0 taco      (1000) users      (100)        0 2023-12-11 20:27:56.327190 mogptk-0.5.1/tests/
--rw-r--r--   0 taco      (1000) users      (100)      726 2023-12-11 16:05:50.000000 mogptk-0.5.1/tests/test.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.334572 mogptk-0.5.2/
+-rw-r--r--   0 taco      (1000) users      (100)      147 2023-12-11 20:08:53.000000 mogptk-0.5.2/.gitignore
+-rw-r--r--   0 taco      (1000) users      (100)     1052 2019-08-30 20:58:49.000000 mogptk-0.5.2/LICENSE
+-rw-r--r--   0 taco      (1000) users      (100)       26 2022-04-24 02:23:55.000000 mogptk-0.5.2/MANIFEST.in
+-rw-r--r--   0 taco      (1000) users      (100)    11267 2024-04-16 15:42:57.334572 mogptk-0.5.2/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)    10679 2023-05-03 14:36:55.000000 mogptk-0.5.2/README.md
+-rw-r--r--   0 taco      (1000) users      (100)     2101 2020-02-07 16:46:12.000000 mogptk-0.5.2/config.mako
+-rw-r--r--   0 taco      (1000) users      (100)       66 2020-02-06 15:45:19.000000 mogptk-0.5.2/head.mako
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.327905 mogptk-0.5.2/mogptk/
+-rw-r--r--   0 taco      (1000) users      (100)      401 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)    58153 2024-04-16 15:39:17.000000 mogptk-0.5.2/mogptk/data.py
+-rw-r--r--   0 taco      (1000) users      (100)    30489 2024-03-28 17:38:57.000000 mogptk-0.5.2/mogptk/dataset.py
+-rw-r--r--   0 taco      (1000) users      (100)     9820 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/documentation.md
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.331239 mogptk-0.5.2/mogptk/gpr/
+-rw-r--r--   0 taco      (1000) users      (100)      260 2022-04-20 16:31:55.000000 mogptk-0.5.2/mogptk/gpr/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     2726 2024-01-25 01:33:06.000000 mogptk-0.5.2/mogptk/gpr/config.py
+-rw-r--r--   0 taco      (1000) users      (100)    18330 2023-12-11 20:18:13.000000 mogptk-0.5.2/mogptk/gpr/kernel.py
+-rw-r--r--   0 taco      (1000) users      (100)    30679 2023-12-11 20:17:55.000000 mogptk-0.5.2/mogptk/gpr/likelihood.py
+-rw-r--r--   0 taco      (1000) users      (100)     4714 2023-12-11 20:17:57.000000 mogptk-0.5.2/mogptk/gpr/mean.py
+-rw-r--r--   0 taco      (1000) users      (100)    38190 2023-12-20 11:35:24.000000 mogptk-0.5.2/mogptk/gpr/model.py
+-rw-r--r--   0 taco      (1000) users      (100)    29726 2023-12-11 20:18:36.000000 mogptk-0.5.2/mogptk/gpr/multioutput.py
+-rw-r--r--   0 taco      (1000) users      (100)    12874 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/gpr/parameter.py
+-rw-r--r--   0 taco      (1000) users      (100)     1209 2023-03-22 02:14:00.000000 mogptk-0.5.2/mogptk/gpr/plot.py
+-rw-r--r--   0 taco      (1000) users      (100)    28808 2023-12-07 23:27:39.000000 mogptk-0.5.2/mogptk/gpr/singleoutput.py
+-rw-r--r--   0 taco      (1000) users      (100)     1719 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/gpr/util.py
+-rw-r--r--   0 taco      (1000) users      (100)     5755 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/init.py
+-rw-r--r--   0 taco      (1000) users      (100)    43453 2023-12-11 16:16:17.000000 mogptk-0.5.2/mogptk/model.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.331239 mogptk-0.5.2/mogptk/models/
+-rw-r--r--   0 taco      (1000) users      (100)        0 2022-03-01 22:37:51.000000 mogptk-0.5.2/mogptk/models/__init__.py
+-rw-r--r--   0 taco      (1000) users      (100)     4694 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/conv.py
+-rw-r--r--   0 taco      (1000) users      (100)     5172 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/csm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7223 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/mohsm.py
+-rw-r--r--   0 taco      (1000) users      (100)    12145 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/mosm.py
+-rw-r--r--   0 taco      (1000) users      (100)     7578 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/sm.py
+-rw-r--r--   0 taco      (1000) users      (100)     5606 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/models/sm_lmc.py
+-rw-r--r--   0 taco      (1000) users      (100)     4715 2022-05-25 17:06:55.000000 mogptk-0.5.2/mogptk/transformer.py
+-rw-r--r--   0 taco      (1000) users      (100)    10263 2023-12-10 02:44:05.000000 mogptk-0.5.2/mogptk/util.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.327905 mogptk-0.5.2/mogptk.egg-info/
+-rw-r--r--   0 taco      (1000) users      (100)    11267 2024-04-16 15:42:57.000000 mogptk-0.5.2/mogptk.egg-info/PKG-INFO
+-rw-r--r--   0 taco      (1000) users      (100)      790 2024-04-16 15:42:57.000000 mogptk-0.5.2/mogptk.egg-info/SOURCES.txt
+-rw-r--r--   0 taco      (1000) users      (100)        1 2024-04-16 15:42:57.000000 mogptk-0.5.2/mogptk.egg-info/dependency_links.txt
+-rw-r--r--   0 taco      (1000) users      (100)       82 2024-04-16 15:42:57.000000 mogptk-0.5.2/mogptk.egg-info/requires.txt
+-rw-r--r--   0 taco      (1000) users      (100)        7 2024-04-16 15:42:57.000000 mogptk-0.5.2/mogptk.egg-info/top_level.txt
+-rw-r--r--   0 taco      (1000) users      (100)       79 2024-04-16 15:42:57.334572 mogptk-0.5.2/setup.cfg
+-rw-r--r--   0 taco      (1000) users      (100)      959 2024-04-16 15:42:53.000000 mogptk-0.5.2/setup.py
+drwxr-xr-x   0 taco      (1000) users      (100)        0 2024-04-16 15:42:57.331239 mogptk-0.5.2/tests/
+-rw-r--r--   0 taco      (1000) users      (100)       65 2024-01-25 01:33:30.000000 mogptk-0.5.2/tests/test.py
```

### Comparing `mogptk-0.5.1/LICENSE` & `mogptk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/PKG-INFO` & `mogptk-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.5.1
+Version: 0.5.2
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
```

### Comparing `mogptk-0.5.1/README.md` & `mogptk-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/config.mako` & `mogptk-0.5.2/config.mako`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/data.py` & `mogptk-0.5.2/mogptk/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,16 +480,16 @@
             dim (int): Input dimension to apply to, if not specified applies to all input dimensions.
 
         Examples:
             >>> data.filter(3, 8)
         
             >>> data.filter('2016-01-15', '2016-06-15')
         """
-        start = self._normalize_x_val(start)
-        end = self._normalize_x_val(end)
+        start = self._normalize_x_val(start, dim=dim)
+        end = self._normalize_x_val(end, dim=dim)
         
         if dim is not None:
             ind = np.logical_and(self.X[:,dim] >= start[dim], self.X[:,dim] < end[dim])
         else:
             ind = np.logical_and(self.X[:,0] >= start[0], self.X[:,0] < end[0])
             for i in range(1,self.get_input_dims()):
                 ind = np.logical_and(ind, np.logical_and(self.X[:,i] >= start[i], self.X[:,i] < end[i]))
@@ -741,20 +741,26 @@
             >>> data = mogptk.LoadFunction(lambda x: np.sin(3*x[:,0]), 0, 10, n=200, var=0.1, name='Sine wave')
             >>> data.remove_range(3, 8)
         
             >>> data = mogptk.LoadCSV('gold.csv', 'Date', 'Price')
             >>> data.remove_range('2016-01-15', '2016-06-15')
         """
         if start is None:
-            start = [np.min(self.X[:,i]) for i in range(self.get_input_dims())]
+            if dim is None:
+                start = [np.min(self.X[:,i]) for i in range(self.get_input_dims())]
+            else:
+                start = [np.min(self.X[:,i]) if i == dim else None for i in range(self.get_input_dims())]
         if end is None:
-            end = [np.max(self.X[:,i]) for i in range(self.get_input_dims())]
+            if dim is None:
+                end = [np.max(self.X[:,i]) for i in range(self.get_input_dims())]
+            else:
+                end = [np.max(self.X[:,i]) if i == dim else None for i in range(self.get_input_dims())]
 
-        start = self._normalize_x_val(start)
-        end = self._normalize_x_val(end)
+        start = self._normalize_x_val(start, dim=dim)
+        end = self._normalize_x_val(end, dim=dim)
 
         if dim is not None:
             mask = np.logical_and(self.X[:,dim] >= start[dim], self.X[:,dim] <= end[dim])
             self._add_range(start[dim], end[dim], dim)
         else:
             mask = np.logical_and(self.X[:,0] >= start[0], self.X[:,0] <= end[0])
             for i in range(1,self.get_input_dims()):
@@ -768,16 +774,16 @@
         Removes observations between `start` and `end` as a percentage of the number of observations. So `0` is the first observation, `0.5` is the middle observation, and `1` is the last observation.
 
         Args:
             start (float): Start percentage in interval [0,1].
             end (float): End percentage in interval [0,1].
             dim (int): Input dimension to apply to, if not specified applies to all input dimensions.
         """
-        start = self._normalize_x_val(start)
-        end = self._normalize_x_val(end)
+        start = self._normalize_x_val(start, dim=dim)
+        end = self._normalize_x_val(end, dim=dim)
 
         xmin = [np.min(self.X[:,i]) for i in range(self.get_input_dims())]
         xmax = [np.max(self.X[:,i]) for i in range(self.get_input_dims())]
         for i in range(self.get_input_dims()):
             start[i] = xmin[i] + max(0.0, min(1.0, start[i])) * (xmax[i]-xmin[i])
             end[i] = xmin[i] + max(0.0, min(1.0, end[i])) * (xmax[i]-xmin[i])
         self.remove_range(start, end, dim)
@@ -1285,22 +1291,29 @@
             val = list(val)
         else:
             val = [val] * self.get_input_dims()
         if len(val) != self.get_input_dims():
             raise ValueError("value must be a scalar or a list of values for each input dimension")
         return val
 
-    def _normalize_x_val(self, val):
+    def _normalize_x_val(self, val, dim=None):
         # normalize input values for X axis, that is: expand to input_dims if a single value, convert values to appropriate dtype
+
         val = self._normalize_val(val)
-        for i in range(self.get_input_dims()):
+        if dim is not None:
             try:
-                val[i] = np.array(val[i]).astype(self.X_dtypes[i]).astype(np.float64)
+                val[dim] = np.array(val[dim]).astype(self.X_dtypes[dim]).astype(np.float64)
             except:
-                raise ValueError("value must be of type %s" % (self.X_dtypes[i],))
+                raise ValueError("value must be of type %s" % (self.X_dtypes[dim],))
+        else:
+            for i in range(self.get_input_dims()):
+                try:
+                    val[i] = np.array(val[i]).astype(self.X_dtypes[i]).astype(np.float64)
+                except:
+                    raise ValueError("value must be of type %s" % (self.X_dtypes[i],))
         return val
 
 def _is_iterable(val):
     return isinstance(val, collections.abc.Iterable) and not isinstance(val, (dict, str))
 
 def _is_homogeneous_type(seq):
     it = iter(seq)
```

### Comparing `mogptk-0.5.1/mogptk/dataset.py` & `mogptk-0.5.2/mogptk/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,36 +96,32 @@
     cols = x_col + y_col
     if y_err_col is not None:
         cols += y_err_col
     df = df[cols]
     if len(df.index) == 0:
         raise ValueError("dataframe cannot be empty")
 
-    input_dims = len(x_col)
-    x_data = df[x_col]
-    x_labels = [str(item) for item in x_col]
-
     dataset = DataSet()
     for i in range(len(y_col)):
         cols = x_col + [y_col[i]]
         if y_err_col is not None:
             cols += [y_err_col[i]]
         channel = df[cols].dropna()
 
         y_err = None
         if y_err_col is not None:
             y_err = channel[y_err_col[i]].values
 
         dataset.append(Data(
-            channel[x_col].values,
+            [channel[col].values for col in x_col],
             channel[y_col[i]].values,
             Y_err=y_err,
             name=name[i],
-            x_labels=x_labels,
-            y_label=str(y_col[i]),
+            x_labels=x_col,
+            y_label=y_col[i],
         ))
     if dataset.get_output_dims() == 1:
         return dataset[0]
     return dataset
 
 ################################################################
 ################################################################
```

### Comparing `mogptk-0.5.1/mogptk/documentation.md` & `mogptk-0.5.2/mogptk/documentation.md`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/config.py` & `mogptk-0.5.2/mogptk/gpr/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         config.device = torch.device('cpu', n)
 
 def use_gpu(n=None):
     """
     Use the GPU instead of the CPU for tensor calculations. This is the default if a GPU is available. If you have more than one GPU, you can use a specific GPU by setting `n`.
     """
     if not torch.cuda.is_available():
-        logger.error("CUDA is not available")
+        print("CUDA is not available")
     elif n is not None and (not isinstance(n, int) or n < 0 or torch.cuda.device_count() <= n):
-        logger.error("CUDA GPU '%s' is not available" % (n,))
+        print("CUDA GPU '%s' is not available" % (n,))
     elif n is None:
         config.device = torch.device('cuda', torch.cuda.current_device())
     else:
         config.device = torch.device('cuda', n)
 
 def print_gpu_information():
     """
```

### Comparing `mogptk-0.5.1/mogptk/gpr/kernel.py` & `mogptk-0.5.2/mogptk/gpr/kernel.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/likelihood.py` & `mogptk-0.5.2/mogptk/gpr/likelihood.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/mean.py` & `mogptk-0.5.2/mogptk/gpr/mean.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/model.py` & `mogptk-0.5.2/mogptk/gpr/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
         return -self.log_marginal_likelihood() - self.log_prior()
 
     def compile(self):
         if self._compiled_forward is None:
             self._compiled_forward = torch.jit.trace(self.forward, ())
 
     def __getstate__(self):
-        state = super().__getstate__()
+        state = self.__dict__.copy()
+        state.pop('_compiled_call_impl', None)
         state['_modules'] = state['_modules'].copy()
         state['_modules'].pop('_compiled_forward', None)
         return state
 
     def __setattr__(self, name, val):
         if hasattr(self, name) and isinstance(getattr(self, name), Parameter):
             raise AttributeError("parameter is read-only, use Parameter.assign()")
```

### Comparing `mogptk-0.5.1/mogptk/gpr/multioutput.py` & `mogptk-0.5.2/mogptk/gpr/multioutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/parameter.py` & `mogptk-0.5.2/mogptk/gpr/parameter.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/plot.py` & `mogptk-0.5.2/mogptk/gpr/plot.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/singleoutput.py` & `mogptk-0.5.2/mogptk/gpr/singleoutput.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/gpr/util.py` & `mogptk-0.5.2/mogptk/gpr/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/init.py` & `mogptk-0.5.2/mogptk/init.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/model.py` & `mogptk-0.5.2/mogptk/model.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/conv.py` & `mogptk-0.5.2/mogptk/models/conv.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/csm.py` & `mogptk-0.5.2/mogptk/models/csm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/mohsm.py` & `mogptk-0.5.2/mogptk/models/mohsm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/mosm.py` & `mogptk-0.5.2/mogptk/models/mosm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/sm.py` & `mogptk-0.5.2/mogptk/models/sm.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/models/sm_lmc.py` & `mogptk-0.5.2/mogptk/models/sm_lmc.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/transformer.py` & `mogptk-0.5.2/mogptk/transformer.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk/util.py` & `mogptk-0.5.2/mogptk/util.py`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/mogptk.egg-info/PKG-INFO` & `mogptk-0.5.2/mogptk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mogptk
-Version: 0.5.1
+Version: 0.5.2
 Summary: Multi-Output Gaussian Process ToolKit
 Home-page: https://github.com/GAMES-UChile/mogptk
 Author: Taco de Wolff, Alejandro Cuevas, Felipe Tobar
 Author-email: tacodewolff@gmail.com
 License: MIT
 Keywords: MOGP,MOSM,GP,Gaussian Process,Multi-Output,Tobar,Parra
 Requires-Python: >=3.6
```

### Comparing `mogptk-0.5.1/mogptk.egg-info/SOURCES.txt` & `mogptk-0.5.2/mogptk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mogptk-0.5.1/setup.py` & `mogptk-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='mogptk',
-      version='0.5.1',
+      version='0.5.2',
       description='Multi-Output Gaussian Process ToolKit',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/GAMES-UChile/mogptk',
       author='Taco de Wolff, Alejandro Cuevas, Felipe Tobar',
       author_email='tacodewolff@gmail.com',
       license='MIT',
```

