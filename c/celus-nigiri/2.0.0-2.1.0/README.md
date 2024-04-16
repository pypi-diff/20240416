# Comparing `tmp/celus_nigiri-2.0.0.tar.gz` & `tmp/celus_nigiri-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celus_nigiri-2.0.0.tar", max compression
+gzip compressed data, was "celus_nigiri-2.1.0.tar", max compression
```

## Comparing `celus_nigiri-2.0.0.tar` & `celus_nigiri-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1052 2022-07-22 09:08:04.346975 celus_nigiri-2.0.0/LICENSE
--rw-r--r--   0        0        0       63 2024-03-18 16:37:21.128669 celus_nigiri-2.0.0/celus_nigiri/__init__.py
--rw-r--r--   0        0        0     3154 2024-03-18 16:37:21.120669 celus_nigiri-2.0.0/celus_nigiri/celus.py
--rw-r--r--   0        0        0    17981 2024-03-18 16:37:51.832703 celus_nigiri-2.0.0/celus_nigiri/client.py
--rw-r--r--   0        0        0     3808 2024-03-18 16:37:21.124669 celus_nigiri-2.0.0/celus_nigiri/counter4.py
--rw-r--r--   0        0        0    19615 2024-03-18 16:38:56.392769 celus_nigiri-2.0.0/celus_nigiri/counter5.py
--rw-r--r--   0        0        0     2716 2024-03-18 16:37:21.124669 celus_nigiri-2.0.0/celus_nigiri/csv_detect/__init__.py
--rw-r--r--   0        0        0      734 2022-12-15 15:30:38.889754 celus_nigiri-2.0.0/celus_nigiri/csv_detect/__main__.py
--rw-r--r--   0        0        0        0 2024-03-18 14:21:20.036714 celus_nigiri-2.0.0/celus_nigiri/download/__init__.py
--rw-r--r--   0        0        0     2249 2024-03-18 14:21:20.040714 celus_nigiri-2.0.0/celus_nigiri/download/__main__.py
--rw-r--r--   0        0        0     3926 2022-07-12 14:45:27.530086 celus_nigiri-2.0.0/celus_nigiri/error_codes.py
--rw-r--r--   0        0        0      212 2024-03-18 16:37:21.124669 celus_nigiri-2.0.0/celus_nigiri/exceptions.py
--rw-r--r--   0        0        0     2143 2024-03-18 16:39:33.444805 celus_nigiri-2.0.0/celus_nigiri/record.py
--rw-r--r--   0        0        0     1614 2024-03-18 16:37:21.128669 celus_nigiri-2.0.0/celus_nigiri/utils.py
--rw-r--r--   0        0        0     1291 2024-03-18 16:43:59.529027 celus_nigiri-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 celus_nigiri-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2022-07-22 09:08:04.346975 celus_nigiri-2.1.0/LICENSE
+-rw-r--r--   0        0        0       63 2024-03-18 16:37:21.128669 celus_nigiri-2.1.0/celus_nigiri/__init__.py
+-rw-r--r--   0        0        0     3154 2024-03-18 16:37:21.120669 celus_nigiri-2.1.0/celus_nigiri/celus.py
+-rw-r--r--   0        0        0    18417 2024-04-15 14:43:20.507022 celus_nigiri-2.1.0/celus_nigiri/client.py
+-rw-r--r--   0        0        0     3808 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/counter4.py
+-rw-r--r--   0        0        0    20034 2024-04-16 09:00:37.721970 celus_nigiri-2.1.0/celus_nigiri/counter5.py
+-rw-r--r--   0        0        0     2716 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/csv_detect/__init__.py
+-rw-r--r--   0        0        0      734 2022-12-15 15:30:38.889754 celus_nigiri-2.1.0/celus_nigiri/csv_detect/__main__.py
+-rw-r--r--   0        0        0        0 2024-03-18 14:21:20.036714 celus_nigiri-2.1.0/celus_nigiri/download/__init__.py
+-rw-r--r--   0        0        0     2249 2024-03-18 14:21:20.040714 celus_nigiri-2.1.0/celus_nigiri/download/__main__.py
+-rw-r--r--   0        0        0     3926 2022-07-12 14:45:27.530086 celus_nigiri-2.1.0/celus_nigiri/error_codes.py
+-rw-r--r--   0        0        0      212 2024-03-18 16:37:21.124669 celus_nigiri-2.1.0/celus_nigiri/exceptions.py
+-rw-r--r--   0        0        0     2143 2024-03-18 16:39:33.444805 celus_nigiri-2.1.0/celus_nigiri/record.py
+-rw-r--r--   0        0        0     1614 2024-03-18 16:37:21.128669 celus_nigiri-2.1.0/celus_nigiri/utils.py
+-rw-r--r--   0        0        0     1291 2024-04-16 09:03:32.150312 celus_nigiri-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 celus_nigiri-2.1.0/PKG-INFO
```

### Comparing `celus_nigiri-2.0.0/LICENSE` & `celus_nigiri-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/celus.py` & `celus_nigiri-2.1.0/celus_nigiri/celus.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/client.py` & `celus_nigiri-2.1.0/celus_nigiri/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,30 @@
         return response.content
 
     def get_available_reports(self, params=None) -> typing.Generator[dict, None, None]:
         content = self.get_available_reports_raw(params=params)
         reports = self.report_to_data(content)
         return reports
 
+    def make_download_url(self, report_type):
+        """
+        Prepare download url of a sushi server
+        """
+        report_type = self._check_report_type(report_type)
+        return "/".join([self.url.rstrip("/"), "reports", report_type])
+
+    def make_download_params(self, extra_params, begin_date, end_date):
+        """
+        Prepare download params which are used to query sushi server
+        """
+        params = self._construct_url_params(extra=extra_params)
+        params["begin_date"] = self._encode_date(begin_date)
+        params["end_date"] = self._encode_date(end_date)
+        return params
+
     def fetch_report_data(
         self,
         report_type,
         begin_date,
         end_date,
         dump_file: typing.Optional[typing.IO] = None,
         params=None,
@@ -252,19 +268,16 @@
         :param report_type:
         :param begin_date:
         :param end_date:
         :param dump_file: where to put file output
         :param params:
         :return:
         """
-        report_type = self._check_report_type(report_type)
-        url = "/".join([self.url.rstrip("/"), "reports", report_type])
-        params = self._construct_url_params(extra=params)
-        params["begin_date"] = self._encode_date(begin_date)
-        params["end_date"] = self._encode_date(end_date)
+        url = self.make_download_url(report_type)
+        params = self.make_download_params(params, begin_date, end_date)
         response = self._make_request(url, params, stream=bool(dump_file))
         if dump_file is not None:
             for data in response.iter_content(1024 * 1024):
                 dump_file.write(data)
             dump_file.seek(0)
         return response
```

### Comparing `celus_nigiri-2.0.0/celus_nigiri/counter4.py` & `celus_nigiri-2.1.0/celus_nigiri/counter4.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/counter5.py` & `celus_nigiri-2.1.0/celus_nigiri/counter5.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,15 @@
         "Access_Type",
         "Access_Method",
         "Data_Type",
         "YOP",
         "Publisher",
         "Platform",
         "Article_Version",
+        "Parent_Data_Type",
     ]
     allowed_item_ids = ALLOWED_ITEM_IDS["IR"]
 
     @classmethod
     def _item_get_title(cls, item):
         return item.get("Item_Parent", {}).get("Item_Name", "")
 
@@ -415,14 +416,22 @@
     def _item_get_item_ids(cls, item):
         return cls._extract_title_ids(item.get("Item_ID", []) or [])
 
     @classmethod
     def _item_get_title_ids(cls, item):
         return cls._extract_title_ids(item.get("Item_Parent", {}).get("Item_ID", []) or [])
 
+    @classmethod
+    def _extract_dimension_data(cls, dimensions: list, record: dict):
+        res = super()._extract_dimension_data(dimensions, record)
+        # enrich result with Parent_Data_Type => it can be useful during processing
+        if parent_data_type := record.get("Item_Parent", {}).get("Data_Type"):
+            res["Parent_Data_Type"] = parent_data_type
+        return res
+
 
 class Counter5IRM1Report(Counter5IRReport):
     dimensions = ["Publisher", "Platform"]
     allowed_item_ids = ALLOWED_ITEM_IDS["IR_M1"]
 
 
 class Counter5TableReport:
```

### Comparing `celus_nigiri-2.0.0/celus_nigiri/csv_detect/__init__.py` & `celus_nigiri-2.1.0/celus_nigiri/csv_detect/__init__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/csv_detect/__main__.py` & `celus_nigiri-2.1.0/celus_nigiri/csv_detect/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/download/__main__.py` & `celus_nigiri-2.1.0/celus_nigiri/download/__main__.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/error_codes.py` & `celus_nigiri-2.1.0/celus_nigiri/error_codes.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/record.py` & `celus_nigiri-2.1.0/celus_nigiri/record.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/celus_nigiri/utils.py` & `celus_nigiri-2.1.0/celus_nigiri/utils.py`

 * *Files identical despite different names*

### Comparing `celus_nigiri-2.0.0/pyproject.toml` & `celus_nigiri-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 "test_*.py" = ["B011"]  # test files should have asserts
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 
 [tool.poetry]
 name = "celus-nigiri"
-version = "2.0.0"
+version = "2.1.0"
 description = "Library for downloading and parsing counter-like data."
 authors = ["Beda Kosata <beda@bigdigdata.com>", "Stepan Henek <stepan@bigdigdata.com>"]
 license = "MIT"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"Topic :: Software Development :: Libraries"
 ]
```

### Comparing `celus_nigiri-2.0.0/PKG-INFO` & `celus_nigiri-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celus-nigiri
-Version: 2.0.0
+Version: 2.1.0
 Summary: Library for downloading and parsing counter-like data.
 License: MIT
 Author: Beda Kosata
 Author-email: beda@bigdigdata.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

