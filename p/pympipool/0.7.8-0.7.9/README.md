# Comparing `tmp/pympipool-0.7.8.tar.gz` & `tmp/pympipool-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.7.8.tar", last modified: Mon Nov 27 13:21:40 2023, max compression
+gzip compressed data, was "pympipool-0.7.9.tar", last modified: Mon Nov 27 14:37:12 2023, max compression
```

## Comparing `pympipool-0.7.8.tar` & `pympipool-0.7.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.518694 pympipool-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-27 13:20:29.000000 pympipool-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 13:20:29.000000 pympipool-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 13:21:40.518694 pympipool-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10971 2023-11-27 13:20:29.000000 pympipool-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.510694 pympipool-0.7.8/pympipool/
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 13:21:40.518694 pympipool-0.7.8/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/backend/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/backend/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/flux/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/flux/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/mpi/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shell/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/shell/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool/slurm/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-27 13:20:29.000000 pympipool-0.7.8/pympipool/slurm/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.514694 pympipool-0.7.8/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 13:21:40.000000 pympipool-0.7.8/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 13:21:40.000000 pympipool-0.7.8/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 13:21:40.000000 pympipool-0.7.8/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-27 13:21:40.000000 pympipool-0.7.8/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-27 13:21:40.000000 pympipool-0.7.8/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-11-27 13:21:38.000000 pympipool-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 13:21:40.518694 pympipool-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 13:20:29.000000 pympipool-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 13:21:40.518694 pympipool-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_shell_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_subprocess_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_with_dynamic_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-11-27 13:20:29.000000 pympipool-0.7.8/tests/test_zmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.556038 pympipool-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-11-27 14:36:07.000000 pympipool-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:36:07.000000 pympipool-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 14:37:12.556038 pympipool-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10971 2023-11-27 14:36:07.000000 pympipool-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.548038 pympipool-0.7.9/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:37:12.556038 pympipool-0.7.9/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/backend/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/flux/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/mpi/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7181 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/shell/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.552038 pympipool-0.7.9/pympipool/slurm/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-27 14:36:07.000000 pympipool-0.7.9/pympipool/slurm/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.548038 pympipool-0.7.9/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13869 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-27 14:37:12.000000 pympipool-0.7.9/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-11-27 14:37:11.000000 pympipool-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:37:12.556038 pympipool-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:36:07.000000 pympipool-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:37:12.556038 pympipool-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_shell_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_subprocess_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_with_dynamic_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2023-11-27 14:36:07.000000 pympipool-0.7.9/tests/test_zmq.py
```

### Comparing `pympipool-0.7.8/LICENSE` & `pympipool-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/PKG-INFO` & `pympipool-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.7.8
+Version: 0.7.9
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
```

### Comparing `pympipool-0.7.8/README.md` & `pympipool-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/__init__.py` & `pympipool-0.7.9/pympipool/__init__.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/backend/mpiexec.py` & `pympipool-0.7.9/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/backend/serial.py` & `pympipool-0.7.9/pympipool/backend/serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/flux/executor.py` & `pympipool-0.7.9/pympipool/flux/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/mpi/executor.py` & `pympipool-0.7.9/pympipool/mpi/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shared/backend.py` & `pympipool-0.7.9/pympipool/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shared/communication.py` & `pympipool-0.7.9/pympipool/shared/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shared/executorbase.py` & `pympipool-0.7.9/pympipool/shared/executorbase.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shared/interface.py` & `pympipool-0.7.9/pympipool/shared/interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shared/thread.py` & `pympipool-0.7.9/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shell/executor.py` & `pympipool-0.7.9/pympipool/shell/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/shell/interactive.py` & `pympipool-0.7.9/pympipool/shell/interactive.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool/slurm/executor.py` & `pympipool-0.7.9/pympipool/slurm/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pympipool.egg-info/PKG-INFO` & `pympipool-0.7.9/pympipool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.7.8
+Version: 0.7.9
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
```

### Comparing `pympipool-0.7.8/pympipool.egg-info/SOURCES.txt` & `pympipool-0.7.9/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/pyproject.toml` & `pympipool-0.7.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["cloudpickle", "mpi4py", "pyzmq", "setuptools", "tqdm", "versioneer[toml]==0.29"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pympipool"
 description = "Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process."
 authors = [
     { name = "Jan Janssen", email = "janssen@lanl.gov" },
```

### Comparing `pympipool-0.7.8/tests/test_flux.py` & `pympipool-0.7.9/tests/test_flux.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_future.py` & `pympipool-0.7.9/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_interface.py` & `pympipool-0.7.9/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_meta.py` & `pympipool-0.7.9/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_parse.py` & `pympipool-0.7.9/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_queue.py` & `pympipool-0.7.9/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_serial.py` & `pympipool-0.7.9/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_shell_interactive.py` & `pympipool-0.7.9/tests/test_shell_interactive.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_subprocess_executor.py` & `pympipool-0.7.9/tests/test_subprocess_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_task.py` & `pympipool-0.7.9/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_with_dynamic_objects.py` & `pympipool-0.7.9/tests/test_with_dynamic_objects.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_worker.py` & `pympipool-0.7.9/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_worker_memory.py` & `pympipool-0.7.9/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.7.8/tests/test_zmq.py` & `pympipool-0.7.9/tests/test_zmq.py`

 * *Files identical despite different names*

