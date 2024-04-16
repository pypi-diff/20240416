# Comparing `tmp/pyqqq-0.8.0.tar.gz` & `tmp/pyqqq-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.8.0.tar", max compression
+gzip compressed data, was "pyqqq-0.8.1.tar", max compression
```

## Comparing `pyqqq-0.8.0.tar` & `pyqqq-0.8.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.8.0/README.md
--rw-r--r--   0        0        0      770 2024-04-16 05:13:52.737353 pyqqq-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      668 2024-04-16 05:13:25.694767 pyqqq-0.8.0/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.8.0/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.8.0/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.8.0/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.8.0/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24284 2024-04-16 05:02:35.915572 pyqqq-0.8.0/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.8.0/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.8.0/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.8.0/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.8.0/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.8.0/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24453 2024-04-16 02:24:46.821820 pyqqq-0.8.0/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.8.0/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.8.0/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.8.0/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.8.0/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.8.0/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.8.0/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.8.0/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.8.0/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.8.0/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.8.0/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.8.0/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.8.0/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.8.0/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.8.0/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.8.0/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.8.0/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.8.0/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.8.0/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.8.0/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.8.0/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-28 03:41:58.980653 pyqqq-0.8.1/README.md
+-rw-r--r--   0        0        0      770 2024-04-16 07:22:34.979272 pyqqq-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      668 2024-04-16 07:09:31.610419 pyqqq-0.8.1/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302843 pyqqq-0.8.1/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-05 03:59:24.168676 pyqqq-0.8.1/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-12 08:13:19.751599 pyqqq-0.8.1/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-28 03:41:58.983583 pyqqq-0.8.1/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-16 07:09:31.610652 pyqqq-0.8.1/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 03:41:58.983800 pyqqq-0.8.1/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-03-04 03:59:43.302986 pyqqq-0.8.1/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 02:04:49.386336 pyqqq-0.8.1/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-28 03:41:58.984873 pyqqq-0.8.1/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-07 02:05:26.670417 pyqqq-0.8.1/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24453 2024-04-16 07:09:31.611164 pyqqq-0.8.1/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-22 01:44:28.626559 pyqqq-0.8.1/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-16 02:21:33.322054 pyqqq-0.8.1/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670533 pyqqq-0.8.1/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6677 2024-04-16 07:14:50.116239 pyqqq-0.8.1/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-12 08:13:19.753178 pyqqq-0.8.1/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-12 08:13:19.753716 pyqqq-0.8.1/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-12 08:13:19.754108 pyqqq-0.8.1/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-22 01:44:28.626857 pyqqq-0.8.1/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 08:13:19.754190 pyqqq-0.8.1/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 07:09:31.611654 pyqqq-0.8.1/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0   462038 2024-04-16 05:47:11.692471 pyqqq-0.8.1/pyqqq/test.ipynb
+-rw-r--r--   0        0        0        0 2024-03-07 02:05:26.670737 pyqqq-0.8.1/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-12 08:13:19.754605 pyqqq-0.8.1/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-16 07:09:31.611787 pyqqq-0.8.1/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:49:01.142004 pyqqq-0.8.1/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-22 01:44:28.626942 pyqqq-0.8.1/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-03-04 03:59:43.304644 pyqqq-0.8.1/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-28 03:41:58.986410 pyqqq-0.8.1/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 02:18:36.457903 pyqqq-0.8.1/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 07:09:31.611989 pyqqq-0.8.1/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-03-04 03:59:43.304764 pyqqq-0.8.1/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.8.1/PKG-INFO
```

### Comparing `pyqqq-0.8.0/README.md` & `pyqqq-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyproject.toml` & `pyqqq-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.8.0"
+version = "0.8.1"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.8.0/pyqqq/__init__.py` & `pyqqq-0.8.1/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.8.1/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.8.1/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.8.1/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.8.1/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.8.1/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.8.1/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.8.1/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.8.1/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.8.1/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/data/domestic.py` & `pyqqq-0.8.1/pyqqq/data/domestic.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,21 +112,22 @@
     Returns:
         pd.DataFrame|None: 기본정보 리스트. 데이터가 없으면 None
 
         - code (str, index): 종목코드
         - isin (str): 국제 증권 식별 번호
         - name (str): 이름
         - market (str): 거래소
+        - type (str): 종목유형. EQUITY(일반상품), ETF, ETN
 
     Examples:
         >>> df = get_ticker_info("005930")
         >>> print(df)
-                isin  name market
+                isin  name market    type
         code
-        005930  KR7005930003  삼성전자  KOSPI
+        005930  KR7005930003  삼성전자  KOSPI  EQUITY
     """
     return _ticker_request('code', code)
 
 
 def find_ticker_info(name: str) -> pd.DataFrame | None:
     """
     종목명으로 기본정보를 조회합니다.
@@ -136,21 +137,21 @@
 
     Returns:
         pd.DataFrame|None: 기본정보 리스트. 데이터가 없으면 None
 
     Examples:
         >>> df = find_ticker_info("삼성")
         >>> print(df.head())
-                isin   name market
+                isin   name market    type
         code
-        000810  KR7000810002   삼성화재  KOSPI
-        000815  KR7000811000  삼성화재우  KOSPI
-        001360  KR7001360007   삼성제약  KOSPI
-        005930  KR7005930003   삼성전자  KOSPI
-        005935  KR7005931001  삼성전자우  KOSPI
+        000810  KR7000810002   삼성화재  KOSPI  EQUITY
+        000815  KR7000811000  삼성화재우  KOSPI  EQUITY
+        001360  KR7001360007   삼성제약  KOSPI  EQUITY
+        005930  KR7005930003   삼성전자  KOSPI  EQUITY
+        005935  KR7005931001  삼성전자우  KOSPI  EQUITY
     """
     return _ticker_request('name', name)
 
 
 def _ticker_request(type: str, value: str):
     url = f"{c.PYQQQ_API_URL}/domestic-stock/tickers"
     params = {
```

### Comparing `pyqqq-0.8.0/pyqqq/data/minutes.py` & `pyqqq-0.8.1/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/data/realtime.py` & `pyqqq-0.8.1/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/data/ticks.py` & `pyqqq-0.8.1/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/datatypes.py` & `pyqqq-0.8.1/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/executors/hook.py` & `pyqqq-0.8.1/pyqqq/executors/hook.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/array.py` & `pyqqq-0.8.1/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/compute.py` & `pyqqq-0.8.1/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/display.py` & `pyqqq-0.8.1/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/kvstore.py` & `pyqqq-0.8.1/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/limiter.py` & `pyqqq-0.8.1/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/logger.py` & `pyqqq-0.8.1/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/market_schedule.py` & `pyqqq-0.8.1/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/mock_api.py` & `pyqqq-0.8.1/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/pyqqq/utils/retry.py` & `pyqqq-0.8.1/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.8.0/PKG-INFO` & `pyqqq-0.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.8.0
+Version: 0.8.1
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

