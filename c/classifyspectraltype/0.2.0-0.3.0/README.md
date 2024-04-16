# Comparing `tmp/classifyspectraltype-0.2.0.tar.gz` & `tmp/classifyspectraltype-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classifyspectraltype-0.2.0.tar", max compression
+gzip compressed data, was "classifyspectraltype-0.3.0.tar", max compression
```

## Comparing `classifyspectraltype-0.2.0.tar` & `classifyspectraltype-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0     1074 2024-04-12 06:32:08.223261 classifyspectraltype-0.2.0/LICENSE
--rw-r--r--   0        0        0     2099 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/README.md
--rw-r--r--   0        0        0      860 2024-04-13 19:17:04.407077 classifyspectraltype-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      555 2024-04-13 19:11:32.467067 classifyspectraltype-0.2.0/src/classifyspectraltype/__init__.py
--rw-r--r--   0        0        0     1431 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/boxplot_table_function.py
--rw-r--r--   0        0        0      902 2024-04-13 06:17:01.963309 classifyspectraltype-0.2.0/src/classifyspectraltype/clean_confidence_intervals.py
--rw-r--r--   0        0        0     2230 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/fetch_exoplanet_dataset.py
--rw-r--r--   0        0        0     2044 2024-04-13 17:53:57.834123 classifyspectraltype-0.2.0/src/classifyspectraltype/split_cross_val.py
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 classifyspectraltype-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-04-12 06:32:08.223261 classifyspectraltype-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2257 2024-04-16 06:51:54.805440 classifyspectraltype-0.3.0/README.md
+-rw-r--r--   0        0        0      951 2024-04-16 06:52:10.576727 classifyspectraltype-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      555 2024-04-13 19:11:32.467067 classifyspectraltype-0.3.0/src/classifyspectraltype/__init__.py
+-rw-r--r--   0        0        0     1429 2024-04-15 23:34:20.348942 classifyspectraltype-0.3.0/src/classifyspectraltype/boxplot_table_function.py
+-rw-r--r--   0        0        0      902 2024-04-13 06:17:01.963309 classifyspectraltype-0.3.0/src/classifyspectraltype/clean_confidence_intervals.py
+-rw-r--r--   0        0        0     2799 2024-04-15 23:34:20.349942 classifyspectraltype-0.3.0/src/classifyspectraltype/fetch_exoplanet_dataset.py
+-rw-r--r--   0        0        0     2044 2024-04-13 17:53:57.834123 classifyspectraltype-0.3.0/src/classifyspectraltype/split_cross_val.py
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 classifyspectraltype-0.3.0/PKG-INFO
```

### Comparing `classifyspectraltype-0.2.0/LICENSE` & `classifyspectraltype-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.2.0/README.md` & `classifyspectraltype-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![codecov](https://codecov.io/gh/DSCI-310-2024/classifyspectraltype/branch/main/graph/badge.svg)](https://codecov.io/gh/DSCI-310-2024/classifyspectraltype)
+
 # classifyspectraltype
 
 `classifyspectraltype` is a Python package tailored for data scientists and analysts focusing on predictive analytics in laptop pricing. This package focuses on data cleaning, file copying, logistic regression modeling, and plot saving functionalities to facilitate a smoother workflow from raw data to insights.
 
 
 ## Installation
```

### Comparing `classifyspectraltype-0.2.0/pyproject.toml` & `classifyspectraltype-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classifyspectraltype"
-version = "0.2.0"
+version = "0.3.0"
 description = "makes the analysis easier!"
 authors = ["DSCI310 Group16"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -13,14 +13,18 @@
 matplotlib = "^3.8.4"
 requests = "^2.31.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 black = "^24.4.0"
+sphinx = "^7.2.6"
+myst_nb = "^1.1.0"
+sphinx-autoapi = "^3.0.0"
+sphinx_rtd_theme = "^2.0.0"
 
 [tool.semantic_release]
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]                                                    # version location
 branch = "main"                                      # branch to make releases of
 changelog_file = "CHANGELOG.md"                      # changelog file
```

### Comparing `classifyspectraltype-0.2.0/src/classifyspectraltype/__init__.py` & `classifyspectraltype-0.3.0/src/classifyspectraltype/__init__.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.2.0/src/classifyspectraltype/boxplot_table_function.py` & `classifyspectraltype-0.3.0/src/classifyspectraltype/boxplot_table_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     Parameters:
     - data: Dataframe used to select our desired column from
     - column_name: Name of the column as a string
     - csv_dir: Path to the directory in which we want the csv files to live
     - box_plot_dir: Path to the directory in which we want the box plot figures to live
 
     Returns:
-    1. A csv with the quantitative descriptions (mean, std, min) for the four bands (FGKM) loaded into
+    - A csv with the quantitative descriptions (mean, std, min) for the four bands (FGKM) loaded into
     the corresponding directory
-    2. A boxplot of each of the four bands loaded into the corresponding directory
+    - A boxplot of each of the four bands loaded into the corresponding directory
     """
 
     # create and save csv for given column provided
     column_csv = data[["st_spectype", column_name]].groupby("st_spectype").describe()
     column_csv2 = column_csv.round(2)
     column_csv2.to_csv(f"{csv_dir}/{column_name}.csv")
```

### Comparing `classifyspectraltype-0.2.0/src/classifyspectraltype/clean_confidence_intervals.py` & `classifyspectraltype-0.3.0/src/classifyspectraltype/clean_confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.2.0/src/classifyspectraltype/fetch_exoplanet_dataset.py` & `classifyspectraltype-0.3.0/src/classifyspectraltype/fetch_exoplanet_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,23 @@
     The dataset is saved under data/raw/Y-M-D_planet-systems.csv,
     along with its processed version under data/processed/planet-systems.csv by default.
 
     Documentation for constructing a TPA call to retrieve the dataset:
     https://exoplanetarchive.ipac.caltech.edu/cgi-bin/TblView/nph-tblView?app=ExoTbls&config=PS
 
     Parameters:
-    - url (str): The URL from which to fetch the data.
-    - output_path (str): The file path where the fetched raw data will be saved.
-
+    - base_url (str): The URL from which to fetch the data.
+    - output_path (str): The file path where the fetched raw data will be saved. This 
+        specifies the location on the local filesystem where the downloaded dataset should be stored.
+    - columns (list[str]): A list of column names to be fetched from the dataset. 
+        This parameter defines which attributes or fields of the data should be included 
+        in the query and subsequently in the returned DataFrame. For instance, if accessing 
+        a database with many columns, this list explicitly states which columns to retrieve, 
+        optimizing the fetching process and ensuring that only relevant data is loaded.
+        
     Returns:
     - pd.DataFrame: A pandas DataFrame containing the fetched data.
 
     """
     # define the directories where we will store the data
     dataset_name = "planet-systems"
     raw_data_dir = Path("data") / "raw"
```

### Comparing `classifyspectraltype-0.2.0/src/classifyspectraltype/split_cross_val.py` & `classifyspectraltype-0.3.0/src/classifyspectraltype/split_cross_val.py`

 * *Files identical despite different names*

### Comparing `classifyspectraltype-0.2.0/PKG-INFO` & `classifyspectraltype-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: classifyspectraltype
-Version: 0.2.0
+Version: 0.3.0
 Summary: makes the analysis easier!
 License: MIT
 Author: DSCI310 Group16
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.4.2,<2.0.0)
 Description-Content-Type: text/markdown
 
+[![codecov](https://codecov.io/gh/DSCI-310-2024/classifyspectraltype/branch/main/graph/badge.svg)](https://codecov.io/gh/DSCI-310-2024/classifyspectraltype)
+
 # classifyspectraltype
 
 `classifyspectraltype` is a Python package tailored for data scientists and analysts focusing on predictive analytics in laptop pricing. This package focuses on data cleaning, file copying, logistic regression modeling, and plot saving functionalities to facilitate a smoother workflow from raw data to insights.
 
 
 ## Installation
```

