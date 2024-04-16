# Comparing `tmp/PyGRF-0.1.5.tar.gz` & `tmp/PyGRF-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRF-0.1.5.tar", last modified: Sun Mar 17 01:19:45 2024, max compression
+gzip compressed data, was "PyGRF-0.1.6.tar", last modified: Tue Apr 16 14:15:01 2024, max compression
```

## Comparing `PyGRF-0.1.5.tar` & `PyGRF-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 01:19:45.898875 PyGRF-0.1.5/
--rw-rw-rw-   0        0        0     1088 2024-03-16 20:44:59.000000 PyGRF-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2014 2024-03-17 01:19:45.898875 PyGRF-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-17 01:19:45.883174 PyGRF-0.1.5/PyGRF/
--rw-rw-rw-   0        0        0    22500 2024-03-17 01:17:20.000000 PyGRF-0.1.5/PyGRF/PyGRF.py
--rw-rw-rw-   0        0        0      105 2024-03-17 01:02:05.000000 PyGRF-0.1.5/PyGRF/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 01:19:45.898875 PyGRF-0.1.5/PyGRF.egg-info/
--rw-rw-rw-   0        0        0     2014 2024-03-17 01:19:45.000000 PyGRF-0.1.5/PyGRF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-03-17 01:19:45.000000 PyGRF-0.1.5/PyGRF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 01:19:45.000000 PyGRF-0.1.5/PyGRF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-17 01:19:45.000000 PyGRF-0.1.5/PyGRF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1263 2024-03-17 00:56:56.000000 PyGRF-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-03-17 01:19:45.898875 PyGRF-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2990 2024-03-17 01:17:52.000000 PyGRF-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:15:01.118996 PyGRF-0.1.6/
+-rw-rw-rw-   0        0        0     1088 2024-03-16 20:45:00.000000 PyGRF-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2151 2024-04-16 14:15:01.103370 PyGRF-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 14:15:01.090365 PyGRF-0.1.6/PyGRF/
+-rw-rw-rw-   0        0        0    22907 2024-04-16 14:02:33.000000 PyGRF-0.1.6/PyGRF/PyGRF.py
+-rw-rw-rw-   0        0        0      105 2024-03-17 01:02:06.000000 PyGRF-0.1.6/PyGRF/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 14:15:01.103370 PyGRF-0.1.6/PyGRF.egg-info/
+-rw-rw-rw-   0        0        0     2151 2024-04-16 14:15:00.000000 PyGRF-0.1.6/PyGRF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-16 14:15:01.000000 PyGRF-0.1.6/PyGRF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 14:15:00.000000 PyGRF-0.1.6/PyGRF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-16 14:15:00.000000 PyGRF-0.1.6/PyGRF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 14:15:00.000000 PyGRF-0.1.6/PyGRF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1263 2024-03-17 00:56:58.000000 PyGRF-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 14:15:01.118996 PyGRF-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2988 2024-04-16 14:14:50.000000 PyGRF-0.1.6/setup.py
```

### Comparing `PyGRF-0.1.5/LICENSE` & `PyGRF-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGRF-0.1.5/PKG-INFO` & `PyGRF-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.1.5
+Version: 0.1.6
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: sklearn
+Requires-Dist: scipy
+Requires-Dist: libpysal
+Requires-Dist: esda
 
 
 # PyGRF
 
 
 
 PyGRF: An improved Python Geographical Random Forest (GRF) model.
```

### Comparing `PyGRF-0.1.5/PyGRF/PyGRF.py` & `PyGRF-0.1.6/PyGRF/PyGRF.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import pandas as pd
 import numpy as np
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.metrics import r2_score
-from scipy.spatial import distance
 from sklearn.utils import resample
+from scipy.spatial import distance
 import libpysal
 from esda import Moran
 
 
 class PyGRFBuilder:
     """
     Python implementation of geographic random forest (PyGRF).
 
     Parameters
     ----------
     band_width: int or float
         - The number (int) of neighbors for fitting local models if kernel is "adaptive".
         - The number (int or float) of distance within which the neighbors are used for model fitting if kernel is "fixed".
-    ntree: int, default=100
+    n_estimators: int, default=100
         The number of trees in the forest.
-    mtry: {“sqrt”, “log2”, None}, int or float, default=1.0
+    max_features: {“sqrt”, “log2”, None}, int or float, default=1.0
         The number of input variables to consider at each split.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html.
     kernel: {"adaptive", "fixed"}, default="adaptive"
         The type of kernel used for determining the neighbors of a data point. Two types are available:
         - If "adaptive", a specific number of neighbors to use for fitting local models.
         - If "fixed", neighbors within a fixed distance for fitting local models.
     train_weighted: bool, default = True
@@ -40,18 +40,18 @@
         Note that this parameter should be true if out of bag (OOB) predictions are needed.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html.
     random_seed: int, instance of Numpy RandomState or None, default=None
         Determine the randomness within the model fitting. This parameter has to be fixed in order to achieve reproducibility in the model fitting process.
         More details please refer to the documentation of scikit-learn at the link: https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html.
     """
 
-    def __init__(self, band_width, ntree=100, mtry=1.0, kernel="adaptive", train_weighted=True, predict_weighted=True,
+    def __init__(self, band_width, n_estimators=100, max_features=1.0, kernel="adaptive", train_weighted=True, predict_weighted=True,
                  resampled=True, n_jobs=None, bootstrap=True, random_seed=None):
-        self.ntree = ntree
-        self.mtry = mtry
+        self.n_estimators = n_estimators
+        self.max_features = max_features
         self.band_width = band_width
         self.kernel = kernel
         self.train_weighted = train_weighted
         self.predict_weighted = predict_weighted
         self.n_jobs = n_jobs
         self.bootstrap = bootstrap
         self.resampled = resampled
@@ -69,35 +69,35 @@
         Parameters
         ----------
         X_train: data frame
             A data frame of the independent variables of training samples.
         y_train: data series
             A data series of the dependent variable of training samples.
         coords: data frame
-            A data frame of the two-dimensional coordinates of training samples.
+            A data frame of the two-dimensional coordinates of training samples. It is recommended to use projected coordinates.
 
         Returns
         -------
         global_oob_prediction: list
             The OOB prediction from the global model
         local_oob_prediction: list
             The OOB prediction from the local models
         """
 
         # save the columns of the training data
         self.train_data_columns = X_train.columns.tolist()
 
         # fit and save the global model, and get the OOB predictions from the global model if bootstrap is True
         if self.bootstrap:
-            rf_global = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.ntree,
-                                              max_features=self.mtry, n_jobs=self.n_jobs,
+            rf_global = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.n_estimators,
+                                              max_features=self.max_features, n_jobs=self.n_jobs,
                                               random_state=self.random_seed)
         else:
-            rf_global = RandomForestRegressor(bootstrap=self.bootstrap, n_estimators=self.ntree,
-                                              max_features=self.mtry, n_jobs=self.n_jobs,
+            rf_global = RandomForestRegressor(bootstrap=self.bootstrap, n_estimators=self.n_estimators,
+                                              max_features=self.max_features, n_jobs=self.n_jobs,
                                               random_state=self.random_seed)
         rf_global.fit(X_train, y_train)
         self.global_model = rf_global
         if self.bootstrap:
             global_oob_prediction = rf_global.oob_prediction_
 
         # create an empty list for saving local models
@@ -140,41 +140,41 @@
 
             # the independent and dependent variables of samples for training local models
             local_X_train = X_train.iloc[idx]
             local_y_train = y_train.iloc[idx]
 
             # build a local model
             if self.bootstrap:
-                rf_local = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.ntree,
-                                                 max_features=self.mtry, n_jobs=self.n_jobs, random_state=self.random_seed)
+                rf_local = RandomForestRegressor(bootstrap=self.bootstrap, oob_score=True, n_estimators=self.n_estimators,
+                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_seed)
             else:
                 rf_local = RandomForestRegressor(bootstrap=self.bootstrap,
-                                                 n_estimators=self.ntree,
-                                                 max_features=self.mtry, n_jobs=self.n_jobs, random_state=self.random_seed)
+                                                 n_estimators=self.n_estimators,
+                                                 max_features=self.max_features, n_jobs=self.n_jobs, random_state=self.random_seed)
 
             # fit a local model using local trianing data, which may be expanded with replacement
             if self.train_weighted:
-                if self.resampled and len(local_X_train) < 2 * self.ntree:
-                    resampled_length = min(2 * self.ntree, 2*len(local_X_train)) - len(local_X_train)
+                if self.resampled and len(local_X_train) < 2 * self.n_estimators:
+                    resampled_length = min(2 * self.n_estimators, 2*len(local_X_train)) - len(local_X_train)
                     more_X_train_resampled, more_y_train_resampled, more_sample_weights_resampled = resample(
                         local_X_train,
                         local_y_train,
                         sample_weights,
                         replace=True,
                         n_samples=resampled_length,
                         random_state=self.random_seed)
                     local_X_train_resampled = pd.concat([local_X_train, more_X_train_resampled], ignore_index=True)
                     local_y_train_resampled = pd.concat([local_y_train, more_y_train_resampled], ignore_index=True)
                     sample_weights_resampled = np.concatenate((sample_weights, more_sample_weights_resampled))
                     rf_local.fit(local_X_train_resampled, local_y_train_resampled, sample_weights_resampled)
                 else:
                     rf_local.fit(local_X_train, local_y_train, sample_weights)
             else:
-                if self.resampled and len(local_X_train) < 2 * self.ntree:
-                    resampled_length = min(2 * self.ntree, 2*len(local_X_train)) - len(local_X_train)
+                if self.resampled and len(local_X_train) < 2 * self.n_estimators:
+                    resampled_length = min(2 * self.n_estimators, 2*len(local_X_train)) - len(local_X_train)
                     more_X_train_resampled, more_y_train_resampled = resample(local_X_train,
                                                                               local_y_train,
                                                                               replace=True,
                                                                               n_samples=resampled_length,
                                                                               random_state=self.random_seed)
                     local_X_train_resampled = pd.concat([local_X_train, more_X_train_resampled], ignore_index=True)
                     local_y_train_resampled = pd.concat([local_y_train, more_y_train_resampled], ignore_index=True)
@@ -197,15 +197,15 @@
         Make predictions for test data using fitted model
 
         Parameters
         ----------
         X_test: data frame
             A data frame of the independent variables of test samples.
         coords_test: data frame
-            A data frame of the two-dimensional coordinates of test samples.
+            A data frame of the two-dimensional coordinates of test samples. It is recommended to use projected coordinates.
         local_weight: float
             A number for combining global and local predictions
 
         Returns
         -------
         predict_combined: list
             A list of predictions combined from global and local predictions.
@@ -311,15 +311,15 @@
     Search for bandwidth and local model weight using incremental spatial autocorrelation (ISA)
 
     Parameters
     ----------
     y: data series
         A data series of dependent variable of samples.
     coords: data frame
-        A data frame of two-dimentional coordinates of samples.
+        A data frame of two-dimentional coordinates of samples. It is recommended to use projected coordinates.
     bw_min: int, default = None
         The minimum band_width for searching.
     bw_max: int, default = None
         The maximum band_width for searching.
     step: int, default = 1
         The step for iterating the band_width between minimum and maximum values.
 
@@ -365,30 +365,30 @@
 
     found_bandwidth, found_moran_I, found_p_value = bandwidth_list[max_index], moran_I_list[max_index], p_value_list[max_index]
     print("bandwidth: {}, moran's I: {}, p-value: {}".format(found_bandwidth, found_moran_I, found_p_value))
 
     return found_bandwidth, found_moran_I, found_p_value
 
 
-def search_bandwidth(X, y, coords, ntree, mtry, bw_min=None, bw_max=None, step=1, train_weighted=True, resampled=True, n_jobs=None,
+def search_bandwidth(X, y, coords, n_estimators, max_features, bw_min=None, bw_max=None, step=1, train_weighted=True, resampled=True, n_jobs=None,
                      random_seed=None):
     """
     Optimize the bandwidth using OOB score
 
     Parameters
     ----------
     X: data frame
         A data frame of independent variables of samples in the data used for searching the optimal bandwidth.
     y: data series
         A data series of dependent variable of samples.
     coords: data frame
-        A data frame of two-dimentional coordinates of samples.
-    ntree: int
+        A data frame of two-dimentional coordinates of samples. It is recommended to use projected coordinates.
+    n_estimators: int
         The number of trees for the PyGRF model.
-    mtry: {“sqrt”, “log2”, None}, int or float
+    max_features: {“sqrt”, “log2”, None}, int or float
         The number of input variables to consider at each split.
     bw_min: int, default = None
         The minimum band_width for searching.
     bw_max: int, default = None
         The maximum band_width for searching.
     step: int, default = 1
         The step for iterating the band_width between minimum and maximum values.
@@ -423,15 +423,15 @@
     df_search_bw = pd.DataFrame(columns=['bandwidth', 'mixed'])
 
     # iterate each band_width between minimum and maximum values
     for current_bw in range(bw_min, bw_max + 1, step):
         band_width_list.append(current_bw)
 
         # fit PyGRF model using the test bandwidth and get the OOB predictions
-        grf = PyGRF(ntree=ntree, mtry=mtry, band_width=current_bw, random_seed=random_seed,
+        grf = PyGRFBuilder(n_estimators=n_estimators, max_features=max_features, band_width=current_bw, random_seed=random_seed,
                     train_weighted=train_weighted)
         y_oob_local, y_oob_global = grf.fit(X, y, coords)
 
         # compute R-squred scores using local OOB predictions and global OOB predictions
         # r_oob_local = r2_score(y, y_oob_local)
         # local_list.append(r_oob_local)
         y_oob_mixed = (np.array(y_oob_local) + np.array(y_oob_global)) / 2
```

### Comparing `PyGRF-0.1.5/PyGRF.egg-info/PKG-INFO` & `PyGRF-0.1.6/PyGRF.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.1.5
+Version: 0.1.6
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: sklearn
+Requires-Dist: scipy
+Requires-Dist: libpysal
+Requires-Dist: esda
 
 
 # PyGRF
 
 
 
 PyGRF: An improved Python Geographical Random Forest (GRF) model.
```

### Comparing `PyGRF-0.1.5/README.md` & `PyGRF-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `PyGRF-0.1.5/setup.py` & `PyGRF-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 # Package meta-data.
 NAME = 'PyGRF'
 DESCRIPTION = 'PyGRF: An improved Python Geographical Random Forest model.'
 URL = 'https://github.com/geoai-lab/PyGRF'
 EMAIL = 'ksun4@buffalo.edu'
 AUTHOR = 'Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 
 # Packages are required for this module to be executed.
 REQUIRED = [
-    # 'pandas', 'numpy', 'sklearn', 'scipy', 'libpysal', 'esda'
+    'pandas', 'numpy', 'sklearn', 'scipy', 'libpysal', 'esda'
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 try:
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
```

