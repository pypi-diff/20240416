# Comparing `tmp/dtool_ibeis-1.1.1.tar.gz` & `tmp/dtool_ibeis-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtool_ibeis-1.1.1.tar", last modified: Sun Jan 29 16:29:59 2023, max compression
+gzip compressed data, was "dtool_ibeis-1.1.2.tar", last modified: Tue Apr 16 04:13:58 2024, max compression
```

## Comparing `dtool_ibeis-1.1.1.tar` & `dtool_ibeis-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:29:59.809892 dtool_ibeis-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-01-29 16:29:59.809892 dtool_ibeis-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:29:59.809892 dtool_ibeis-1.1.1/dtool_ibeis/
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/__SQLITE__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      488 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39616 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    65949 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/depcache_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/depcache_object.py
--rw-r--r--   0 runner    (1001) docker     (123)   116757 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/depcache_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    25424 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/example_depcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/example_depcache2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/experimental_features.py
--rw-r--r--   0 runner    (1001) docker     (123)    34624 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/input_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   126252 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/sql_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/dtool_ibeis/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 16:29:59.809892 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-01-29 16:29:59.000000 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-29 16:29:59.000000 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 16:29:59.000000 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-01-29 16:29:59.000000 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-29 16:29:59.000000 dtool_ibeis-1.1.1/dtool_ibeis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 16:29:59.809892 dtool_ibeis-1.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9294 2023-01-29 16:29:53.000000 dtool_ibeis-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:13:58.185513 dtool_ibeis-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23650 2024-04-16 04:13:58.185513 dtool_ibeis-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:13:58.145513 dtool_ibeis-1.1.2/dtool_ibeis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/__SQLITE__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39616 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65949 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/depcache_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/depcache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116757 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/depcache_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25598 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/example_depcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8579 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/example_depcache2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/experimental_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34624 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/input_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126252 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/sql_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/dtool_ibeis/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:13:58.149513 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23650 2024-04-16 04:13:58.000000 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 04:13:58.000000 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:13:58.000000 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-04-16 04:13:58.000000 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 04:13:58.000000 dtool_ibeis-1.1.2/dtool_ibeis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 04:13:58.185513 dtool_ibeis-1.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9648 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:13:58.149513 dtool_ibeis-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 04:12:54.000000 dtool_ibeis-1.1.2/tests/test_import.py
```

### Comparing `dtool_ibeis-1.1.1/LICENSE` & `dtool_ibeis-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/README.rst` & `dtool_ibeis-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/__SQLITE__.py` & `dtool_ibeis-1.1.2/dtool_ibeis/__SQLITE__.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/base.py` & `dtool_ibeis-1.1.2/dtool_ibeis/base.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/depcache_control.py` & `dtool_ibeis-1.1.2/dtool_ibeis/depcache_control.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/depcache_object.py` & `dtool_ibeis-1.1.2/dtool_ibeis/depcache_object.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/depcache_table.py` & `dtool_ibeis-1.1.2/dtool_ibeis/depcache_table.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/example_depcache.py` & `dtool_ibeis-1.1.2/dtool_ibeis/example_depcache.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,18 @@
 def testdata_depc(fname=None):
     """
     Example of local registration
     """
 
     import dtool_ibeis
     import vtool_ibeis as vt
-    gpath_list = ut.lmap(ut.grab_test_imgpath, ut.get_valid_test_imgkeys(),
+    # imgkeys = ut.get_valid_test_imgkeys()
+    imgkeys = ['airport', 'amazon', 'astro', 'carl', 'lowcontrast', 'paraview',
+               'parrot', 'pm5644', 'stars', 'tsukuba_l', 'tsukuba_r']
+    gpath_list = ut.lmap(ut.grab_test_imgpath, imgkeys,
                          verbose=False)
 
     dummy_root = 'dummy_annot'
 
     def get_root_uuid(aid_list):
         return ut.lmap(ut.hashable_to_uuid, aid_list)
```

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/example_depcache2.py` & `dtool_ibeis-1.1.2/dtool_ibeis/example_depcache2.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/experimental_features.py` & `dtool_ibeis-1.1.2/dtool_ibeis/experimental_features.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/input_helpers.py` & `dtool_ibeis-1.1.2/dtool_ibeis/input_helpers.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/sql_control.py` & `dtool_ibeis-1.1.2/dtool_ibeis/sql_control.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis/util.py` & `dtool_ibeis-1.1.2/dtool_ibeis/util.py`

 * *Files identical despite different names*

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis.egg-info/SOURCES.txt` & `dtool_ibeis-1.1.2/dtool_ibeis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 dtool_ibeis/input_helpers.py
 dtool_ibeis/sql_control.py
 dtool_ibeis/util.py
 dtool_ibeis.egg-info/PKG-INFO
 dtool_ibeis.egg-info/SOURCES.txt
 dtool_ibeis.egg-info/dependency_links.txt
 dtool_ibeis.egg-info/requires.txt
-dtool_ibeis.egg-info/top_level.txt
+dtool_ibeis.egg-info/top_level.txt
+tests/test_import.py
```

### Comparing `dtool_ibeis-1.1.1/dtool_ibeis.egg-info/requires.txt` & `dtool_ibeis-1.1.2/dtool_ibeis.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,167 +1,195 @@
-ubelt
-utool
+ubelt>=1.3.4
+utool>=2.2.0
 
 [:python_version < "3.10" and python_version >= "3.9"]
-cachetools
+cachetools>=4.2.0
 
 [:python_version < "3.11" and python_version >= "3.10"]
-cachetools
+cachetools>=5.0.0
 
 [:python_version < "3.7" and python_version >= "3.6"]
-cachetools
+cachetools>=4.0.0
 
 [:python_version < "3.8" and python_version >= "3.7"]
-cachetools
+cachetools>=5.0.0
 
 [:python_version < "3.9" and python_version >= "3.8"]
-cachetools
+cachetools>=4.0.0
 
 [:python_version < "4.0" and python_version >= "3.11"]
-cachetools
+cachetools>=5.0.0
 
 [all]
-codecov
-guitool_ibeis
-pytest-timeout
-requests
-ubelt
-utool
-vtool_ibeis
-xdoctest
+ubelt>=1.3.4
+utool>=2.2.0
+xdoctest>=1.1.3
+pytest-timeout>=1.4.2
+requests>=2.27.1
+vtool_ibeis>=2.3.0
+guitool_ibeis>=2.2.0
 
 [all-strict]
-codecov==2.0.15
-guitool_ibeis==2.1.2
+ubelt==1.3.4
+utool==2.2.0
+xdoctest==1.1.3
 pytest-timeout==1.4.2
-requests==2.25.1
-ubelt==1.2.2
-utool==2.1.7
-vtool_ibeis==2.2.0
-xdoctest==0.14.0
+requests==2.27.1
+vtool_ibeis==2.3.0
+guitool_ibeis==2.2.0
 
 [all-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [all-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.10" and python_version >= "3.9"]
 cachetools==4.2.0
+pytest==8.1.1
 coverage==5.3.1
 
-[all-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
-
 [all-strict:python_version < "3.11" and python_version >= "3.10"]
 cachetools==5.0.0
-pytest==6.2.5
+pytest==8.1.1
+
+[all-strict:python_version < "3.12" and python_version >= "3.11"]
+pytest==8.1.1
+
+[all-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [all-strict:python_version < "3.4" and python_version >= "2.7"]
 coverage==5.3.1
 
 [all-strict:python_version < "3.5" and python_version >= "3.4"]
 coverage==4.3.4
 
 [all-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.6" and python_version >= "3.5"]
 coverage==5.3.1
 
 [all-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [all-strict:python_version < "3.7" and python_version >= "3.6"]
 cachetools==4.0.0
 coverage==6.1.1
 
-[all-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
-
 [all-strict:python_version < "3.8" and python_version >= "3.7"]
 cachetools==5.0.0
+pytest==4.6.0
 coverage==6.1.1
 
 [all-strict:python_version < "3.9" and python_version >= "3.8"]
 cachetools==4.0.0
+pytest==8.1.1
 coverage==6.1.1
 
 [all-strict:python_version < "4.0" and python_version >= "3.11"]
 cachetools==5.0.0
-pytest==7.0.0
+
+[all-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
 
 [all-strict:python_version >= "3.10"]
 coverage==6.1.1
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [all:python_version < "2.7" and python_version >= "2.6"]
-coverage
+coverage>=4.5
 
 [all:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.10" and python_version >= "3.9"]
-cachetools
-coverage
-
-[all:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+cachetools>=4.2.0
+pytest>=8.1.1
+coverage>=5.3.1
 
 [all:python_version < "3.11" and python_version >= "3.10"]
-cachetools
-pytest
+cachetools>=5.0.0
+pytest>=8.1.1
+
+[all:python_version < "3.12" and python_version >= "3.11"]
+pytest>=8.1.1
+
+[all:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [all:python_version < "3.4" and python_version >= "2.7"]
-coverage
+coverage>=5.3.1
 
 [all:python_version < "3.5" and python_version >= "3.4"]
-coverage
+coverage>=4.3.4
 
 [all:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.6" and python_version >= "3.5"]
-coverage
+coverage>=5.3.1
 
 [all:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [all:python_version < "3.7" and python_version >= "3.6"]
-cachetools
-coverage
-
-[all:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+cachetools>=4.0.0
+coverage>=6.1.1
 
 [all:python_version < "3.8" and python_version >= "3.7"]
-cachetools
-coverage
+cachetools>=5.0.0
+pytest>=4.6.0
+coverage>=6.1.1
 
 [all:python_version < "3.9" and python_version >= "3.8"]
-cachetools
-coverage
+cachetools>=4.0.0
+pytest>=8.1.1
+coverage>=6.1.1
 
 [all:python_version < "4.0" and python_version >= "3.11"]
-cachetools
-pytest
+cachetools>=5.0.0
+
+[all:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
 [all:python_version >= "3.10"]
-coverage
+coverage>=6.1.1
 
 [all:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
+
+[docs]
+sphinx>=5.0.1
+sphinx-autobuild>=2021.3.14
+sphinx_rtd_theme>=1.0.0
+sphinxcontrib-napoleon>=0.7
+sphinx-autoapi>=1.8.4
+Pygments>=2.9.0
+myst_parser>=0.18.0
+sphinx-reredirects>=0.0.1
+
+[docs-strict]
+sphinx==5.0.1
+sphinx-autobuild==2021.3.14
+sphinx_rtd_theme==1.0.0
+sphinxcontrib-napoleon==0.7
+sphinx-autoapi==1.8.4
+Pygments==2.9.0
+myst_parser==0.18.0
+sphinx-reredirects==0.0.1
 
 [graphics]
 
 [graphics-strict]
 
 [graphics-strict:python_version < "3.10" and python_version >= "3.9"]
 opencv-python==3.4.15.55
@@ -187,39 +215,39 @@
 [graphics-strict:python_version < "3.9" and python_version >= "3.8"]
 opencv-python==3.4.15.55
 
 [graphics-strict:python_version < "4.0" and python_version >= "3.11"]
 opencv-python==4.5.5.64
 
 [graphics:python_version < "3.10" and python_version >= "3.9"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "3.11" and python_version >= "3.10"]
-opencv-python
+opencv-python>=4.5.4.58
 
 [graphics:python_version < "3.4" and python_version >= "2.7"]
-opencv-python
+opencv-python>=3.1.0.0
 
 [graphics:python_version < "3.5" and python_version >= "3.4"]
-opencv-python
+opencv-python>=3.1.0.5
 
 [graphics:python_version < "3.6" and python_version >= "3.5"]
-opencv-python
+opencv-python>=3.1.0.2
 
 [graphics:python_version < "3.7" and python_version >= "3.6"]
-opencv-python
+opencv-python>=3.4.13.47
 
 [graphics:python_version < "3.8" and python_version >= "3.7"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "3.9" and python_version >= "3.8"]
-opencv-python
+opencv-python>=3.4.15.55
 
 [graphics:python_version < "4.0" and python_version >= "3.11"]
-opencv-python
+opencv-python>=4.5.5.64
 
 [headless]
 
 [headless-strict]
 
 [headless-strict:python_version < "3.10" and python_version >= "3.9"]
 opencv-python-headless==3.4.15.55
@@ -245,49 +273,53 @@
 [headless-strict:python_version < "3.9" and python_version >= "3.8"]
 opencv-python-headless==3.4.15.55
 
 [headless-strict:python_version < "4.0" and python_version >= "3.11"]
 opencv-python-headless==4.5.5.64
 
 [headless:python_version < "3.10" and python_version >= "3.9"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "3.11" and python_version >= "3.10"]
-opencv-python-headless
+opencv-python-headless>=4.5.4.58
 
 [headless:python_version < "3.4" and python_version >= "2.7"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.5" and python_version >= "3.4"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.6" and python_version >= "3.5"]
-opencv-python-headless
+opencv-python-headless>=3.4.2.16
 
 [headless:python_version < "3.7" and python_version >= "3.6"]
-opencv-python-headless
+opencv-python-headless>=3.4.13.47
 
 [headless:python_version < "3.8" and python_version >= "3.7"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "3.9" and python_version >= "3.8"]
-opencv-python-headless
+opencv-python-headless>=3.4.15.55
 
 [headless:python_version < "4.0" and python_version >= "3.11"]
-opencv-python-headless
+opencv-python-headless>=4.5.5.64
 
 [optional]
-guitool_ibeis
+guitool_ibeis>=2.2.0
 
 [optional-strict]
-guitool_ibeis==2.1.2
+guitool_ibeis==2.2.0
+
+[runtime]
+ubelt>=1.3.4
+utool>=2.2.0
 
 [runtime-strict]
-ubelt==1.2.2
-utool==2.1.7
+ubelt==1.3.4
+utool==2.2.0
 
 [runtime-strict:python_version < "3.10" and python_version >= "3.9"]
 cachetools==4.2.0
 
 [runtime-strict:python_version < "3.11" and python_version >= "3.10"]
 cachetools==5.0.0
 
@@ -299,128 +331,150 @@
 
 [runtime-strict:python_version < "3.9" and python_version >= "3.8"]
 cachetools==4.0.0
 
 [runtime-strict:python_version < "4.0" and python_version >= "3.11"]
 cachetools==5.0.0
 
+[runtime:python_version < "3.10" and python_version >= "3.9"]
+cachetools>=4.2.0
+
+[runtime:python_version < "3.11" and python_version >= "3.10"]
+cachetools>=5.0.0
+
+[runtime:python_version < "3.7" and python_version >= "3.6"]
+cachetools>=4.0.0
+
+[runtime:python_version < "3.8" and python_version >= "3.7"]
+cachetools>=5.0.0
+
+[runtime:python_version < "3.9" and python_version >= "3.8"]
+cachetools>=4.0.0
+
+[runtime:python_version < "4.0" and python_version >= "3.11"]
+cachetools>=5.0.0
+
 [tests]
-codecov
-pytest-timeout
-requests
-vtool_ibeis
-xdoctest
+xdoctest>=1.1.3
+pytest-timeout>=1.4.2
+requests>=2.27.1
+vtool_ibeis>=2.3.0
 
 [tests-strict]
-codecov==2.0.15
+xdoctest==1.1.3
 pytest-timeout==1.4.2
-requests==2.25.1
-vtool_ibeis==2.2.0
-xdoctest==0.14.0
+requests==2.27.1
+vtool_ibeis==2.3.0
 
 [tests-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [tests-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.10" and python_version >= "3.9"]
+pytest==8.1.1
 coverage==5.3.1
 
-[tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
-
 [tests-strict:python_version < "3.11" and python_version >= "3.10"]
-pytest==6.2.5
+pytest==8.1.1
+
+[tests-strict:python_version < "3.12" and python_version >= "3.11"]
+pytest==8.1.1
+
+[tests-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [tests-strict:python_version < "3.4" and python_version >= "2.7"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.5" and python_version >= "3.4"]
 coverage==4.3.4
 
 [tests-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.6" and python_version >= "3.5"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [tests-strict:python_version < "3.7" and python_version >= "3.6"]
 coverage==6.1.1
 
-[tests-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
-
 [tests-strict:python_version < "3.8" and python_version >= "3.7"]
+pytest==4.6.0
 coverage==6.1.1
 
 [tests-strict:python_version < "3.9" and python_version >= "3.8"]
+pytest==8.1.1
 coverage==6.1.1
 
-[tests-strict:python_version < "4.0" and python_version >= "3.11"]
-pytest==7.0.0
+[tests-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
 
 [tests-strict:python_version >= "3.10"]
 coverage==6.1.1
 
 [tests-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [tests:python_version < "2.7" and python_version >= "2.6"]
-coverage
+coverage>=4.5
 
 [tests:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.10" and python_version >= "3.9"]
-coverage
-
-[tests:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+pytest>=8.1.1
+coverage>=5.3.1
 
 [tests:python_version < "3.11" and python_version >= "3.10"]
-pytest
+pytest>=8.1.1
+
+[tests:python_version < "3.12" and python_version >= "3.11"]
+pytest>=8.1.1
+
+[tests:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [tests:python_version < "3.4" and python_version >= "2.7"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.5" and python_version >= "3.4"]
-coverage
+coverage>=4.3.4
 
 [tests:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.6" and python_version >= "3.5"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [tests:python_version < "3.7" and python_version >= "3.6"]
-coverage
-
-[tests:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+coverage>=6.1.1
 
 [tests:python_version < "3.8" and python_version >= "3.7"]
-coverage
+pytest>=4.6.0
+coverage>=6.1.1
 
 [tests:python_version < "3.9" and python_version >= "3.8"]
-coverage
+pytest>=8.1.1
+coverage>=6.1.1
 
-[tests:python_version < "4.0" and python_version >= "3.11"]
-pytest
+[tests:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
 [tests:python_version >= "3.10"]
-coverage
+coverage>=6.1.1
 
 [tests:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
```

### Comparing `dtool_ibeis-1.1.1/pyproject.toml` & `dtool_ibeis-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,34 @@
 [tool.xcookie]
 tags = [ "erotemic", "purepy", "github", "cv2"]
 mod_name = "dtool_ibeis"
 repo_name = "dtool_ibeis"
 rel_mod_parent_dpath = "."
 os = [ "linux", "osx", "win",]
 ci_pypy_versions = []
-supported_python_versions = ["3.7", "3.8", "3.9", "3.10", "3.11"]
 description = "dtool_ibeis - a dependency aware cache for ibeis"
 url="https://github.com/Erotemic/dtool_ibeis"
 author="Jon Crall"
+min_python = 3.8
 author_email="erotemic@gmail.com"
 dev_status = "beta"
 license = "Apache 2"
 autostage = true
 version = "{mod_dpath}/__init__.py::__version__"
 
 [tool.pytest.ini_options]
-addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
-filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
+addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=docs"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
+filterwarnings = [
+    "default",
+    "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning",
+    "ignore:.*Define the __nice__ method for.*:Warning",
+    "ignore:.*private pytest class or function.*:Warning",
+]
+
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
 omit = [ "dtool_ibeis/__main__.py", "*/setup.py",]
```

### Comparing `dtool_ibeis-1.1.1/setup.py` & `dtool_ibeis-1.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Generated by ~/code/xcookie/xcookie/builders/setup.py
 # based on part ~/code/xcookie/xcookie/rc/setup.py.in
 import sys
-from os.path import exists
+import re
+from os.path import exists, dirname, join
 from setuptools import find_packages
 from setuptools import setup
 
 
 def parse_version(fpath):
     """
     Statically parse the version number from a python file
@@ -49,16 +50,14 @@
     """
     Parse the description in the README file
 
     CommandLine:
         pandoc --from=markdown --to=rst --output=README.rst README.md
         python -c "import setup; print(setup.parse_description())"
     """
-    from os.path import dirname, join, exists
-
     readme_fpath = join(dirname(__file__), "README.rst")
     # This breaks on pip install, so check that it exists.
     if exists(readme_fpath):
         with open(readme_fpath, "r") as f:
             text = f.read()
         return text
     return ""
@@ -73,18 +72,18 @@
         fname (str): path to requirements file
         versions (bool | str, default=False):
             If true include version specs.
             If strict, then pin to the minimum version.
 
     Returns:
         List[str]: list of requirements items
-    """
-    from os.path import exists, dirname, join
-    import re
 
+    CommandLine:
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
+    """
     require_fpath = fname
 
     def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
 
         line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
@@ -194,60 +193,63 @@
 #             raise KeyError(versions)
 #     requirements = [r.replace(' ', '') for r in requirements]
 #     return requirements
 
 
 NAME = "dtool_ibeis"
 INIT_PATH = "dtool_ibeis/__init__.py"
-VERSION = parse_version("dtool_ibeis/__init__.py")
+VERSION = parse_version(INIT_PATH)
 
 if __name__ == "__main__":
     setupkw = {}
 
-    setupkw["install_requires"] = parse_requirements("requirements/runtime.txt")
+    setupkw["install_requires"] = parse_requirements(
+        "requirements/runtime.txt", versions="loose"
+    )
     setupkw["extras_require"] = {
-        "all": parse_requirements("requirements.txt"),
-        "tests": parse_requirements("requirements/tests.txt"),
-        "optional": parse_requirements("requirements/optional.txt"),
-        "headless": parse_requirements("requirements/headless.txt"),
-        "graphics": parse_requirements("requirements/graphics.txt"),
-        # Strict versions
+        "all": parse_requirements("requirements.txt", versions="loose"),
+        "headless": parse_requirements("requirements/headless.txt", versions="loose"),
+        "graphics": parse_requirements("requirements/graphics.txt", versions="loose"),
+        "docs": parse_requirements("requirements/docs.txt", versions="loose"),
+        "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+        "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+        "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+        "all-strict": parse_requirements("requirements.txt", versions="strict"),
         "headless-strict": parse_requirements(
             "requirements/headless.txt", versions="strict"
         ),
         "graphics-strict": parse_requirements(
             "requirements/graphics.txt", versions="strict"
         ),
-        "all-strict": parse_requirements("requirements.txt", versions="strict"),
+        "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
+        "optional-strict": parse_requirements(
+            "requirements/optional.txt", versions="strict"
+        ),
         "runtime-strict": parse_requirements(
             "requirements/runtime.txt", versions="strict"
         ),
         "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
-        "optional-strict": parse_requirements(
-            "requirements/optional.txt", versions="strict"
-        ),
     }
-
     setupkw["name"] = NAME
     setupkw["version"] = VERSION
     setupkw["author"] = "Jon Crall"
     setupkw["author_email"] = "erotemic@gmail.com"
     setupkw["url"] = "https://github.com/Erotemic/dtool_ibeis"
     setupkw["description"] = "dtool_ibeis - a dependency aware cache for ibeis"
     setupkw["long_description"] = parse_description()
     setupkw["long_description_content_type"] = "text/x-rst"
     setupkw["license"] = "Apache 2"
     setupkw["packages"] = find_packages(".")
-    setupkw["python_requires"] = ">=3.7"
+    setupkw["python_requires"] = ">=3.8"
     setupkw["classifiers"] = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ]
     setup(**setupkw)
```

