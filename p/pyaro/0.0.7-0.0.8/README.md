# Comparing `tmp/pyaro-0.0.7.tar.gz` & `tmp/pyaro-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaro-0.0.7.tar", last modified: Mon Feb  5 12:43:43 2024, max compression
+gzip compressed data, was "pyaro-0.0.8.tar", last modified: Tue Apr 16 15:44:15 2024, max compression
```

## Comparing `pyaro-0.0.7.tar` & `pyaro-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.961758 pyaro-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-02-05 12:43:30.000000 pyaro-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-02-05 12:43:43.961758 pyaro-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-02-05 12:43:30.000000 pyaro-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-05 12:43:43.961758 pyaro-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-05 12:43:30.000000 pyaro-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.957758 pyaro-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.957758 pyaro-0.0.7/src/pyaro/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.961758 pyaro-0.0.7/src/pyaro/csvreader/
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/csvreader/CSVTimeseriesReader.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/csvreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/pandas_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.961758 pyaro-0.0.7/src/pyaro/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/AutoFilterReaderEngine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    26414 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Station.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/Wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-05 12:43:30.000000 pyaro-0.0.7/src/pyaro/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.961758 pyaro-0.0.7/src/pyaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-05 12:43:43.000000 pyaro-0.0.7/src/pyaro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:43:43.961758 pyaro-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-05 12:43:30.000000 pyaro-0.0.7/tests/test_CSVTimeSeriesReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-04-16 15:44:11.000000 pyaro-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:44:15.393234 pyaro-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-16 15:44:11.000000 pyaro-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-16 15:44:15.397235 pyaro-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 15:44:11.000000 pyaro-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.389234 pyaro-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/csvreader/
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/csvreader/CSVTimeseriesReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/csvreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/pandas_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/AutoFilterReaderEngine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26414 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Station.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/Wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-16 15:44:11.000000 pyaro-0.0.8/src/pyaro/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/src/pyaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4656 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 15:44:15.000000 pyaro-0.0.8/src/pyaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:44:15.393234 pyaro-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-16 15:44:11.000000 pyaro-0.0.8/tests/test_CSVTimeSeriesReader.py
```

### Comparing `pyaro-0.0.7/LICENSE` & `pyaro-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/PKG-INFO` & `pyaro-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaro
-Version: 0.0.7
+Version: 0.0.8
 Summary: pyaro py-aerocom reader objects
 Home-page: https://pyaro.readthedocs.io
 Author: Heiko Klein, Daniel Heinesen
 Author-email: Heiko.Klein@met.no
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -32,15 +32,15 @@
 The goal of pyro was threefold.
 
 1. A simple interface for different types of air-pollution databases
 2. A programatic interface to these databases easily usable by large applications like [PyAerocom](https://pyaerocom.readthedocs.io)
 3. Easy extension for air-pollution database providers or programmers giving the users (1. or 2.) direct access
     their databases without the need of a new API.
 
-A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers>).
+A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers).
 
 
 ## Installation
 `python -m pip install 'pyaro@git+https://github.com/metno/pyaro.git'`
 
 This will install pyaro and all its dependencies (numpy).
```

### Comparing `pyaro-0.0.7/README.md` & `pyaro-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 The goal of pyro was threefold.
 
 1. A simple interface for different types of air-pollution databases
 2. A programatic interface to these databases easily usable by large applications like [PyAerocom](https://pyaerocom.readthedocs.io)
 3. Easy extension for air-pollution database providers or programmers giving the users (1. or 2.) direct access
     their databases without the need of a new API.
 
-A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers>).
+A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers).
 
 
 ## Installation
 `python -m pip install 'pyaro@git+https://github.com/metno/pyaro.git'`
 
 This will install pyaro and all its dependencies (numpy).
```

### Comparing `pyaro-0.0.7/setup.cfg` & `pyaro-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyaro
-version = 0.0.7
+version = 0.0.8
 author = Heiko Klein, Daniel Heinesen
 author_email = Heiko.Klein@met.no
 description = pyaro py-aerocom reader objects
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3 :: Only
```

### Comparing `pyaro-0.0.7/src/pyaro/csvreader/CSVTimeseriesReader.py` & `pyaro-0.0.8/src/pyaro/csvreader/CSVTimeseriesReader.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,25 +62,33 @@
         :csvreader_kwargs: kwargs send directly to csv.reader module
         :filters: default auto-filter filters
         """
         self._filename = filename
         self._stations = {}
         self._data = {}  # var -> {data-array}
         self._set_filters(filters)
+        self._extra_metadata = tuple(set(columns.keys()) - set(self.col_keys()))
         if country_lookup:
             lookupISO2 = _lookup_function()
         with open(self._filename, newline="") as csvfile:
             crd = csv.reader(csvfile, **csvreader_kwargs)
             for row in crd:
                 r = {}
+                extra_metadata = {}
                 for t in self.col_keys():
                     if isinstance(columns[t], str):
                         r[t] = columns[t]
                     else:
                         r[t] = row[columns[t]]
+                for t in self._extra_metadata:
+                    if isinstance(columns[t], str):
+                        extra_metadata[t] = columns[t]
+                    else:
+                        extra_metadata[t] = row[columns[t]]
+
                 for t in (
                     "value",
                     "latitude",
                     "longitude",
                     "altitude",
                     "standard_deviation",
                 ):
@@ -114,24 +122,30 @@
                             "end_time",
                             "flag",
                             "standard_deviation",
                         )
                     ]
                 )
                 if not r["station"] in self._stations:
+
+                    station_fields = {
+                        "station": r["station"],
+                        "longitude": r["longitude"],
+                        "latitude": r["latitude"],
+                        "altitude": r["altitude"],
+                        "country": r["country"],
+                        "url": "",
+                        "long_name": r["station"],
+                    }
+                    station_metadata = {
+                        key: extra_metadata[key] for key in self._extra_metadata
+                    }
+
                     self._stations[r["station"]] = Station(
-                        {
-                            "station": r["station"],
-                            "longitude": r["longitude"],
-                            "latitude": r["latitude"],
-                            "altitude": r["altitude"],
-                            "country": r["country"],
-                            "url": "",
-                            "long_name": r["station"],
-                        }
+                        station_fields, station_metadata
                     )
 
     @classmethod
     def col_keys(cls):
         """Column keys possible to initialize with this reader.
 
         :return: list of columns possible to initialize with columns argument of this reader
```

### Comparing `pyaro-0.0.7/src/pyaro/plugins.py` & `pyaro-0.0.8/src/pyaro/plugins.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/AutoFilterReaderEngine.py` & `pyaro-0.0.8/src/pyaro/timeseries/AutoFilterReaderEngine.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Data.py` & `pyaro-0.0.8/src/pyaro/timeseries/Data.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Engine.py` & `pyaro-0.0.8/src/pyaro/timeseries/Engine.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Filter.py` & `pyaro-0.0.8/src/pyaro/timeseries/Filter.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Reader.py` & `pyaro-0.0.8/src/pyaro/timeseries/Reader.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Station.py` & `pyaro-0.0.8/src/pyaro/timeseries/Station.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,31 +10,39 @@
     td = Station()
     print(td.station)
     print(td["station"])
     ```
 
     """
 
-    def __init__(self, fields: dict = None) -> None:
+    def __init__(self, fields: dict = None, metadata: dict = None) -> None:
         self._fields = {
             "station": "",
             "latitude": float("nan"),
             "longitude": float("nan"),
             "altitude": float("nan"),
             "long_name": "",
             "country": "",
             "url": "",
         }
+        self._metadata = {}
+        if metadata:
+            self._metadata = metadata
         if fields:
             self.set_fields(fields)
         pass
 
     def __getitem__(self, key):
         """access the data as a dict"""
-        return self._fields[key]
+        if key in self._fields:
+            return self._fields[key]
+        elif key in self._metadata:
+            return self._metadata[key]
+        else:
+            return KeyError(f"key {key} not found in station")
 
     def keys(self):
         """all available data-fields, excluding variable and units which are
         considered metadata"""
         return self._fields.keys()
 
     def set_fields(self, fields: dict):
@@ -109,9 +117,13 @@
     def url(self) -> str:
         """url to more information about the station
 
         :return: url
         """
         return self._fields["url"]
 
+    @property
+    def metadata(self) -> dict:
+        return self._metadata
+
     def __str__(self):
         return self._fields.__str__()
```

### Comparing `pyaro-0.0.7/src/pyaro/timeseries/Wrappers.py` & `pyaro-0.0.8/src/pyaro/timeseries/Wrappers.py`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/src/pyaro.egg-info/PKG-INFO` & `pyaro-0.0.8/src/pyaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaro
-Version: 0.0.7
+Version: 0.0.8
 Summary: pyaro py-aerocom reader objects
 Home-page: https://pyaro.readthedocs.io
 Author: Heiko Klein, Daniel Heinesen
 Author-email: Heiko.Klein@met.no
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -32,15 +32,15 @@
 The goal of pyro was threefold.
 
 1. A simple interface for different types of air-pollution databases
 2. A programatic interface to these databases easily usable by large applications like [PyAerocom](https://pyaerocom.readthedocs.io)
 3. Easy extension for air-pollution database providers or programmers giving the users (1. or 2.) direct access
     their databases without the need of a new API.
 
-A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers>).
+A few existing implementations of pyaro can be found at [pyaerocom-readers](https://github.com/metno/pyaro-readers).
 
 
 ## Installation
 `python -m pip install 'pyaro@git+https://github.com/metno/pyaro.git'`
 
 This will install pyaro and all its dependencies (numpy).
```

### Comparing `pyaro-0.0.7/src/pyaro.egg-info/SOURCES.txt` & `pyaro-0.0.8/src/pyaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaro-0.0.7/tests/test_CSVTimeSeriesReader.py` & `pyaro-0.0.8/tests/test_CSVTimeSeriesReader.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,14 +48,38 @@
         ) as ts:
             count = 0
             for var in ts.variables():
                 count += len(ts.data(var))
             self.assertEqual(count, 208)
             self.assertEqual(len(ts.stations()), 2)
 
+    def test_init_extra_columns(self):
+        columns = {
+            "variable": 0,
+            "station": 1,
+            "longitude": 2,
+            "latitude": 3,
+            "value": 4,
+            "units": 5,
+            "start_time": 6,
+            "end_time": 7,
+            "altitude": "0",
+            "country": "NO",
+            "standard_deviation": "NaN",
+            "flag": "0",
+            "area_classification": 8,
+        }
+        with pyaro.open_timeseries(
+            "csv_timeseries", *[self.file], **{"filters": [], "columns": columns}
+        ) as ts:
+            areas = ["Rural", "Urban"]
+            stations = ts.stations()
+            self.assertEqual(stations["station1"]["area_classification"], areas[0])
+            self.assertEqual(stations["station2"]["area_classification"], areas[1])
+
     def test_data(self):
         engines = pyaro.list_timeseries_engines()
         with engines["csv_timeseries"].open(
             filename=self.file,
             filters=[pyaro.timeseries.filters.get("countries", include=["NO"])],
         ) as ts:
             for var in ts.variables():
@@ -95,17 +119,15 @@
                     end_time=data.end_times,
                     latitude=data.latitudes,
                     longitude=data.longitudes,
                     altitude=data.altitudes,
                     flag=data.flags,
                     standard_deviation=data.standard_deviations,
                 )
-            self.assertEqual(
-                (2**rounds) * old_size, len(data), "data append by array"
-            )
+            self.assertEqual((2**rounds) * old_size, len(data), "data append by array")
 
     def test_stationfilter(self):
         engine = pyaro.list_timeseries_engines()["csv_timeseries"]
         sfilter = pyaro.timeseries.filters.get("stations", exclude=["station1"])
         with engine.open(self.file, filters=[sfilter]) as ts:
             count = 0
             for var in ts.variables():
```

