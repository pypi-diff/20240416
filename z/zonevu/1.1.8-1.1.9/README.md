# Comparing `tmp/zonevu-1.1.8-py3-none-any.whl.zip` & `tmp/zonevu-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1643335 bytes, number of entries: 805
+Zip file size: 1643345 bytes, number of entries: 805
 -rw-r--r--  2.0 fat       36 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/.gitignore
 -rw-r--r--  2.0 fat        2 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/@plugins_snapshot.json
 -rw-r--r--  2.0 fat     8174 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/__future__.data.json
 -rw-r--r--  2.0 fat     1632 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/__future__.meta.json
 -rw-r--r--  2.0 fat   180427 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_ast.data.json
 -rw-r--r--  2.0 fat     1649 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_ast.meta.json
 -rw-r--r--  2.0 fat    62778 b- defN 80-Jan-01 00:00 zonevu/.mypy_cache/3.11/_codecs.data.json
@@ -775,15 +775,15 @@
 -rw-r--r--  2.0 fat     1896 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/all_wells_to_storage.py
 -rw-r--r--  2.0 fat     1536 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/one_geomodel_save.py
 -rw-r--r--  2.0 fat     1248 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/one_project_save.py
 -rw-r--r--  2.0 fat     1390 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/one_seismic_save.py
 -rw-r--r--  2.0 fat     1271 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/one_well_to_storage.py
 -rw-r--r--  2.0 fat      846 b- defN 80-Jan-01 00:00 zonevu/Examples/Save/stratcolumn_save.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 zonevu/Services/__init__.py
--rw-r--r--  2.0 fat    10448 b- defN 80-Jan-01 00:00 zonevu/Services/Client.py
+-rw-r--r--  2.0 fat    10465 b- defN 80-Jan-01 00:00 zonevu/Services/Client.py
 -rw-r--r--  2.0 fat     1207 b- defN 80-Jan-01 00:00 zonevu/Services/CompanyService.py
 -rw-r--r--  2.0 fat     3354 b- defN 80-Jan-01 00:00 zonevu/Services/CompletionsService.py
 -rw-r--r--  2.0 fat     6857 b- defN 80-Jan-01 00:00 zonevu/Services/CoordinatesService.py
 -rw-r--r--  2.0 fat     4076 b- defN 80-Jan-01 00:00 zonevu/Services/DocumentService.py
 -rw-r--r--  2.0 fat     2356 b- defN 80-Jan-01 00:00 zonevu/Services/EndPoint.py
 -rw-r--r--  2.0 fat     1028 b- defN 80-Jan-01 00:00 zonevu/Services/Error.py
 -rw-r--r--  2.0 fat     7162 b- defN 80-Jan-01 00:00 zonevu/Services/GeomodelService.py
@@ -797,11 +797,11 @@
 -rw-r--r--  2.0 fat     2351 b- defN 80-Jan-01 00:00 zonevu/Services/SurveyService.py
 -rw-r--r--  2.0 fat     2738 b- defN 80-Jan-01 00:00 zonevu/Services/Utils.py
 -rw-r--r--  2.0 fat     2015 b- defN 80-Jan-01 00:00 zonevu/Services/WellData.py
 -rw-r--r--  2.0 fat     3810 b- defN 80-Jan-01 00:00 zonevu/Services/WelllogService.py
 -rw-r--r--  2.0 fat     9328 b- defN 80-Jan-01 00:00 zonevu/Services/WellService.py
 -rw-r--r--  2.0 fat     2002 b- defN 80-Jan-01 00:00 zonevu/Services/WelltopService.py
 -rw-r--r--  2.0 fat     5908 b- defN 80-Jan-01 00:00 zonevu/Zonevu.py
--rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 zonevu-1.1.8.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 zonevu-1.1.8.dist-info/WHEEL
-?rw-r--r--  2.0 fat    86308 b- defN 16-Jan-01 00:00 zonevu-1.1.8.dist-info/RECORD
-805 files, 25582049 bytes uncompressed, 1501611 bytes compressed:  94.1%
+-rw-r--r--  2.0 fat     1058 b- defN 80-Jan-01 00:00 zonevu-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 zonevu-1.1.9.dist-info/WHEEL
+?rw-r--r--  2.0 fat    86308 b- defN 16-Jan-01 00:00 zonevu-1.1.9.dist-info/RECORD
+805 files, 25582066 bytes uncompressed, 1501621 bytes compressed:  94.1%
```

## zipnote {}

```diff
@@ -2400,17 +2400,17 @@
 
 Filename: zonevu/Services/WelltopService.py
 Comment: 
 
 Filename: zonevu/Zonevu.py
 Comment: 
 
-Filename: zonevu-1.1.8.dist-info/METADATA
+Filename: zonevu-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: zonevu-1.1.8.dist-info/WHEEL
+Filename: zonevu-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: zonevu-1.1.8.dist-info/RECORD
+Filename: zonevu-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zonevu/Services/Client.py

```diff
@@ -37,15 +37,15 @@
 
         # Setup backoff strategy
         self._session = requests.Session()
         # Define the retry strategy  status_forcelist=[429, 500, 502, 503, 504]
         retry_strategy = Retry(
             total=5,  # Total number of retries status_forcelist=[429, 500, 502, 503, 504]to allow
             status_forcelist=[429],  # List of status codes to retry on
-            allowed_methods=["HEAD", "GET", "PUT", "DELETE", "OPTIONS", "TRACE"],  # List of methods to retry on
+            allowed_methods=["HEAD", "GET", "PUT", "POST", "PATCH", "DELETE", "OPTIONS", "TRACE"],  # List of methods to retry on
             backoff_factor=1  # A factor to multiply the delay between retries
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         self._session.mount("https://", adapter)
 
     def make_url(self, relativeUrl: str, query_params: Optional[Dict[str, Any]] = None, include_units: bool = True):
         if query_params is None:
```

## Comparing `zonevu-1.1.8.dist-info/METADATA` & `zonevu-1.1.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zonevu
-Version: 1.1.8
+Version: 1.1.9
 Summary: ZoneVu Web API Python Package
 Home-page: https://www.ubiterra.com/
 License: MIT
 Author: Ubiterra
 Author-email: support@ubiterra.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

## Comparing `zonevu-1.1.8.dist-info/RECORD` & `zonevu-1.1.9.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -774,15 +774,15 @@
 zonevu/Examples/Save/all_wells_to_storage.py,sha256=lOlhNe117-X1EFEONh6eM86OuTgtD1J4cyLGMzofG5w,1896
 zonevu/Examples/Save/one_geomodel_save.py,sha256=PnONsAX8EmgZ_cGLNa2cYYJTS-HqY1x0JMi5UbycgHQ,1536
 zonevu/Examples/Save/one_project_save.py,sha256=AvvZTHYs1gEQNDFZcjzoFUaZh3sFCkSz_ynJhzeVB8c,1248
 zonevu/Examples/Save/one_seismic_save.py,sha256=0x6yDueau1wKXDV-dSMikpQDBc8O5GyKROFgjh2-wP8,1390
 zonevu/Examples/Save/one_well_to_storage.py,sha256=Z4wG-5qDsAZV51j5EWCJIE9qRBkbMabm_IoFpA_Urb8,1271
 zonevu/Examples/Save/stratcolumn_save.py,sha256=h1RSSiTJYhmaH3cPdENLmp6s0AzGFskPqpFpKAc7PQU,846
 zonevu/Services/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-zonevu/Services/Client.py,sha256=8FaflQseDW4eN8PA0Dp_MDJU-CGHIA4WUve8pgfSvHc,10448
+zonevu/Services/Client.py,sha256=8vhvIheiYvRm51vOX_5XM94sYzBGSByb7tNf9DA2HMs,10465
 zonevu/Services/CompanyService.py,sha256=CcP7FYgERoDq-vAerDPPcIprqZfqZG74sD6OCdw39ZM,1207
 zonevu/Services/CompletionsService.py,sha256=DI18hvEgwV1c5uvXBjM2bIkyqD4Ncphl_BfPrBdRX1Q,3354
 zonevu/Services/CoordinatesService.py,sha256=fw3jss0eeDV6AFD4fEEGvcSL3xxRWaF7RgQ5XqU2rjs,6857
 zonevu/Services/DocumentService.py,sha256=CXz4jptnPo4MLXeV17KWr0mxTSoG3gkFuzs1l5nKP8w,4076
 zonevu/Services/EndPoint.py,sha256=Gixd6b07Fqdg5ZWXLFeMbuf0XQmJhJvy71xiPNhBYOE,2356
 zonevu/Services/Error.py,sha256=NLpMPWRGpA5aX9xFaKo2bNIO8BDqXzU7oshjZXzbxgE,1028
 zonevu/Services/GeomodelService.py,sha256=QuBvB6NPPHZgumxYFX6nTwkeWoQLhqEn4O-XplMIDWk,7162
@@ -796,10 +796,10 @@
 zonevu/Services/SurveyService.py,sha256=QYEH6VKKuPbeRNamun256q30_D1rtESQbFLm5nIMWTU,2351
 zonevu/Services/Utils.py,sha256=3y_H9ouSNzZoyvRcFhI4eFPqrk61RPMnNEVoKdAo6M0,2738
 zonevu/Services/WellData.py,sha256=JRl7SDoLyl57-41du7TrQk0Hn820LDWgWAzfX5X85pQ,2015
 zonevu/Services/WelllogService.py,sha256=43XlmWVynJJMaKeFMyE4aas3nd4CyIFxA7QoQewIPgA,3810
 zonevu/Services/WellService.py,sha256=VpQoMv0_kYbOXXxp5e0rZqlonFR9lqXrp_w75uuaUk4,9328
 zonevu/Services/WelltopService.py,sha256=85DFGT3DSrqZIxyam8JM8PZ_PNqeq3v0LhrgPJoLM_8,2002
 zonevu/Zonevu.py,sha256=ouU3muL7hcqMdArEKcTcOJhsCkpsmTcNQII8g-a9cJE,5908
-zonevu-1.1.8.dist-info/METADATA,sha256=dz6pDu-tMB-Zy126XD0p9FoJIRwL0VnZez6nJXM47fo,1058
-zonevu-1.1.8.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-zonevu-1.1.8.dist-info/RECORD,,
+zonevu-1.1.9.dist-info/METADATA,sha256=ijH0gNYP3gjZHyr_1b52Kl3H-rn-nAPbbYKLp9bhqEo,1058
+zonevu-1.1.9.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+zonevu-1.1.9.dist-info/RECORD,,
```

