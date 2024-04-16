# Comparing `tmp/pyqqq-0.7.8.tar.gz` & `tmp/pyqqq-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.8.tar", max compression
+gzip compressed data, was "pyqqq-0.7.9.tar", max compression
```

## Comparing `pyqqq-0.7.8.tar` & `pyqqq-0.7.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.8/README.md
--rw-r--r--   0        0        0      770 2024-04-16 02:24:53.820646 pyqqq-0.7.8/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.8/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.8/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.8/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.8/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.8/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24284 2024-04-16 02:24:46.821115 pyqqq-0.7.8/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.8/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.8/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.8/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.8/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.8/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24453 2024-04-16 02:24:46.821820 pyqqq-0.7.8/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.8/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.8/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.8/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.8/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.8/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.8/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.8/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.8/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.8/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38134 2024-04-16 02:24:46.843534 pyqqq-0.7.8/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.8/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.8/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.7.8/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.8/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.8/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.8/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.8/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.8/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.7.8/pyqqq/utils/mock_api.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.8/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.9/README.md
+-rw-r--r--   0        0        0      770 2024-04-16 05:04:55.155142 pyqqq-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.9/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.9/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.9/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.9/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.9/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-16 05:02:35.915572 pyqqq-0.7.9/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.9/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.9/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.9/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.9/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.9/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24453 2024-04-16 02:24:46.821820 pyqqq-0.7.9/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.9/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.9/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.9/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.9/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.9/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.9/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.9/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.9/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.9/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38035 2024-04-16 05:04:16.530450 pyqqq-0.7.9/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.9/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.9/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.7.9/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.9/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.9/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.9/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.9/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.9/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.7.9/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.9/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.9/PKG-INFO
```

### Comparing `pyqqq-0.7.8/README.md` & `pyqqq-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyproject.toml` & `pyqqq-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.8"
+version = "0.7.9"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.8/pyqqq/__init__.py` & `pyqqq-0.7.9/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.9/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.9/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.9/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.9/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.9/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.9/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.9/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.9/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.9/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/data/domestic.py` & `pyqqq-0.7.9/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/data/minutes.py` & `pyqqq-0.7.9/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/data/realtime.py` & `pyqqq-0.7.9/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/data/ticks.py` & `pyqqq-0.7.9/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/datatypes.py` & `pyqqq-0.7.9/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/executors/hook.py` & `pyqqq-0.7.9/pyqqq/executors/hook.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,15 @@
                 if asset_stop_loss_threshold is not None:
                     # 사용자가 지정한 종목별 stop loss 레벨이 음수가 아닌 경우, 음수로 변환
                     if np.sign(asset_stop_loss_threshold) == 1:
                         asset_stop_loss_threshold *= -1
 
                     if p.current_pnl <= asset_stop_loss_threshold:
                         self.stock_broker.create_order(
-                            asset_code=p.asset_code,
-                            side=OrderSide.SELL,
-                            quantity=p.quantity,
+                            p.asset_code, OrderSide.SELL, p.quantity
                         )
 
     async def monitor_take_profit(
         self, positions: List, take_profit_config: Dict = {}
     ) -> None:
         logger.info("monitor_take_profit")
 
@@ -345,17 +343,15 @@
                 asset_take_profit_threshold = take_profit_config.get(p.asset_code)
                 if asset_take_profit_threshold is not None:
                     # 사용자가 지정한 종목별 take profit 레벨을 양수로 변환
                     asset_take_profit_threshold = abs(asset_take_profit_threshold)
 
                     if p.current_pnl >= asset_take_profit_threshold:
                         self.stock_broker.create_order(
-                            asset_code=p.asset_code,
-                            quantity=p.quantity,
-                            side=OrderSide.SELL,
+                            p.asset_code, OrderSide.SELL, p.quantity
                         )
 
     def execute_trades(self, trade_signals: List) -> None:
         """
         매매 지시에 따른 주문 제출
         - 매도 지시 먼저 완료 후 매수 지시 진행
         """
@@ -372,34 +368,34 @@
             asset_code = ts[0]
             price = int(ts[1])
             quantity = abs(int(ts[2]))
             side = OrderSide.SELL
             order_type = OrderType.LIMIT if price > 0 else OrderType.MARKET
 
             self.stock_broker.create_order(
-                asset_code=asset_code,
-                price=price,
-                quantity=quantity,
-                side=side,
-                order_type=order_type,
+                asset_code,
+                side,
+                quantity,
+                order_type,
+                price,
             )
 
         for ts in buy_signals:
             asset_code = ts[0]
             price = int(ts[1])
             quantity = abs(int(ts[2]))
             side = OrderSide.BUY
             order_type = OrderType.LIMIT if price > 0 else OrderType.MARKET
 
             self.stock_broker.create_order(
-                asset_code=asset_code,
-                price=price,
-                quantity=quantity,
-                side=side,
-                order_type=order_type,
+                asset_code,
+                side,
+                quantity,
+                order_type,
+                price,
             )
 
     def is_trading_day(self) -> bool:
         schedule = self.get_market_schedule()
 
         return not schedule.full_day_closed
 
@@ -748,28 +744,26 @@
             if not isinstance(order_id, int):
                 raise TypeError("Order ID must be an integer.")
             if not isinstance(quantity, int):
                 raise TypeError("Quantity must be an integer.")
 
             if quantity < 0:
                 # 취소 주문. quantity만큼 취소 주문 제출
-                self.stock_broker.cancel_order(
-                    order_id=order_id, asset_code=code, quantity=abs(quantity)
-                )
+                if self.brokerage == "kis":
+                    self.stock_broker.cancel_order(order_id, abs(quantity))
+                else:
+                    self.stock_broker.cancel_order(order_id, code, abs(quantity))
 
             elif quantity > 0:
                 if not isinstance(price, int):
                     raise TypeError("Price must be an integer.")
 
                 # 정정 주문. quantity를 price에 정정 주문 제출
                 self.stock_broker.update_order(
-                    org_order_id=order_id,
-                    asset_code=code,
-                    price=price,
-                    quantity=quantity,
+                    order_id, code, OrderType.LIMIT, price, quantity
                 )
 
     async def handle_pending_orders(
         self, pending_orders: List[Tuple[str, List]]
     ) -> None:
         """
         미체결 주문 처리 방식
@@ -782,23 +776,25 @@
             trade_instructions = await maybe_awaitable(
                 self.strategy_module.handle_pending_orders(
                     pending_orders, self.stock_broker
                 )
             )
             if type(trade_instructions) == list and len(trade_instructions) > 0:
                 self.handle_pending_orders_executor(trade_instructions)
-
         else:
             for orders in pending_orders:
                 for po in orders:
-                    self.stock_broker.cancel_order(
-                        order_id=po.order_id,
-                        asset_code=po.asset_code,
-                        quantity=po.pending_quantity,
-                    )
+                    if self.brokerage == "kis":
+                        self.stock_broker.cancel_order(po.order_no, po.pending_quantity)
+                    else:
+                        self.stock_broker.cancel_order(
+                            po.order_no,
+                            po.asset_code,
+                            po.pending_quantity,
+                        )
 
     async def on_market_open(self):
         """
         장 시작 시 최초에 1회 실행되는 함수
         사용자가 설정하는 전략 함수
         """
         if self._has_hook("on_market_open"):
```

### Comparing `pyqqq-0.7.8/pyqqq/utils/array.py` & `pyqqq-0.7.9/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/compute.py` & `pyqqq-0.7.9/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/display.py` & `pyqqq-0.7.9/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/kvstore.py` & `pyqqq-0.7.9/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/limiter.py` & `pyqqq-0.7.9/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/logger.py` & `pyqqq-0.7.9/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.9/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/mock_api.py` & `pyqqq-0.7.9/pyqqq/utils/mock_api.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/pyqqq/utils/retry.py` & `pyqqq-0.7.9/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.8/PKG-INFO` & `pyqqq-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.8
+Version: 0.7.9
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

