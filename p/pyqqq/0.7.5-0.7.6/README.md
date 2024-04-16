# Comparing `tmp/pyqqq-0.7.5.tar.gz` & `tmp/pyqqq-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.5.tar", max compression
+gzip compressed data, was "pyqqq-0.7.6.tar", max compression
```

## Comparing `pyqqq-0.7.5.tar` & `pyqqq-0.7.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.5/README.md
--rw-r--r--   0        0        0      770 2024-04-15 01:46:57.812691 pyqqq-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.5/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.5/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.5/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.5/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.5/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.5/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.5/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.5/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.5/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.5/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.5/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.5/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.5/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.5/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.5/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.5/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.5/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.5/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.5/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.5/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.5/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38287 2024-04-12 09:46:36.906208 pyqqq-0.7.5/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.5/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.5/pyqqq/utils/array.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.5/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.5/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.5/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.5/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.5/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.5/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.6/README.md
+-rw-r--r--   0        0        0      770 2024-04-15 09:44:45.938070 pyqqq-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.6/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.6/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.6/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.6/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.6/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.6/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.6/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.6/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.6/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.6/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.6/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.6/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.6/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.6/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.6/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.6/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.6/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.6/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.6/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.6/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.6/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38287 2024-04-15 04:43:35.649317 pyqqq-0.7.6/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.6/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.6/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-15 09:13:47.987198 pyqqq-0.7.6/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.6/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.6/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.6/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.6/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.6/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.6/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.6/PKG-INFO
```

### Comparing `pyqqq-0.7.5/README.md` & `pyqqq-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyproject.toml` & `pyqqq-0.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.5"
+version = "0.7.6"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.5/pyqqq/__init__.py` & `pyqqq-0.7.6/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.6/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.6/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.6/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.6/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.6/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.6/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.6/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.6/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.6/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/data/domestic.py` & `pyqqq-0.7.6/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/data/minutes.py` & `pyqqq-0.7.6/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/data/realtime.py` & `pyqqq-0.7.6/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/data/ticks.py` & `pyqqq-0.7.6/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/datatypes.py` & `pyqqq-0.7.6/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/executors/hook.py` & `pyqqq-0.7.6/pyqqq/executors/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,15 +229,15 @@
         elif "market_open_time" in config:
             market_open_time = config.get("market_open_time")
             if type(market_open_time) != dtm.time:
                 raise Exception("market_open_time must be time type")
 
             tm = dtm.datetime.combine(dtm.date.today(), market_open_time)
             if tm < self.market_open_time:
-                raise Exception("market_open_time must be later than market open time")
+                raise Exception("market_open_time must be earlier than market open time")
 
             self.market_open_time_margin = tm - self.market_open_time
 
         if "close_market_time_margin" in config:
             close_market_time_margin = config.get("close_market_time_margin")
             if type(close_market_time_margin) == dtm.timedelta:
                 self.market_close_time_margin = close_market_time_margin
@@ -254,15 +254,15 @@
             market_close_time = config.get("market_close_time")
             if type(market_close_time) != dtm.time:
                 raise Exception("market_close_time must be time type")
 
             tm = dtm.datetime.combine(dtm.date.today(), market_close_time)
             if tm > self.market_close_time:
                 raise Exception(
-                    "market_close_time must be earlier than market close time"
+                    "market_close_time must be later than market close time"
                 )
 
             self.market_close_time_margin = self.market_close_time - tm
 
         if "before_market_open_schedule" in config:
             before_market_open_schedule = config.get("before_market_open_schedule")
             if type(before_market_open_schedule) == int:
```

### Comparing `pyqqq-0.7.5/pyqqq/utils/array.py` & `pyqqq-0.7.6/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/display.py` & `pyqqq-0.7.6/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/kvstore.py` & `pyqqq-0.7.6/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/limiter.py` & `pyqqq-0.7.6/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/logger.py` & `pyqqq-0.7.6/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.6/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/pyqqq/utils/retry.py` & `pyqqq-0.7.6/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.5/PKG-INFO` & `pyqqq-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.5
+Version: 0.7.6
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

