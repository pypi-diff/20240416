# Comparing `tmp/SparseEdges-20240418.tar.gz` & `tmp/SparseEdges-20240419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SparseEdges-20240418.tar", last modified: Tue Apr 16 13:10:07 2024, max compression
+gzip compressed data, was "SparseEdges-20240419.tar", last modified: Tue Apr 16 13:23:43 2024, max compression
```

## Comparing `SparseEdges-20240418.tar` & `SparseEdges-20240419.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:10:07.525815 SparseEdges-20240418/
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     1082 2024-04-16 12:46:33.000000 SparseEdges-20240418/LICENSE
--rw-r--r--   0 laurentperrinet   (501) staff       (20)      117 2024-04-16 12:46:33.000000 SparseEdges-20240418/MANIFEST.in
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     1229 2024-04-16 13:10:07.525327 SparseEdges-20240418/PKG-INFO
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     1598 2024-04-16 12:46:33.000000 SparseEdges-20240418/README.md
-drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:10:07.522727 SparseEdges-20240418/SparseEdges/
--rw-r--r--   0 laurentperrinet   (501) staff       (20)    41182 2024-04-16 12:46:33.000000 SparseEdges-20240418/SparseEdges/EdgeFactory.py
--rw-r--r--   0 laurentperrinet   (501) staff       (20)    73544 2024-04-16 13:09:21.000000 SparseEdges-20240418/SparseEdges/SparseEdges.py
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     2339 2024-04-16 13:07:02.000000 SparseEdges-20240418/SparseEdges/__init__.py
-drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:10:07.524497 SparseEdges-20240418/SparseEdges.egg-info/
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     1229 2024-04-16 13:10:07.000000 SparseEdges-20240418/SparseEdges.egg-info/PKG-INFO
--rw-r--r--   0 laurentperrinet   (501) staff       (20)      290 2024-04-16 13:10:07.000000 SparseEdges-20240418/SparseEdges.egg-info/SOURCES.txt
--rw-r--r--   0 laurentperrinet   (501) staff       (20)        1 2024-04-16 13:10:07.000000 SparseEdges-20240418/SparseEdges.egg-info/dependency_links.txt
--rw-r--r--   0 laurentperrinet   (501) staff       (20)       46 2024-04-16 13:10:07.000000 SparseEdges-20240418/SparseEdges.egg-info/requires.txt
--rw-r--r--   0 laurentperrinet   (501) staff       (20)       12 2024-04-16 13:10:07.000000 SparseEdges-20240418/SparseEdges.egg-info/top_level.txt
--rw-r--r--   0 laurentperrinet   (501) staff       (20)       38 2024-04-16 13:10:07.525911 SparseEdges-20240418/setup.cfg
--rw-r--r--   0 laurentperrinet   (501) staff       (20)     1849 2024-04-16 12:46:33.000000 SparseEdges-20240418/setup.py
+drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:23:43.377436 SparseEdges-20240419/
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     1082 2024-04-16 12:46:33.000000 SparseEdges-20240419/LICENSE
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)      117 2024-04-16 12:46:33.000000 SparseEdges-20240419/MANIFEST.in
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     1229 2024-04-16 13:23:43.376961 SparseEdges-20240419/PKG-INFO
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     1598 2024-04-16 12:46:33.000000 SparseEdges-20240419/README.md
+drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:23:43.374396 SparseEdges-20240419/SparseEdges/
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)    41182 2024-04-16 12:46:33.000000 SparseEdges-20240419/SparseEdges/EdgeFactory.py
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)    73544 2024-04-16 13:10:39.000000 SparseEdges-20240419/SparseEdges/SparseEdges.py
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     2339 2024-04-16 13:10:50.000000 SparseEdges-20240419/SparseEdges/__init__.py
+drwxr-xr-x   0 laurentperrinet   (501) staff       (20)        0 2024-04-16 13:23:43.376134 SparseEdges-20240419/SparseEdges.egg-info/
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     1229 2024-04-16 13:23:43.000000 SparseEdges-20240419/SparseEdges.egg-info/PKG-INFO
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)      290 2024-04-16 13:23:43.000000 SparseEdges-20240419/SparseEdges.egg-info/SOURCES.txt
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)        1 2024-04-16 13:23:43.000000 SparseEdges-20240419/SparseEdges.egg-info/dependency_links.txt
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)       46 2024-04-16 13:23:43.000000 SparseEdges-20240419/SparseEdges.egg-info/requires.txt
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)       12 2024-04-16 13:23:43.000000 SparseEdges-20240419/SparseEdges.egg-info/top_level.txt
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)       38 2024-04-16 13:23:43.377563 SparseEdges-20240419/setup.cfg
+-rw-r--r--   0 laurentperrinet   (501) staff       (20)     1849 2024-04-16 12:46:33.000000 SparseEdges-20240419/setup.py
```

### Comparing `SparseEdges-20240418/LICENSE` & `SparseEdges-20240419/LICENSE`

 * *Files identical despite different names*

### Comparing `SparseEdges-20240418/PKG-INFO` & `SparseEdges-20240419/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SparseEdges
-Version: 20240418
+Version: 20240419
 Summary: SparseEdges: A bio-inspired sparse representation of edges in natural images.
 Home-page: https://github.com/bicv/SparseEdges
-Download-URL: https://github.com/bicv/SparseEdges/tarball/20240418
+Download-URL: https://github.com/bicv/SparseEdges/tarball/20240419
 Author: Laurent Perrinet INT - CNRS
 Author-email: Laurent.Perrinet@univ-amu.fr
 License: GPLv2
 Keywords: computational neuroscience,simulation,analysis,visualization,biologically-inspired,computer vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `SparseEdges-20240418/README.md` & `SparseEdges-20240419/README.md`

 * *Files identical despite different names*

### Comparing `SparseEdges-20240418/SparseEdges/EdgeFactory.py` & `SparseEdges-20240419/SparseEdges/EdgeFactory.py`

 * *Files identical despite different names*

### Comparing `SparseEdges-20240418/SparseEdges/SparseEdges.py` & `SparseEdges-20240419/SparseEdges/SparseEdges.py`

 * *Files identical despite different names*

### Comparing `SparseEdges-20240418/SparseEdges/__init__.py` & `SparseEdges-20240419/SparseEdges/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Laurent Perrinet INT - CNRS"
-__version__ = '20240418'
+__version__ = '20240419'
 __licence__ = 'GPLv2'
 from .SparseEdges import SparseEdges, KL, TV
 from .EdgeFactory import EdgeFactory
 
 def adjust_spines(ax, spines):
     for loc, spine in ax.spines.iteritems():
         if loc in spines:
```

### Comparing `SparseEdges-20240418/SparseEdges.egg-info/PKG-INFO` & `SparseEdges-20240419/SparseEdges.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: SparseEdges
-Version: 20240418
+Version: 20240419
 Summary: SparseEdges: A bio-inspired sparse representation of edges in natural images.
 Home-page: https://github.com/bicv/SparseEdges
-Download-URL: https://github.com/bicv/SparseEdges/tarball/20240418
+Download-URL: https://github.com/bicv/SparseEdges/tarball/20240419
 Author: Laurent Perrinet INT - CNRS
 Author-email: Laurent.Perrinet@univ-amu.fr
 License: GPLv2
 Keywords: computational neuroscience,simulation,analysis,visualization,biologically-inspired,computer vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `SparseEdges-20240418/setup.py` & `SparseEdges-20240419/setup.py`

 * *Files identical despite different names*

