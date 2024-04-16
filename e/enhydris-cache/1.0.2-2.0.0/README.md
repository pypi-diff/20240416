# Comparing `tmp/enhydris-cache-1.0.2.tar.gz` & `tmp/enhydris-cache-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhydris-cache-1.0.2.tar", last modified: Mon Jul 31 11:00:42 2023, max compression
+gzip compressed data, was "enhydris-cache-2.0.0.tar", last modified: Tue Apr 16 19:27:54 2024, max compression
```

## Comparing `enhydris-cache-1.0.2.tar` & `enhydris-cache-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      483 2023-07-31 10:58:32.000000 enhydris-cache-1.0.2/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      716 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2004 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      795 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      704 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1418 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      225 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4802 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/enhydris_cache/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      147 2023-07-31 10:59:01.000000 enhydris-cache-1.0.2/enhydris_cache/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4604 2022-03-25 09:40:54.000000 enhydris-cache-1.0.2/enhydris_cache/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2220 2022-03-25 09:08:52.000000 enhydris-cache-1.0.2/enhydris_cache/enhydris_cache.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/enhydris_cache.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2004 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      548 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-31 10:48:14.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       15 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1706 2023-07-31 10:58:32.000000 enhydris-cache-1.0.2/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15960 2022-03-25 09:40:54.000000 enhydris-cache-1.0.2/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4740 2022-03-25 09:28:10.000000 enhydris-cache-1.0.2/tests/test_enhydris_cache.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:27:54.685561 enhydris-cache-2.0.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      697 2024-04-16 19:24:29.000000 enhydris-cache-2.0.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      716 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2338 2024-04-16 19:27:54.685561 enhydris-cache-2.0.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      795 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:27:54.681561 enhydris-cache-2.0.0/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      704 2024-04-16 15:17:14.000000 enhydris-cache-2.0.0/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1418 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      225 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4802 2024-04-16 15:17:14.000000 enhydris-cache-2.0.0/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:27:54.681561 enhydris-cache-2.0.0/enhydris_cache/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      147 2024-04-16 19:27:26.000000 enhydris-cache-2.0.0/enhydris_cache/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4604 2024-04-16 15:17:14.000000 enhydris-cache-2.0.0/enhydris_cache/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2621 2024-04-16 15:53:39.000000 enhydris-cache-2.0.0/enhydris_cache/enhydris_cache.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:27:54.681561 enhydris-cache-2.0.0/enhydris_cache.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2338 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      548 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-31 10:48:14.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       37 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       15 2024-04-16 19:27:54.000000 enhydris-cache-2.0.0/enhydris_cache.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-16 19:27:54.685561 enhydris-cache-2.0.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1754 2024-04-16 19:21:41.000000 enhydris-cache-2.0.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:27:54.681561 enhydris-cache-2.0.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:16.000000 enhydris-cache-2.0.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16130 2024-04-16 16:14:52.000000 enhydris-cache-2.0.0/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4859 2024-04-16 15:47:41.000000 enhydris-cache-2.0.0/tests/test_enhydris_cache.py
```

### Comparing `enhydris-cache-1.0.2/LICENSE` & `enhydris-cache-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/PKG-INFO` & `enhydris-cache-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: enhydris-cache
-Version: 1.0.2
+Version: 2.0.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/enhydris-cache
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: enhydris-cache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Click>=7.0
+Requires-Dist: enhydris-api-client<5,>=4
 
 ==============
 enhydris-cache
 ==============
 
 
 .. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
@@ -43,14 +46,21 @@
 * Documentation: https://enhydris-cache.readthedocs.io.
 
 
 =======
 History
 =======
 
+2.0.0 (2024-04-16)
+==================
+
+- Requires enhydris-api-client v.4, and therefore htimeseries v.7, and
+  therefore Python 3.9 or later. See the enhydris-api-client v.4 release
+  notes for more information.
+
 1.0.2 (2023-07-31)
 ==================
 
 - Allow running with enhydris-api-client v.3
 
 1.0.1 (2022-03-25)
 ==================
```

### Comparing `enhydris-cache-1.0.2/README.rst` & `enhydris-cache-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/docs/api.rst` & `enhydris-cache-2.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/docs/conf.py` & `enhydris-cache-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/docs/usage.rst` & `enhydris-cache-2.0.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/enhydris_cache/cli.py` & `enhydris-cache-2.0.0/enhydris_cache/cli.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/enhydris_cache/enhydris_cache.py` & `enhydris-cache-2.0.0/enhydris_cache/enhydris_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime as dt
 
+import pandas as pd
 from enhydris_api_client import EnhydrisApiClient
 from htimeseries import HTimeseries
 
 
 class TimeseriesCache(object):
     def __init__(self, timeseries_group):
         self.timeseries_group = timeseries_group
@@ -37,21 +38,31 @@
             return HTimeseries()
 
     def _get_timeseries_end_date(self, timeseries):
         try:
             end_date = timeseries.data.index[-1]
         except IndexError:
             # Timeseries is totally empty; no start and end date
-            end_date = dt.datetime(1, 1, 1, 0, 0)
+            end_date = dt.datetime(1, 1, 1, 0, 0, tzinfo=dt.timezone.utc)
         return end_date
 
     def _append_newer_timeseries(self, start_date, old_ts):
         with EnhydrisApiClient(self.base_url, token=self.auth_token) as api_client:
             ts = api_client.read_tsdata(
                 self.station_id,
                 self.timeseries_group_id,
                 self.timeseries_id,
                 start_date=start_date,
             )
             new_data = ts.data
-            ts.data = old_ts.data.append(new_data, verify_integrity=True, sort=False)
+
+            # For appending to work properly, both time series need to have the same
+            # tz.
+            if len(old_ts.data):
+                new_data.index = new_data.index.tz_convert(old_ts.data.index.tz)
+            else:
+                old_ts.data.index = old_ts.data.index.tz_convert(new_data.index.tz)
+
+            ts.data = pd.concat(
+                [old_ts.data, new_data], verify_integrity=True, sort=False
+            )
         return ts
```

### Comparing `enhydris-cache-1.0.2/enhydris_cache.egg-info/PKG-INFO` & `enhydris-cache-2.0.0/enhydris_cache.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: enhydris-cache
-Version: 1.0.2
+Version: 2.0.0
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/enhydris-cache
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: enhydris-cache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Click>=7.0
+Requires-Dist: enhydris-api-client<5,>=4
 
 ==============
 enhydris-cache
 ==============
 
 
 .. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
@@ -43,14 +46,21 @@
 * Documentation: https://enhydris-cache.readthedocs.io.
 
 
 =======
 History
 =======
 
+2.0.0 (2024-04-16)
+==================
+
+- Requires enhydris-api-client v.4, and therefore htimeseries v.7, and
+  therefore Python 3.9 or later. See the enhydris-api-client v.4 release
+  notes for more information.
+
 1.0.2 (2023-07-31)
 ==================
 
 - Allow running with enhydris-api-client v.3
 
 1.0.1 (2022-03-25)
 ==================
```

### Comparing `enhydris-cache-1.0.2/enhydris_cache.egg-info/SOURCES.txt` & `enhydris-cache-2.0.0/enhydris_cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.2/setup.py` & `enhydris-cache-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["Click>=7.0", "enhydris-api-client>=2.0.1,<4"]
+requirements = ["Click>=7.0", "enhydris-api-client>=4,<5"]
 
 test_requirements = []
 
 
 def get_version():
     scriptdir = os.path.dirname(os.path.abspath(__file__))
     init_py_path = os.path.join(scriptdir, "enhydris_cache", "__init__.py")
@@ -27,17 +27,18 @@
     author="Antonis Christofides",
     author_email="antonis@antonischristofides.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     description="Utilities for spatial integration of time series",
     entry_points={"console_scripts": ["enhydris-cache=enhydris_cache.cli:main"]},
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/x-rst",
```

### Comparing `enhydris-cache-1.0.2/tests/test_cli.py` & `enhydris-cache-2.0.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime as dt
 import json
 import os
 import shutil
 import sys
 import tempfile
 import textwrap
 from io import StringIO
@@ -273,32 +274,35 @@
                     )
                 )
             )
         cli.App(self.configfilename).run()
         self.assertTrue(os.path.exists(logfilename))
 
 
+UTC_PLUS_2 = dt.timezone(dt.timedelta(hours=2))
+
+
 @skipUnless(os.getenv("ENHYDRIS_CACHE_E2E_TEST"), "set ENHYDRIS_CACHE_E2E_TEST")
 class EnhydrisCacheE2eTestCase(TestCase):
     test_timeseries1 = textwrap.dedent(
         """\
-        2014-01-01 08:00,11.00,
-        2014-01-02 08:00,12.00,
-        2014-01-03 08:00,13.00,
-        2014-01-04 08:00,14.00,
-        2014-01-05 08:00,15.00,
+        2014-01-01 08:00,11.0,
+        2014-01-02 08:00,12.0,
+        2014-01-03 08:00,13.0,
+        2014-01-04 08:00,14.0,
+        2014-01-05 08:00,15.0,
         """
     )
     test_timeseries2 = textwrap.dedent(
         """\
-        2014-07-01 08:00,9.11,
-        2014-07-02 08:00,9.12,
-        2014-07-03 08:00,9.13,
-        2014-07-04 08:00,9.14,
-        2014-07-05 08:00,9.15,
+        2014-07-01 08:00,9.1,
+        2014-07-02 08:00,9.2,
+        2014-07-03 08:00,9.3,
+        2014-07-04 08:00,9.4,
+        2014-07-05 08:00,9.5,
         """
     )
     timeseries1_top = "".join(test_timeseries1.splitlines(True)[:-1])
     timeseries2_top = "".join(test_timeseries2.splitlines(True)[:-1])
     timeseries1_bottom = test_timeseries1.splitlines(True)[-1]
     timeseries2_bottom = test_timeseries2.splitlines(True)[-1]
 
@@ -338,21 +342,21 @@
             )
 
         # Add some data (all but the last record) to the database
         self.api_client.post_tsdata(
             self.station_id,
             self.timeseries_group_id,
             self.timeseries1_id,
-            HTimeseries(StringIO(self.timeseries1_top)),
+            HTimeseries(StringIO(self.timeseries1_top), default_tzinfo=UTC_PLUS_2),
         )
         self.api_client.post_tsdata(
             self.station_id,
             self.timeseries_group_id,
             self.timeseries2_id,
-            HTimeseries(StringIO(self.timeseries2_top)),
+            HTimeseries(StringIO(self.timeseries2_top), default_tzinfo=UTC_PLUS_2),
         )
 
         # Prepare a configuration file (some tests override it)
         with open(self.config_file, "w") as f:
             f.write(
                 textwrap.dedent(
                     """\
@@ -419,21 +423,21 @@
         self.assertEqual(c.getvalue().replace("\r", ""), self.timeseries2_top)
 
         # Append a record to the database for each timeseries
         self.api_client.post_tsdata(
             self.station_id,
             self.timeseries_group_id,
             self.timeseries1_id,
-            HTimeseries(StringIO(self.timeseries1_bottom)),
+            HTimeseries(StringIO(self.timeseries1_bottom), default_tzinfo=UTC_PLUS_2),
         )
         self.api_client.post_tsdata(
             self.station_id,
             self.timeseries_group_id,
             self.timeseries2_id,
-            HTimeseries(StringIO(self.timeseries2_bottom)),
+            HTimeseries(StringIO(self.timeseries2_bottom), default_tzinfo=UTC_PLUS_2),
         )
 
         # Execute the application again
         application.run()
 
         # Check that the files are what they should be
         with open("file1", newline="\n") as f:
```

### Comparing `enhydris-cache-1.0.2/tests/test_enhydris_cache.py` & `enhydris-cache-2.0.0/tests/test_enhydris_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,31 +32,35 @@
     ),
 }
 test_timeseries["42_top"] = "".join(test_timeseries["42_all"].splitlines(True)[:-1])
 test_timeseries["43_top"] = "".join(test_timeseries["43_all"].splitlines(True)[:-1])
 test_timeseries["42_bottom"] = test_timeseries["42_all"].splitlines(True)[-1]
 test_timeseries["43_bottom"] = test_timeseries["43_all"].splitlines(True)[-1]
 
+UTC_PLUS_2 = dt.timezone(dt.timedelta(hours=2))
+
 
 def mock_read_tsdata(
     station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None
 ):
     result = _get_hts_object(timeseries_id, start_date)
     _set_hts_attributes(result, timeseries_id)
     return result
 
 
 def _get_hts_object(timeseries_id, start_date):
     timeseries_top = HTimeseries(
-        StringIO(test_timeseries["{}_top".format(timeseries_id)])
+        StringIO(test_timeseries[f"{timeseries_id}_top"]), default_tzinfo=UTC_PLUS_2
     )
-    if start_date is None or start_date == dt.datetime(1, 1, 1, 0, 1):
+    if start_date is None or start_date < dt.datetime(1, 1, 2, 0, 0, tzinfo=UTC_PLUS_2):
         return timeseries_top
     assert start_date == timeseries_top.data.index[-1] + dt.timedelta(minutes=1)
-    result = HTimeseries(StringIO(test_timeseries["{}_bottom".format(timeseries_id)]))
+    result = HTimeseries(
+        StringIO(test_timeseries[f"{timeseries_id}_bottom"]), default_tzinfo=UTC_PLUS_2
+    )
     return result
 
 
 def _set_hts_attributes(hts, timeseries_id):
     hts.time_step = "D"
     hts.precision = 0 if timeseries_id == 42 else 2
     hts.comment = "Très importante"
```

