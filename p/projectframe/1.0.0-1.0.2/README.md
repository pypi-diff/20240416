# Comparing `tmp/projectframe-1.0.0.tar.gz` & `tmp/projectframe-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectframe-1.0.0.tar", max compression
+gzip compressed data, was "projectframe-1.0.2.tar", max compression
```

## Comparing `projectframe-1.0.0.tar` & `projectframe-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 projectframe-1.0.0/LICENSE.md
--rwxr-xr-x   0        0        0     1001 2023-04-19 18:21:41.948676 projectframe-1.0.0/README.md
--rw-r--r--   0        0        0      608 2022-08-30 13:55:30.000000 projectframe-1.0.0/projectframe/__init__.py
--rwxr-xr-x   0        0        0       98 2022-08-26 16:03:58.000000 projectframe-1.0.0/projectframe/core/__init__.py
--rwxr-xr-x   0        0        0    10765 2023-04-03 20:02:18.197569 projectframe-1.0.0/projectframe/core/core.py
--rwxr-xr-x   0        0        0      107 2022-08-26 16:04:25.000000 projectframe-1.0.0/projectframe/engines/__init__.py
--rw-r--r--   0        0        0     4670 2023-03-24 01:23:11.864411 projectframe-1.0.0/projectframe/engines/pandas_engine.py
--rw-r--r--   0        0        0     7842 2022-09-06 14:35:13.000000 projectframe-1.0.0/projectframe/engines/pandas_h5.py
--rwxr-xr-x   0        0        0      241 2022-08-30 13:55:00.000000 projectframe-1.0.0/projectframe/objects/__init__.py
--rw-r--r--   0        0        0     3675 2022-10-05 19:43:28.000000 projectframe-1.0.0/projectframe/objects/frame.py
--rw-r--r--   0        0        0     6206 2023-03-15 21:39:52.773501 projectframe-1.0.0/projectframe/objects/multiframe.py
--rw-r--r--   0        0        0     5928 2023-02-01 17:08:16.215371 projectframe-1.0.0/projectframe/objects/obsframe.py
--rw-r--r--   0        0        0     5551 2022-09-06 18:32:38.000000 projectframe-1.0.0/projectframe/objects/unstructured.py
--rw-r--r--   0        0        0     1994 2023-05-07 12:07:10.643799 projectframe-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 projectframe-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 projectframe-1.0.2/LICENSE.md
+-rwxr-xr-x   0        0        0     1001 2023-04-19 18:21:41.948676 projectframe-1.0.2/README.md
+-rw-r--r--   0        0        0      608 2023-05-17 13:21:03.996924 projectframe-1.0.2/projectframe/__init__.py
+-rwxr-xr-x   0        0        0       98 2022-08-26 16:03:58.000000 projectframe-1.0.2/projectframe/core/__init__.py
+-rwxr-xr-x   0        0        0    10765 2023-04-03 20:02:18.197569 projectframe-1.0.2/projectframe/core/core.py
+-rwxr-xr-x   0        0        0      107 2022-08-26 16:04:25.000000 projectframe-1.0.2/projectframe/engines/__init__.py
+-rw-r--r--   0        0        0     4670 2023-03-24 01:23:11.864411 projectframe-1.0.2/projectframe/engines/pandas_engine.py
+-rw-r--r--   0        0        0     7842 2022-09-06 14:35:13.000000 projectframe-1.0.2/projectframe/engines/pandas_h5.py
+-rwxr-xr-x   0        0        0      241 2022-08-30 13:55:00.000000 projectframe-1.0.2/projectframe/objects/__init__.py
+-rw-r--r--   0        0        0     3675 2022-10-05 19:43:28.000000 projectframe-1.0.2/projectframe/objects/frame.py
+-rw-r--r--   0        0        0     6206 2023-03-15 21:39:52.773501 projectframe-1.0.2/projectframe/objects/multiframe.py
+-rw-r--r--   0        0        0     5928 2023-02-01 17:08:16.215371 projectframe-1.0.2/projectframe/objects/obsframe.py
+-rw-r--r--   0        0        0     5551 2022-09-06 18:32:38.000000 projectframe-1.0.2/projectframe/objects/unstructured.py
+-rw-r--r--   0        0        0     1990 2024-04-16 18:31:16.856869 projectframe-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 projectframe-1.0.2/PKG-INFO
```

### Comparing `projectframe-1.0.0/LICENSE.md` & `projectframe-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/README.md` & `projectframe-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/__init__.py` & `projectframe-1.0.2/projectframe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .objects.frame import Frame
 from .objects.multiframe import MultiFrame, MultiIntervalFrame
 from .objects.unstructured import UnstructuredLookup
 from .objects.obsframe import ObsFrame, ObsIntervalFrame
 
 
 # This is extracted automatically by the top-level setup.py.
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __author__ = "Kyle S. Smith"
 
 
 __doc__ = """\
 API
 ======
```

### Comparing `projectframe-1.0.0/projectframe/core/core.py` & `projectframe-1.0.2/projectframe/core/core.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/engines/pandas_engine.py` & `projectframe-1.0.2/projectframe/engines/pandas_engine.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/engines/pandas_h5.py` & `projectframe-1.0.2/projectframe/engines/pandas_h5.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/objects/frame.py` & `projectframe-1.0.2/projectframe/objects/frame.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/objects/multiframe.py` & `projectframe-1.0.2/projectframe/objects/multiframe.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/objects/obsframe.py` & `projectframe-1.0.2/projectframe/objects/obsframe.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/projectframe/objects/unstructured.py` & `projectframe-1.0.2/projectframe/objects/unstructured.py`

 * *Files identical despite different names*

### Comparing `projectframe-1.0.0/pyproject.toml` & `projectframe-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "projectframe"
-version = "1.0.0"
+version = "1.0.2"
 description = "Python package for multi-dimensional tabular data"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/projectframe"
 documentation = "https://www.biosciencestack.com/static/projectframe/docs/index.html"
 keywords = ["project", "interval", "ailist", "frame"]
 readme = 'README.md'
@@ -25,29 +25,29 @@
                     "Topic :: Scientific/Engineering :: Bio-Informatics"
                   ]
 packages = [{ include = "projectframe" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
-cython = "^0.29.32"
-pandas = "^1.5.2"
-ailist = "^2.1.0"
+cython = "^3.0.0"
+pandas = "^2.0.0"
+ailist = "^2.1.3"
 tabulate = "^0.9.0"
-linear_segment = "^1.0.0"
-intervalframe = "^1.1.1"
+linear_segment = "^1.1.2"
+intervalframe = "^1.1.6"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
-            "cython>=0.29.32",
+            "cython>=3.0.0",
             "numpy>=1.23.5",
-            "pandas>=1.5.2",
+            "pandas>=2.0.0",
             "setuptools>=65.5.0",
             ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.cibuildwheel]
 skip = "cp36-* cp37-* cp38-* cp39-* pp37-* pp38-* *-manylinux_i686 *_ppc64le *_s390x *-musllinux*"
 build-verbosity = "3"
```

### Comparing `projectframe-1.0.0/PKG-INFO` & `projectframe-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectframe
-Version: 1.0.0
+Version: 1.0.2
 Summary: Python package for multi-dimensional tabular data
 Home-page: https://github.com/kylessmith/projectframe
 License: GPL-2.0-or-later
 Keywords: project,interval,ailist,frame
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -17,27 +17,27 @@
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ailist (>=2.1.0,<3.0.0)
-Requires-Dist: cython (>=0.29.32,<0.30.0)
-Requires-Dist: intervalframe (>=1.1.1,<2.0.0)
-Requires-Dist: linear_segment (>=1.0.0,<2.0.0)
+Requires-Dist: ailist (>=2.1.3,<3.0.0)
+Requires-Dist: cython (>=3.0.0,<4.0.0)
+Requires-Dist: intervalframe (>=1.1.6,<2.0.0)
+Requires-Dist: linear_segment (>=1.1.2,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/projectframe/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/projectframe
 Description-Content-Type: text/markdown
 
 # ProjectFrame for data manipulation
```

