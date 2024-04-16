# Comparing `tmp/utilsforecast-0.1.3.tar.gz` & `tmp/utilsforecast-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsforecast-0.1.3.tar", last modified: Tue Apr  9 20:12:39 2024, max compression
+gzip compressed data, was "utilsforecast-0.1.4.tar", last modified: Tue Apr 16 17:22:25 2024, max compression
```

## Comparing `utilsforecast-0.1.3.tar` & `utilsforecast-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 20:12:39.018118 utilsforecast-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.014117 utilsforecast-0.1.3/utilsforecast/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/feature_engineering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/grouped_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    27214 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/target_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-09 20:12:31.000000 utilsforecast-0.1.3/utilsforecast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 20:12:39.014117 utilsforecast-0.1.3/utilsforecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 20:12:38.000000 utilsforecast-0.1.3/utilsforecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-09 20:12:39.000000 utilsforecast-0.1.3/utilsforecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:22:25.578601 utilsforecast-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-16 17:22:25.578601 utilsforecast-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:22:25.578601 utilsforecast-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:22:25.574601 utilsforecast-0.1.4/utilsforecast/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30009 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/feature_engineering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/grouped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21756 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27369 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/target_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-04-16 17:22:18.000000 utilsforecast-0.1.4/utilsforecast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:22:25.574601 utilsforecast-0.1.4/utilsforecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 17:22:25.000000 utilsforecast-0.1.4/utilsforecast.egg-info/top_level.txt
```

### Comparing `utilsforecast-0.1.3/CONTRIBUTING.md` & `utilsforecast-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/LICENSE` & `utilsforecast-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/PKG-INFO` & `utilsforecast-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.3
+Version: 0.1.4
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
 Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: numba; extra == "dev"
 Requires-Dist: polars; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
 Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: numba; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.3/README.md` & `utilsforecast-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/settings.ini` & `utilsforecast-0.1.4/settings.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utilsforecast
 lib_name = utilsforecast
-version = 0.1.3
+version = 0.1.4
 min_python = 3.8
 license = apache2
 black_formatting = True
 doc_path = _docs
 lib_path = utilsforecast
 nbs_path = nbs
 recursive = True
```

### Comparing `utilsforecast-0.1.3/setup.py` & `utilsforecast-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/_modidx.py` & `utilsforecast-0.1.4/utilsforecast/_modidx.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/compat.py` & `utilsforecast-0.1.4/utilsforecast/compat.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/data.py` & `utilsforecast-0.1.4/utilsforecast/data.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/evaluation.py` & `utilsforecast-0.1.4/utilsforecast/evaluation.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/feature_engineering.py` & `utilsforecast-0.1.4/utilsforecast/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/grouped_array.py` & `utilsforecast-0.1.4/utilsforecast/grouped_array.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/losses.py` & `utilsforecast-0.1.4/utilsforecast/losses.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/plotting.py` & `utilsforecast-0.1.4/utilsforecast/plotting.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/preprocessing.py` & `utilsforecast-0.1.4/utilsforecast/preprocessing.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/processing.py` & `utilsforecast-0.1.4/utilsforecast/processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,18 +547,22 @@
         s = s.astype(dtype)
     else:
         s = s.cast(dtype)
     return s
 
 # %% ../nbs/processing.ipynb 67
 def value_cols_to_numpy(
-    df: DataFrame, id_col: str, time_col: str, target_col: str
+    df: DataFrame, id_col: str, time_col: str, target_col: Optional[str]
 ) -> np.ndarray:
-    exclude_cols = [id_col, time_col, target_col]
-    value_cols = [target_col] + [col for col in df.columns if col not in exclude_cols]
+    exclude_cols = [id_col, time_col]
+    if target_col is not None:
+        exclude_cols.append(target_col)
+    value_cols = [col for col in df.columns if col not in exclude_cols]
+    if target_col is not None:
+        value_cols = [target_col, *value_cols]
     data = to_numpy(df[value_cols])
     if data.dtype not in (np.float32, np.float64):
         data = data.astype(np.float32)
     return data
 
 # %% ../nbs/processing.ipynb 68
 def make_future_dataframe(
@@ -594,15 +598,18 @@
             "df1 and df2 must be pandas or polars dataframes of the same type. "
             f"Got type(df1): '{type(df1)}', type(df2): '{type(df2)}'"
         )
     return out
 
 # %% ../nbs/processing.ipynb 74
 def process_df(
-    df: DataFrame, id_col: str, time_col: str, target_col: str
+    df: DataFrame,
+    id_col: str,
+    time_col: str,
+    target_col: Optional[str],
 ) -> Tuple[Series, np.ndarray, np.ndarray, np.ndarray, Optional[np.ndarray]]:
     """Extract components from dataframe
 
     Parameters
     ----------
     df : pandas or polars DataFrame
         Input dataframe with id, times and target values.
@@ -657,15 +664,15 @@
         self.target_col = target_col
 
     def process(
         self, df: DataFrame
     ) -> Tuple[Series, np.ndarray, np.ndarray, np.ndarray, Optional[np.ndarray]]:
         return process_df(df, self.id_col, self.time_col, self.target_col)
 
-# %% ../nbs/processing.ipynb 80
+# %% ../nbs/processing.ipynb 81
 def _single_split(
     df: DataFrame,
     i_window: int,
     n_windows: int,
     h: int,
     id_col: str,
     time_col: str,
@@ -722,15 +729,15 @@
             group_by(cutoffs, id_col)
             .agg(pl.col(time_col).head(1))
             .explode(pl.col(time_col))
             .rename({time_col: "cutoff"})
         )
     return cutoffs, train_mask, valid_mask
 
-# %% ../nbs/processing.ipynb 81
+# %% ../nbs/processing.ipynb 82
 def backtest_splits(
     df: DataFrame,
     n_windows: int,
     h: int,
     id_col: str,
     time_col: str,
     freq: Union[int, str, pd.offsets.BaseOffset],
@@ -754,15 +761,15 @@
             step_size=step_size,
             input_size=input_size,
         )
         train = filter_with_mask(df, train_mask)
         valid = filter_with_mask(df, valid_mask)
         yield cutoffs, train, valid
 
-# %% ../nbs/processing.ipynb 85
+# %% ../nbs/processing.ipynb 86
 def add_insample_levels(
     df: DataFrame,
     models: List[str],
     level: List[Union[int, float]],
     id_col: str = "unique_id",
     target_col: str = "y",
 ) -> DataFrame:
```

### Comparing `utilsforecast-0.1.3/utilsforecast/target_transforms.py` & `utilsforecast-0.1.4/utilsforecast/target_transforms.py`

 * *Files identical despite different names*

### Comparing `utilsforecast-0.1.3/utilsforecast/validation.py` & `utilsforecast-0.1.4/utilsforecast/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,14 @@
         raise ValueError(
             "Time column contains timestamps but the specified frequency is an integer. "
             "Please provide a valid pandas or polars offset, e.g. `freq='D'` or `freq='1d'`."
         )
     # try to catch pandas frequency in polars dataframe
     if isinstance(times, pl_Series) and isinstance(freq, str):
         missing_n = re.search(r"\d+", freq) is None
-        uppercase = re.sub("\d+", "", freq).isupper()
+        uppercase = re.sub(r"\d+", "", freq).isupper()
         if missing_n or uppercase:
             raise ValueError(
                 "You must specify a valid polars offset when using polars dataframes. "
                 "You can find the available offsets in "
                 "https://pola-rs.github.io/polars/py-polars/html/reference/expressions/api/polars.Expr.dt.offset_by.html"
             )
```

### Comparing `utilsforecast-0.1.3/utilsforecast.egg-info/PKG-INFO` & `utilsforecast-0.1.4/utilsforecast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsforecast
-Version: 0.1.3
+Version: 0.1.4
 Summary: Forecasting utilities
 Home-page: https://github.com/Nixtla/utilsforecast
 Author: Nixtla
 Author-email: business@nixtla.io
 License: Apache Software License 2.0
 Keywords: time-series analysis forecasting
 Classifier: Development Status :: 4 - Beta
@@ -27,23 +27,23 @@
 Requires-Dist: plotly-resampler; extra == "plotting"
 Provides-Extra: scalers
 Requires-Dist: numba; extra == "scalers"
 Requires-Dist: scipy; extra == "scalers"
 Provides-Extra: polars
 Requires-Dist: polars; extra == "polars"
 Provides-Extra: dev
+Requires-Dist: pyarrow; extra == "dev"
+Requires-Dist: nbdev; extra == "dev"
 Requires-Dist: datasetsforecast==0.0.8; extra == "dev"
-Requires-Dist: plotly; extra == "dev"
+Requires-Dist: scipy; extra == "dev"
 Requires-Dist: plotly-resampler; extra == "dev"
+Requires-Dist: plotly; extra == "dev"
+Requires-Dist: numba; extra == "dev"
 Requires-Dist: polars; extra == "dev"
-Requires-Dist: pyarrow; extra == "dev"
 Requires-Dist: pandas[plot]; extra == "dev"
-Requires-Dist: numba; extra == "dev"
-Requires-Dist: scipy; extra == "dev"
-Requires-Dist: nbdev; extra == "dev"
 
 utilsforecast
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Install
```

### Comparing `utilsforecast-0.1.3/utilsforecast.egg-info/SOURCES.txt` & `utilsforecast-0.1.4/utilsforecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

