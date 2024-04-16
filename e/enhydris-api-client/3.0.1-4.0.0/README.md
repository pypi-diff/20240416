# Comparing `tmp/enhydris-api-client-3.0.1.tar.gz` & `tmp/enhydris-api-client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhydris-api-client-3.0.1.tar", last modified: Sun Apr 14 15:04:41 2024, max compression
+gzip compressed data, was "enhydris-api-client-4.0.0.tar", last modified: Tue Apr 16 19:19:20 2024, max compression
```

## Comparing `enhydris-api-client-3.0.1.tar` & `enhydris-api-client-4.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1764 2024-04-14 15:01:34.000000 enhydris-api-client-3.0.1/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      828 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.1/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      143 2022-03-25 09:49:03.000000 enhydris-api-client-3.0.1/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6839 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4146 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/enhydris_api_client/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     9394 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/enhydris_api_client/__init__.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6839 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      525 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-27 19:13:39.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       20 2024-04-14 15:04:41.000000 enhydris-api-client-3.0.1/enhydris_api_client.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1500 2024-04-14 15:02:29.000000 enhydris-api-client-3.0.1/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-14 15:04:41.376180 enhydris-api-client-3.0.1/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1838 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     7745 2022-12-04 15:39:55.000000 enhydris-api-client-3.0.1/tests/test_e2e.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6100 2022-10-31 07:39:21.000000 enhydris-api-client-3.0.1/tests/test_e2e.py.orig
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5326 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_misc.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2983 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_station.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3787 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_timeseries.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3210 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_timeseriesgroup.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     6213 2022-12-04 14:55:30.000000 enhydris-api-client-3.0.1/tests/test_tsdata.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2040 2024-04-16 19:09:54.000000 enhydris-api-client-4.0.0/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      828 2022-03-25 09:49:03.000000 enhydris-api-client-4.0.0/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      143 2022-03-25 09:49:03.000000 enhydris-api-client-4.0.0/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7391 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4422 2024-04-16 12:45:44.000000 enhydris-api-client-4.0.0/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/enhydris_api_client/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     9339 2024-04-16 14:10:24.000000 enhydris-api-client-4.0.0/enhydris_api_client/__init__.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7391 2024-04-16 19:19:20.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      525 2024-04-16 19:19:20.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-16 19:19:20.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-27 19:13:39.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2024-04-16 19:19:20.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       20 2024-04-16 19:19:20.000000 enhydris-api-client-4.0.0/enhydris_api_client.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1500 2024-04-16 19:18:09.000000 enhydris-api-client-4.0.0/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-16 19:19:20.582979 enhydris-api-client-4.0.0/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2478 2024-04-16 15:04:46.000000 enhydris-api-client-4.0.0/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     7864 2024-04-16 15:08:01.000000 enhydris-api-client-4.0.0/tests/test_e2e.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6124 2024-04-16 12:59:52.000000 enhydris-api-client-4.0.0/tests/test_e2e.py.orig
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5326 2024-04-16 12:14:48.000000 enhydris-api-client-4.0.0/tests/test_misc.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2983 2024-04-16 12:14:48.000000 enhydris-api-client-4.0.0/tests/test_station.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3787 2024-04-16 12:14:48.000000 enhydris-api-client-4.0.0/tests/test_timeseries.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3210 2024-04-16 12:14:48.000000 enhydris-api-client-4.0.0/tests/test_timeseriesgroup.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     6398 2024-04-16 15:10:51.000000 enhydris-api-client-4.0.0/tests/test_tsdata.py
```

### Comparing `enhydris-api-client-3.0.1/HISTORY.rst` & `enhydris-api-client-4.0.0/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 =======
 History
 =======
 
+4.0.0 (2024-04-16)
+==================
+
+- Requires htimeseries 7.
+- When downloading time series data without specifying the time zone, it
+  uses the ``display_timezone`` of that Enhydris station, whereas in
+  3.x.x it used UTC. The behaviour is now similar to that of 2.x.x.
+
 3.0.1 (2024-04-14)
 ==================
 
 - Compatible with htimeseries 4 to 7.
 
 3.0.0 (2022-12-04)
 ==================
 
 - Requires Enhydris 4 and htimeseries 4, and therefore requires aware
   HTimeseries objects.
-- Requires specifying time zone when downloading time series data.
+- Supports specifying time zone when downloading time series data.
 - Support for creating, retrieving, updating, and deleting time series
   groups.
 
 2.0.1 (2021-08-31)
 ==================
 
 - Updated dependences (the version of htimeseries required was too old).
```

### Comparing `enhydris-api-client-3.0.1/LICENSE` & `enhydris-api-client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/PKG-INFO` & `enhydris-api-client-4.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhydris-api-client
-Version: 3.0.1
+Version: 4.0.0
 Summary: Python API client for Enhydris
 Home-page: https://github.com/openmeteo/enhydris-api-client
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: iso8601
 Requires-Dist: requests<3,>=1
-Requires-Dist: htimeseries<8,>=4
+Requires-Dist: htimeseries<8,>=7
 
 ===================
 enhydris-api-client
 ===================
 
 
 .. image:: https://img.shields.io/pypi/v/enhydris_api_client.svg
@@ -113,50 +113,61 @@
 | **.get_timeseries(station_id, timeseries_group_id, timeseries_id)**
 | **.post_timeseries(station_id, timeseries_group_id, data)**
 | **.delete_timeseries(station_id, timeseries_group_id, timeseries_id)**
 
 Methods that create, retrieve or delete time series. Similar to the ones
 for station. ``list_timeseries()`` returns a list of dictionaries.
 
-| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone="UTC")**
+| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone=None)**
 | **.post_tsdata(station_id, timeseries_group_id, timeseries_id, ts)**
-| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone="UTC")**
+| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone=None)**
 
 Methods that retrieve or update time series data.
 
 ``read_ts_data()`` retrieves the time series data into a htimeseries
 object that it returns. If ``start_date`` and/or ``end_date`` (aware
 datetime objects) are specified, only the part of the time series
 between these dates is retrieved. The timestamps are returned in the
-specified time zone.
+specified time zone. If unspecified, then they are returned in the time
+zone specified by the station's display_timezone_.
 
 ``post_tsdata() `` posts a time series to Enhydris, appending the
 records to any already existing.  ``ts`` is a htimeseries object.
 
 ``get_ts_end_date()`` returns a ``datetime`` object which is the last
 timestamp of the time series. If the time series is empty it returns
 ``None``. The returned timestamp is always naive, but it is in the specified
-``timezone``.
+``timezone`` (or the station's display_timezone_ if unspecified).
+
+.. _display_timezone: https://enhydris.readthedocs.io/en/latest/dev/database.html#enhydris.models.Gentity.display_timezone
 
 
 =======
 History
 =======
 
+4.0.0 (2024-04-16)
+==================
+
+- Requires htimeseries 7.
+- When downloading time series data without specifying the time zone, it
+  uses the ``display_timezone`` of that Enhydris station, whereas in
+  3.x.x it used UTC. The behaviour is now similar to that of 2.x.x.
+
 3.0.1 (2024-04-14)
 ==================
 
 - Compatible with htimeseries 4 to 7.
 
 3.0.0 (2022-12-04)
 ==================
 
 - Requires Enhydris 4 and htimeseries 4, and therefore requires aware
   HTimeseries objects.
-- Requires specifying time zone when downloading time series data.
+- Supports specifying time zone when downloading time series data.
 - Support for creating, retrieving, updating, and deleting time series
   groups.
 
 2.0.1 (2021-08-31)
 ==================
 
 - Updated dependences (the version of htimeseries required was too old).
```

### Comparing `enhydris-api-client-3.0.1/README.rst` & `enhydris-api-client-4.0.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -89,26 +89,29 @@
 | **.get_timeseries(station_id, timeseries_group_id, timeseries_id)**
 | **.post_timeseries(station_id, timeseries_group_id, data)**
 | **.delete_timeseries(station_id, timeseries_group_id, timeseries_id)**
 
 Methods that create, retrieve or delete time series. Similar to the ones
 for station. ``list_timeseries()`` returns a list of dictionaries.
 
-| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone="UTC")**
+| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone=None)**
 | **.post_tsdata(station_id, timeseries_group_id, timeseries_id, ts)**
-| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone="UTC")**
+| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone=None)**
 
 Methods that retrieve or update time series data.
 
 ``read_ts_data()`` retrieves the time series data into a htimeseries
 object that it returns. If ``start_date`` and/or ``end_date`` (aware
 datetime objects) are specified, only the part of the time series
 between these dates is retrieved. The timestamps are returned in the
-specified time zone.
+specified time zone. If unspecified, then they are returned in the time
+zone specified by the station's display_timezone_.
 
 ``post_tsdata() `` posts a time series to Enhydris, appending the
 records to any already existing.  ``ts`` is a htimeseries object.
 
 ``get_ts_end_date()`` returns a ``datetime`` object which is the last
 timestamp of the time series. If the time series is empty it returns
 ``None``. The returned timestamp is always naive, but it is in the specified
-``timezone``.
+``timezone`` (or the station's display_timezone_ if unspecified).
+
+.. _display_timezone: https://enhydris.readthedocs.io/en/latest/dev/database.html#enhydris.models.Gentity.display_timezone
```

### Comparing `enhydris-api-client-3.0.1/enhydris_api_client/__init__.py` & `enhydris-api-client-4.0.0/enhydris_api_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import copy
 from io import StringIO
 from urllib.parse import urljoin
 
 try:
     from zoneinfo import ZoneInfo
 except ImportError:
     from backports.zoneinfo import ZoneInfo
@@ -186,62 +187,59 @@
     def read_tsdata(
         self,
         station_id,
         timeseries_group_id,
         timeseries_id,
         start_date=None,
         end_date=None,
-        timezone="UTC",
+        timezone=None,
     ):
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
             f"timeseries/{timeseries_id}/data/",
         )
         params = {"fmt": "hts"}
-        tzinfo = ZoneInfo(timezone)
+        tzinfo = ZoneInfo(timezone) if timezone else None
         dates_are_aware = (start_date is None or start_date.tzinfo is not None) and (
             end_date is None or end_date.tzinfo is not None
         )
         if not dates_are_aware:
             raise ValueError("start_date and end_date must be aware")
-        params["start_date"] = (
-            start_date and start_date.astimezone(tzinfo).isoformat()[:19]
-        )
-        params["end_date"] = end_date and end_date.astimezone(tzinfo).isoformat()[:19]
+        params["start_date"] = start_date and start_date.isoformat()
+        params["end_date"] = end_date and end_date.isoformat()
         params["timezone"] = timezone
         self.response = self.session.get(url, params=params)
         self.check_response()
         if self.response.text:
-            return HTimeseries(
-                StringIO(self.response.text), default_tzinfo=ZoneInfo(timezone)
-            )
+            return HTimeseries(StringIO(self.response.text), default_tzinfo=tzinfo)
         else:
             return HTimeseries()
 
     def post_tsdata(self, station_id, timeseries_group_id, timeseries_id, ts):
         f = StringIO()
+        data = copy(ts.data)
         try:
-            ts.data.index = ts.data.index.tz_convert("UTC")
+            data.index = data.index.tz_convert("UTC")
         except AttributeError:
-            assert ts.data.empty
-        ts.data.to_csv(f, header=False)
+            assert data.empty
+        data.to_csv(f, header=False)
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
             f"timeseries/{timeseries_id}/data/",
         )
         self.response = self.session.post(
             url, data={"timeseries_records": f.getvalue(), "timezone": "UTC"}
         )
         self.check_response()
         return self.response.text
 
     def get_ts_end_date(
-        self, station_id, timeseries_group_id, timeseries_id, timezone="UTC"
+        self, station_id, timeseries_group_id, timeseries_id, timezone=None
     ):
         url = urljoin(
             self.base_url,
             f"api/stations/{station_id}/timeseriesgroups/{timeseries_group_id}/"
             f"timeseries/{timeseries_id}/bottom/",
         )
         self.response = self.session.get(url, params={"timezone": timezone})
```

### Comparing `enhydris-api-client-3.0.1/enhydris_api_client.egg-info/PKG-INFO` & `enhydris-api-client-4.0.0/enhydris_api_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enhydris-api-client
-Version: 3.0.1
+Version: 4.0.0
 Summary: Python API client for Enhydris
 Home-page: https://github.com/openmeteo/enhydris-api-client
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: iso8601
 Requires-Dist: requests<3,>=1
-Requires-Dist: htimeseries<8,>=4
+Requires-Dist: htimeseries<8,>=7
 
 ===================
 enhydris-api-client
 ===================
 
 
 .. image:: https://img.shields.io/pypi/v/enhydris_api_client.svg
@@ -113,50 +113,61 @@
 | **.get_timeseries(station_id, timeseries_group_id, timeseries_id)**
 | **.post_timeseries(station_id, timeseries_group_id, data)**
 | **.delete_timeseries(station_id, timeseries_group_id, timeseries_id)**
 
 Methods that create, retrieve or delete time series. Similar to the ones
 for station. ``list_timeseries()`` returns a list of dictionaries.
 
-| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone="UTC")**
+| **.read_tsdata(station_id, timeseries_group_id, timeseries_id, start_date=None, end_date=None, timezone=None)**
 | **.post_tsdata(station_id, timeseries_group_id, timeseries_id, ts)**
-| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone="UTC")**
+| **.get_ts_end_date(station_id, timeseries_group_id, timeseries_id, timezone=None)**
 
 Methods that retrieve or update time series data.
 
 ``read_ts_data()`` retrieves the time series data into a htimeseries
 object that it returns. If ``start_date`` and/or ``end_date`` (aware
 datetime objects) are specified, only the part of the time series
 between these dates is retrieved. The timestamps are returned in the
-specified time zone.
+specified time zone. If unspecified, then they are returned in the time
+zone specified by the station's display_timezone_.
 
 ``post_tsdata() `` posts a time series to Enhydris, appending the
 records to any already existing.  ``ts`` is a htimeseries object.
 
 ``get_ts_end_date()`` returns a ``datetime`` object which is the last
 timestamp of the time series. If the time series is empty it returns
 ``None``. The returned timestamp is always naive, but it is in the specified
-``timezone``.
+``timezone`` (or the station's display_timezone_ if unspecified).
+
+.. _display_timezone: https://enhydris.readthedocs.io/en/latest/dev/database.html#enhydris.models.Gentity.display_timezone
 
 
 =======
 History
 =======
 
+4.0.0 (2024-04-16)
+==================
+
+- Requires htimeseries 7.
+- When downloading time series data without specifying the time zone, it
+  uses the ``display_timezone`` of that Enhydris station, whereas in
+  3.x.x it used UTC. The behaviour is now similar to that of 2.x.x.
+
 3.0.1 (2024-04-14)
 ==================
 
 - Compatible with htimeseries 4 to 7.
 
 3.0.0 (2022-12-04)
 ==================
 
 - Requires Enhydris 4 and htimeseries 4, and therefore requires aware
   HTimeseries objects.
-- Requires specifying time zone when downloading time series data.
+- Supports specifying time zone when downloading time series data.
 - Support for creating, retrieving, updating, and deleting time series
   groups.
 
 2.0.1 (2021-08-31)
 ==================
 
 - Updated dependences (the version of htimeseries required was too old).
```

### Comparing `enhydris-api-client-3.0.1/enhydris_api_client.egg-info/SOURCES.txt` & `enhydris-api-client-4.0.0/enhydris_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/setup.py` & `enhydris-api-client-4.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["iso8601", "requests>=1,<3", "htimeseries>=4,<8"]
+requirements = ["iso8601", "requests>=1,<3", "htimeseries>=7,<8"]
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     author="Antonis Christofides",
@@ -37,10 +37,10 @@
     include_package_data=True,
     name="enhydris-api-client",
     packages=find_packages(include=["enhydris_api_client"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/openmeteo/enhydris-api-client",
-    version="3.0.1",
+    version="4.0.0",
     zip_safe=False,
 )
```

### Comparing `enhydris-api-client-3.0.1/tests/test_e2e.py` & `enhydris-api-client-4.0.0/tests/test_e2e.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,23 @@
 
 import pandas as pd
 import requests
 from htimeseries import HTimeseries
 
 from enhydris_api_client import EnhydrisApiClient
 
-from . import test_timeseries_hts
+from . import AssertFrameEqualMixin, test_timeseries_htimeseries
+
+UTC_PLUS_2 = dt.timezone(dt.timedelta(hours=2))
 
 
 @skipUnless(
     os.getenv("ENHYDRIS_API_CLIENT_E2E_TEST"), "Set ENHYDRIS_API_CLIENT_E2E_TEST"
 )
-class EndToEndTestCase(TestCase):
+class EndToEndTestCase(AssertFrameEqualMixin, TestCase):
     """End-to-end test against a real Enhydris instance.
     To execute this test, specify the ENHYDRIS_API_CLIENT_E2E_TEST environment variable
     like this:
         ENHYDRIS_API_CLIENT_E2E_TEST='
             {"base_url": "http://localhost:8001",
              "token": "topsecrettokenkey",
              "owner_id": 9,
@@ -127,66 +129,66 @@
         self.assertEqual(timeseries["type"], "Regularized")
 
         # Post time series data
         self.client.post_tsdata(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
-            test_timeseries_hts,
+            test_timeseries_htimeseries,
         )
 
         # Get the last date and check it
         date = self.client.get_ts_end_date(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
         )
-        self.assertEqual(date, dt.datetime(2014, 1, 5, 8, 0))
+        self.assertEqual(date, dt.datetime(2014, 1, 5, 7, 0))
 
-        # Get the last date in a different timezone from UTC
+        # Get the last date in a different timezone from the default
         date = self.client.get_ts_end_date(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
             timezone="Etc/GMT-5",
         )
-        self.assertEqual(date, dt.datetime(2014, 1, 5, 13, 0))
+        self.assertEqual(date, dt.datetime(2014, 1, 5, 11, 0))
 
         # Get all time series data and check it
         hts = self.client.read_tsdata(
             tmp_station_id, self.timeseries_group_id, self.timeseries_id
         )
         try:
             # Compatibility with older Python or pandas versions (such as Python 3.7
             # with pandas 0.23): comparison may fail if tzinfo, although practically the
             # same thing, is a different object
             if hts.data.index.tz.offset == dt.timedelta(0):
                 hts.data.index = hts.data.index.tz_convert(dt.timezone.utc)
         except AttributeError:
             pass
-        pd.testing.assert_frame_equal(hts.data, test_timeseries_hts.data)
+        self.assert_frame_loosely_equal(hts.data, test_timeseries_htimeseries.data)
 
         # The other attributes should have been set too.
         self.assertTrue(hasattr(hts, "variable"))
 
         # Get part of the time series data and check it
         hts = self.client.read_tsdata(
             tmp_station_id,
             self.timeseries_group_id,
             self.timeseries_id,
-            start_date=dt.datetime(2014, 1, 3, 8, 0, tzinfo=dt.timezone.utc),
-            end_date=dt.datetime(2014, 1, 4, 8, 0, tzinfo=dt.timezone.utc),
+            start_date=dt.datetime(2014, 1, 3, 8, 0, tzinfo=UTC_PLUS_2),
+            end_date=dt.datetime(2014, 1, 4, 8, 0, tzinfo=UTC_PLUS_2),
             timezone="Etc/GMT-1",
         )
         expected_result = HTimeseries(
             StringIO(
                 textwrap.dedent(
                     """\
-                    2014-01-03 09:00,13.0,
-                    2014-01-04 09:00,14.0,
+                    2014-01-03 07:00,13.0,
+                    2014-01-04 07:00,14.0,
                     """
                 )
             ),
             default_tzinfo=ZoneInfo("Etc/GMT-1"),
         )
         try:
             # Compatibility with older Python or pandas versions (such as Python 3.7
```

### Comparing `enhydris-api-client-3.0.1/tests/test_e2e.py.orig` & `enhydris-api-client-4.0.0/tests/test_e2e.py.orig`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import pandas as pd
 import requests
 from htimeseries import HTimeseries
 
 from enhydris_api_client import EnhydrisApiClient
 
-from . import test_timeseries_hts
+from . import test_timeseries_htimeseries
 
 
 @skipUnless(
     os.getenv("ENHYDRIS_API_CLIENT_E2E_TEST"), "Set ENHYDRIS_API_CLIENT_E2E_TEST"
 )
 class EndToEndTestCase(TestCase):
     """End-to-end test against a real Enhydris instance.
@@ -120,28 +120,28 @@
         self.assertEqual(timeseries["type"], "Regularized")
 
         # Post time series data
         self.client.post_tsdata(
             self.station_id,
             self.timeseries_group_id,
             self.timeseries_id,
-            test_timeseries_hts,
+            test_timeseries_htimeseries,
         )
 
         # Get the last date and check it
         date = self.client.get_ts_end_date(
             self.station_id, self.timeseries_group_id, self.timeseries_id
         )
         self.assertEqual(date, dt.datetime(2014, 1, 5, 8, 0))
 
         # Get all time series data and check it
         hts = self.client.read_tsdata(
             self.station_id, self.timeseries_group_id, self.timeseries_id
         )
-        pd.testing.assert_frame_equal(hts.data, test_timeseries_hts.data)
+        pd.testing.assert_frame_equal(hts.data, test_timeseries_htimeseries.data)
 
         # The other attributes should have been set too.
         self.assertTrue(hasattr(hts, "variable"))
 
         # Get part of the time series data and check it
         hts = self.client.read_tsdata(
             self.station_id,
```

### Comparing `enhydris-api-client-3.0.1/tests/test_misc.py` & `enhydris-api-client-4.0.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/tests/test_station.py` & `enhydris-api-client-4.0.0/tests/test_station.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/tests/test_timeseries.py` & `enhydris-api-client-4.0.0/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/tests/test_timeseriesgroup.py` & `enhydris-api-client-4.0.0/tests/test_timeseriesgroup.py`

 * *Files identical despite different names*

### Comparing `enhydris-api-client-3.0.1/tests/test_tsdata.py` & `enhydris-api-client-4.0.0/tests/test_tsdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 import datetime as dt
+from copy import copy
 from io import StringIO
 from unittest import TestCase
 
-import pandas as pd
 import requests
 from htimeseries import HTimeseries
 
 from enhydris_api_client import EnhydrisApiClient
 
 from . import (
+    AssertFrameEqualMixin,
     mock_session,
     test_timeseries_csv,
     test_timeseries_csv_bottom,
-    test_timeseries_hts,
+    test_timeseries_htimeseries,
 )
 
+TEST_TIMESERIES_HTS = f"Timezone=+0200\r\n\r\n{test_timeseries_csv}"
 
-@mock_session(**{"get.return_value.text": test_timeseries_csv})
-class ReadTsDataTestCase(TestCase):
+
+@mock_session(**{"get.return_value.text": TEST_TIMESERIES_HTS})
+class ReadTsDataTestCase(TestCase, AssertFrameEqualMixin):
     url = "http://example.com/api/stations/41/timeseriesgroups/42/timeseries/43/data/"
 
     def _read_tsdata(self, **extra_args):
         self.client = EnhydrisApiClient("http://example.com")
         return self.client.read_tsdata(41, 42, 43, **extra_args)
 
     def test_makes_request(self, m):
         self._read_tsdata()
         m.return_value.get.assert_called_once_with(
             self.url,
             params={
                 "fmt": "hts",
                 "start_date": None,
                 "end_date": None,
-                "timezone": "UTC",
+                "timezone": None,
             },
         )
 
     def test_returns_data(self, m):
         ahts = self._read_tsdata()
-        pd.testing.assert_frame_equal(ahts.data, test_timeseries_hts.data)
+        self.assert_frame_equal(ahts.data, test_timeseries_htimeseries.data)
 
     def test_uses_timezone(self, m):
         self._read_tsdata(timezone="UTC")
         m.return_value.get.assert_called_once_with(
             self.url,
             params={
                 "fmt": "hts",
                 "start_date": None,
                 "end_date": None,
                 "timezone": "UTC",
             },
         )
 
 
-class ReadTsDataWithStartAndEndDateTestCase(TestCase):
-    @mock_session(**{"get.return_value.text": test_timeseries_csv})
+class ReadTsDataWithStartAndEndDateTestCase(TestCase, AssertFrameEqualMixin):
+    @mock_session(**{"get.return_value.text": TEST_TIMESERIES_HTS})
     def setUp(self, mock_requests_session):
         self.mock_requests_session = mock_requests_session
         self.client = EnhydrisApiClient("https://mydomain.com")
 
     def _make_request(self, start_tzinfo, end_tzinfo):
         self.data = self.client.read_tsdata(
             41,
@@ -71,82 +74,82 @@
     def test_makes_request(self):
         self._make_request(dt.timezone.utc, dt.timezone.utc)
         self.mock_requests_session.return_value.get.assert_called_once_with(
             "https://mydomain.com/api/stations/41/timeseriesgroups/42/timeseries/43/"
             "data/",
             params={
                 "fmt": "hts",
-                "start_date": "2019-06-12T00:00:00",
-                "end_date": "2019-06-13T15:25:00",
-                "timezone": "UTC",
+                "start_date": "2019-06-12T00:00:00+00:00",
+                "end_date": "2019-06-13T15:25:00+00:00",
+                "timezone": None,
             },
         )
 
     def test_returns_data(self):
         self._make_request(dt.timezone.utc, dt.timezone.utc)
-        pd.testing.assert_frame_equal(self.data.data, test_timeseries_hts.data)
+        self.assert_frame_equal(self.data.data, test_timeseries_htimeseries.data)
 
     def test_checks_that_start_date_is_aware(self):
         with self.assertRaises(ValueError):
             self._make_request(None, dt.timezone.utc)
 
     def test_checks_that_end_date_is_aware(self):
         with self.assertRaises(ValueError):
             self._make_request(dt.timezone.utc, None)
 
 
-class ReadEmptyTsDataTestCase(TestCase):
+class ReadEmptyTsDataTestCase(TestCase, AssertFrameEqualMixin):
     @mock_session(**{"get.return_value.text": ""})
     def test_returns_data(self, mock_requests_session):
         self.client = EnhydrisApiClient("https://mydomain.com")
         self.data = self.client.read_tsdata(41, 42, 43)
-        pd.testing.assert_frame_equal(self.data.data, HTimeseries().data)
+        self.assert_frame_equal(self.data.data, HTimeseries().data)
 
 
 class ReadTsDataErrorTestCase(TestCase):
     @mock_session(**{"get.return_value.status_code": 404})
     def test_raises_exception_on_error(self, mock_requests_session):
         self.client = EnhydrisApiClient("https://mydomain.com")
         with self.assertRaises(requests.HTTPError):
             self.client.read_tsdata(41, 42, 43)
 
 
 class PostTsDataTestCase(TestCase):
     @mock_session()
     def test_makes_request(self, mock_requests_session):
         client = EnhydrisApiClient("https://mydomain.com")
-        if hasattr(test_timeseries_hts, "timezone"):
-            del test_timeseries_hts.timezone
-        client.post_tsdata(41, 42, 43, test_timeseries_hts)
+        client.post_tsdata(41, 42, 43, test_timeseries_htimeseries)
         f = StringIO()
-        test_timeseries_hts.data.to_csv(f, header=False)
+        data = copy(test_timeseries_htimeseries.data)
+        data.index = data.index.tz_convert("UTC")
+        data.to_csv(f, header=False)
         mock_requests_session.return_value.post.assert_called_once_with(
             "https://mydomain.com/api/stations/41/timeseriesgroups/42/timeseries/43/"
             "data/",
             data={"timeseries_records": f.getvalue(), "timezone": "UTC"},
         )
 
     @mock_session(**{"post.return_value.status_code": 404})
     def test_raises_exception_on_error(self, mock_requests_session):
         client = EnhydrisApiClient("https://mydomain.com")
         with self.assertRaises(requests.HTTPError):
-            client.post_tsdata(41, 42, 43, test_timeseries_hts)
+            client.post_tsdata(41, 42, 43, test_timeseries_htimeseries)
 
 
 @mock_session(**{"get.return_value.text": test_timeseries_csv_bottom})
 class GetTsEndDateTestCase(TestCase):
     url = "http://mydom.com/api/stations/41/timeseriesgroups/42/timeseries/43/bottom/"
 
     def _get_ts_end_date(self, **extra_args):
         self.client = EnhydrisApiClient("http://mydom.com")
         return self.client.get_ts_end_date(41, 42, 43, **extra_args)
 
     def test_makes_request(self, m):
         self._get_ts_end_date()
-        m.return_value.get.assert_called_once_with(self.url, params={"timezone": "UTC"})
+        m.return_value.get.assert_called_once_with(self.url, params={"timezone": None})
 
     def test_returns_date(self, m):
         result = self._get_ts_end_date()
         self.assertEqual(result, dt.datetime(2014, 1, 5, 8, 0))
 
     def test_uses_timezone(self, m):
         self._get_ts_end_date(timezone="Etc/GMT-2")
```

