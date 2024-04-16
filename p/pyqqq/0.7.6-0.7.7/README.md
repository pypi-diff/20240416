# Comparing `tmp/pyqqq-0.7.6.tar.gz` & `tmp/pyqqq-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.6.tar", max compression
+gzip compressed data, was "pyqqq-0.7.7.tar", max compression
```

## Comparing `pyqqq-0.7.6.tar` & `pyqqq-0.7.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.6/README.md
--rw-r--r--   0        0        0      770 2024-04-15 09:44:45.938070 pyqqq-0.7.6/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.6/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.6/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.6/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.6/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.6/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.6/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.6/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.6/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.6/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.6/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.6/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.6/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.6/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.6/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.6/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.6/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.6/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.6/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.6/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.6/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.6/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38287 2024-04-15 04:43:35.649317 pyqqq-0.7.6/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.6/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.6/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-15 09:13:47.987198 pyqqq-0.7.6/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.6/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.6/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.6/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.6/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.6/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.6/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.7/README.md
+-rw-r--r--   0        0        0      770 2024-04-16 01:30:30.423944 pyqqq-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.7/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.7/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.7/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.7/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.7/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.7/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.7/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.7/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.7/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.7/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.7/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.7/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.7/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.7/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.7/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.7/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.7/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.7/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.7/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.7/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.7/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38085 2024-04-16 01:29:47.617925 pyqqq-0.7.7/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.7/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.7/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-15 09:13:47.987198 pyqqq-0.7.7/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.7/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.7/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.7/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.7/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.7/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.7/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.7/PKG-INFO
```

### Comparing `pyqqq-0.7.6/README.md` & `pyqqq-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyproject.toml` & `pyqqq-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.6"
+version = "0.7.7"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.6/pyqqq/__init__.py` & `pyqqq-0.7.7/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.7/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.7/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.7/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.7/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.7/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.7/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.7/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.7/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.7/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/data/domestic.py` & `pyqqq-0.7.7/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/data/minutes.py` & `pyqqq-0.7.7/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/data/realtime.py` & `pyqqq-0.7.7/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/data/ticks.py` & `pyqqq-0.7.7/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/datatypes.py` & `pyqqq-0.7.7/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/executors/hook.py` & `pyqqq-0.7.7/pyqqq/executors/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -776,15 +776,15 @@
         - 디폴트 설정은 취소 주문을 접수하도록 구현
 
         * 사용자가 override할 수 있도록 구현
         """
         if self._has_hook("handle_pending_orders"):
             logger.info(f"[EXECUTOR] Call handle_pending_orders hook")
             trade_instructions = await self.strategy_module.handle_pending_orders(
-                pending_orders=pending_orders, broker=self.stock_broker
+                pending_orders, self.stock_broker
             )
             if type(trade_instructions) == list and len(trade_instructions) > 0:
                 self.handle_pending_orders_executor(trade_instructions)
 
         else:
             for code, orders in pending_orders:
                 for po in orders:
@@ -803,18 +803,18 @@
             account_info = self.stock_broker.get_account()
             positions = self.stock_broker.get_positions()
             pending_orders = self.stock_broker.get_pending_orders()
 
             logger.info(f"[EXECUTOR] Call on_market_open hook")
             trade_signals = await maybe_awaitable(
                 self.strategy_module.on_market_open(
-                    account_info=account_info,
-                    pending_orders=pending_orders,
-                    positions=positions,
-                    broker=self.stock_broker,
+                    account_info,
+                    pending_orders,
+                    positions,
+                    self.stock_broker,
                 )
             )
 
             if type(trade_signals) == list and len(trade_signals) > 0:
                 self.validate_trade_signal(trade_signals, tag="on_market_open")
                 self.execute_trades(trade_signals=trade_signals)
 
@@ -851,18 +851,18 @@
             account_info = self.stock_broker.get_account()
             positions = self.stock_broker.get_positions()
             pending_orders = self.stock_broker.get_pending_orders()
 
             logger.info(f"[EXECUTOR] Call on_market_close hook")
             trade_signals = await maybe_awaitable(
                 self.strategy_module.on_market_close(
-                    account_info=account_info,
-                    pending_orders=pending_orders,
-                    positions=positions,
-                    broker=self.stock_broker,
+                    account_info,
+                    pending_orders,
+                    positions,
+                    self.stock_broker,
                 )
             )
 
             if type(trade_signals) == list and len(trade_signals) > 0:
                 self.validate_trade_signal(trade_signals, tag="on_market_close")
                 self.execute_trades(trade_signals=trade_signals)
 
@@ -906,35 +906,35 @@
             account_info = self.stock_broker.get_account()
             positions = self.stock_broker.get_positions()
             pending_orders = self.stock_broker.get_pending_orders()
 
             logger.info(f"[EXECUTOR] Call on_before_market_open hook")
             await maybe_awaitable(
                 self.strategy_module.on_before_market_open(
-                    account_info=account_info,
-                    pending_orders=pending_orders,
-                    positions=positions,
-                    broker=self.stock_broker,
+                    account_info,
+                    pending_orders,
+                    positions,
+                    self.stock_broker,
                 )
             )
 
     async def on_after_market_close(self):
         """매일 장 종료 후 1회 실행되는 함수"""
         if self._has_hook("on_after_market_close"):
             account_info = self.stock_broker.get_account()
             positions = self.stock_broker.get_positions()
             pending_orders = self.stock_broker.get_pending_orders()
 
             logger.info(f"[EXECUTOR] Call on_after_market_close hook")
             await maybe_awaitable(
                 self.strategy_module.on_after_market_close(
-                    account_info=account_info,
-                    pending_orders=pending_orders,
-                    positions=positions,
-                    broker=self.stock_broker,
+                    account_info,
+                    pending_orders,
+                    positions,
+                    self.stock_broker,
                 )
             )
 
 
 async def maybe_awaitable(result):
     if asyncio.iscoroutine(result) or isinstance(result, asyncio.Future):
         return await result
```

### Comparing `pyqqq-0.7.6/pyqqq/utils/array.py` & `pyqqq-0.7.7/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/compute.py` & `pyqqq-0.7.7/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/display.py` & `pyqqq-0.7.7/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/kvstore.py` & `pyqqq-0.7.7/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/limiter.py` & `pyqqq-0.7.7/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/logger.py` & `pyqqq-0.7.7/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.7/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/pyqqq/utils/retry.py` & `pyqqq-0.7.7/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.6/PKG-INFO` & `pyqqq-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.6
+Version: 0.7.7
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

