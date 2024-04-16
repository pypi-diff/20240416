# Comparing `tmp/pylammpsmpi-0.2.8.tar.gz` & `tmp/pylammpsmpi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylammpsmpi-0.2.8.tar", last modified: Mon Nov 27 14:36:03 2023, max compression
+gzip compressed data, was "pylammpsmpi-0.2.9.tar", last modified: Tue Nov 28 06:52:12 2023, max compression
```

## Comparing `pylammpsmpi-0.2.8.tar` & `pylammpsmpi-0.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/pylammpsmpi/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/pylammpsmpi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/pylammpsmpi/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13918 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/mpi/lmpmpi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26684 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)    14979 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19542 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/pylammpsmpi/wrapper/extended.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-11-27 14:36:03.000000 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-11-27 14:36:03.000000 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 14:36:03.000000 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-27 14:36:03.000000 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-27 14:36:03.000000 pylammpsmpi-0.2.8/pylammpsmpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-11-27 14:35:59.000000 pylammpsmpi-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 14:36:03.386399 pylammpsmpi-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/tests/test_ase_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-11-27 14:34:46.000000 pylammpsmpi-0.2.8/tests/test_pylammpsmpi_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.680818 pylammpsmpi-0.2.9/pylammpsmpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/pylammpsmpi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/pylammpsmpi/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13918 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/mpi/lmpmpi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26684 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14979 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19542 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/pylammpsmpi/wrapper/extended.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7854 2023-11-28 06:52:12.000000 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-11-28 06:52:12.000000 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 06:52:12.000000 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-28 06:52:12.000000 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-28 06:52:12.000000 pylammpsmpi-0.2.9/pylammpsmpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-11-28 06:52:09.000000 pylammpsmpi-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 06:52:12.684818 pylammpsmpi-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/tests/test_ase_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2023-11-28 06:50:57.000000 pylammpsmpi-0.2.9/tests/test_pylammpsmpi_local.py
```

### Comparing `pylammpsmpi-0.2.8/LICENSE` & `pylammpsmpi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/PKG-INFO` & `pylammpsmpi-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parallel Lammps Python interface - control a mpi4py parallel LAMMPS instance from a serial python process or a Jupyter notebook
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mpi4py<=3.1.5,>=3.1.4
-Requires-Dist: pympipool<=0.7.5,>=0.7.0
+Requires-Dist: pympipool<=0.7.9,>=0.7.0
 Requires-Dist: numpy<=1.26.2,>=1.23.5
 Provides-Extra: ase
 Requires-Dist: ase<=3.22.1,>=3.20.1; extra == "ase"
 Requires-Dist: scipy<=1.11.4,>=1.9.3; extra == "ase"
 
 # pylammpsmpi - Parallel Lammps Python interface
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pylammpsmpi/badge.svg)](https://coveralls.io/github/pyiron/pylammpsmpi)
```

### Comparing `pylammpsmpi-0.2.8/README.md` & `pylammpsmpi-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi/mpi/lmpmpi.py` & `pylammpsmpi-0.2.9/pylammpsmpi/mpi/lmpmpi.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi/wrapper/ase.py` & `pylammpsmpi-0.2.9/pylammpsmpi/wrapper/ase.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi/wrapper/base.py` & `pylammpsmpi-0.2.9/pylammpsmpi/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi/wrapper/concurrent.py` & `pylammpsmpi-0.2.9/pylammpsmpi/wrapper/concurrent.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi/wrapper/extended.py` & `pylammpsmpi-0.2.9/pylammpsmpi/wrapper/extended.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi.egg-info/PKG-INFO` & `pylammpsmpi-0.2.9/pylammpsmpi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylammpsmpi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parallel Lammps Python interface - control a mpi4py parallel LAMMPS instance from a serial python process or a Jupyter notebook
 Author-email: Jan Janssen <janssen@mpie.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2018, Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
         All rights reserved.
         
@@ -46,15 +46,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mpi4py<=3.1.5,>=3.1.4
-Requires-Dist: pympipool<=0.7.5,>=0.7.0
+Requires-Dist: pympipool<=0.7.9,>=0.7.0
 Requires-Dist: numpy<=1.26.2,>=1.23.5
 Provides-Extra: ase
 Requires-Dist: ase<=3.22.1,>=3.20.1; extra == "ase"
 Requires-Dist: scipy<=1.11.4,>=1.9.3; extra == "ase"
 
 # pylammpsmpi - Parallel Lammps Python interface
 [![Coverage Status](https://coveralls.io/repos/github/pyiron/pylammpsmpi/badge.svg)](https://coveralls.io/github/pyiron/pylammpsmpi)
```

### Comparing `pylammpsmpi-0.2.8/pylammpsmpi.egg-info/SOURCES.txt` & `pylammpsmpi-0.2.9/pylammpsmpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/pyproject.toml` & `pylammpsmpi-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "mpi4py>=3.1.4,<=3.1.5",
-    "pympipool>=0.7.0,<=0.7.5",
+    "pympipool>=0.7.0,<=0.7.9",
     "numpy>=1.23.5,<=1.26.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pyiron/pylammpsmpi"
 Documentation = "https://github.com/pyiron/pylammpsmpi"
```

### Comparing `pylammpsmpi-0.2.8/tests/test_ase_constraints.py` & `pylammpsmpi-0.2.9/tests/test_ase_constraints.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/tests/test_base.py` & `pylammpsmpi-0.2.9/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/tests/test_concurrent.py` & `pylammpsmpi-0.2.9/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `pylammpsmpi-0.2.8/tests/test_pylammpsmpi_local.py` & `pylammpsmpi-0.2.9/tests/test_pylammpsmpi_local.py`

 * *Files identical despite different names*

