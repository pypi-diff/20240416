# Comparing `tmp/geoinsight-0.7.0.tar.gz` & `tmp/geoinsight-0.8.1.tar.gz`

## Comparing `geoinsight-0.7.0.tar` & `geoinsight-0.8.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.7.0/geoinsight/__init__.py
--rw-r--r--   0        0        0   143950 2020-02-02 00:00:00.000000 geoinsight-0.7.0/geoinsight/api.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.7.0/geoinsight/util.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 geoinsight-0.7.0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.7.0/LICENSE
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 geoinsight-0.7.0/README.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 geoinsight-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 geoinsight-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 geoinsight-0.8.1/geoinsight/__init__.py
+-rw-r--r--   0        0        0   162148 2020-02-02 00:00:00.000000 geoinsight-0.8.1/geoinsight/api.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 geoinsight-0.8.1/geoinsight/util.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 geoinsight-0.8.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geoinsight-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 geoinsight-0.8.1/README.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 geoinsight-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 geoinsight-0.8.1/PKG-INFO
```

### Comparing `geoinsight-0.7.0/geoinsight/api.py` & `geoinsight-0.8.1/geoinsight/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -187,28 +187,28 @@
         """
 
         # Endpoint
         endpoint = '/destination_source_overview'
 
         return requests.get(self.url + endpoint, headers=self.headers)
 
-    def dst_refresh_stats_open(self):
-        """ GET dst_refresh_stats_open
+    def dst_refresh_open(self):
+        """ GET dst_refresh_open
 
 
 
         Returns
         -----------
             response:
-                {dst_refresh_stats_open} response object
+                {dst_refresh_open} response object
 
         """
 
         # Endpoint
-        endpoint = '/dst_refresh_stats_open'
+        endpoint = '/dst_refresh_open'
 
         return requests.get(self.url + endpoint, headers=self.headers)
 
     def is_token_valid(self):
         """ GET is_token_valid
 
 
@@ -999,27 +999,31 @@
         body = {
                  "_col_name": _col_name,
                  "_col_pkey": _col_pkey
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_cell_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_cell_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_cell_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, region, neighbor, children, properties} response object
@@ -1032,42 +1036,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_cell_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_cell_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_cell_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the DGGS cell ??
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | ...
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, region, neighbor, children, properties} response object
@@ -1082,43 +1096,53 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_cell_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_cell_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_cell_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the cell of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, region, neighbor, children, properties} response object
@@ -1133,41 +1157,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_cell_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_cell_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_cell_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the entire cell definition with region, center, children and neighbors of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, region, neighbors, children, properties} response object
@@ -1180,28 +1214,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_cell_by_point(self, _x, _y, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_cell_by_point(self, _x, _y, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_cell_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the cell of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _x : float
@@ -1210,14 +1250,18 @@
                 float | Y of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, region, neighbors, children, properties} response object
@@ -1234,42 +1278,52 @@
             logging.error('{}: {} is not {}'.format('_y', _y, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_x": _x,
                  "_y": _y,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_center_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_center_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_center_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, properties} response object
@@ -1282,42 +1336,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_center_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_center_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_center_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the center of the DGGS cell.
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | ...
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, properties} response object
@@ -1332,43 +1396,53 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_center_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_center_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_center_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the center of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, properties} response object
@@ -1383,41 +1457,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_center_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_center_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_center_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the centers of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, properties} response object
@@ -1430,28 +1514,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_center_by_point(self, _y, _x, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_center_by_point(self, _y, _x, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_center_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the center of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _y : float
@@ -1460,14 +1550,18 @@
                 float | X of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, center, properties} response object
@@ -1484,42 +1578,52 @@
             logging.error('{}: {} is not {}'.format('_x', _x, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_y": _y,
                  "_x": _x,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_children_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_children_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_children_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, children, properties} response object
@@ -1532,42 +1636,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_children_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_children_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_children_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the children of the DGGS cell.
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | ...
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, children, properties} response object
@@ -1582,43 +1696,53 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_children_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_children_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_children_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the children of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, children, properties} response object
@@ -1633,41 +1757,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_children_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_children_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_children_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the children of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, children, properties} response object
@@ -1680,28 +1814,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_children_by_point(self, _x, _y, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_children_by_point(self, _x, _y, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_children_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the children of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _x : float
@@ -1710,14 +1850,18 @@
                 float | Y of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, children, properties} response object
@@ -1734,24 +1878,30 @@
             logging.error('{}: {} is not {}'.format('_y', _y, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_x": _x,
                  "_y": _y,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
     def isea3h_data_aoi_delete(self, _id):
         """ POST isea3h_data_aoi_delete
@@ -2217,16 +2367,16 @@
                  "_col_name": _col_name,
                  "_col_dtype": _col_dtype,
                  "_col_pkey": _col_pkey
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_data_dst_refresh_stats(self, _id):
-        """ POST isea3h_data_dst_refresh_stats
+    def isea3h_data_dst_refresh(self, _id):
+        """ POST isea3h_data_dst_refresh
 
 
 
         Parameters
         ------------
             _id : str
                 str |
@@ -2235,15 +2385,15 @@
         -----------
             response:
                 {} response object
 
         """
 
         # Endpoint
-        endpoint = '/rpc/isea3h_data_dst_refresh_stats'
+        endpoint = '/rpc/isea3h_data_dst_refresh'
 
         # Field type check
         if type(_id) != str and _id is not None:
             logging.error('{}: {} is not {}'.format('_id', _id, 'text'))
 
         # Body
         body = {
@@ -2356,27 +2506,31 @@
         body = {
                  "_id": _id,
                  "_detail": _detail
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_gid_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_gid_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_gid_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, properties} response object
@@ -2389,42 +2543,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_gid_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_gid_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_gid_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | Resolution for children cells
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, properties} response object
@@ -2439,43 +2603,53 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_gid_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_gid_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_gid_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the GID of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, properties} response object
@@ -2490,41 +2664,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_gid_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_gid_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_gid_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the centers of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, properties} response object
@@ -2537,28 +2721,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_gid_by_point(self, _x, _y, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_gid_by_point(self, _x, _y, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_gid_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the GID of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _x : float
@@ -2567,14 +2757,18 @@
                 float | Y of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, properties} response object
@@ -2591,24 +2785,30 @@
             logging.error('{}: {} is not {}'.format('_y', _y, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_x": _x,
                  "_y": _y,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
     def isea3h_insert_cell(self, _values, _res):
         """ POST isea3h_insert_cell
@@ -2642,27 +2842,31 @@
         body = {
                  "_values": _values,
                  "_res": _res
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_neighbor_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_neighbor_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_neighbor_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, neighbor, properties} response object
@@ -2675,42 +2879,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_neighbor_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_neighbor_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_neighbor_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the neighbors of the DGGS cell.
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | ...
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, neighbor, properties} response object
@@ -2725,43 +2939,53 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_neighbor_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_neighbor_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_neighbor_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the neighbors of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, neighbor, properties} response object
@@ -2776,41 +3000,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_neighbor_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_neighbor_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_neighbor_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the neighbor of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, neighbor, properties} response object
@@ -2823,28 +3057,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_neighbor_by_point(self, _x, _y, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_neighbor_by_point(self, _x, _y, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_neighbor_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the neighbors of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _x : float
@@ -2853,14 +3093,18 @@
                 float | Y of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, neighbor, properties} response object
@@ -2877,42 +3121,52 @@
             logging.error('{}: {} is not {}'.format('_y', _y, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_x": _x,
                  "_y": _y,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_region_by_aoi(self, _aoi, _res=2, _data=[], _limit=10000):
+    def isea3h_region_by_aoi(self, _aoi, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_region_by_aoi
 
             This endpoint uses an area of interest(`_aoi`) and a cell resolution (`_res`) to find the cells, within that resolution, that intersect that area. It returns the GID of the DGGS cell.
 
         Parameters
         ------------
             _aoi : str
                 str | Area of interest
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, region, properties} response object
@@ -2925,42 +3179,52 @@
         # Field type check
         if type(_aoi) != str and _aoi is not None:
             logging.error('{}: {} is not {}'.format('_aoi', _aoi, 'text'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_aoi": _aoi,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_region_by_cell(self, _gid, _gid_res, _res=2, _data=[], _limit=10000):
+    def isea3h_region_by_cell(self, _gid, _gid_res, _res=2, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_region_by_cell
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the region of the DGGS cell.
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Grid cell ID
             _gid_res : int
                 int | ...
             _res : int
                 int | Optional, default is 2 | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | Max number of resulting records
 
         Returns
         -----------
             response:
                 {gid, quad, res, region, properties} response object
@@ -2975,23 +3239,29 @@
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_gid_res) != int and _gid_res is not None:
             logging.error('{}: {} is not {}'.format('_gid_res', _gid_res, 'integer'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
     def isea3h_region_by_cell_ras2dggs(self, _gid, _gid_res, _res=2, _limit=10000):
         """ POST isea3h_region_by_cell_ras2dggs
@@ -3035,29 +3305,33 @@
                  "_gid_res": _gid_res,
                  "_res": _res,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_region_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _limit=10000):
+    def isea3h_region_by_geojson(self, _geojson='{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}', _res=4, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_region_by_geojson
 
             This endpoint tasks a target resolution(`_res`) and a geojson geometry. It returns the region of the DGGS that intersects with a polygon/point given in geojson.
 
         Parameters
         ------------
             _geojson : dict
                 dict | Optional, default is '{"type":"Polygon","coordinates":[[[-180,90],[180,90],[180,-90],[-180,-90],[-180,90]]]}' | polygon feature in geojson format
             _res : int
                 int | Optional, default is 4 | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 | ...
 
         Returns
         -----------
             response:
                 {gid, quad, res, region, properties} response object
@@ -3072,41 +3346,51 @@
             logging.error('{}: {} is not {}'.format('_geojson', _geojson, 'json'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'smallint'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_geojson": _geojson,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_region_by_gid(self, _gid, _res, _data=[], _limit=10000):
+    def isea3h_region_by_gid(self, _gid, _res, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_region_by_gid
 
             This endpoint takes a list of `hex16` global identifiers `[_gid]` and a target resolution  `_res`. It returns the regions of the DGGS cells that match the given GIDs
 
         Parameters
         ------------
             _gid : str[]
                 str[] | Resolution level
             _res : int
                 int | Resolution level
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, region, properties} response object
@@ -3119,28 +3403,34 @@
         # Field type check
         if type(_gid) != list:
             logging.error('{}: {} is not {}'.format('_gid', _gid, 'ARRAY'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_gid": _gid,
                  "_res": _res,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
-    def isea3h_region_by_point(self, _x, _y, _res, _srid=4326, _data=[], _limit=10000):
+    def isea3h_region_by_point(self, _x, _y, _res, _srid=4326, _data=[], _startdate=None, _enddate=None, _limit=10000):
         """ POST isea3h_region_by_point
 
             This endpoint tasks a target resolution(`_res`) and a latitude/longitude(`_y`/`_x`) coordinate pair. It returns the region of the DGGS that intersects with that point.
 
         Parameters
         ------------
             _x : float
@@ -3149,14 +3439,18 @@
                 float | Y of the point
             _res : int
                 int | Resolution level
             _srid : int
                 int | Optional, default is 4326 | Spatial Reference System ID
             _data : str[]
                 str[] | Optional, default is [] |
+            _startdate : str
+                str | Optional, default is None |
+            _enddate : str
+                str | Optional, default is None |
             _limit : int
                 int | Optional, default is 10000 |
 
         Returns
         -----------
             response:
                 {gid, quad, res, region, properties} response object
@@ -3173,24 +3467,30 @@
             logging.error('{}: {} is not {}'.format('_y', _y, 'numeric'))
         if type(_res) != int and _res is not None:
             logging.error('{}: {} is not {}'.format('_res', _res, 'integer'))
         if type(_srid) != int and _srid is not None:
             logging.error('{}: {} is not {}'.format('_srid', _srid, 'integer'))
         if type(_data) != list:
             logging.error('{}: {} is not {}'.format('_data', _data, 'ARRAY'))
+        if type(_startdate) != str and _startdate is not None:
+            logging.error('{}: {} is not {}'.format('_startdate', _startdate, 'timestamp without time zone'))
+        if type(_enddate) != str and _enddate is not None:
+            logging.error('{}: {} is not {}'.format('_enddate', _enddate, 'timestamp without time zone'))
         if type(_limit) != int and _limit is not None:
             logging.error('{}: {} is not {}'.format('_limit', _limit, 'integer'))
 
         # Body
         body = {
                  "_x": _x,
                  "_y": _y,
                  "_res": _res,
                  "_srid": _srid,
                  "_data": _data,
+                 "_startdate": _startdate,
+                 "_enddate": _enddate,
                  "_limit": _limit
                 }
 
         return requests.post(self.url + endpoint, json=body, headers=self.headers)
 
     def isea3h_region_get_1435(self, _gid, _res):
         """ POST isea3h_region_get_1435
```

### Comparing `geoinsight-0.7.0/geoinsight/util.py` & `geoinsight-0.8.1/geoinsight/util.py`

 * *Files identical despite different names*

### Comparing `geoinsight-0.7.0/.gitignore` & `geoinsight-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geoinsight-0.7.0/README.md` & `geoinsight-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `geoinsight-0.7.0/pyproject.toml` & `geoinsight-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "geoinsight"
-version = "0.7.0"
+version = "0.8.1"
 authors = [
   {name="GeoInsight", email="info@geoinsight.ai"},
 ]
 description = "GeoInsight Python Package"
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `geoinsight-0.7.0/PKG-INFO` & `geoinsight-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: geoinsight
-Version: 0.7.0
+Version: 0.8.1
 Summary: GeoInsight Python Package
 Author-email: GeoInsight <info@geoinsight.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

