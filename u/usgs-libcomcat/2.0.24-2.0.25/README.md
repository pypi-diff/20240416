# Comparing `tmp/usgs-libcomcat-2.0.24.tar.gz` & `tmp/usgs_libcomcat-2.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usgs-libcomcat-2.0.24.tar", last modified: Fri Apr  5 17:52:35 2024, max compression
+gzip compressed data, was "usgs_libcomcat-2.0.25.tar", last modified: Tue Apr 16 16:09:28 2024, max compression
```

## Comparing `usgs-libcomcat-2.0.24.tar` & `usgs_libcomcat-2.0.25.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2263 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       51 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3954 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1583 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/setup.cfg
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.906095 usgs-libcomcat-2.0.24/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.910095 usgs-libcomcat-2.0.24/src/libcomcat/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       93 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18456 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/_version.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.910095 usgs-libcomcat-2.0.24/src/libcomcat/bin/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:51:21.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/__init__.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     7957 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/findid.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    19989 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getcsv.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    16608 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/geteventhist.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8607 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getmags.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11005 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getpager.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12388 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getphases.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15973 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/bin/getproduct.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    42526 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/classes.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.914095 usgs-libcomcat-2.0.24/src/libcomcat/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/economy.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/fatality.xml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        5 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.cpg
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   546979 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.dbf
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      143 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.prj
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)  1612740 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shp
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2028 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    76040 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/dataframes.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      864 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/exceptions.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2278 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/logging.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25810 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/search.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      327 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/test_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11702 2024-04-05 17:33:03.000000 usgs-libcomcat-2.0.24/src/libcomcat/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-05 17:52:35.918095 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8030 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1079 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      295 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      380 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       15 2024-04-05 17:52:35.000000 usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.035595 usgs_libcomcat-2.0.25/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2263 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       51 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8024 2024-04-16 16:09:28.035595 usgs_libcomcat-2.0.25/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3954 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1577 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-16 16:09:28.035595 usgs_libcomcat-2.0.25/setup.cfg
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.023595 usgs_libcomcat-2.0.25/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.023595 usgs_libcomcat-2.0.25/src/libcomcat/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       93 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18456 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/_version.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.027595 usgs_libcomcat-2.0.25/src/libcomcat/bin/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/__init__.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     7957 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/findid.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    19989 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/getcsv.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    16608 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/geteventhist.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8607 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/getmags.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11005 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/getpager.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12388 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/getphases.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15973 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/bin/getproduct.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    42526 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/classes.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.031595 usgs_libcomcat-2.0.25/src/libcomcat/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   324036 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/economy.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   214515 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/fatality.xml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        5 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.cpg
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)   546979 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.dbf
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      143 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.prj
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)  1612740 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.shp
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2028 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.shx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    76040 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/dataframes.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      864 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/exceptions.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2278 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/logging.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25810 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/search.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      327 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/test_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11702 2024-04-16 16:08:07.000000 usgs_libcomcat-2.0.25/src/libcomcat/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-16 16:09:28.031595 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8024 2024-04-16 16:09:27.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     1079 2024-04-16 16:09:28.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-16 16:09:27.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      295 2024-04-16 16:09:27.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      380 2024-04-16 16:09:28.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       15 2024-04-16 16:09:28.000000 usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/top_level.txt
```

### Comparing `usgs-libcomcat-2.0.24/LICENSE.md` & `usgs_libcomcat-2.0.25/LICENSE.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/PKG-INFO` & `usgs_libcomcat-2.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.24
+Version: 2.0.25
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -57,15 +57,15 @@
         are in the public domain. You may use the maps in any manner, including
         modifying the content and design, electronic dissemination, and offset
         printing. The primary authors, Tom Patterson and Nathaniel Vaughn Kelso, and
         all other contributors renounce all financial claim to the maps and invites you
         to use them for personal, educational, and commercial purposes."
         
 Keywords: comcat,earthquake
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: esi_utils_geo
 Requires-Dist: esi_utils_time
 Requires-Dist: esi_utils_io
 Requires-Dist: fiona>=1.8.20
 Requires-Dist: h5py
```

### Comparing `usgs-libcomcat-2.0.24/README.md` & `usgs_libcomcat-2.0.25/README.md`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/pyproject.toml` & `usgs_libcomcat-2.0.25/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 description = "Python wrapper around ComCat web API"
 authors = [
     {name = "Mike Hearne", email="mhearne@usgs.gov"},
     {name = "Heather Hunsinger", email="hhunsinger@usgs.gov"},
 ]
 license = {file = "LICENSE.md"}
 readme = "README.md"
-requires-python = ">=3.7,<3.11"
+requires-python = ">=3.7"
 
 keywords = ["comcat", "earthquake"]
 
 dependencies = [
     "esi_utils_geo",
     "esi_utils_time",
     "esi_utils_io",
```

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/_version.py` & `usgs_libcomcat-2.0.25/src/libcomcat/_version.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/findid.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/findid.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/getcsv.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/getcsv.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/geteventhist.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/geteventhist.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/getmags.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/getmags.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/getpager.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/getpager.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/getphases.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/getphases.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/bin/getproduct.py` & `usgs_libcomcat-2.0.25/src/libcomcat/bin/getproduct.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/classes.py` & `usgs_libcomcat-2.0.25/src/libcomcat/classes.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/data/economy.xml` & `usgs_libcomcat-2.0.25/src/libcomcat/data/economy.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/data/fatality.xml` & `usgs_libcomcat-2.0.25/src/libcomcat/data/fatality.xml`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.dbf` & `usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.dbf`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shp` & `usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.shp`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/data/ne_50m_admin_0_countries.shx` & `usgs_libcomcat-2.0.25/src/libcomcat/data/ne_50m_admin_0_countries.shx`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/dataframes.py` & `usgs_libcomcat-2.0.25/src/libcomcat/dataframes.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/exceptions.py` & `usgs_libcomcat-2.0.25/src/libcomcat/exceptions.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/logging.py` & `usgs_libcomcat-2.0.25/src/libcomcat/logging.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/search.py` & `usgs_libcomcat-2.0.25/src/libcomcat/search.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/libcomcat/utils.py` & `usgs_libcomcat-2.0.25/src/libcomcat/utils.py`

 * *Files identical despite different names*

### Comparing `usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/PKG-INFO` & `usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usgs-libcomcat
-Version: 2.0.24
+Version: 2.0.25
 Summary: Python wrapper around ComCat web API
 Author-email: Mike Hearne <mhearne@usgs.gov>, Heather Hunsinger <hhunsinger@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -57,15 +57,15 @@
         are in the public domain. You may use the maps in any manner, including
         modifying the content and design, electronic dissemination, and offset
         printing. The primary authors, Tom Patterson and Nathaniel Vaughn Kelso, and
         all other contributors renounce all financial claim to the maps and invites you
         to use them for personal, educational, and commercial purposes."
         
 Keywords: comcat,earthquake
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: esi_utils_geo
 Requires-Dist: esi_utils_time
 Requires-Dist: esi_utils_io
 Requires-Dist: fiona>=1.8.20
 Requires-Dist: h5py
```

### Comparing `usgs-libcomcat-2.0.24/src/usgs_libcomcat.egg-info/SOURCES.txt` & `usgs_libcomcat-2.0.25/src/usgs_libcomcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

