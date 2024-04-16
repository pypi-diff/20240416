# Comparing `tmp/evaporation-2.0.0.tar.gz` & `tmp/evaporation-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evaporation-2.0.0.tar", last modified: Mon Apr  1 07:31:58 2024, max compression
+gzip compressed data, was "evaporation-2.0.1.tar", last modified: Tue Apr 16 20:38:29 2024, max compression
```

## Comparing `evaporation-2.0.0.tar` & `evaporation-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 07:31:58.113681 evaporation-2.0.0/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      738 2024-04-01 07:24:28.000000 evaporation-2.0.0/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      713 2022-03-05 20:43:05.000000 evaporation-2.0.0/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:43:05.000000 evaporation-2.0.0/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2283 2024-04-01 07:31:58.113681 evaporation-2.0.0/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      753 2022-03-05 20:43:05.000000 evaporation-2.0.0/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 07:31:58.109681 evaporation-2.0.0/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4639 2022-03-05 20:43:05.000000 evaporation-2.0.0/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1394 2022-03-05 20:43:05.000000 evaporation-2.0.0/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:43:05.000000 evaporation-2.0.0/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:43:05.000000 evaporation-2.0.0/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     8586 2022-03-05 20:43:05.000000 evaporation-2.0.0/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 07:31:58.109681 evaporation-2.0.0/evaporation/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      144 2024-04-01 07:28:14.000000 evaporation-2.0.0/evaporation/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    27668 2024-04-01 07:00:15.000000 evaporation-2.0.0/evaporation/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    16265 2024-04-01 07:27:26.000000 evaporation-2.0.0/evaporation/evaporation.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 07:31:58.113681 evaporation-2.0.0/evaporation.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2283 2024-04-01 07:31:57.000000 evaporation-2.0.0/evaporation.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      512 2024-04-01 07:31:58.000000 evaporation-2.0.0/evaporation.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-01 07:31:57.000000 evaporation-2.0.0/evaporation.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       50 2024-04-01 07:31:57.000000 evaporation-2.0.0/evaporation.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:37:01.000000 evaporation-2.0.0/evaporation.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       34 2024-04-01 07:31:57.000000 evaporation-2.0.0/evaporation.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       12 2024-04-01 07:31:57.000000 evaporation-2.0.0/evaporation.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-01 07:31:58.113681 evaporation-2.0.0/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1674 2024-04-01 05:32:32.000000 evaporation-2.0.0/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-01 07:31:58.113681 evaporation-2.0.0/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:43:05.000000 evaporation-2.0.0/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    41360 2024-04-01 07:27:26.000000 evaporation-2.0.0/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9334 2022-03-05 20:43:05.000000 evaporation-2.0.0/tests/test_evaporation.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:38:29.839954 evaporation-2.0.1/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      798 2024-04-16 20:36:10.000000 evaporation-2.0.1/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      713 2022-03-05 20:43:05.000000 evaporation-2.0.1/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:43:05.000000 evaporation-2.0.1/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2343 2024-04-16 20:38:29.839954 evaporation-2.0.1/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      753 2022-03-05 20:43:05.000000 evaporation-2.0.1/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:38:29.839954 evaporation-2.0.1/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4639 2022-03-05 20:43:05.000000 evaporation-2.0.1/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1394 2022-03-05 20:43:05.000000 evaporation-2.0.1/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:43:05.000000 evaporation-2.0.1/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:43:05.000000 evaporation-2.0.1/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     8586 2022-03-05 20:43:05.000000 evaporation-2.0.1/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:38:29.839954 evaporation-2.0.1/evaporation/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      144 2024-04-16 20:38:00.000000 evaporation-2.0.1/evaporation/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    27668 2024-04-01 07:00:15.000000 evaporation-2.0.1/evaporation/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    16265 2024-04-01 07:27:26.000000 evaporation-2.0.1/evaporation/evaporation.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:38:29.839954 evaporation-2.0.1/evaporation.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2343 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      512 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       50 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-03-31 20:37:01.000000 evaporation-2.0.1/evaporation.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       34 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       12 2024-04-16 20:38:29.000000 evaporation-2.0.1/evaporation.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-16 20:38:29.839954 evaporation-2.0.1/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1674 2024-04-16 20:36:10.000000 evaporation-2.0.1/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 20:38:29.839954 evaporation-2.0.1/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:43:05.000000 evaporation-2.0.1/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    41243 2024-04-16 20:36:10.000000 evaporation-2.0.1/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9334 2022-03-05 20:43:05.000000 evaporation-2.0.1/tests/test_evaporation.py
```

### Comparing `evaporation-2.0.0/HISTORY.rst` & `evaporation-2.0.1/HISTORY.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+2.0.1 (2024-04-16)
+==================
+
+- Allow hspatial 4.
+
 2.0.0 (2024-04-01)
 ==================
 
 - Updated some dependencies, notably hspatial 2, which entails
   htimeseries 6.
 
 1.0.1 (2021-09-01)
```

### Comparing `evaporation-2.0.0/LICENSE` & `evaporation-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/PKG-INFO` & `evaporation-2.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaporation
-Version: 2.0.0
+Version: 2.0.1
 Summary: Calculation of evaporation and transpiration
 Home-page: https://github.com/openmeteo/evaporation
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: evaporation
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: iso8601
-Requires-Dist: hspatial<4,>=3
+Requires-Dist: hspatial<5,>=3
 
 ===========
 evaporation
 ===========
 
 
 .. image:: https://img.shields.io/pypi/v/evaporation.svg
@@ -45,14 +45,19 @@
 * Documentation: https://evaporation.readthedocs.io.
 
 
 =======
 History
 =======
 
+2.0.1 (2024-04-16)
+==================
+
+- Allow hspatial 4.
+
 2.0.0 (2024-04-01)
 ==================
 
 - Updated some dependencies, notably hspatial 2, which entails
   htimeseries 6.
 
 1.0.1 (2021-09-01)
```

### Comparing `evaporation-2.0.0/README.rst` & `evaporation-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/docs/api.rst` & `evaporation-2.0.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/docs/conf.py` & `evaporation-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/docs/usage.rst` & `evaporation-2.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/evaporation/cli.py` & `evaporation-2.0.1/evaporation/cli.py`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/evaporation/evaporation.py` & `evaporation-2.0.1/evaporation/evaporation.py`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/evaporation.egg-info/PKG-INFO` & `evaporation-2.0.1/evaporation.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evaporation
-Version: 2.0.0
+Version: 2.0.1
 Summary: Calculation of evaporation and transpiration
 Home-page: https://github.com/openmeteo/evaporation
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Keywords: evaporation
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Click>=7.0
 Requires-Dist: iso8601
-Requires-Dist: hspatial<4,>=3
+Requires-Dist: hspatial<5,>=3
 
 ===========
 evaporation
 ===========
 
 
 .. image:: https://img.shields.io/pypi/v/evaporation.svg
@@ -45,14 +45,19 @@
 * Documentation: https://evaporation.readthedocs.io.
 
 
 =======
 History
 =======
 
+2.0.1 (2024-04-16)
+==================
+
+- Allow hspatial 4.
+
 2.0.0 (2024-04-01)
 ==================
 
 - Updated some dependencies, notably hspatial 2, which entails
   htimeseries 6.
 
 1.0.1 (2021-09-01)
```

### Comparing `evaporation-2.0.0/evaporation.egg-info/SOURCES.txt` & `evaporation-2.0.1/evaporation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evaporation-2.0.0/setup.py` & `evaporation-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["Click>=7.0", "iso8601", "hspatial>=3,<4"]
+requirements = ["Click>=7.0", "iso8601", "hspatial>=3,<5"]
 
 test_requirements = []
 
 
 def get_version():
     scriptdir = os.path.dirname(os.path.abspath(__file__))
     init_py_path = os.path.join(scriptdir, "evaporation", "__init__.py")
```

### Comparing `evaporation-2.0.0/tests/test_cli.py` & `evaporation-2.0.1/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         shutil.rmtree(self.tempdir)
 
     def setup_input_file(self, step, basename, value, missing=None):
         filename = os.path.join(self.tempdir, basename + ".hts")
         timestamp = step == "hourly" and "2014-10-01 15:00" or "2014-07-06"
         with open(filename, "w") as f:
             f.write("Title={}\n".format(basename.replace("_", " ").capitalize()))
-            f.write("Timezone=CVT (UTC-0100)\n")
+            f.write("Timezone=-0100\n")
             if missing != "location":
                 f.write("Location=-16.25 16.217 4326\n")
             if missing != "altitude":
                 f.write("Altitude={}\n".format(step == "hourly" and "8" or "100"))
             f.write("\n{},{},\n".format(timestamp, value))
 
     def setup_hourly_input_files(self, missing=None):
@@ -494,15 +494,14 @@
         expected_result = pd.DataFrame(
             data={"value": [0.63], "flags": [""]},
             columns=("value", "flags"),
             index=[dt.datetime(2014, 10, 1, 15, 0, tzinfo=t.data.index.tz)],
         )
         expected_result.index.name = "date"
         pd.testing.assert_frame_equal(t.data, expected_result, check_less_precise=2)
-        self.assertEqual(t.data.index.tz.name, "CVT")
         self.assertEqual(t.data.index.tz.offset, dt.timedelta(hours=-1))
 
     def test_daily(self):
         self.setup_daily_input_files()
         self.setup_config_file("D")
 
         # Verify the output file doesn't exist yet
@@ -518,15 +517,14 @@
         expected_result = pd.DataFrame(
             data={"value": [3.9], "flags": [""]},
             columns=["value", "flags"],
             index=[dt.datetime(2014, 7, 6, tzinfo=t.data.index.tz)],
         )
         expected_result.index.name = "date"
         pd.testing.assert_frame_equal(t.data, expected_result, check_less_precise=1)
-        self.assertEqual(t.data.index.tz.name, "CVT")
         self.assertEqual(t.data.index.tz.offset, dt.timedelta(hours=-1))
 
     def test_missing_location(self):
         self.setup_hourly_input_files(missing="location")
         self.setup_config_file("H")
         msg = (
             "Incorrect or unspecified or inconsistent locations in the time series "
```

### Comparing `evaporation-2.0.0/tests/test_evaporation.py` & `evaporation-2.0.1/tests/test_evaporation.py`

 * *Files identical despite different names*

