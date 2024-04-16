# Comparing `tmp/epochalyst-0.2.tar.gz` & `tmp/epochalyst-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochalyst-0.2.tar", last modified: Tue Apr  2 11:55:01 2024, max compression
+gzip compressed data, was "epochalyst-0.3.tar", last modified: Tue Apr 16 15:34:47 2024, max compression
```

## Comparing `epochalyst-0.2.tar` & `epochalyst-0.3.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.669842 epochalyst-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 11:54:53.000000 epochalyst-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 11:55:01.669842 epochalyst-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 11:54:53.000000 epochalyst-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.661842 epochalyst-0.2/epochalyst/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_caching/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_caching/_cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_logging/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_pipeline/_custom_data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/logging/section_separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/training/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/pretrain_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/training_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/transformation/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.669842 epochalyst-0.2/epochalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 11:54:53.000000 epochalyst-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:55:01.669842 epochalyst-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 15:34:39.000000 epochalyst-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 15:34:47.414889 epochalyst-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-16 15:34:39.000000 epochalyst-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.406889 epochalyst-0.3/epochalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_caching/_cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_logging/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_pipeline/_custom_data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/logging/section_separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/pipeline/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/image_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/models/timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/pretrain_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/training_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 15:34:39.000000 epochalyst-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:34:47.414889 epochalyst-0.3/setup.cfg
```

### Comparing `epochalyst-0.2/LICENSE` & `epochalyst-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epochalyst-0.2/PKG-INFO` & `epochalyst-0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.2
+Version: 0.3
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: torch>=2.1.0
-Requires-Dist: agogos==0.3.4
+Requires-Dist: agogos==0.4
 
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Dark.png#gh-light-mode-only)
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Light.png#gh-dark-mode-only)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/epochalyst.svg)](https://pypi.org/project/epochalyst/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/epochalyst.svg?label=PyPI%20downloads)](https://pypi.org/project/epochalyst/)
 
@@ -48,20 +48,32 @@
 ```
 
 ## Imports
 
 ### Caching
 
 For caching some imports are only required, these have to be manually installed when needed
+
 - dask >= 2023.12.0 & dask-expr
 - pandas >= 1.3.0
 - polars
 - pyarrow >= 6.0.0 (Read parquet files)
 - annotated-types >= 0.6.0
 
+### Model
+
+There is support for using timm models. To be able to do so the user must manually install timm.
+- timm >= 0.9.16
+
+### Augmentation
+
+There is also implementations of augmentations that are not in commonly used packages. Most of these are for time series data but there are implmenetations for CutMix and MixUp for images that can be used in the pipeline. To be able to use these the user must manually install kornia.
+
+- kornia >= 0.7.2
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.2/README.md` & `epochalyst-0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -33,20 +33,32 @@
 ```
 
 ## Imports
 
 ### Caching
 
 For caching some imports are only required, these have to be manually installed when needed
+
 - dask >= 2023.12.0 & dask-expr
 - pandas >= 1.3.0
 - polars
 - pyarrow >= 6.0.0 (Read parquet files)
 - annotated-types >= 0.6.0
 
+### Model
+
+There is support for using timm models. To be able to do so the user must manually install timm.
+- timm >= 0.9.16
+
+### Augmentation
+
+There is also implementations of augmentations that are not in commonly used packages. Most of these are for time series data but there are implmenetations for CutMix and MixUp for images that can be used in the pipeline. To be able to use these the user must manually install kornia.
+
+- kornia >= 0.7.2
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.2/epochalyst/_core/_caching/_cacher.py` & `epochalyst-0.3/epochalyst/_core/_caching/_cacher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,43 @@
 import glob
 import os
 import pickle
-from typing import Any, TypedDict, Literal
+import sys
+from typing import Any, Literal, TypedDict
 
-import dask.array as da
-import dask.dataframe as dd
-import numpy as np
-import pandas as pd
-import polars as pl
+try:
+    import dask.array as da
+    import dask.dataframe as dd
+except ImportError:
+    """User doesn't require these packages"""
+
+try:
+    import numpy as np
+except ImportError:
+    """User doesn't require these packages"""
+
+try:
+    import pandas as pd
+except ImportError:
+    """User doesn't require these packages"""
+
+try:
+    import polars as pl
+except ImportError:
+    """User doen't require these packages"""
 
 from epochalyst._core._logging._logger import _Logger
 
+if sys.version_info < (3, 11):
+    from typing_extensions import NotRequired
+else:
+    from typing import NotRequired
 
-class _CacheArgs(TypedDict):
+
+class CacheArgs(TypedDict):
     """The cache arguments.
 
     Currently listed cache_args are supported. If more are required, create a new GitHub issue.
 
     The following keys are supported:
         - output_data_type: The type of the output data.
             - "dask_array": The output data is a Dask array.
@@ -25,49 +46,56 @@
             - "dask_dataframe": The output data is a Dask dataframe.
             - "polars_dataframe": The output data is a Polars dataframe.
         - storage_type: The type of the storage.
             - ".npy": The storage type is a NumPy file.
             - ".parquet": The storage type is a Parquet file.
             - ".csv": The storage type is a CSV file.
             - ".npy_stack": The storage type is a NumPy stack.
-            - ".pkl": The storage type is a pickle file
+            - ".pkl": The storage type is a pickle file.
         - storage_path: The path to the storage.
+        - read_args: The arguments for reading the data.
+        - store_args: The arguments for storing the data.
 
     :param output_data_type: The type of the output data.
     :param storage_type: The type of the storage.
     :param storage_path: The path to the storage.
+    :param read_args: The optional additional arguments for reading the data.
+    :param store_args: The optional additional arguments for storing the data.
     """
 
     output_data_type: Literal[
         "dask_array",
         "numpy_array",
         "pandas_dataframe",
         "dask_dataframe",
         "polars_dataframe",
     ]
     storage_type: Literal[".npy", ".parquet", ".csv", ".npy_stack", ".pkl"]
-    storage_path: str  # TODO(Jeffrey) Allow str | bytes | os.PathLike[str] | os.PathLike[bytes] instead of just str
+    storage_path: str
+    read_args: NotRequired[dict[str, Any]]
+    store_args: NotRequired[dict[str, Any]]
 
 
 class _Cacher(_Logger):
     """The cacher is a flexible class that allows for caching of any data.
 
     The cacher uses cache_args to determine if the data is already cached and if so, return the cached data.
     cache_args is a dictionary that contains the arguments to determine if the data is already cached.
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
-        def _cache_exists(name: str, cache_args: _CacheArgs | None = None) -> bool: # Check if the cache exists
+        def cache_exists(name: str, cache_args: _CacheArgs | None = None) -> bool: # Check if the cache exists
 
         def _get_cache(name: str, cache_args: _CacheArgs | None = None) -> Any: # Load the cache
 
         def _store_cache(name: str, data: Any, cache_args: _CacheArgs | None = None) -> None: # Store data
     """
 
-    def _cache_exists(self, name: str, cache_args: _CacheArgs | None = None) -> bool:
+    def cache_exists(self, name: str, cache_args: CacheArgs | None = None) -> bool:
         """Check if the cache exists.
 
         :param cache_args: The cache arguments.
         :return: True if the cache exists, False otherwise.
         """
         if not cache_args:
             return False
@@ -76,15 +104,15 @@
         if "storage_type" not in cache_args or "storage_path" not in cache_args:
             raise ValueError("cache_args must contain storage_type and storage_path")
 
         storage_type = cache_args["storage_type"]
         storage_path = cache_args["storage_path"]
 
         self.log_to_debug(
-            f"Checking if cache exists for type: {storage_type} and path: {storage_path}"
+            f"Checking if cache exists for type: {storage_type} and path: {storage_path}",
         )
 
         # If storage path does not end a slash, add it
         if storage_path[-1] != "/":
             storage_path += "/"
 
         # Check if path exists
@@ -92,239 +120,235 @@
 
         if storage_type == ".npy":
             path_exists = os.path.exists(storage_path + name + ".npy")
         elif storage_type == ".parquet":
             path_exists = os.path.exists(storage_path + name + ".parquet")
         elif storage_type == ".csv":
             # Check if the file exists or if there are any parts inside the folder
-            path_exists = (
-                os.path.exists(storage_path + name + ".csv")
-                or glob.glob(storage_path + name + "/*.part") != []
-            )
+            path_exists = os.path.exists(storage_path + name + ".csv") or glob.glob(storage_path + name + "/*.part") != []
         elif storage_type == ".npy_stack":
             path_exists = os.path.exists(storage_path + name)
         elif storage_type == ".pkl":
             path_exists = os.path.exists(storage_path + name + ".pkl")
 
         self.log_to_debug(
-            f"Cache exists is {path_exists} for type: {storage_type} and path: {storage_path}"
+            f"Cache exists is {path_exists} for type: {storage_type} and path: {storage_path}",
         )
 
         return path_exists
 
-    def _get_cache(self, name: str, cache_args: _CacheArgs | None = None) -> Any:
+    def _get_cache(self, name: str, cache_args: CacheArgs | None = None) -> Any:  # noqa: ANN401 C901 PLR0911 PLR0912
         """Load the cache.
 
         :param name: The name of the cache.
         :param cache_args: The cache arguments.
         :return: The cached data.
         """
-
         # Check if cache_args is empty
         if not cache_args:
             raise ValueError("cache_args is empty")
 
         # Check if storage type, storage_path and output_data_type are in cache_args
-        if (
-            "storage_type" not in cache_args
-            or "storage_path" not in cache_args
-            or "output_data_type" not in cache_args
-        ):
+        if "storage_type" not in cache_args or "storage_path" not in cache_args or "output_data_type" not in cache_args:
             raise ValueError(
-                "cache_args must contain storage_type, storage_path and output_data_type"
+                "cache_args must contain storage_type, storage_path and output_data_type",
             )
 
         storage_type = cache_args["storage_type"]
         storage_path = cache_args["storage_path"]
         output_data_type = cache_args["output_data_type"]
+        read_args = cache_args.get("read_args", {})
 
         # If storage path does not end a slash, add it
         if storage_path[-1] != "/":
             storage_path += "/"
 
         # Load the cache
         if storage_type == ".npy":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .npy file from {storage_path + name}")
             if output_data_type == "numpy_array":
-                return np.load(storage_path + name + ".npy")
-            elif output_data_type == "dask_array":
-                return da.from_array(np.load(storage_path + name + ".npy"))
-            else:
-                self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for loading .npy file."
-                )
-                raise ValueError(
-                    "output_data_type must be numpy_array or dask_array, other types not supported yet"
-                )
-        elif storage_type == ".parquet":
+                return np.load(storage_path + name + ".npy", **read_args)
+            if output_data_type == "dask_array":
+                return da.from_array(np.load(storage_path + name + ".npy"), **read_args)
+
+            self.log_to_debug(
+                f"Invalid output data type: {output_data_type}, for loading .npy file.",
+            )
+            raise ValueError(
+                "output_data_type must be numpy_array or dask_array, other types not supported yet",
+            )
+        if storage_type == ".parquet":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .parquet file from {storage_path + name}")
             if output_data_type == "pandas_dataframe":
-                return pd.read_parquet(storage_path + name + ".parquet")
-            elif output_data_type == "dask_dataframe":
-                return dd.read_parquet(storage_path + name + ".parquet")
-            elif output_data_type == "numpy_array":
-                return pd.read_parquet(storage_path + name + ".parquet").to_numpy()
-            elif output_data_type == "dask_array":
-                return dd.read_parquet(storage_path + name + ".parquet").to_dask_array()
-            elif output_data_type == "polars_dataframe":
-                return pl.read_parquet(storage_path + name + ".parquet")
-            else:
-                self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for loading .parquet file."
-                )
-                raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet"
-                )
-        elif storage_type == ".csv":
+                return pd.read_parquet(storage_path + name + ".parquet", **read_args)
+            if output_data_type == "dask_dataframe":
+                return dd.read_parquet(storage_path + name + ".parquet", **read_args)
+            if output_data_type == "numpy_array":
+                return pd.read_parquet(
+                    storage_path + name + ".parquet",
+                    **read_args,
+                ).to_numpy()
+            if output_data_type == "dask_array":
+                return dd.read_parquet(
+                    storage_path + name + ".parquet",
+                    **read_args,
+                ).to_dask_array()
+            if output_data_type == "polars_dataframe":
+                return pl.read_parquet(storage_path + name + ".parquet", **read_args)
+
+            self.log_to_debug(
+                f"Invalid output data type: {output_data_type}, for loading .parquet file.",
+            )
+            raise ValueError(
+                "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet",
+            )
+        if storage_type == ".csv":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .csv file from {storage_path + name}")
             if output_data_type == "pandas_dataframe":
-                return pd.read_csv(storage_path + name + ".csv")
-            elif output_data_type == "dask_dataframe":
-                return dd.read_csv(storage_path + name + "/*.part")
-            elif output_data_type == "polars_dataframe":
-                return pl.read_csv(storage_path + name + ".csv")
-            else:
-                self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for loading .csv file."
-                )
-                raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet"
-                )
-        elif storage_type == ".npy_stack":
+                return pd.read_csv(storage_path + name + ".csv", **read_args)
+            if output_data_type == "dask_dataframe":
+                return dd.read_csv(storage_path + name + "/*.part", **read_args)
+            if output_data_type == "polars_dataframe":
+                return pl.read_csv(storage_path + name + ".csv", **read_args)
+
+            self.log_to_debug(
+                f"Invalid output data type: {output_data_type}, for loading .csv file.",
+            )
+            raise ValueError(
+                "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet",
+            )
+        if storage_type == ".npy_stack":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .npy_stack file from {storage_path + name}")
             if output_data_type == "dask_array":
-                return da.from_npy_stack(storage_path + name)
-            else:
-                self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for loading .npy_stack file."
-                )
-                raise ValueError(
-                    "output_data_type must be dask_array, other types not supported yet"
-                )
-        elif storage_type == ".pkl":
-            # Load the pickle file
+                return da.from_npy_stack(storage_path + name, **read_args)
+
             self.log_to_debug(
-                f"Loading pickle file from {storage_path + name + '.pkl'}"
+                f"Invalid output data type: {output_data_type}, for loading .npy_stack file.",
             )
-            return pickle.load(open(storage_path + name + ".pkl", "rb"))
-        else:
-            self.log_to_debug(f"Invalid storage type: {storage_type}")
             raise ValueError(
-                "storage_type must be .npy, .parquet, .csv, or .npy_stack, other types not supported yet"
+                "output_data_type must be dask_array, other types not supported yet",
+            )
+        if storage_type == ".pkl":
+            # Load the pickle file
+            self.log_to_debug(
+                f"Loading pickle file from {storage_path + name + '.pkl'}",
             )
+            with open(storage_path + name + ".pkl", "rb") as file:
+                return pickle.load(file, **read_args)  # noqa: S301
 
-    def _store_cache(
-        self, name: str, data: Any, cache_args: _CacheArgs | None = None
-    ) -> None:
+        self.log_to_debug(f"Invalid storage type: {storage_type}")
+        raise ValueError(
+            "storage_type must be .npy, .parquet, .csv, or .npy_stack, other types not supported yet",
+        )
+
+    def _store_cache(self, name: str, data: Any, cache_args: CacheArgs | None = None) -> None:  # noqa: ANN401 C901 PLR0915 PLR0912
         """Store one set of data.
 
         :param name: The name of the cache.
         :param data: The data to store.
         :param cache_args: The cache arguments.
         """
-
         # Check if cache_args is empty
         if not cache_args:
             raise ValueError("cache_args is empty")
 
         # Check if storage type, storage_path and output_data_type are in cache_args
-        if (
-            "storage_type" not in cache_args
-            or "storage_path" not in cache_args
-            or "output_data_type" not in cache_args
-        ):
+        if "storage_type" not in cache_args or "storage_path" not in cache_args or "output_data_type" not in cache_args:
             raise ValueError(
-                "cache_args must contain storage_type, storage_path and output_data_type"
+                "cache_args must contain storage_type, storage_path and output_data_type",
             )
 
         storage_type = cache_args["storage_type"]
         storage_path = cache_args["storage_path"]
         output_data_type = cache_args["output_data_type"]
+        store_args = cache_args.get("store_args", {})
 
         # If storage path does not end a slash, add it
         if storage_path[-1] != "/":
             storage_path += "/"
 
         # Store the cache
         if storage_type == ".npy":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .npy file to {storage_path + name}")
             if output_data_type == "numpy_array":
-                np.save(storage_path + name + ".npy", data)
+                np.save(storage_path + name + ".npy", data, **store_args)
             elif output_data_type == "dask_array":
-                np.save(storage_path + name + ".npy", data.compute())
+                np.save(storage_path + name + ".npy", data.compute(), **store_args)
             else:
                 self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for storing .npy file."
+                    f"Invalid output data type: {output_data_type}, for storing .npy file.",
                 )
                 raise ValueError(
-                    "output_data_type must be numpy_array or dask_array, other types not supported yet"
+                    "output_data_type must be numpy_array or dask_array, other types not supported yet",
                 )
         elif storage_type == ".parquet":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .parquet file to {storage_path + name}")
-            if output_data_type == "pandas_dataframe":
-                data.to_parquet(storage_path + name + ".parquet")
-            elif output_data_type == "dask_dataframe":
-                data.to_parquet(storage_path + name + ".parquet")
+            if output_data_type in {"pandas_dataframe", "dask_dataframe"}:
+                data.to_parquet(storage_path + name + ".parquet", **store_args)
             elif output_data_type == "numpy_array":
-                pd.DataFrame(data).to_parquet(storage_path + name + ".parquet")
+                pd.DataFrame(data).to_parquet(
+                    storage_path + name + ".parquet",
+                    **store_args,
+                )
             elif output_data_type == "dask_array":
                 new_dd = dd.from_dask_array(data)
                 new_dd = new_dd.rename(
-                    columns={col: str(col) for col in new_dd.columns}
+                    columns={col: str(col) for col in new_dd.columns},
                 )
-                new_dd.to_parquet(storage_path + name + ".parquet")
+                new_dd.to_parquet(storage_path + name + ".parquet", **store_args)
             elif output_data_type == "polars_dataframe":
-                data.write_parquet(storage_path + name + ".parquet")
+                data.write_parquet(storage_path + name + ".parquet", **store_args)
             else:
                 self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for storing .parquet file."
+                    f"Invalid output data type: {output_data_type}, for storing .parquet file.",
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet",
                 )
         elif storage_type == ".csv":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .csv file to {storage_path + name}")
             if output_data_type == "pandas_dataframe":
-                data.to_csv(storage_path + name + ".csv", index=False)
+                data.to_csv(storage_path + name + ".csv", **({"index": False} | store_args))
             elif output_data_type == "dask_dataframe":
-                data.to_csv(storage_path + name, index=False)
+                data.to_csv(storage_path + name, **({"index": False} | store_args))
             elif output_data_type == "polars_dataframe":
-                data.write_csv(storage_path + name + ".csv")
+                data.write_csv(storage_path + name + ".csv", **store_args)
             else:
                 self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for storing .csv file."
+                    f"Invalid output data type: {output_data_type}, for storing .csv file.",
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet",
                 )
         elif storage_type == ".npy_stack":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .npy_stack file to {storage_path + name}")
             if output_data_type == "dask_array":
-                da.to_npy_stack(storage_path + name, data)
+                da.to_npy_stack(storage_path + name, data, **store_args)
             else:
                 self.log_to_debug(
-                    f"Invalid output data type: {output_data_type}, for storing .npy_stack file."
+                    f"Invalid output data type: {output_data_type}, for storing .npy_stack file.",
                 )
                 raise ValueError(
-                    "output_data_type must be numpy_array other types not supported yet"
+                    "output_data_type must be numpy_array other types not supported yet",
                 )
         elif storage_type == ".pkl":
             # Store the pickle file
             self.log_to_debug(f"Storing pickle file to {storage_path + name + '.pkl'}")
-            pickle.dump(
-                data,
-                open(storage_path + name + ".pkl", "wb"),
-                protocol=pickle.HIGHEST_PROTOCOL,
-            )
+            with open(storage_path + name + ".pkl", "wb") as f:
+                pickle.dump(
+                    data,
+                    f,
+                    **({"protocol": pickle.HIGHEST_PROTOCOL} | store_args),
+                )
         else:
             self.log_to_debug(f"Invalid storage type: {storage_type}")
             raise ValueError(
-                "storage_type must be .npy, .parquet, .csv or .npy_stack, other types not supported yet"
+                "storage_type must be .npy, .parquet, .csv or .npy_stack, other types not supported yet",
             )
```

### Comparing `epochalyst-0.2/epochalyst/_core/_logging/_logger.py` & `epochalyst-0.3/epochalyst/_core/_logging/_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+"""_Logger add abstract logging functionality to other classes."""
 from abc import abstractmethod
 from typing import Any
+
 from epochalyst.logging.section_separator import print_section_separator
 
 
 class _Logger:
     """Logger abstract class for logging methods.
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
         @abstractmethod
         def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
 
         @abstractmethod
         def log_to_debug(self, message: str) -> None: # Logs to debugger if implemented
 
@@ -27,55 +30,61 @@
         def log_section_separator(self, message: str) -> None: # Logs a section separator
     """
 
     @abstractmethod
     def log_to_terminal(self, message: str) -> None:
         """Log terminal method, if no logging override with empty.
 
-        :param message: The message to log."""
+        :param message: The message to log.
+        """
         raise NotImplementedError(
-            f"Log terminal method not implemented for {self.__class__.__name__}"
+            f"Log terminal method not implemented for {self.__class__.__name__}",
         )
 
     @abstractmethod
     def log_to_debug(self, message: str) -> None:
         """Log debug method, if no logging override with empty.
 
-        :param message: The message to log."""
+        :param message: The message to log.
+        """
         raise NotImplementedError(
-            f"Log debug method not implemented for {self.__class__}"
+            f"Log debug method not implemented for {self.__class__}",
         )
 
     @abstractmethod
     def log_to_warning(self, message: str) -> None:
         """Log warning method, if no logging override with empty.
 
-        :param message: The message to log."""
+        :param message: The message to log.
+        """
         raise NotImplementedError(
-            f"Log warning method not implemented for {self.__class__}"
+            f"Log warning method not implemented for {self.__class__}",
         )
 
     @abstractmethod
     def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None:
         """Log external method, if no logging override with empty.
 
-        :param message: The message to log."""
+        :param message: The message to log.
+        """
         raise NotImplementedError(
-            f"Log external method not implemented for {self.__class__}"
+            f"Log external method not implemented for {self.__class__}",
         )
 
     @abstractmethod
     def external_define_metric(self, metric: str, metric_type: str) -> None:
-        """Define metric for external. Example: (wandb.define_metric("Training/Train Loss", summary="min"))
+        """Define metric for external. Example: (wandb.define_metric("Training/Train Loss", summary="min")).
 
         :param metric: The metric to define.
-        :param metric_type: The type of the metric."""
+        :param metric_type: The type of the metric.
+        """
         raise NotImplementedError(
-            f"External define metric method not implemented for {self.__class__}"
+            f"External define metric method not implemented for {self.__class__}",
         )
 
     @abstractmethod
     def log_section_separator(self, message: str) -> None:
         """Log section separator method, if no logging override with empty.
 
-        :param message: The message to log."""
+        :param message: The message to log.
+        """
         print_section_separator(message)
```

### Comparing `epochalyst-0.2/epochalyst/logging/section_separator.py` & `epochalyst-0.3/epochalyst/logging/section_separator.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,12 @@
     except OSError:
         separator_length = 200
     separator_char = "="
     title_char = " "
     separator = separator_char * separator_length
     title_padding = (separator_length - len(title)) // 2
     centered_title = (
-        f"{title_char * title_padding}{title}{title_char * title_padding}"
-        if len(title) % 2 == 0
-        else f"{title_char * title_padding}{title}{title_char * (title_padding + 1)}"
+        f"{title_char * title_padding}{title}{title_char * title_padding}" if len(title) % 2 == 0 else f"{title_char * title_padding}{title}{title_char * (title_padding + 1)}"
     )
     print("\n" * spacing)  # noqa: T201
     print(f"{separator}\n{centered_title}\n{separator}")  # noqa: T201
     print("\n" * spacing)  # noqa: T201
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/ensemble.py` & `epochalyst-0.3/epochalyst/pipeline/model/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,88 +1,62 @@
-from agogos.training import ParallelTrainingSystem
+"""ModelPipeline connects multiple transforming and training systems for extended training functionality."""
 from typing import Any
-from epochalyst._core._caching._cacher import _CacheArgs
 
+from agogos.training import Pipeline
 
-class EnsemblePipeline(ParallelTrainingSystem):
-    """EnsemblePipeline is the class used to create the pipeline for the model. (Currently same implementation as agogos pipeline)
+from epochalyst._core._caching._cacher import CacheArgs
 
-    :param steps: Trainers to ensemble
+
+class ModelPipeline(Pipeline):
+    """ModelPipeline is the class used to create the pipeline for the model. (Currently same implementation as agogos pipeline).
+
+    :param x_sys: The system to transform the input data.
+    :param y_sys: The system to transform the label data.
+    :param train_sys: The system to train the model.
+    :param pred_sys: The system to predict the output.
+    :param label_sys: The system to transform the labels after training. (Very optional)
     """
 
-    def get_x_cache_exists(self, cache_args: _CacheArgs) -> bool:
-        """Get status of x
+    def __post_init__(self) -> None:
+        """Post init method for the Pipeline class.
 
-        :param cache_args: Cache arguments
-        :return: Whether cache exists
+        Currently does nothing.
         """
-        if len(self.steps) == 0:
-            return False
+        return super().__post_init__()
+
+    def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:  # noqa: ANN401
+        """Train the system.
+
+        :param x: The input to the system.
+        :param y: The expected output of the system.
+        :return: The input and output of the system.
+        """
+        return super().train(x, y, **train_args)
 
-        for step in self.steps:
-            if not step.get_x_cache_exists(cache_args):
-                return False
+    def predict(self, x: Any, **pred_args: Any) -> Any:  # noqa: ANN401
+        """Predict the output of the system.
 
-        return True
+        :param x: The input to the system.
+        :return: The output of the system.
+        """
+        return super().predict(x, **pred_args)
 
-    def get_y_cache_exists(self, cache_args: _CacheArgs) -> bool:
-        """Get status of y cache
+    def get_x_cache_exists(self, cache_args: CacheArgs) -> bool:
+        """Get status of x.
 
         :param cache_args: Cache arguments
         :return: Whether cache exists
         """
-        if len(self.steps) == 0:
+        if self.x_sys is None:
             return False
+        return self.x_sys.cache_exists(self.x_sys.get_hash(), cache_args)
 
-        for step in self.steps:
-            if not step.get_y_cache_exists(cache_args):
-                return False
-
-        return True
-
-    def concat(
-        self, original_data: Any, data_to_concat: Any, weight: float = 1.0
-    ) -> Any:
-        """Concatenate the trained data.
-
-        :param original_data: First input data
-        :param data_to_concat: Second input data
-        :param weight: Weight of data to concat
-        :return: Concatenated data
+    def get_y_cache_exists(self, cache_args: CacheArgs) -> bool:
+        """Get status of y cache.
+
+        :param cache_args: Cache arguments
+        :return: Whether cache exists
         """
-        if original_data is None:
-            if data_to_concat is None:
-                return None
-            return data_to_concat * weight
-
-        return original_data + data_to_concat * weight
-
-    # def __post_init__(self) -> None:
-    #     """Post init method for the EnsemblePipeline class.
-    #
-    #     Currently does nothing."""
-    #     return super().__post_init__()
-    #
-    # def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
-    #     """Train the system.
-    #
-    #     :param x: The input to the system.
-    #     :param y: The expected output of the system.
-    #     :return: The input and output of the system.
-    #     """
-    #     return super().train(x, y, **train_args)
-    #
-    #
-    # def predict(self, x: Any, **pred_args: Any) -> Any:
-    #     """Predict the output of the system.
-    #
-    #     :param x: The input to the system.
-    #     :return: The output of the system.
-    #     """
-    #     return super().predict(x, **pred_args)
-    #
-    # def concat(
-    #     self, original_data: Any, data_to_concat: Any, weight: float = 1.0
-    # ) -> Any:
-    #     if data_to_concat is None:
-    #         return original_data
-    #     return original_data + data_to_concat * weight
+        if self.y_sys is None:
+            return False
+
+        return self.y_sys.cache_exists(self.y_sys.get_hash(), cache_args)
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/model/training/pretrain_block.py` & `epochalyst-0.3/epochalyst/pipeline/model/training/pretrain_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+"""PretrainBlock to implement modules such as scalers."""
 from abc import abstractmethod
+from dataclasses import dataclass
 from typing import Any
 
 from joblib import hash
 
-from dataclasses import dataclass
-
 from epochalyst.pipeline.model.training.training_block import TrainingBlock
 
 
 @dataclass
 class PretrainBlock(TrainingBlock):
-    """Pretrain block class
+    """Pretrain block class.
 
-    Parameters:
+    Parameters
+    ----------
     - test_size : float
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
         @abstractmethod
         def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
 
         @abstractmethod
         def custom_predict(self, x: Any, **pred_args: Any) -> Any: # Predict pretrain block method.
 
@@ -29,51 +31,46 @@
 
         def train_split_hash(self, train_indices: list[int]) -> str: # Split the hash on train split
 
     Usage:
     .. code-block:: python
         from epochalyst.pipeline.model.training.pretrain_block import PretrainBlock
 
+
         class CustomPretrainBlock(PretrainBlock):
             def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
                 return x, y
 
             def custom_predict(self, x: Any, **pred_args: Any) -> Any:
                 return x
 
+
         custom_pretrain_block = CustomPretrainBlock()
 
         x, y = custom_pretrain_block.train(x, y)
         x = custom_pretrain_block.predict(x)
     """
 
     test_size: float = 0.2
 
     @abstractmethod
-    def pretrain_train(
-        self,
-        x: Any,
-        y: Any,
-        train_indices: list[int],
-        *,
-        save_pretrain: bool = True,
-        save_pretrain_with_split: bool = False,
-    ) -> tuple[Any, Any]:
+    def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:  # noqa: ANN401
         """Train pretrain block method.
 
         :param x: The input to the system.
         :param y: The expected output of the system.
         :param train_indices: The indices to train on.
         :param save_pretrain: Whether to save the pretrain.
-        :param save_pretrain_with_split: Whether to save the pretrain with a cross validation split."""
+        :param save_pretrain_with_split: Whether to save the pretrain with a cross validation split.
+        """
         raise NotImplementedError(
-            f"Train method not implemented for {self.__class__.__name__}"
+            f"Train method not implemented for {self.__class__.__name__}",
         )
 
-    def custom_train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
+    def custom_train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:  # noqa: ANN401
         """Call the pretrain train method.
 
         :param x: The input to the system.
         :param y: The expected output of the system.
         :param train_args: The train arguments.
         :return: The input and output of the system.
         """
@@ -86,14 +83,14 @@
             y,
             train_indices,
             save_pretrain=save_pretrain,
             save_pretrain_with_split=save_pretrain_with_split,
         )
 
     def train_split_hash(self, train_indices: list[int]) -> str:
-        """Split the hash on train split
+        """Split the hash on train split.
 
         :param train_indices: Train indices
         :return: Split hash
         """
         self._hash = hash(self.get_hash() + str(train_indices))
         return self._hash
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/model/training/torch_trainer.py` & `epochalyst-0.3/epochalyst/pipeline/model/training/torch_trainer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,55 @@
+"""TorchTrainer is a module that allows for the training of Torch models."""
 import copy
 import functools
 import gc
-from dataclasses import dataclass
+from collections.abc import Callable
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Annotated, Any, Callable, List, TypeVar
+from typing import Annotated, Any, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 import torch
 from annotated_types import Gt, Interval
 from torch import Tensor, nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
-from torch.utils.data import Dataset, TensorDataset, DataLoader
+from torch.utils.data import DataLoader, Dataset, TensorDataset
 from tqdm import tqdm
 
 from epochalyst._core._pipeline._custom_data_parallel import _CustomDataParallel
 from epochalyst.logging.section_separator import print_section_separator
 from epochalyst.pipeline.model.training.training_block import TrainingBlock
 
 T = TypeVar("T", bound=Dataset)  # type: ignore[type-arg]
 T_co = TypeVar("T_co", covariant=True)
 
 
 @dataclass
 class TorchTrainer(TrainingBlock):
     """Abstract class for torch trainers, override necessary functions for custom implementation.
 
-    Parameters:
+    Parameters
+    ----------
     - `model` (nn.Module): The model to train.
     - `optimizer` (functools.partial[Optimizer]): Optimizer to use for training.
     - `criterion` (nn.Module): Criterion to use for training.
     - `scheduler` (Callable[[Optimizer], LRScheduler] | None): Scheduler to use for training.
     - `epochs` (int): Number of epochs
     - `batch_size` (int): Batch size
     - `patience` (int): Patience for early stopping
     - `test_size` (float): Relative size of the test set
+    - `to_predict` (str): Whether to predict on the test set, all data or none
+    - `model_name` (str): Name of the model
+    - `n_folds` (float): Number of folds for cross validation (0 for train full,
+    - `fold` (int): Fold number
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
         @abstractmethod
         def log_to_terminal(self, message: str) -> None:
             # Logs to terminal if implemented
 
         @abstractmethod
         def log_to_debug(self, message: str) -> None:
@@ -70,21 +78,25 @@
 
         def custom_predict(self, x: Any, **pred_args: Any) -> Any:
             # Implements torch prediction. If you are going to override this method and not use any other functionality, inherit from TrainingBlock.
 
         def predict_on_loader(loader: DataLoader[tuple[Tensor, ...]]) -> npt.NDArray[np.float32]:
             # Predict using a dataloader.
 
-        def create_datasets(x: npt.NDArray[np.float32], y: npt.NDArray[np.float32], train_indices: list[int], test_indices: list[int], cache_size: int = -1) -> tuple[Dataset[tuple[Tensor, ...]], Dataset[tuple[Tensor, ...]]]:
+        def create_datasets(
+            x: npt.NDArray[np.float32], y: npt.NDArray[np.float32], train_indices: list[int], test_indices: list[int], cache_size: int = -1
+        ) -> tuple[Dataset[tuple[Tensor, ...]], Dataset[tuple[Tensor, ...]]]:
             # Create the datasets for training and validation.
 
         def create_prediction_dataset(x: npt.NDArray[np.float32]) -> Dataset[tuple[Tensor, ...]]:
             # Create the prediction dataset.
 
-        def create_dataloaders(train_dataset: Dataset[tuple[Tensor, ...]], test_dataset: Dataset[tuple[Tensor, ...]]) -> tuple[DataLoader[tuple[Tensor, ...]], DataLoader[tuple[Tensor, ...]]]:
+        def create_dataloaders(
+            train_dataset: Dataset[tuple[Tensor, ...]], test_dataset: Dataset[tuple[Tensor, ...]]
+        ) -> tuple[DataLoader[tuple[Tensor, ...]], DataLoader[tuple[Tensor, ...]]]:
             # Create the dataloaders for training and validation.
 
         def update_model_directory(model_directory: str) -> None:
             # Update the model directory for caching (default: tm).
 
     Usage:
     .. code-block:: python
@@ -105,32 +117,45 @@
         criterion = MSELoss()
         scheduler = functools.partial(StepLR, step_size=1, gamma=0.1)
         epochs = 10
         batch_size = 32
         patience = 5
         test_size = 0.2
 
-        trainer = MyTorchTrainer(model=model, optimizer=optimizer, criterion=criterion, scheduler=scheduler, epochs=epochs, batch_size=batch_size, patience=patience, test_size=test_size)
+        trainer = MyTorchTrainer(model=model, optimizer=optimizer, criterion=criterion, scheduler=scheduler,
+                                 epochs=epochs, batch_size=batch_size, patience=patience, test_size=test_size)
 
         x, y = trainer.train(x, y)
         x = trainer.predict(x)
     """
 
     model: nn.Module
     optimizer: functools.partial[Optimizer]
     criterion: nn.Module
     scheduler: Callable[[Optimizer], LRScheduler] | None = None
     epochs: Annotated[int, Gt(0)] = 10
     batch_size: Annotated[int, Gt(0)] = 32
     patience: Annotated[int, Gt(0)] = 5
     test_size: Annotated[float, Interval(ge=0, le=1)] = 0.2  # Hashing purposes
+    to_predict: str = "test"
+    model_name: str = "MODEL_NAME_NOT_SPECIFIED"  # No spaces allowed
+
+    _fold: int = field(default=-1, init=False, repr=False, compare=False)
+    n_folds: float = field(default=-1, init=True, repr=False, compare=False)
 
     def __post_init__(self) -> None:
         """Post init method for the TorchTrainer class."""
-
+        # Make sure to_predict is either "test" or "all" or "none"
+        if self.to_predict not in ["test", "all", "none"]:
+            raise ValueError("to_predict should be either 'test', 'all' or 'none'")
+
+        if self.n_folds == -1:
+            raise ValueError(
+                "Please specify the number of folds for cross validation or set n_folds to 0 for train full.",
+            )
         self.save_model_to_disk = True
         self.model_directory = "tm"
         self.best_model_state_dict: dict[Any, Any] = {}
 
         # Set optimizer
         self.initialized_optimizer = self.optimizer(self.model.parameters())
 
@@ -152,107 +177,166 @@
 
         self.model.to(self.device)
 
         # Early stopping
         self.last_val_loss = np.inf
         self.lowest_val_loss = np.inf
 
+        # Check validity of model_name
+        if " " in self.model_name:
+            raise ValueError("Spaces in model_name not allowed")
+
         super().__post_init__()
 
-    def custom_train(
-        self,
-        x: npt.NDArray[np.float32],
-        y: npt.NDArray[np.float32],
-        **train_args: Any,
-    ) -> tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
+    def custom_train(self, x: npt.NDArray[np.float32], y: npt.NDArray[np.float32], **train_args: Any) -> tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
         """Train the model.
 
         :param x: The input to the system.
         :param y: The expected output of the system.
-
-        Keyword Arguments:
-        :param train_indices: The indices to train on.
-        :param test_indices: The indices to test on.
-        :param cache_size: The cache size.
-        :param save_model: Whether to save the model.
-        :param fold: Fold number if running cv
+        :param train_args: The keyword arguments.
+            - train_indices: The indices to train on.
+            - test_indices: The indices to test on.
+            - save_model: Whether to save the model.
+            - fold: Fold number if running cv.
         :return: The input and output of the system.
         """
         train_indices = train_args.get("train_indices")
         if train_indices is None:
             raise ValueError("train_indices not provided")
         test_indices = train_args.get("test_indices")
         if test_indices is None:
             raise ValueError("test_indices not provided")
-        cache_size = train_args.get("cache_size", -1)
         save_model = train_args.get("save_model", True)
-        fold = train_args.get("fold", -1)
+        self._fold = train_args.get("fold", -1)
 
         self.save_model_to_disk = save_model
 
         # Create datasets
         train_dataset, test_dataset = self.create_datasets(
-            x, y, train_indices, test_indices, cache_size=cache_size
+            x,
+            y,
+            train_indices,
+            test_indices,
         )
 
         # Create dataloaders
         train_loader, test_loader = self.create_dataloaders(train_dataset, test_dataset)
 
-        concat_dataset: Dataset[Any] = self._concat_datasets(
-            train_dataset, test_dataset, train_indices, test_indices
-        )
-        pred_dataloader = DataLoader(
-            concat_dataset, batch_size=self.batch_size, shuffle=False
-        )
-
         if self._model_exists():
             self.log_to_terminal(
-                f"Model exists in {self.model_directory}/{self.get_hash()}.pt, loading model"
+                f"Model exists in {self.model_directory}/{self.get_hash()}.pt, loading model",
             )
             self._load_model()
             # Return the predictions
-            return self.predict_on_loader(pred_dataloader), y
+
+            return self._predict_after_train(
+                x,
+                y,
+                train_dataset,
+                test_dataset,
+                train_indices,
+                test_indices,
+            )
 
         self.log_to_terminal(f"Training model: {self.model.__class__.__name__}")
         self.log_to_debug(f"Training model: {self.model.__class__.__name__}")
 
         # Train the model
         self.log_to_terminal(f"Training model for {self.epochs} epochs")
 
         train_losses: list[float] = []
         val_losses: list[float] = []
 
         self.lowest_val_loss = np.inf
         if len(test_loader) == 0:
             self.log_to_warning(
-                f"Doing train full, model will be trained for {self.epochs} epochs"
+                f"Doing train full, model will be trained for {self.epochs} epochs",
             )
 
-        self._training_loop(train_loader, test_loader, train_losses, val_losses, fold)
+        self._training_loop(
+            train_loader,
+            test_loader,
+            train_losses,
+            val_losses,
+            self._fold,
+        )
 
         self.log_to_terminal(
-            f"Done training the model: {self.model.__class__.__name__}"
+            f"Done training the model: {self.model.__class__.__name__}",
         )
 
         # Revert to the best model
         if self.best_model_state_dict:
             self.log_to_terminal(
-                f"Reverting to model with best validation loss {self.lowest_val_loss}"
+                f"Reverting to model with best validation loss {self.lowest_val_loss}",
             )
             self.model.load_state_dict(self.best_model_state_dict)
 
         if save_model:
             self._save_model()
 
-        return self.predict_on_loader(pred_dataloader), y
+        return self._predict_after_train(
+            x,
+            y,
+            train_dataset,
+            test_dataset,
+            train_indices,
+            test_indices,
+        )
 
-    def custom_predict(
-        self, x: npt.NDArray[np.float32], **pred_args: Any
-    ) -> npt.NDArray[np.float32]:
-        """Predict on the test data
+    def _predict_after_train(
+        self,
+        x: npt.NDArray[np.float32],
+        y: npt.NDArray[np.float32],
+        train_dataset: Dataset[Any],
+        test_dataset: Dataset[Any],
+        train_indices: list[int],
+        test_indices: list[int],
+    ) -> tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
+        """Predict after training the model.
+
+        :param x: The input to the system.
+        :param y: The expected output of the system.
+        :param train_dataset: The training dataset.
+        :param test_dataset: The test dataset.
+        :param train_indices: The indices to train on.
+        :param test_indices: The indices to test on.
+
+        :return: The predictions and the expected output.
+        """
+        match self.to_predict:
+            case "all":
+                concat_dataset: Dataset[Any] = self._concat_datasets(
+                    train_dataset,
+                    test_dataset,
+                    train_indices,
+                    test_indices,
+                )
+                pred_dataloader = DataLoader(
+                    concat_dataset,
+                    batch_size=self.batch_size,
+                    shuffle=False,
+                    collate_fn=(
+                        collate_fn if hasattr(concat_dataset, "__getitems__") else None  # type: ignore[arg-type]
+                    ),
+                )
+                return self.predict_on_loader(pred_dataloader), y
+            case "test":
+                train_loader, test_loader = self.create_dataloaders(
+                    train_dataset,
+                    test_dataset,
+                )
+                return self.predict_on_loader(test_loader), y[test_indices]
+            case "none":
+                return x, y
+            case _:
+                raise ValueError("to_predict should be either 'test', 'all' or 'none")
+
+    def custom_predict(self, x: Any, **pred_args: Any) -> npt.NDArray[np.float32]:  # noqa: ANN401
+        """Predict on the test data.
 
         :param x: The input to the system.
         :return: The output of the system.
         """
         self._load_model()
 
         print_section_separator(f"Predicting model: {self.model.__class__.__name__}")
@@ -260,68 +344,104 @@
 
         # Parse pred_args
         curr_batch_size = pred_args.get("batch_size", self.batch_size)
 
         # Create dataset
         pred_dataset = self.create_prediction_dataset(x)
         pred_dataloader = DataLoader(
-            pred_dataset, batch_size=curr_batch_size, shuffle=False
+            pred_dataset,
+            batch_size=curr_batch_size,
+            shuffle=False,
+            collate_fn=(collate_fn if hasattr(pred_dataset, "__getitems__") else None),  # type: ignore[arg-type]
         )
 
-        # Predict
-        return self.predict_on_loader(pred_dataloader)
+        predictions = []
+        for i in range(int(self.n_folds)):
+            self.log_to_terminal(f"Predicting with model fold {i + 1}/{self.n_folds}")
+            self._fold = i  # set the fold, which updates the hash
+            self._load_model()  # load the model for this fold
+            predictions.append(self.predict_on_loader(pred_dataloader))
+
+        # Average the predictions using numpy
+        test_predictions = np.array(predictions)
+
+        return np.mean(test_predictions, axis=0)
 
     def predict_on_loader(
-        self, loader: DataLoader[tuple[Tensor, ...]]
+        self,
+        loader: DataLoader[tuple[Tensor, ...]],
     ) -> npt.NDArray[np.float32]:
         """Predict on the loader.
 
         :param loader: The loader to predict on.
         :return: The predictions.
         """
         self.log_to_terminal("Predicting on the test data")
         self.model.eval()
         predictions = []
+        # Create a new dataloader from the dataset of the input dataloader with collate_fn
+        loader = DataLoader(
+            loader.dataset,
+            batch_size=loader.batch_size,
+            shuffle=False,
+            collate_fn=(
+                collate_fn if hasattr(loader.dataset, "__getitems__") else None  # type: ignore[arg-type]
+            ),
+        )
         with torch.no_grad(), tqdm(loader, unit="batch", disable=False) as tepoch:
             for data in tepoch:
                 X_batch = data[0].to(self.device).float()
 
                 y_pred = self.model(X_batch).cpu().numpy()
                 predictions.extend(y_pred)
 
         self.log_to_terminal("Done predicting")
         return np.array(predictions)
 
+    def get_hash(self) -> str:
+        """Get the hash of the block.
+
+        Override the get_hash method to include the fold number in the hash.
+
+        :return: The hash of the block.
+        """
+        result = f"{self._hash}_{self.n_folds}"
+        if self._fold != -1:
+            result += f"_f{self._fold}"
+        return result
+
     def create_datasets(
         self,
         x: npt.NDArray[np.float32],
         y: npt.NDArray[np.float32],
         train_indices: list[int],
         test_indices: list[int],
-        cache_size: int = -1,
     ) -> tuple[Dataset[tuple[Tensor, ...]], Dataset[tuple[Tensor, ...]]]:
         """Create the datasets for training and validation.
 
         :param x: The input data.
         :param y: The target variable.
         :param train_indices: The indices to train on.
         :param test_indices: The indices to test on.
         :return: The training and validation datasets.
         """
         train_dataset = TensorDataset(
-            torch.tensor(x[train_indices]), torch.tensor(y[train_indices])
+            torch.tensor(x[train_indices]),
+            torch.tensor(y[train_indices]),
         )
         test_dataset = TensorDataset(
-            torch.tensor(x[test_indices]), torch.tensor(y[test_indices])
+            torch.tensor(x[test_indices]),
+            torch.tensor(y[test_indices]),
         )
 
         return train_dataset, test_dataset
 
     def create_prediction_dataset(
-        self, x: npt.NDArray[np.float32]
+        self,
+        x: npt.NDArray[np.float32],
     ) -> Dataset[tuple[Tensor, ...]]:
         """Create the prediction dataset.
 
         :param x: The input data.
         :return: The prediction dataset.
         """
         return TensorDataset(torch.tensor(x))
@@ -334,28 +454,40 @@
         """Create the dataloaders for training and validation.
 
         :param train_dataset: The training dataset.
         :param test_dataset: The validation dataset.
         :return: The training and validation dataloaders.
         """
         train_loader = DataLoader(
-            train_dataset, batch_size=self.batch_size, shuffle=True
+            train_dataset,
+            batch_size=self.batch_size,
+            shuffle=True,
+            collate_fn=(collate_fn if hasattr(train_dataset, "__getitems__") else None),  # type: ignore[arg-type]
         )
         test_loader = DataLoader(
-            test_dataset, batch_size=self.batch_size, shuffle=False
+            test_dataset,
+            batch_size=self.batch_size,
+            shuffle=False,
+            collate_fn=(collate_fn if hasattr(test_dataset, "__getitems__") else None),  # type: ignore[arg-type]
         )
         return train_loader, test_loader
 
     def update_model_directory(self, model_directory: str) -> None:
         """Update the model directory.
 
         :param model_directory: The model directory.
         """
         self.model_directory = model_directory
 
+    def save_model_to_external(self) -> None:
+        """Save model to external database."""
+        self.log_to_warning(
+            "Saving model to external is not implemented for TorchTrainer, if you want uploaded models. Please overwrite",
+        )
+
     def _training_loop(
         self,
         train_loader: DataLoader[tuple[Tensor, ...]],
         test_loader: DataLoader[tuple[Tensor, ...]],
         train_losses: list[float],
         val_losses: list[float],
         fold: int = -1,
@@ -382,71 +514,78 @@
             train_losses.append(train_loss)
 
             # Log train loss
             self.log_to_external(
                 message={
                     f"Training/Train Loss{fold_no}": train_losses[-1],
                     "epoch": epoch,
-                }
+                },
             )
 
             # Compute validation loss
             if len(test_loader) > 0:
                 self.last_val_loss = self._val_one_epoch(
-                    test_loader, desc=f"Epoch {epoch} Valid"
+                    test_loader,
+                    desc=f"Epoch {epoch} Valid",
                 )
                 self.log_to_debug(f"Epoch {epoch} Valid Loss: {self.last_val_loss}")
                 val_losses.append(self.last_val_loss)
 
                 # Log validation loss and plot train/val loss against each other
                 self.log_to_external(
                     message={
                         f"Validation/Validation Loss{fold_no}": val_losses[-1],
                         "epoch": epoch,
-                    }
+                    },
                 )
 
                 self.log_to_external(
                     message={
                         "type": "wandb_plot",
                         "plot_type": "line_series",
                         "data": {
                             "xs": list(
-                                range(epoch + 1)
+                                range(epoch + 1),
                             ),  # Ensure it's a list, not a range object
                             "ys": [train_losses, val_losses],
                             "keys": [f"Train{fold_no}", f"Validation{fold_no}"],
                             "title": f"Training/Loss{fold_no}",
                             "xname": "Epoch",
                         },
-                    }
+                    },
                 )
 
                 # Early stopping
                 if self._early_stopping():
                     self.log_to_external(
-                        message={f"Epochs{fold_no}": (epoch + 1) - self.patience}
+                        message={f"Epochs{fold_no}": (epoch + 1) - self.patience},
                     )
                     break
 
             # Log the trained epochs to wandb if we finished training
             self.log_to_external(message={f"Epochs{fold_no}": epoch + 1})
 
     def _train_one_epoch(
-        self, dataloader: DataLoader[tuple[Tensor, ...]], epoch: int
+        self,
+        dataloader: DataLoader[tuple[Tensor, ...]],
+        epoch: int,
     ) -> float:
         """Train the model for one epoch.
 
         :param dataloader: Dataloader for the training data.
         :param epoch: Epoch number.
         :return: Average loss for the epoch.
         """
         losses = []
         self.model.train()
-        pbar = tqdm(dataloader, unit="batch", desc=f"Epoch {epoch} Train")
+        pbar = tqdm(
+            dataloader,
+            unit="batch",
+            desc=f"Epoch {epoch} Train ({self.initialized_optimizer.param_groups[0]['lr']})",
+        )
         for batch in pbar:
             X_batch, y_batch = batch
             X_batch = X_batch.to(self.device).float()
             y_batch = y_batch.to(self.device).float()
 
             # Forward pass
             y_pred = self.model(X_batch).squeeze(1)
@@ -468,15 +607,17 @@
         # Remove the cuda cache
         torch.cuda.empty_cache()
         gc.collect()
 
         return sum(losses) / len(losses)
 
     def _val_one_epoch(
-        self, dataloader: DataLoader[tuple[Tensor, ...]], desc: str
+        self,
+        dataloader: DataLoader[tuple[Tensor, ...]],
+        desc: str,
     ) -> float:
         """Compute validation loss of the model for one epoch.
 
         :param dataloader: Dataloader for the testing data.
         :param desc: Description for the tqdm progress bar.
         :return: Average loss for the epoch.
         """
@@ -498,37 +639,37 @@
                 pbar.set_description(desc=desc)
                 pbar.set_postfix(loss=sum(losses) / len(losses))
         return sum(losses) / len(losses)
 
     def _save_model(self) -> None:
         """Save the model in the model_directory folder."""
         self.log_to_terminal(
-            f"Saving model to {self.model_directory}/{self.get_hash()}.pt"
+            f"Saving model to {self.model_directory}/{self.get_hash()}.pt",
         )
         path = Path(self.model_directory)
         if not Path.exists(path):
             Path.mkdir(path)
 
         torch.save(self.model, f"{self.model_directory}/{self.get_hash()}.pt")
         self.log_to_terminal(
-            f"Model saved to {self.model_directory}/{self.get_hash()}.pt"
+            f"Model saved to {self.model_directory}/{self.get_hash()}.pt",
         )
+        self.save_model_to_external()
 
     def _load_model(self) -> None:
         """Load the model from the model_directory folder."""
-
         # Check if the model exists
         if not Path(f"{self.model_directory}/{self.get_hash()}.pt").exists():
             raise FileNotFoundError(
-                f"Model not found in {self.model_directory}/{self.get_hash()}.pt"
+                f"Model not found in {self.model_directory}/{self.get_hash()}.pt",
             )
 
         # Load model
         self.log_to_terminal(
-            f"Loading model from {self.model_directory}/{self.get_hash()}.pt"
+            f"Loading model from {self.model_directory}/{self.get_hash()}.pt",
         )
         checkpoint = torch.load(f"{self.model_directory}/{self.get_hash()}.pt")
 
         # Load the weights from the checkpoint
         if isinstance(checkpoint, nn.DataParallel):
             model = checkpoint.module
         else:
@@ -537,109 +678,131 @@
         # Set the current model to the loaded model
         if isinstance(self.model, nn.DataParallel):
             self.model.module.load_state_dict(model.state_dict())
         else:
             self.model.load_state_dict(model.state_dict())
 
         self.log_to_terminal(
-            f"Model loaded from {self.model_directory}/{self.get_hash()}.pt"
+            f"Model loaded from {self.model_directory}/{self.get_hash()}.pt",
         )
 
     def _model_exists(self) -> bool:
         """Check if the model exists in the model_directory folder."""
-        return (
-            Path(f"{self.model_directory}/{self.get_hash()}.pt").exists()
-            and self.save_model_to_disk
-        )
+        return Path(f"{self.model_directory}/{self.get_hash()}.pt").exists() and self.save_model_to_disk
 
     def _early_stopping(self) -> bool:
         """Check if early stopping should be performed.
 
         :return: Whether to perform early stopping.
         """
-
         # Store the best model so far based on validation loss
-        if self.last_val_loss < self.lowest_val_loss:
-            self.lowest_val_loss = self.last_val_loss
-            self.best_model_state_dict = copy.deepcopy(self.model.state_dict())
-            self.early_stopping_counter = 0
-        else:
-            self.early_stopping_counter += 1
-            if self.early_stopping_counter >= self.patience:
-                self.log_to_terminal(
-                    f"Early stopping after {self.early_stopping_counter} epochs"
-                )
-                return True
+        if self.patience != -1:
+            if self.last_val_loss < self.lowest_val_loss:
+                self.lowest_val_loss = self.last_val_loss
+                self.best_model_state_dict = copy.deepcopy(self.model.state_dict())
+                self.early_stopping_counter = 0
+            else:
+                self.early_stopping_counter += 1
+                if self.early_stopping_counter >= self.patience:
+                    self.log_to_terminal(
+                        f"Early stopping after {self.early_stopping_counter} epochs",
+                    )
+                    return True
         return False
 
     def _concat_datasets(
         self,
         train_dataset: T,
         test_dataset: T,
-        train_indices: list[int],
-        test_indices: list[int],
+        train_indices: list[int] | npt.NDArray[np.int32],
+        test_indices: list[int] | npt.NDArray[np.int32],
     ) -> Dataset[T_co]:
-        """
-        Concatenate the training and test datasets according to original order specified by train_indices and test_indices.
+        """Concatenate the training and test datasets according to original order specified by train_indices and test_indices.
 
         :param train_dataset: The training dataset.
         :param test_dataset: The test dataset.
         :param train_indices: The indices for the training data.
         :param test_indices: The indices for the test data.
         :return: A new dataset containing the concatenated data in the original order.
         """
-
         return TrainTestDataset(
-            train_dataset, test_dataset, train_indices, test_indices
+            train_dataset,
+            test_dataset,
+            list(train_indices),
+            list(test_indices),
         )
 
 
+def collate_fn(batch: tuple[Tensor, ...]) -> tuple[Tensor, ...]:
+    """Collate function for the dataloader.
+
+    :param batch: The batch to collate.
+    :return: Collated batch.
+    """
+    X, y = batch
+    return X, y
+
+
 class TrainTestDataset(Dataset[T_co]):
     """Dataset as a concatenation of multiple datasets.
 
     This class is useful to assemble different existing datasets.
 
     :param train_dataset: The train dataset
     :param test_dataset: The test dataset
     :param train_indices: The train indices
     :param test_indices: The test indices
     """
 
     train_dataset: Dataset[T_co]
     test_dataset: Dataset[T_co]
-    train_indices: List[int]
-    test_indices: List[int]
+    train_indices: list[int]
+    test_indices: list[int]
 
     def __init__(
         self,
         train_dataset: Dataset[T_co],
         test_dataset: Dataset[T_co],
-        train_indices: List[int],
-        test_indices: List[int],
+        train_indices: list[int],
+        test_indices: list[int],
     ) -> None:
+        """Initialize TrainTestDataset.
+
+        :param train_dataset: The train dataset.
+        :param test_dataset: The test dataset.
+        :param train_indices: The train indices.
+        :param test_indices: The test indices.
+        """
         super().__init__()
-        assert len(train_dataset) == len(  # type: ignore[arg-type]
-            train_indices
-        ), "Train_dataset should be the same length as train_indices"
-        assert len(test_dataset) == len(  # type: ignore[arg-type]
-            test_indices
-        ), "Test_dataset should be the same length as test_indices"
+        if len(train_dataset) != len(train_indices):  # type: ignore[arg-type]
+            raise ValueError("Train_dataset should be the same length as train_indices")
+        if len(test_dataset) != len(test_indices):  # type: ignore[arg-type]
+            raise ValueError("Test_dataset should be the same length as test_indices")
         self.train_dataset = train_dataset
         self.test_dataset = test_dataset
         self.train_indices = train_indices
         self.test_indices = test_indices
 
     def __len__(self) -> int:
+        """Get the length of the dataset.
+
+        :return: The length of the dataset.
+        """
         return len(self.train_dataset) + len(self.test_dataset)  # type: ignore[arg-type]
 
     def __getitem__(self, idx: int) -> T_co:
+        """Get the item at an idx.
+
+        :param idx: Index to retrieve.
+        :return: Value to return.
+        """
         if idx < 0:
             if -idx > len(self):
                 raise ValueError(
-                    "absolute value of index should not exceed dataset length"
+                    "absolute value of index should not exceed dataset length",
                 )
             idx = len(self) + idx
 
         item = self.train_dataset[0]
 
         if idx in self.train_indices:
             train_index = self.train_indices.index(idx)
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/model/training/training.py` & `epochalyst-0.3/epochalyst/pipeline/model/training/training.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,32 @@
+"""TrainingPipeline for creating a sequential pipeline of TrainType classes."""
 from typing import Any
+
 from agogos.training import TrainingSystem, TrainType
 
+from epochalyst._core._caching._cacher import CacheArgs, _Cacher
 from epochalyst._core._logging._logger import _Logger
-from epochalyst._core._caching._cacher import _Cacher, _CacheArgs
 
 
 class TrainingPipeline(TrainingSystem, _Cacher, _Logger):
     """The training pipeline. This is the class used to create the pipeline for the training of the model.
 
     :param steps: The steps to train the model.
     """
 
-    def train(
-        self, x: Any, y: Any, cache_args: _CacheArgs | None = None, **train_args: Any
-    ) -> tuple[Any, Any]:
+    def train(self, x: Any, y: Any, cache_args: CacheArgs | None = None, **train_args: Any) -> tuple[Any, Any]:  # noqa: ANN401
         """Train the system.
 
         :param x: The input to the system.
         :param y: The expected output of the system.
         :return: The input and output of the system.
         """
-        if (
-            cache_args
-            and self._cache_exists(name=self.get_hash() + "x", cache_args=cache_args)
-            and self._cache_exists(name=self.get_hash() + "y", cache_args=cache_args)
-        ):
+        if cache_args and self.cache_exists(name=self.get_hash() + "x", cache_args=cache_args) and self.cache_exists(name=self.get_hash() + "y", cache_args=cache_args):
             self.log_to_terminal(
-                f"Cache exists for training pipeline with hash: {self.get_hash()}. Using the cache."
+                f"Cache exists for training pipeline with hash: {self.get_hash()}. Using the cache.",
             )
             x = self._get_cache(name=self.get_hash() + "x", cache_args=cache_args)
             y = self._get_cache(name=self.get_hash() + "y", cache_args=cache_args)
             return x, y
 
         if self.get_steps():
             self.log_section_separator("Training Pipeline")
@@ -50,44 +46,43 @@
                 continue
 
             step_cache_args = step_args.get("cache_args", None)
             if step_cache_args is None:
                 self.log_to_debug(f"{step} is not given cache_args")
                 continue
 
-            step_cache_exists = step._cache_exists(
-                step.get_hash() + "x", step_cache_args
-            ) and step._cache_exists(step.get_hash() + "y", step_cache_args)
+            step_cache_exists = step.cache_exists(
+                step.get_hash() + "x",
+                step_cache_args,
+            ) and step.cache_exists(step.get_hash() + "y", step_cache_args)
             if step_cache_exists:
                 self.log_to_debug(
-                    f"Cache exists for {step}, moving index of steps to {i}"
+                    f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         x, y = super().train(x, y, **train_args)
 
         if cache_args:
             self._store_cache(name=self.get_hash() + "x", data=x, cache_args=cache_args)
             self._store_cache(name=self.get_hash() + "y", data=y, cache_args=cache_args)
 
         # Set steps to original in case class is called again (case: train -> predict)
         self.steps = self.all_steps
 
         return x, y
 
-    def predict(
-        self, x: Any, cache_args: _CacheArgs | None = None, **pred_args: Any
-    ) -> Any:
+    def predict(self, x: Any, cache_args: CacheArgs | None = None, **pred_args: Any) -> Any:  # noqa: ANN401
         """Predict the output of the system.
 
         :param x: The input to the system.
         :param cache_args: The cache arguments.
         :return: The output of the system.
         """
-        if cache_args and self._cache_exists(self.get_hash() + "p", cache_args):
+        if cache_args and self.cache_exists(self.get_hash() + "p", cache_args):
             return self._get_cache(self.get_hash() + "p", cache_args)
 
         if self.get_steps():
             self.log_section_separator("Prediction Pipeline")
 
         self.all_steps = self.get_steps()
 
@@ -104,20 +99,21 @@
                 continue
 
             step_cache_args = step_args.get("cache_args", None)
             if step_cache_args is None:
                 self.log_to_debug(f"{step} is not given cache_args")
                 continue
 
-            step_cache_exists = step._cache_exists(
-                step.get_hash() + "p", step_cache_args
+            step_cache_exists = step.cache_exists(
+                step.get_hash() + "p",
+                step_cache_args,
             )
             if step_cache_exists:
                 self.log_to_debug(
-                    f"Cache exists for {step}, moving index of steps to {i}"
+                    f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         x = super().predict(x, **pred_args)
 
         self._store_cache(self.get_hash() + "p", x, cache_args) if cache_args else None
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation.py` & `epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+"""TransformationPipeline that extends from TransformingSystem, _Cacher and _Logger."""
 from dataclasses import dataclass
 from typing import Any
+
 from agogos.transforming import TransformingSystem, TransformType
 
+from epochalyst._core._caching._cacher import CacheArgs, _Cacher
 from epochalyst._core._logging._logger import _Logger
-from epochalyst._core._caching._cacher import _Cacher, _CacheArgs
 
 
 @dataclass
 class TransformationPipeline(TransformingSystem, _Cacher, _Logger):
     """TransformationPipeline is the class used to create the pipeline for the transformation of the data.
 
     ### Parameters:
     - `steps` (List[Union[Transformer, TransformationPipeline]]): The steps to transform the data. Can be a list of any Transformer type.
     - `title` (str): The title of the pipeline. (Default: "Transformation Pipeline")
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
         @abstractmethod
         def log_to_terminal(self, message: str) -> None: # Log the message to the terminal.
 
         @abstractmethod
         def log_to_debug(self, message: str) -> None: # Log the message to the debug file.
 
@@ -53,27 +56,24 @@
         pipeline = MyTransformationPipeline(steps=[step1, step2])
 
         data = pipeline.transform(data)
     """
 
     title: str = "Transformation Pipeline"  # The title of the pipeline since transformation pipeline can be used for multiple purposes. (Feature, Label, etc.)
 
-    def transform(
-        self, data: Any, cache_args: _CacheArgs | None = None, **transform_args: Any
-    ) -> Any:
+    def transform(self, data: Any, cache_args: CacheArgs | None = None, **transform_args: Any) -> Any:  # noqa: ANN401
         """Transform the input data.
 
         :param data: The input data.
         :param cache_args: The cache arguments.
         :return: The transformed data.
         """
-
-        if cache_args and self._cache_exists(self.get_hash(), cache_args):
+        if cache_args and self.cache_exists(self.get_hash(), cache_args):
             self.log_to_terminal(
-                f"Cache exists for {self.title} with hash: {self.get_hash()}. Using the cache."
+                f"Cache exists for {self.title} with hash: {self.get_hash()}. Using the cache.",
             )
             return self._get_cache(self.get_hash(), cache_args)
 
         if self.get_steps():
             self.log_section_separator(self.title)
 
         self.all_steps = self.get_steps()
@@ -91,18 +91,18 @@
                 continue
 
             step_cache_args = step_args.get("cache_args", None)
             if step_cache_args is None:
                 self.log_to_debug(f"{step} is not given cache_args")
                 continue
 
-            step_cache_exists = step._cache_exists(step.get_hash(), step_cache_args)
+            step_cache_exists = step.cache_exists(step.get_hash(), step_cache_args)
             if step_cache_exists:
                 self.log_to_debug(
-                    f"Cache exists for {step}, moving index of steps to {i}"
+                    f"Cache exists for {step}, moving index of steps to {i}",
                 )
                 self.steps = self.all_steps[i:]
 
         data = super().transform(data, **transform_args)
 
         if cache_args:
             self._store_cache(self.get_hash(), data, cache_args)
```

### Comparing `epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation_block.py` & `epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+"""TransformationBlock module than can be extended by implementing the custom_transform method."""
+from abc import abstractmethod
 from typing import Any
+
 from agogos.transforming import Transformer
+
+from epochalyst._core._caching._cacher import CacheArgs, _Cacher
 from epochalyst._core._logging._logger import _Logger
-from epochalyst._core._caching._cacher import _Cacher, _CacheArgs
-from abc import abstractmethod
 
 
 class TransformationBlock(Transformer, _Cacher, _Logger):
     """The transformation block is a flexible block that allows for transformation of any data.
 
-    Methods:
+    Methods
+    -------
     .. code-block:: python
         @abstractmethod
         def custom_transform(self, data: Any, **transform_args) -> Any: # Custom transformation implementation
 
         @abstractmethod
         def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
 
@@ -47,40 +51,38 @@
             "storage_type": ".npy",
             "storage_path": "data/processed",
         }
 
         data = custom_transformation_block.transform(data, cache=cache_args)
     """
 
-    def transform(
-        self, data: Any, cache_args: _CacheArgs | None = None, **transform_args: Any
-    ) -> Any:
+    def transform(self, data: Any, cache_args: CacheArgs | None = None, **transform_args: Any) -> Any:  # noqa: ANN401
         """Transform the input data using a custom method.
 
         :param data: The input data.
         :param cache_args: The cache arguments.
         :return: The transformed data.
         """
-
-        if cache_args and self._cache_exists(
-            name=self.get_hash(), cache_args=cache_args
+        if cache_args and self.cache_exists(
+            name=self.get_hash(),
+            cache_args=cache_args,
         ):
             self.log_to_terminal(
-                f"Cache exists for {self.__class__} with hash: {self.get_hash()}. Using the cache."
+                f"Cache exists for {self.__class__} with hash: {self.get_hash()}. Using the cache.",
             )
             return self._get_cache(name=self.get_hash(), cache_args=cache_args)
 
         data = self.custom_transform(data, **transform_args)
         if cache_args:
             self._store_cache(name=self.get_hash(), data=data, cache_args=cache_args)
         return data
 
     @abstractmethod
-    def custom_transform(self, data: Any, **transform_args: Any) -> Any:
+    def custom_transform(self, data: Any, **transform_args: Any) -> Any:  # noqa: ANN401
         """Transform the input data using a custom method.
 
         :param data: The input data.
         :return: The transformed data.
         """
         raise NotImplementedError(
-            f"Custom transform method not implemented for {self.__class__}"
+            f"Custom transform method not implemented for {self.__class__}",
         )
```

### Comparing `epochalyst-0.2/epochalyst.egg-info/PKG-INFO` & `epochalyst-0.3/epochalyst.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.2
+Version: 0.3
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
 Requires-Dist: torch>=2.1.0
-Requires-Dist: agogos==0.3.4
+Requires-Dist: agogos==0.4
 
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Dark.png#gh-light-mode-only)
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Light.png#gh-dark-mode-only)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/epochalyst.svg)](https://pypi.org/project/epochalyst/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/epochalyst.svg?label=PyPI%20downloads)](https://pypi.org/project/epochalyst/)
 
@@ -48,20 +48,32 @@
 ```
 
 ## Imports
 
 ### Caching
 
 For caching some imports are only required, these have to be manually installed when needed
+
 - dask >= 2023.12.0 & dask-expr
 - pandas >= 1.3.0
 - polars
 - pyarrow >= 6.0.0 (Read parquet files)
 - annotated-types >= 0.6.0
 
+### Model
+
+There is support for using timm models. To be able to do so the user must manually install timm.
+- timm >= 0.9.16
+
+### Augmentation
+
+There is also implementations of augmentations that are not in commonly used packages. Most of these are for time series data but there are implmenetations for CutMix and MixUp for images that can be used in the pipeline. To be able to use these the user must manually install kornia.
+
+- kornia >= 0.7.2
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.2/epochalyst.egg-info/SOURCES.txt` & `epochalyst-0.3/epochalyst.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -21,10 +21,16 @@
 epochalyst/pipeline/model/__init__.py
 epochalyst/pipeline/model/model.py
 epochalyst/pipeline/model/training/__init__.py
 epochalyst/pipeline/model/training/pretrain_block.py
 epochalyst/pipeline/model/training/torch_trainer.py
 epochalyst/pipeline/model/training/training.py
 epochalyst/pipeline/model/training/training_block.py
+epochalyst/pipeline/model/training/augmentation/__init__.py
+epochalyst/pipeline/model/training/augmentation/image_augmentations.py
+epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
+epochalyst/pipeline/model/training/augmentation/utils.py
+epochalyst/pipeline/model/training/models/__init__.py
+epochalyst/pipeline/model/training/models/timm.py
 epochalyst/pipeline/model/transformation/__init__.py
 epochalyst/pipeline/model/transformation/transformation.py
 epochalyst/pipeline/model/transformation/transformation_block.py
```

