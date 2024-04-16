# Comparing `tmp/pyqqq-0.7.7.tar.gz` & `tmp/pyqqq-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.7.tar", max compression
+gzip compressed data, was "pyqqq-0.7.8.tar", max compression
```

## Comparing `pyqqq-0.7.7.tar` & `pyqqq-0.7.8.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.7/README.md
--rw-r--r--   0        0        0      770 2024-04-16 01:30:30.423944 pyqqq-0.7.7/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.7/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.7/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.7/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.7/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.7/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.7/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.7/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.7/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.7/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.7/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.7/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.7/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.7/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.7/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.7/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.7/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.7/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.7/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.7/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.7/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.7/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    38085 2024-04-16 01:29:47.617925 pyqqq-0.7.7/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.7/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.7/pyqqq/utils/array.py
--rw-r--r--   0        0        0     3205 2024-04-15 09:13:47.987198 pyqqq-0.7.7/pyqqq/utils/compute.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.7/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.7/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.7/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.7/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.7/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.7/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.8/README.md
+-rw-r--r--   0        0        0      770 2024-04-16 02:24:53.820646 pyqqq-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.8/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.8/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.8/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.8/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.8/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24284 2024-04-16 02:24:46.821115 pyqqq-0.7.8/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.8/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.8/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.8/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.8/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.8/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24453 2024-04-16 02:24:46.821820 pyqqq-0.7.8/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.8/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.8/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.8/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.8/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.8/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.8/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.8/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.8/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.8/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38134 2024-04-16 02:24:46.843534 pyqqq-0.7.8/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:10:29.432687 pyqqq-0.7.8/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.8/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     3205 2024-04-16 02:15:48.378231 pyqqq-0.7.8/pyqqq/utils/compute.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.8/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.8/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.8/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.8/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.8/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0    10571 2024-04-16 02:24:46.823810 pyqqq-0.7.8/pyqqq/utils/mock_api.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.8/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.8/PKG-INFO
```

### Comparing `pyqqq-0.7.7/README.md` & `pyqqq-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyproject.toml` & `pyqqq-0.7.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.7"
+version = "0.7.8"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.7/pyqqq/__init__.py` & `pyqqq-0.7.8/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.8/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.8/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.8/pyqqq/brokerage/ebest/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 from pyqqq.brokerage.ebest.domestic_stock import EBestDomesticStock
 from pyqqq.brokerage.ebest.oauth import EBestAuth
 from pyqqq.data.realtime import get_all_last_trades
 from pyqqq.datatypes import *
 from pyqqq.utils.logger import get_logger
 from pyqqq.utils.market_schedule import get_market_schedule
+from pyqqq.utils.mock_api import with_mock
 from typing import List, Optional, Set
 import datetime as dtm
 import pandas as pd
 
 
 @dataclass
 class EBestStockPosition:
@@ -82,14 +83,15 @@
         auth (EBestAuth): 인증 정보
     """
 
     def __init__(self, auth: EBestAuth):
         self.stock_api = EBestDomesticStock(auth)
         self.logger = get_logger(__name__)
 
+    @with_mock()
     def get_account(self) -> dict:
         """
         계좌 정보를 조회합니다.
 
         Returns:
             dict: 계좌 정보
 
@@ -118,14 +120,15 @@
             "purchase_amount": purchase_amount,
             "evaluated_amount": evaluated_amount,
             "pnl_amount": pnl_amount,
             "pnl_rate": pnl_rate,
         }
         return result
 
+    @with_mock()
     def get_possible_quantity(
         self, asset_code: str, order_type: OrderType = OrderType.MARKET, price: int = 0
     ) -> dict:
         """
         주문 가능 수량을 조회합니다.
 
         Args:
@@ -155,14 +158,15 @@
             "reusable_amount": output2["RuseObjAmt"],
             "price": int(Decimal(output1["OrdPrc"])),
             "quantity": output2["OrdAbleQty"],
             "amount": output2["OrdAbleAmt"],
         }
         return result
 
+    @with_mock()
     def get_positions(self) -> List[EBestStockPosition]:
         """
         보유 종목을 조회합니다.
 
         Returns:
             List[EBestStockPosition]: 보유 종목 정보 리스트
         """
@@ -200,14 +204,15 @@
                     result.append(position)
 
             if cts_expcode.strip() == "":
                 fetching = False
 
         return result
 
+    @with_mock()
     def get_historical_daily_data(
         self,
         asset_code: str,
         first_date: dtm.date,
         last_date: dtm.date,
         adjusted_price: bool = False,
     ) -> pd.DataFrame:
@@ -415,14 +420,15 @@
                     }
                 )
 
         df = pd.DataFrame(result)
         df.set_index("code", inplace=True)
         return df
 
+    @with_mock()
     def create_order(
         self,
         asset_code: str,
         side: OrderSide,
         quantity: int,
         order_type: OrderType = OrderType.MARKET,
         price: int = 0,
@@ -484,14 +490,15 @@
             ord_cndi_tp_code=__get_ord_cndi_tp_code(),
         )
 
         print(r)
 
         return r["output2"]["OrdNo"]
 
+    @with_mock()
     def update_order(
         self,
         org_order_no: str,
         asset_code: str,
         order_type: OrderType,
         price: int,
         quantity: int = 0,
@@ -542,14 +549,15 @@
             __get_ord_prc_ptn_code(),
             __get_ord_cndi_tp_code(),
             price,
         )
 
         return r["output2"]["OrdNo"]
 
+    @with_mock()
     def cancel_order(self, org_order_no: str, asset_code: str, quantity: int) -> str:
         """
         주문을 취소합니다.
 
         Args:
             org_order_no (str): 원주문번호
             quantity (int): 취소 수량
```

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.8/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.8/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.8/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.8/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.8/pyqqq/brokerage/kis/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 from decimal import Decimal
 from pyqqq.brokerage.kis.domestic_stock import KISDomesticStock
 from pyqqq.brokerage.kis.oauth import KISAuth
 from pyqqq.data.realtime import get_all_last_trades
 from pyqqq.datatypes import *
 from pyqqq.utils.market_schedule import get_market_schedule
+from pyqqq.utils.mock_api import with_mock
 from typing import List, Optional
 import datetime as dtm
 import pandas as pd
 
 
 @dataclass
 class KISStockPosition:
@@ -400,14 +401,15 @@
                     'low_price': item['low'],
                 })
 
         df = pd.DataFrame(result)
         df.set_index('code', inplace=True)
         return df
 
+    @with_mock()
     def create_order(self,
                      asset_code: str,
                      side: OrderSide,
                      quantity: int,
                      order_type: OrderType = OrderType.MARKET,
                      price: int = 0) -> str:
 
@@ -467,14 +469,15 @@
             __get_order_type_code(),
             quantity,
             price,
         )
 
         return r['output']['ODNO']
 
+    @with_mock()
     def update_order(self,
                      org_order_no: str,
                      order_type: OrderType,
                      price: int,
                      quantity: int = 0) -> str:
 
         """
@@ -527,14 +530,15 @@
             quantity,
             price,
             qty_all_ord_yn
         )
 
         return r['output']['ODNO']
 
+    @with_mock()
     def cancel_order(self, org_order_no: str, quantity: int = 0) -> str:
         """
         주문을 취소합니다.
 
         Args:
             org_order_no (str): 원주문번호
             quantity (int): 취소 수량 (일부 취소의 경우 지정)
```

### Comparing `pyqqq-0.7.7/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.8/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/data/domestic.py` & `pyqqq-0.7.8/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/data/minutes.py` & `pyqqq-0.7.8/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/data/realtime.py` & `pyqqq-0.7.8/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/data/ticks.py` & `pyqqq-0.7.8/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/datatypes.py` & `pyqqq-0.7.8/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/executors/hook.py` & `pyqqq-0.7.8/pyqqq/executors/hook.py`

 * *Files 0% similar despite different names*

```diff
@@ -775,22 +775,24 @@
         미체결 주문 처리 방식
         - 디폴트 설정은 취소 주문을 접수하도록 구현
 
         * 사용자가 override할 수 있도록 구현
         """
         if self._has_hook("handle_pending_orders"):
             logger.info(f"[EXECUTOR] Call handle_pending_orders hook")
-            trade_instructions = await self.strategy_module.handle_pending_orders(
-                pending_orders, self.stock_broker
+            trade_instructions = await maybe_awaitable(
+                self.strategy_module.handle_pending_orders(
+                    pending_orders, self.stock_broker
+                )
             )
             if type(trade_instructions) == list and len(trade_instructions) > 0:
                 self.handle_pending_orders_executor(trade_instructions)
 
         else:
-            for code, orders in pending_orders:
+            for orders in pending_orders:
                 for po in orders:
                     self.stock_broker.cancel_order(
                         order_id=po.order_id,
                         asset_code=po.asset_code,
                         quantity=po.pending_quantity,
                     )
```

### Comparing `pyqqq-0.7.7/pyqqq/utils/array.py` & `pyqqq-0.7.8/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/compute.py` & `pyqqq-0.7.8/pyqqq/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/display.py` & `pyqqq-0.7.8/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/kvstore.py` & `pyqqq-0.7.8/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/limiter.py` & `pyqqq-0.7.8/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/logger.py` & `pyqqq-0.7.8/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.8/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/pyqqq/utils/retry.py` & `pyqqq-0.7.8/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.7/PKG-INFO` & `pyqqq-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.7
+Version: 0.7.8
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

