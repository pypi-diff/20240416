# Comparing `tmp/funlib.persistence-0.3.0.tar.gz` & `tmp/funlib_persistence-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funlib.persistence-0.3.0.tar", last modified: Wed Mar 27 19:30:47 2024, max compression
+gzip compressed data, was "funlib_persistence-0.4.0.tar", last modified: Tue Apr 16 15:33:17 2024, max compression
```

## Comparing `funlib.persistence-0.3.0.tar` & `funlib_persistence-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.332257 funlib.persistence-0.3.0/funlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.332257 funlib.persistence-0.3.0/funlib/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/funlib/persistence/arrays/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/arrays/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/arrays/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/arrays/freezable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/funlib/persistence/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/graphs/graph_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/graphs/pgsql_graph_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    23168 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/graphs/sql_graph_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/graphs/sqlite_graph_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/funlib/persistence/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/funlib.persistence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-27 19:30:47.000000 funlib.persistence-0.3.0/funlib.persistence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-27 19:30:47.000000 funlib.persistence-0.3.0/funlib.persistence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:30:47.000000 funlib.persistence-0.3.0/funlib.persistence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 19:30:47.000000 funlib.persistence-0.3.0/funlib.persistence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 19:30:47.000000 funlib.persistence-0.3.0/funlib.persistence.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:30:47.336257 funlib.persistence-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/tests/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-03-27 19:30:39.000000 funlib.persistence-0.3.0/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.913056 funlib_persistence-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-16 15:33:17.913056 funlib_persistence-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.905057 funlib_persistence-0.4.0/funlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.909057 funlib_persistence-0.4.0/funlib/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.909057 funlib_persistence-0.4.0/funlib/persistence/arrays/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/arrays/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24454 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/arrays/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/arrays/freezable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.909057 funlib_persistence-0.4.0/funlib/persistence/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/graphs/graph_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/graphs/pgsql_graph_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23168 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/graphs/sql_graph_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/graphs/sqlite_graph_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/funlib/persistence/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.913056 funlib_persistence-0.4.0/funlib.persistence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-16 15:33:17.000000 funlib_persistence-0.4.0/funlib.persistence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-16 15:33:17.000000 funlib_persistence-0.4.0/funlib.persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:33:17.000000 funlib_persistence-0.4.0/funlib.persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-16 15:33:17.000000 funlib_persistence-0.4.0/funlib.persistence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 15:33:17.000000 funlib_persistence-0.4.0/funlib.persistence.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:33:17.913056 funlib_persistence-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:33:17.909057 funlib_persistence-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/tests/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15530 2024-04-16 15:33:13.000000 funlib_persistence-0.4.0/tests/test_graph.py
```

### Comparing `funlib.persistence-0.3.0/LICENSE` & `funlib_persistence-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/PKG-INFO` & `funlib_persistence-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: funlib.persistence
-Version: 0.3.0
+Version: 0.4.0
 Summary: Interfaces for data (arrays and graphs) and storage formats (databases and file formats)
 Author-email: William Patton <pattonw@hhmi.org>, Jan Funke <funkej@hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: funlib.geometry
 Requires-Dist: networkx
 Requires-Dist: zarr
 Requires-Dist: pymongo
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: psycopg2-binary
+Requires-Dist: fsspec
 Provides-Extra: dev
 Requires-Dist: coverage>=5.0.3; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-psycopg2; extra == "dev"
```

### Comparing `funlib.persistence-0.3.0/README.md` & `funlib_persistence-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib/persistence/arrays/array.py` & `funlib_persistence-0.4.0/funlib/persistence/arrays/array.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib/persistence/arrays/datasets.py` & `funlib_persistence-0.4.0/funlib/persistence/arrays/datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 from .array import Array
 
 from funlib.geometry import Coordinate, Roi
 
 import zarr
+from zarr.n5 import N5FSStore
 import h5py
 import json
 import logging
 import os
 import shutil
-from typing import Optional, Union
+from typing import Optional, Union, Sequence
 
 logger = logging.getLogger(__name__)
 
 
+def get_url(node: Union[zarr.Group, zarr.Array]) -> str:
+    store = node.store
+    if hasattr(store, "path"):
+        if hasattr(store, "fs"):
+            if isinstance(store.fs.protocol, Sequence):
+                protocol = store.fs.protocol[0]
+            else:
+                protocol = store.fs.protocol
+        else:
+            protocol = "file"
+
+        # fsstore keeps the protocol in the path, but not s3store
+        if "://" in store.path:
+            store_path = store.path.split("://")[-1]
+        else:
+            store_path = store.path
+        return f"{protocol}://{store_path}"
+    else:
+        raise ValueError(
+            f"The store associated with this object has type {type(store)}, which "
+            "cannot be resolved to a url"
+        )
+
+
 def separate_store_path(store, path):
     """
     sometimes you can pass a total os path to node, leading to
     an empty('') node.path attribute.
     the correct way is to separate path to container(.n5, .zarr)
     from path to array within a container.
 
@@ -45,20 +70,22 @@
         RuntimeError: returned if the node array is in the parent group,
         or the group itself is the root group
 
     Returns:
         zarr.hierarchy.Group : parent group that contains input group/array
     """
 
-    store_path, node_path = separate_store_path(node.store.path, node.path)
+    path = get_url(node)
+
+    store_path, node_path = separate_store_path(path, node.path)
     if node_path == "":
-        raise RuntimeError(
-            f"{node.name} is in the root group of the {node.store.path} store."
-        )
+        raise RuntimeError(f"{node.name} is in the root group of the {path} store.")
     else:
+        if store_path.endswith(".n5"):
+            store_path = N5FSStore(store_path)
         return zarr.open(store=store_path, path=os.path.split(node_path)[0], mode="r")
 
 
 def check_for_multiscale(group):
     """check if multiscale attribute exists in the input group and for any parent level group
 
     Args:
@@ -208,15 +235,15 @@
     voxel_size = None
     offset = None
     units = None
 
     if multiscales is not None:
         logger.info("Found multiscales attributes")
         scale = os.path.relpath(
-            separate_store_path(ds.store.path, ds.path)[1], multiscale_group.path
+            separate_store_path(get_url(ds), ds.path)[1], multiscale_group.path
         )
         if isinstance(ds.store, (zarr.n5.N5Store, zarr.n5.N5FSStore)):
             for level in multiscales[0]["datasets"]:
                 if level["path"] == scale:
 
                     voxel_size = level["transform"]["scale"]
                     offset = level["transform"]["translate"]
@@ -395,15 +422,15 @@
         chunk_shape = ds.chunks
 
         logger.debug("opened zarr dataset %s in %s", ds_name, filename)
         return Array(ds, roi, voxel_size, chunk_shape=chunk_shape)
 
     elif filename.endswith(".n5"):
         logger.debug("opening N5 dataset %s in %s", ds_name, filename)
-        ds = zarr.open(filename, mode=mode)[ds_name]
+        ds = zarr.open(N5FSStore(filename), mode=mode)[ds_name]
 
         voxel_size, offset = _read_voxel_size_offset(ds, "F")
         shape = Coordinate(ds.shape[-len(voxel_size) :])
         roi = Roi(offset, voxel_size * shape)
 
         chunk_shape = ds.chunks
```

### Comparing `funlib.persistence-0.3.0/funlib/persistence/graphs/graph_database.py` & `funlib_persistence-0.4.0/funlib/persistence/graphs/graph_database.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib/persistence/graphs/pgsql_graph_database.py` & `funlib_persistence-0.4.0/funlib/persistence/graphs/pgsql_graph_database.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib/persistence/graphs/sql_graph_database.py` & `funlib_persistence-0.4.0/funlib/persistence/graphs/sql_graph_database.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib/persistence/graphs/sqlite_graph_database.py` & `funlib_persistence-0.4.0/funlib/persistence/graphs/sqlite_graph_database.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/funlib.persistence.egg-info/PKG-INFO` & `funlib_persistence-0.4.0/funlib.persistence.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: funlib.persistence
-Version: 0.3.0
+Version: 0.4.0
 Summary: Interfaces for data (arrays and graphs) and storage formats (databases and file formats)
 Author-email: William Patton <pattonw@hhmi.org>, Jan Funke <funkej@hhmi.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: funlib.geometry
 Requires-Dist: networkx
 Requires-Dist: zarr
 Requires-Dist: pymongo
 Requires-Dist: numpy
 Requires-Dist: h5py
 Requires-Dist: psycopg2-binary
+Requires-Dist: fsspec
 Provides-Extra: dev
 Requires-Dist: coverage>=5.0.3; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-psycopg2; extra == "dev"
```

### Comparing `funlib.persistence-0.3.0/funlib.persistence.egg-info/SOURCES.txt` & `funlib_persistence-0.4.0/funlib.persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/pyproject.toml` & `funlib_persistence-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "funlib.geometry",
     "networkx",
     "zarr",
     "pymongo",
     "numpy",
     "h5py",
     "psycopg2-binary",
+    "fsspec",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "funlib.persistence.__version__" }
 
 [project.optional-dependencies]
 dev = ['coverage>=5.0.3', 'pytest', 'black', 'mypy', 'types-psycopg2']
```

### Comparing `funlib.persistence-0.3.0/tests/test_array.py` & `funlib_persistence-0.4.0/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/tests/test_datasets.py` & `funlib_persistence-0.4.0/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `funlib.persistence-0.3.0/tests/test_graph.py` & `funlib_persistence-0.4.0/tests/test_graph.py`

 * *Files identical despite different names*

