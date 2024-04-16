# Comparing `tmp/ckanext-dcor_depot-0.9.8.tar.gz` & `tmp/ckanext-dcor_depot-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-dcor_depot-0.9.8.tar", last modified: Tue Oct 26 12:16:12 2021, max compression
+gzip compressed data, was "ckanext-dcor_depot-0.9.9.tar", last modified: Tue Oct 26 15:04:23 2021, max compression
```

## Comparing `ckanext-dcor_depot-0.9.8.tar` & `ckanext-dcor_depot-0.9.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.610464 ckanext-dcor_depot-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      157 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-26 12:16:12.610464 ckanext-dcor_depot-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4392 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.606464 ckanext-dcor_depot-0.9.8/ckanext/
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.606464 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-10-26 12:15:43.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/_version_save.py
--rw-r--r--   0 runner    (1001) docker     (121)     4711 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.606464 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/
--rw-r--r--   0 runner    (1001) docker     (121)     4195 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6782 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     7319 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     9481 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan_ancillaries_hdf5.json
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan_ancillaries_tdms.json
--rw-r--r--   0 runner    (1001) docker     (121)      500 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan_associate_tdms.json
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan_ignore.json
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/unpack.py
--rw-r--r--   0 runner    (1001) docker     (121)     7578 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/figshare.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/figshare_dois.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13314 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/internal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1031 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/orgs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.606464 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1572 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_depotize_archive.py
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_internal_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_internal_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      114 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 12:16:12.610464 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-26 12:16:12.000000 ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-26 12:16:12.610464 ckanext-dcor_depot-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2021-10-26 12:15:34.000000 ckanext-dcor_depot-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.538042 ckanext-dcor_depot-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3618 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-26 15:04:23.538042 ckanext-dcor_depot-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4392 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.534042 ckanext-dcor_depot-0.9.9/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.534042 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7095 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2021-10-26 15:03:49.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/_version_save.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4711 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.534042 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/
+-rw-r--r--   0 runner    (1001) docker     (121)     4195 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6782 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7319 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9481 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan_ancillaries_hdf5.json
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan_ancillaries_tdms.json
+-rw-r--r--   0 runner    (1001) docker     (121)      500 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan_associate_tdms.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan_ignore.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/unpack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7578 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/figshare.py
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/figshare_dois.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13314 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/internal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/orgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.534042 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1572 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_depotize_archive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_internal_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_internal_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2509 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-26 15:04:23.538042 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4858 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-26 15:04:23.000000 ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-26 15:04:23.538042 ckanext-dcor_depot-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2228 2021-10-26 15:03:35.000000 ckanext-dcor_depot-0.9.9/setup.py
```

### Comparing `ckanext-dcor_depot-0.9.8/CHANGELOG` & `ckanext-dcor_depot-0.9.9/CHANGELOG`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.9.9
+ - fix: avoid race conditions during symlinking
 0.9.8
  - fix: support calling symlink_user_dataset twice
 0.9.7
  - fix: upgrade_internal CLI did not work if non-.rtdc files
    (e.g. unimportant images) were missing
 0.9.6
  - ref: change background job ID to "{package_id}_{position}_symlink"
```

### Comparing `ckanext-dcor_depot-0.9.8/LICENSE` & `ckanext-dcor_depot-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/PKG-INFO` & `ckanext-dcor_depot-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dcor_depot
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manages data storage for CKAN/DCOR (import, symlink, etc.)
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_depot
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dcor_depot-0.9.8/README.rst` & `ckanext-dcor_depot-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/_version.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/_version.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/cli.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depot.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depot.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/__init__.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/__init__.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/check.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/check.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/convert.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/convert.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/scan_ignore.json` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/scan_ignore.json`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/depotize/unpack.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/depotize/unpack.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/figshare.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/figshare.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/internal.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/internal.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/jobs.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/jobs.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,10 +21,19 @@
                   / pkg["id"][2:4]
                   / "{}_{}_{}".format(pkg["name"],
                                       resource["id"],
                                       resource["name"]))
     if not depot_path.parent.exists():
         depot_path.parent.mkdir(exist_ok=True, parents=True)
     # move file to depot and create symlink back
-    path = pathlib.Path(path)
-    path.rename(depot_path)
-    path.symlink_to(depot_path)
+    try:
+        path.rename(depot_path)
+    except FileNotFoundError:
+        # somebody else was faster (avoid race conditions)
+        if not depot_path.exists():
+            raise
+    try:
+        path.symlink_to(depot_path)
+    except FileNotFoundError:
+        # somebody else was faster (avoid race conditions)
+        if not path.is_symlink():
+            raise
```

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/paths.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/paths.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/plugin.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/helper_methods.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_depotize_archive.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_depotize_archive.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_internal_import.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_internal_import.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_internal_upgrade.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_internal_upgrade.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_jobs.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext/dcor_depot/tests/test_scan.py` & `ckanext-dcor_depot-0.9.9/ckanext/dcor_depot/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/PKG-INFO` & `ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-dcor-depot
-Version: 0.9.8
+Version: 0.9.9
 Summary: Manages data storage for CKAN/DCOR (import, symlink, etc.)
 Home-page: https://github.com/DCOR-dev/ckanext-dcor_depot
 Author: Paul Müller
 Author-email: dev@craban.de
 License: AGPLv3+
 Keywords: CKAN,DCOR,RT-DC
 Platform: UNKNOWN
```

### Comparing `ckanext-dcor_depot-0.9.8/ckanext_dcor_depot.egg-info/SOURCES.txt` & `ckanext-dcor_depot-0.9.9/ckanext_dcor_depot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-dcor_depot-0.9.8/setup.py` & `ckanext-dcor_depot-0.9.9/setup.py`

 * *Files identical despite different names*

