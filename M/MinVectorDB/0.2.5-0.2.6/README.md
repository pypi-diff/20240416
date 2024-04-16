# Comparing `tmp/minvectordb-0.2.5.tar.gz` & `tmp/minvectordb-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minvectordb-0.2.5.tar", last modified: Mon Apr 15 05:22:21 2024, max compression
+gzip compressed data, was "minvectordb-0.2.6.tar", last modified: Tue Apr 16 06:40:02 2024, max compression
```

## Comparing `minvectordb-0.2.5.tar` & `minvectordb-0.2.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645943 minvectordb-0.2.5/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.5/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645464 minvectordb-0.2.5/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    17717 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.5/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-15 05:22:21.000000 minvectordb-0.2.5/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    17717 2024-04-15 05:22:21.645708 minvectordb-0.2.5/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    16402 2024-04-15 04:50:27.000000 minvectordb-0.2.5/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.639970 minvectordb-0.2.5/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-08 06:55:08.000000 minvectordb-0.2.5/min_vec/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.640289 minvectordb-0.2.5/min_vec/api/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.5/min_vec/api/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11729 2024-04-15 03:57:26.000000 minvectordb-0.2.5/min_vec/api/api.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.640646 minvectordb-0.2.5/min_vec/computational_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.5/min_vec/computational_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      931 2024-04-13 16:15:59.000000 minvectordb-0.2.5/min_vec/computational_layer/engines.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.641230 minvectordb-0.2.5/min_vec/configs/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.5/min_vec/configs/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2896 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/configs/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-15 03:56:30.000000 minvectordb-0.2.5/min_vec/configs/parameters_validator.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.642668 minvectordb-0.2.5/min_vec/data_structures/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.5/min_vec/data_structures/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.5/min_vec/data_structures/fields_mapper.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.5/min_vec/data_structures/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/data_structures/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.5/min_vec/data_structures/limited_dict.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2587 2024-04-12 07:35:09.000000 minvectordb-0.2.5/min_vec/data_structures/limited_sort.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.5/min_vec/data_structures/scaler.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.643803 minvectordb-0.2.5/min_vec/execution_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.5/min_vec/execution_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2541 2024-04-13 15:41:43.000000 minvectordb-0.2.5/min_vec/execution_layer/cluster_worker.py
--rw-r--r--   0 guobingming   (501) staff       (20)    19860 2024-04-15 02:51:07.000000 minvectordb-0.2.5/min_vec/execution_layer/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9989 2024-04-13 15:53:22.000000 minvectordb-0.2.5/min_vec/execution_layer/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.5/min_vec/execution_layer/session.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.644117 minvectordb-0.2.5/min_vec/storage_layer/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.5/min_vec/storage_layer/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    16973 2024-04-13 15:51:50.000000 minvectordb-0.2.5/min_vec/storage_layer/storage.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.644518 minvectordb-0.2.5/min_vec/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.5/min_vec/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.5/min_vec/utils/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-15 05:22:21.645982 minvectordb-0.2.5/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1470 2024-04-12 09:51:44.000000 minvectordb-0.2.5/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-15 05:22:21.645152 minvectordb-0.2.5/test/
--rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.5/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.5/test/test_initial.py
--rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.5/test/test_save_and_query.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.631423 minvectordb-0.2.6/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 minvectordb-0.2.6/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630909 minvectordb-0.2.6/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    17718 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1102 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 minvectordb-0.2.6/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      173 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-16 06:40:02.000000 minvectordb-0.2.6/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    17718 2024-04-16 06:40:02.631180 minvectordb-0.2.6/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    16402 2024-04-15 04:50:27.000000 minvectordb-0.2.6/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.627604 minvectordb-0.2.6/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)      115 2024-04-15 13:22:42.000000 minvectordb-0.2.6/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.627849 minvectordb-0.2.6/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 minvectordb-0.2.6/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11906 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/api/api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.628091 minvectordb-0.2.6/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 minvectordb-0.2.6/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      931 2024-04-13 16:15:59.000000 minvectordb-0.2.6/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.628450 minvectordb-0.2.6/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 minvectordb-0.2.6/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2896 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/configs/config.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-15 03:56:30.000000 minvectordb-0.2.6/min_vec/configs/parameters_validator.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.629234 minvectordb-0.2.6/min_vec/data_structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 minvectordb-0.2.6/min_vec/data_structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-04-03 03:58:31.000000 minvectordb-0.2.6/min_vec/data_structures/fields_mapper.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 minvectordb-0.2.6/min_vec/data_structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1545 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/data_structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1282 2024-04-13 15:42:07.000000 minvectordb-0.2.6/min_vec/data_structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2587 2024-04-12 07:35:09.000000 minvectordb-0.2.6/min_vec/data_structures/limited_sort.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3811 2024-04-12 09:25:04.000000 minvectordb-0.2.6/min_vec/data_structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.629879 minvectordb-0.2.6/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 minvectordb-0.2.6/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2541 2024-04-13 15:41:43.000000 minvectordb-0.2.6/min_vec/execution_layer/cluster_worker.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    20159 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9989 2024-04-13 15:53:22.000000 minvectordb-0.2.6/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 minvectordb-0.2.6/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630090 minvectordb-0.2.6/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 minvectordb-0.2.6/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    17239 2024-04-16 06:35:02.000000 minvectordb-0.2.6/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630340 minvectordb-0.2.6/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 minvectordb-0.2.6/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3389 2024-04-15 04:05:21.000000 minvectordb-0.2.6/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-16 06:40:02.631464 minvectordb-0.2.6/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1471 2024-04-15 13:22:42.000000 minvectordb-0.2.6/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-16 06:40:02.630688 minvectordb-0.2.6/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 minvectordb-0.2.6/test/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1834 2024-04-15 04:04:57.000000 minvectordb-0.2.6/test/test_initial.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    11844 2024-04-12 07:35:09.000000 minvectordb-0.2.6/test/test_save_and_query.py
```

### Comparing `minvectordb-0.2.5/LICENSE` & `minvectordb-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/MinVectorDB.egg-info/PKG-INFO` & `minvectordb-0.2.6/MinVectorDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.5
-Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
+Version: 0.2.6
+Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `minvectordb-0.2.5/MinVectorDB.egg-info/SOURCES.txt` & `minvectordb-0.2.6/MinVectorDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/PKG-INFO` & `minvectordb-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.5
-Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
+Version: 0.2.6
+Summary: MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `minvectordb-0.2.5/README.md` & `minvectordb-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/api/api.py` & `minvectordb-0.2.6/min_vec/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,22 @@
         'n_clusters': int,
         'chunk_size': int,
         'distance': str,
         'index_mode': str,
         'dtypes': str,
         'use_cache': bool,
         'scaler_bits': (None, int),
-        'n_threads': (None, int)
+        'n_threads': (None, int),
+        'warm_up': bool
     }, func_name='MinVectorDB')
     def __init__(
             self, dim: int, database_path: str, n_clusters: int = 16, chunk_size: int = 100_000,
             distance: str = 'cosine', index_mode: str = 'IVF-FLAT', dtypes: str = 'float32',
-            use_cache: bool = True, scaler_bits: int = 8, n_threads: int = None
+            use_cache: bool = True, scaler_bits: int = 8, n_threads: int = None,
+            warm_up: bool = False
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
@@ -65,14 +67,15 @@
                 Options are 'float16', 'float32' or 'float64'.
             use_cache (bool): Whether to use cache for query. Default is True.
             scaler_bits (int): The number of bits for scalar quantization.
                 Options are 8, 16, or 32. The default is None, which means no scalar quantization.
                 The 8 for 8-bit, 16 for 16-bit, and 32 for 32-bit.
             n_threads (int): The number of threads to use for parallel processing. Default is None, which means using
                 twice the number of CPU cores.
+            warm_up (bool): Whether to warm up the database. Default is False.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
         raise_if(ValueError, chunk_size <= 1, 'chunk_size must greater than 1')
         raise_if(ValueError, distance not in ('cosine', 'L2'), 'distance must be "cosine" or "L2"')
@@ -99,29 +102,30 @@
             database_path=database_path,
             n_clusters=n_clusters,
             chunk_size=chunk_size,
             distance=distance,
             index_mode=index_mode,
             logger=logger,
             dtypes=dtypes,
-            scaler_bits=scaler_bits
+            scaler_bits=scaler_bits,
+            warm_up=warm_up
         )
         self._data_loader = self._matrix_serializer.iterable_dataloader
         self._id_filter = self._matrix_serializer.id_filter
 
         self._timer = Timer()
         self._use_cache = use_cache
         self._distance = distance
 
         raise_if(TypeError, n_threads is not None and not isinstance(n_threads, int), "n_threads must be an integer.")
         raise_if(ValueError, n_threads is not None and n_threads <= 0, "n_threads must be greater than 0.")
 
         self._query = Query(
             matrix_serializer=self._matrix_serializer,
-            n_threads=n_threads if n_threads else 2 * os.cpu_count()
+            n_threads=n_threads if n_threads else min(32, os.cpu_count() + 4)
         )
 
         self._query.query.clear_cache()
 
         self._most_recent_query_report = {}
 
     @unavailable_if_deleted
```

### Comparing `minvectordb-0.2.5/min_vec/computational_layer/engines.py` & `minvectordb-0.2.6/min_vec/computational_layer/engines.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/configs/config.py` & `minvectordb-0.2.6/min_vec/configs/config.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/configs/parameters_validator.py` & `minvectordb-0.2.6/min_vec/configs/parameters_validator.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/fields_mapper.py` & `minvectordb-0.2.6/min_vec/data_structures/fields_mapper.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/filter.py` & `minvectordb-0.2.6/min_vec/data_structures/filter.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/kmeans.py` & `minvectordb-0.2.6/min_vec/data_structures/kmeans.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/limited_dict.py` & `minvectordb-0.2.6/min_vec/data_structures/limited_dict.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/limited_sort.py` & `minvectordb-0.2.6/min_vec/data_structures/limited_sort.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/data_structures/scaler.py` & `minvectordb-0.2.6/min_vec/data_structures/scaler.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/execution_layer/cluster_worker.py` & `minvectordb-0.2.6/min_vec/execution_layer/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/execution_layer/matrix_serializer.py` & `minvectordb-0.2.6/min_vec/execution_layer/matrix_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
             database_path: str,
             distance: str,
             logger: Logger,
             n_clusters: int = 16,
             chunk_size: int = 1_000_000,
             index_mode: str = 'IVF-FLAT',
             dtypes: str = 'float32',
-            scaler_bits=None
+            scaler_bits=None,
+            warm_up: bool = False
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
@@ -46,14 +47,15 @@
             index_mode (str): The index mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             scaler_bits (int): The number of bits for scalar quantization. Default is None.
                 Options are 8, 16, 32. If None, scalar quantization will not be used.
                 The 8 bits for uint8, 16 bits for uint16, 32 bits for uint32.
+            warm_up (bool): Whether to warm up the database. Default is False.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         self.last_commit_time = None
         # set commit flag, if the flag is True, the database will not be saved
         self.COMMIT_FLAG = True
@@ -92,15 +94,16 @@
         self.scaler = None
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
         # initialize the storage worker
         self.storage_worker = StorageWorker(self.database_path_parent, self.dim,
                                             self.chunk_size,
-                                            quantizer=None if self.scaler_bits is None else self.scaler)
+                                            quantizer=None if self.scaler_bits is None else self.scaler,
+                                            warm_up=warm_up)
 
         self.logger.info(f"Initializing database folder path: '{'.mvdb'.join(database_path.split('.mvdb')[:-1])}/'")
 
         # ============== Loading or create one empty database ==============
         # first of all, initialize a database
         self.database = []
         self.indices = []
@@ -352,14 +355,17 @@
                 self.ann_model.save(self.database_path_parent / 'ann_model.mvdb')
 
             self.reset_database()
 
             # save params
             self.storage_worker.write_file_attributes({'index_mode': self.index_mode})
 
+            if self.scaler_bits is not None:
+                self.scaler.save(self.database_path_parent / 'sq_model.mvdb')
+
             self.COMMIT_FLAG = True
 
             self.last_commit_time = datetime.now()
 
     def _generate_new_id(self):
         """
         Generate a new ID for the vector.
```

### Comparing `minvectordb-0.2.5/min_vec/execution_layer/query.py` & `minvectordb-0.2.6/min_vec/execution_layer/query.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/min_vec/storage_layer/storage.py` & `minvectordb-0.2.6/min_vec/storage_layer/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from min_vec.configs.config import config
 from min_vec.data_structures.limited_dict import LimitedDict
 
 
 class StorageWorker:
     """The worker class for reading and writing data to the files."""
 
-    def __init__(self, database_path, dimension, chunk_size, quantizer=None):
+    def __init__(self, database_path, dimension, chunk_size, quantizer=None, warm_up=False):
         self.database_path = Path(database_path)
         self.database_chunk_path = self.database_path / 'chunk_data'
         self.database_chunk_indices_path = self.database_path / 'chunk_indices_data'
         self.database_chunk_fields_path = self.database_path / 'chunk_fields_data'
 
         self.database_cluster_path = self.database_path / 'cluster_data'
         self.database_cluster_indices_path = self.database_path / 'cluster_indices_data'
@@ -32,18 +32,29 @@
 
         self.cluster_last_file_shape = {}
 
         self.cache = LimitedDict(max_size=config.MVDB_DATALOADER_BUFFER_SIZE)
 
         self.quantizer = quantizer
 
+        if warm_up:
+            self.warm_up()
+
     def file_exists(self):
         return ((self.database_chunk_path / 'chunk_0').exists()
                 or (self.database_cluster_path / 'cluster_0_0').exists())
 
+    def warm_up(self):
+        """Load the data from the file to the memory."""
+        if not self.file_exists():
+            return
+
+        for data, indices, fields in self.read():
+            pass
+
     def _return_if_in_memory(self, filename, reverse=False):
         res = self.cache.get(filename, None)
 
         if res is None:
             return None
 
         if reverse:
```

### Comparing `minvectordb-0.2.5/min_vec/utils/utils.py` & `minvectordb-0.2.6/min_vec/utils/utils.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/setup.py` & `minvectordb-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.2.5",
-    description='MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed database' \
+    version="0.2.6",
+    description='MinVectorDB is a pure Python-implemented, lightweight, serverless vector, locally deployed database' \
                 'that offers clear and concise Python APIs, aimed at lowering the barrier to ' \
                 'the use of vector databases.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

### Comparing `minvectordb-0.2.5/test/test_initial.py` & `minvectordb-0.2.6/test/test_initial.py`

 * *Files identical despite different names*

### Comparing `minvectordb-0.2.5/test/test_save_and_query.py` & `minvectordb-0.2.6/test/test_save_and_query.py`

 * *Files identical despite different names*

