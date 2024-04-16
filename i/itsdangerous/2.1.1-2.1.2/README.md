# Comparing `tmp/itsdangerous-2.1.1.tar.gz` & `tmp/itsdangerous-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "itsdangerous-2.1.1.tar", last modified: Wed Mar  9 16:23:31 2022, max compression
+gzip compressed data, was "itsdangerous-2.1.2.tar", last modified: Thu Mar 24 15:11:46 2022, max compression
```

## Comparing `itsdangerous-2.1.1.tar` & `itsdangerous-2.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.898426 itsdangerous-2.1.1/
--rw-r--r--   0 david     (1000) david     (1000)     6961 2022-03-09 16:21:58.000000 itsdangerous-2.1.1/CHANGES.rst
--rw-r--r--   0 david     (1000) david     (1000)     1475 2020-04-15 00:11:47.000000 itsdangerous-2.1.1/LICENSE.rst
--rw-r--r--   0 david     (1000) david     (1000)      159 2021-02-24 17:21:29.000000 itsdangerous-2.1.1/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)     2928 2022-03-09 16:23:31.898426 itsdangerous-2.1.1/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1813 2022-02-16 18:56:13.000000 itsdangerous-2.1.1/README.rst
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.895093 itsdangerous-2.1.1/docs/
--rw-r--r--   0 david     (1000) david     (1000)      581 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/Makefile
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.895093 itsdangerous-2.1.1/docs/_static/
--rw-r--r--   0 david     (1000) david     (1000)     6629 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/_static/itsdangerous-logo-sidebar.png
--rw-r--r--   0 david     (1000) david     (1000)    18971 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/_static/itsdangerous-logo.png
--rw-r--r--   0 david     (1000) david     (1000)       45 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/changes.rst
--rw-r--r--   0 david     (1000) david     (1000)     5230 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/concepts.rst
--rw-r--r--   0 david     (1000) david     (1000)     2097 2021-05-21 03:28:07.000000 itsdangerous-2.1.1/docs/conf.py
--rw-r--r--   0 david     (1000) david     (1000)      139 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/encoding.rst
--rw-r--r--   0 david     (1000) david     (1000)      332 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/exceptions.rst
--rw-r--r--   0 david     (1000) david     (1000)     1654 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/index.rst
--rw-r--r--   0 david     (1000) david     (1000)       71 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/license.rst
--rw-r--r--   0 david     (1000) david     (1000)      752 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/docs/make.bat
--rw-r--r--   0 david     (1000) david     (1000)     3485 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/serializer.rst
--rw-r--r--   0 david     (1000) david     (1000)     1263 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/signer.rst
--rw-r--r--   0 david     (1000) david     (1000)      689 2020-05-12 23:46:49.000000 itsdangerous-2.1.1/docs/timed.rst
--rw-r--r--   0 david     (1000) david     (1000)      615 2020-04-15 00:11:47.000000 itsdangerous-2.1.1/docs/url_safe.rst
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.895093 itsdangerous-2.1.1/requirements/
--rw-r--r--   0 david     (1000) david     (1000)     1048 2022-02-16 18:57:23.000000 itsdangerous-2.1.1/requirements/dev.txt
--rw-r--r--   0 david     (1000) david     (1000)     1349 2022-02-16 18:57:19.000000 itsdangerous-2.1.1/requirements/docs.txt
--rw-r--r--   0 david     (1000) david     (1000)      551 2022-02-16 18:57:20.000000 itsdangerous-2.1.1/requirements/tests.txt
--rw-r--r--   0 david     (1000) david     (1000)      299 2022-02-16 18:57:20.000000 itsdangerous-2.1.1/requirements/typing.txt
--rw-r--r--   0 david     (1000) david     (1000)     2022 2022-03-09 16:23:31.898426 itsdangerous-2.1.1/setup.cfg
--rw-r--r--   0 david     (1000) david     (1000)       57 2020-04-15 00:53:14.000000 itsdangerous-2.1.1/setup.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.891759 itsdangerous-2.1.1/src/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.895093 itsdangerous-2.1.1/src/itsdangerous/
--rw-r--r--   0 david     (1000) david     (1000)      876 2022-03-09 16:21:58.000000 itsdangerous-2.1.1/src/itsdangerous/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)      450 2022-02-16 18:56:11.000000 itsdangerous-2.1.1/src/itsdangerous/_json.py
--rw-r--r--   0 david     (1000) david     (1000)     1419 2021-10-06 15:02:22.000000 itsdangerous-2.1.1/src/itsdangerous/encoding.py
--rw-r--r--   0 david     (1000) david     (1000)     3206 2021-05-11 02:32:43.000000 itsdangerous-2.1.1/src/itsdangerous/exc.py
--rw-r--r--   0 david     (1000) david     (1000)        0 2020-08-31 19:21:18.000000 itsdangerous-2.1.1/src/itsdangerous/py.typed
--rw-r--r--   0 david     (1000) david     (1000)    11144 2021-10-06 15:02:22.000000 itsdangerous-2.1.1/src/itsdangerous/serializer.py
--rw-r--r--   0 david     (1000) david     (1000)     9367 2021-05-18 15:11:39.000000 itsdangerous-2.1.1/src/itsdangerous/signer.py
--rw-r--r--   0 david     (1000) david     (1000)     8109 2022-03-09 16:11:24.000000 itsdangerous-2.1.1/src/itsdangerous/timed.py
--rw-r--r--   0 david     (1000) david     (1000)     2402 2021-10-06 15:02:22.000000 itsdangerous-2.1.1/src/itsdangerous/url_safe.py
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.895093 itsdangerous-2.1.1/src/itsdangerous.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)     2928 2022-03-09 16:23:31.000000 itsdangerous-2.1.1/src/itsdangerous.egg-info/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     1101 2022-03-09 16:23:31.000000 itsdangerous-2.1.1/src/itsdangerous.egg-info/SOURCES.txt
--rw-r--r--   0 david     (1000) david     (1000)        1 2022-03-09 16:23:31.000000 itsdangerous-2.1.1/src/itsdangerous.egg-info/dependency_links.txt
--rw-r--r--   0 david     (1000) david     (1000)       13 2022-03-09 16:23:31.000000 itsdangerous-2.1.1/src/itsdangerous.egg-info/top_level.txt
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.891759 itsdangerous-2.1.1/tests/
-drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-09 16:23:31.898426 itsdangerous-2.1.1/tests/test_itsdangerous/
--rw-r--r--   0 david     (1000) david     (1000)        0 2019-09-07 13:33:04.000000 itsdangerous-2.1.1/tests/test_itsdangerous/__init__.py
--rw-r--r--   0 david     (1000) david     (1000)     1004 2020-08-31 16:15:39.000000 itsdangerous-2.1.1/tests/test_itsdangerous/test_encoding.py
--rw-r--r--   0 david     (1000) david     (1000)     6830 2020-08-31 19:21:18.000000 itsdangerous-2.1.1/tests/test_itsdangerous/test_serializer.py
--rw-r--r--   0 david     (1000) david     (1000)     3435 2020-08-31 19:21:18.000000 itsdangerous-2.1.1/tests/test_itsdangerous/test_signer.py
--rw-r--r--   0 david     (1000) david     (1000)     3807 2022-03-09 16:11:24.000000 itsdangerous-2.1.1/tests/test_itsdangerous/test_timed.py
--rw-r--r--   0 david     (1000) david     (1000)      793 2020-08-31 19:21:18.000000 itsdangerous-2.1.1/tests/test_itsdangerous/test_url_safe.py
--rw-r--r--   0 david     (1000) david     (1000)      533 2022-02-16 18:56:11.000000 itsdangerous-2.1.1/tox.ini
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.049640 itsdangerous-2.1.2/
+-rw-r--r--   0 david     (1000) david     (1000)     7083 2022-03-24 15:10:29.000000 itsdangerous-2.1.2/CHANGES.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1475 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/LICENSE.rst
+-rw-r--r--   0 david     (1000) david     (1000)      159 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)     2928 2022-03-24 15:11:46.049640 itsdangerous-2.1.2/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     1813 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/README.rst
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/docs/
+-rw-r--r--   0 david     (1000) david     (1000)      581 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/Makefile
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/docs/_static/
+-rw-r--r--   0 david     (1000) david     (1000)     6629 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/_static/itsdangerous-logo-sidebar.png
+-rw-r--r--   0 david     (1000) david     (1000)    18971 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/_static/itsdangerous-logo.png
+-rw-r--r--   0 david     (1000) david     (1000)       45 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/changes.rst
+-rw-r--r--   0 david     (1000) david     (1000)     5230 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/concepts.rst
+-rw-r--r--   0 david     (1000) david     (1000)     2097 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/conf.py
+-rw-r--r--   0 david     (1000) david     (1000)      139 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/encoding.rst
+-rw-r--r--   0 david     (1000) david     (1000)      332 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/exceptions.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1654 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/index.rst
+-rw-r--r--   0 david     (1000) david     (1000)       71 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/license.rst
+-rw-r--r--   0 david     (1000) david     (1000)      752 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/docs/make.bat
+-rw-r--r--   0 david     (1000) david     (1000)     3485 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/serializer.rst
+-rw-r--r--   0 david     (1000) david     (1000)     1263 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/signer.rst
+-rw-r--r--   0 david     (1000) david     (1000)      689 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/docs/timed.rst
+-rw-r--r--   0 david     (1000) david     (1000)      615 2022-03-09 20:29:16.000000 itsdangerous-2.1.2/docs/url_safe.rst
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/requirements/
+-rw-r--r--   0 david     (1000) david     (1000)     1048 2022-03-09 20:29:32.000000 itsdangerous-2.1.2/requirements/dev.txt
+-rw-r--r--   0 david     (1000) david     (1000)     1349 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/requirements/docs.txt
+-rw-r--r--   0 david     (1000) david     (1000)      551 2022-03-09 20:29:32.000000 itsdangerous-2.1.2/requirements/tests.txt
+-rw-r--r--   0 david     (1000) david     (1000)      299 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/requirements/typing.txt
+-rw-r--r--   0 david     (1000) david     (1000)     2022 2022-03-24 15:11:46.049640 itsdangerous-2.1.2/setup.cfg
+-rw-r--r--   0 david     (1000) david     (1000)       57 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/setup.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/src/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/src/itsdangerous/
+-rw-r--r--   0 david     (1000) david     (1000)      876 2022-03-24 15:10:29.000000 itsdangerous-2.1.2/src/itsdangerous/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)      450 2022-03-09 20:29:32.000000 itsdangerous-2.1.2/src/itsdangerous/_json.py
+-rw-r--r--   0 david     (1000) david     (1000)     1419 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/encoding.py
+-rw-r--r--   0 david     (1000) david     (1000)     3206 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/exc.py
+-rw-r--r--   0 david     (1000) david     (1000)        0 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/py.typed
+-rw-r--r--   0 david     (1000) david     (1000)    11144 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/serializer.py
+-rw-r--r--   0 david     (1000) david     (1000)     9367 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/signer.py
+-rw-r--r--   0 david     (1000) david     (1000)     8174 2022-03-24 15:02:27.000000 itsdangerous-2.1.2/src/itsdangerous/timed.py
+-rw-r--r--   0 david     (1000) david     (1000)     2402 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/src/itsdangerous/url_safe.py
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.049640 itsdangerous-2.1.2/src/itsdangerous.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     2928 2022-03-24 15:11:45.000000 itsdangerous-2.1.2/src/itsdangerous.egg-info/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     1101 2022-03-24 15:11:46.000000 itsdangerous-2.1.2/src/itsdangerous.egg-info/SOURCES.txt
+-rw-r--r--   0 david     (1000) david     (1000)        1 2022-03-24 15:11:45.000000 itsdangerous-2.1.2/src/itsdangerous.egg-info/dependency_links.txt
+-rw-r--r--   0 david     (1000) david     (1000)       13 2022-03-24 15:11:46.000000 itsdangerous-2.1.2/src/itsdangerous.egg-info/top_level.txt
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.046307 itsdangerous-2.1.2/tests/
+drwxr-xr-x   0 david     (1000) david     (1000)        0 2022-03-24 15:11:46.049640 itsdangerous-2.1.2/tests/test_itsdangerous/
+-rw-r--r--   0 david     (1000) david     (1000)        0 2019-09-07 13:33:04.000000 itsdangerous-2.1.2/tests/test_itsdangerous/__init__.py
+-rw-r--r--   0 david     (1000) david     (1000)     1004 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/tests/test_itsdangerous/test_encoding.py
+-rw-r--r--   0 david     (1000) david     (1000)     6830 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/tests/test_itsdangerous/test_serializer.py
+-rw-r--r--   0 david     (1000) david     (1000)     3435 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/tests/test_itsdangerous/test_signer.py
+-rw-r--r--   0 david     (1000) david     (1000)     3807 2022-03-09 20:29:32.000000 itsdangerous-2.1.2/tests/test_itsdangerous/test_timed.py
+-rw-r--r--   0 david     (1000) david     (1000)      793 2022-03-09 20:29:27.000000 itsdangerous-2.1.2/tests/test_itsdangerous/test_url_safe.py
+-rw-r--r--   0 david     (1000) david     (1000)      533 2022-03-09 20:29:32.000000 itsdangerous-2.1.2/tox.ini
```

### Comparing `itsdangerous-2.1.1/CHANGES.rst` & `itsdangerous-2.1.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Version 2.1.2
+-------------
+
+Released 2022-03-24
+
+-   Handle date overflow in timed unsign on 32-bit systems. :pr:`299`
+
+
 Version 2.1.1
 -------------
 
 Released 2022-03-09
 
 -   Handle date overflow in timed unsign. :pr:`296`
```

### Comparing `itsdangerous-2.1.1/LICENSE.rst` & `itsdangerous-2.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/PKG-INFO` & `itsdangerous-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itsdangerous
-Version: 2.1.1
+Version: 2.1.2
 Summary: Safely pass data to untrusted environments and back.
 Home-page: https://palletsprojects.com/p/itsdangerous/
 Author: Armin Ronacher
 Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
```

### Comparing `itsdangerous-2.1.1/README.rst` & `itsdangerous-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/Makefile` & `itsdangerous-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/_static/itsdangerous-logo-sidebar.png` & `itsdangerous-2.1.2/docs/_static/itsdangerous-logo-sidebar.png`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/_static/itsdangerous-logo.png` & `itsdangerous-2.1.2/docs/_static/itsdangerous-logo.png`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/concepts.rst` & `itsdangerous-2.1.2/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/conf.py` & `itsdangerous-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/index.rst` & `itsdangerous-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/make.bat` & `itsdangerous-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/serializer.rst` & `itsdangerous-2.1.2/docs/serializer.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/signer.rst` & `itsdangerous-2.1.2/docs/signer.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/timed.rst` & `itsdangerous-2.1.2/docs/timed.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/docs/url_safe.rst` & `itsdangerous-2.1.2/docs/url_safe.rst`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/requirements/dev.txt` & `itsdangerous-2.1.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/requirements/docs.txt` & `itsdangerous-2.1.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/requirements/tests.txt` & `itsdangerous-2.1.2/requirements/tests.txt`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/setup.cfg` & `itsdangerous-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous/__init__.py` & `itsdangerous-2.1.2/src/itsdangerous/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 from .signer import NoneAlgorithm as NoneAlgorithm
 from .signer import Signer as Signer
 from .timed import TimedSerializer as TimedSerializer
 from .timed import TimestampSigner as TimestampSigner
 from .url_safe import URLSafeSerializer as URLSafeSerializer
 from .url_safe import URLSafeTimedSerializer as URLSafeTimedSerializer
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
```

### Comparing `itsdangerous-2.1.1/src/itsdangerous/encoding.py` & `itsdangerous-2.1.2/src/itsdangerous/encoding.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous/exc.py` & `itsdangerous-2.1.2/src/itsdangerous/exc.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous/serializer.py` & `itsdangerous-2.1.2/src/itsdangerous/serializer.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous/signer.py` & `itsdangerous-2.1.2/src/itsdangerous/signer.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous/timed.py` & `itsdangerous-2.1.2/src/itsdangerous/timed.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,17 @@
 
         # Signature is *not* okay. Raise a proper error now that we have
         # split the value and the timestamp.
         if sig_error is not None:
             if ts_int is not None:
                 try:
                     ts_dt = self.timestamp_to_datetime(ts_int)
-                except (ValueError, OSError) as exc:
+                except (ValueError, OSError, OverflowError) as exc:
                     # Windows raises OSError
+                    # 32-bit raises OverflowError
                     raise BadTimeSignature(
                         "Malformed timestamp", payload=value
                     ) from exc
 
             raise BadTimeSignature(str(sig_error), payload=value, date_signed=ts_dt)
 
         # Signature was okay but the timestamp is actually not there or
```

### Comparing `itsdangerous-2.1.1/src/itsdangerous/url_safe.py` & `itsdangerous-2.1.2/src/itsdangerous/url_safe.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/src/itsdangerous.egg-info/PKG-INFO` & `itsdangerous-2.1.2/src/itsdangerous.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itsdangerous
-Version: 2.1.1
+Version: 2.1.2
 Summary: Safely pass data to untrusted environments and back.
 Home-page: https://palletsprojects.com/p/itsdangerous/
 Author: Armin Ronacher
 Author-email: armin.ronacher@active-4.com
 Maintainer: Pallets
 Maintainer-email: contact@palletsprojects.com
 License: BSD-3-Clause
```

### Comparing `itsdangerous-2.1.1/src/itsdangerous.egg-info/SOURCES.txt` & `itsdangerous-2.1.2/src/itsdangerous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tests/test_itsdangerous/test_encoding.py` & `itsdangerous-2.1.2/tests/test_itsdangerous/test_encoding.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tests/test_itsdangerous/test_serializer.py` & `itsdangerous-2.1.2/tests/test_itsdangerous/test_serializer.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tests/test_itsdangerous/test_signer.py` & `itsdangerous-2.1.2/tests/test_itsdangerous/test_signer.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tests/test_itsdangerous/test_timed.py` & `itsdangerous-2.1.2/tests/test_itsdangerous/test_timed.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tests/test_itsdangerous/test_url_safe.py` & `itsdangerous-2.1.2/tests/test_itsdangerous/test_url_safe.py`

 * *Files identical despite different names*

### Comparing `itsdangerous-2.1.1/tox.ini` & `itsdangerous-2.1.2/tox.ini`

 * *Files identical despite different names*

