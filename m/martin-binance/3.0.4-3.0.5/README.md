# Comparing `tmp/martin_binance-3.0.4.tar.gz` & `tmp/martin_binance-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin_binance-3.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "martin_binance-3.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `martin_binance-3.0.4.tar` & `martin_binance-3.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1079 2024-04-14 17:58:18.433261 martin_binance-3.0.4/LICENSE
--rwxr-xr-x   0        0        0     3854 2024-04-14 17:58:18.433261 martin_binance-3.0.4/README.md
--rwxr-xr-x   0        0        0     1890 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/__init__.py
--rw-r--r--   0        0        0     5007 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2786 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    13214 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/exchange_simulator.py
--rwxr-xr-x   0        0        0     4180 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/backtest/optimizer.py
--rw-r--r--   0        0        0     4705 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/client.py
--rw-r--r--   0        0        0     6935 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/db_utils.py
--rwxr-xr-x   0        0        0   139916 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/executor.py
--rw-r--r--   0        0        0    15709 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/lib.py
--rw-r--r--   0        0        0     2253 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/params.py
--rw-r--r--   0        0        0      485 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    14650 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1269 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/service/relaunch.service
--rw-r--r--   0        0        0    82430 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/strategy_base.py
--rw-r--r--   0        0        0     7151 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/telegram_utils.py
--rw-r--r--   0        0        0     7217 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_0_BTCUSDT.py
--rw-r--r--   0        0        0     7219 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_1_BTCUSDT.py
--rw-r--r--   0        0        0     7223 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
--rwxr-xr-x   0        0        0     7212 2024-04-14 17:58:18.469260 martin_binance-3.0.4/martin_binance/templates/cli_3_BTCUSDT.py
--rw-r--r--   0        0        0   237568 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/funds_rate.db
--rw-r--r--   0        0        0     1723 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/ms_cfg.toml
--rw-r--r--   0        0        0      639 2024-04-14 17:58:18.473260 martin_binance-3.0.4/martin_binance/templates/trial_params.json
--rw-r--r--   0        0        0     1424 2024-04-14 17:58:18.473260 martin_binance-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 martin_binance-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-16 12:48:01.803069 martin_binance-3.0.5/LICENSE
+-rwxr-xr-x   0        0        0     3854 2024-04-16 12:48:01.803069 martin_binance-3.0.5/README.md
+-rwxr-xr-x   0        0        0     1890 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/__init__.py
+-rw-r--r--   0        0        0     5007 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2786 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    13214 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/exchange_simulator.py
+-rwxr-xr-x   0        0        0     4165 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/backtest/optimizer.py
+-rw-r--r--   0        0        0     4705 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/client.py
+-rw-r--r--   0        0        0     6935 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/db_utils.py
+-rwxr-xr-x   0        0        0   139919 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/executor.py
+-rw-r--r--   0        0        0    15709 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/lib.py
+-rw-r--r--   0        0        0     3287 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/params.py
+-rw-r--r--   0        0        0      485 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    14650 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1269 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/service/relaunch.service
+-rw-r--r--   0        0        0    82424 2024-04-16 12:48:01.839069 martin_binance-3.0.5/martin_binance/strategy_base.py
+-rw-r--r--   0        0        0     7151 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/telegram_utils.py
+-rw-r--r--   0        0        0     7217 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_0_BTCUSDT.py
+-rw-r--r--   0        0        0     7219 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_1_BTCUSDT.py
+-rw-r--r--   0        0        0     7223 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py
+-rwxr-xr-x   0        0        0     7212 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/cli_3_BTCUSDT.py
+-rw-r--r--   0        0        0   237568 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/funds_rate.db
+-rw-r--r--   0        0        0     1723 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/ms_cfg.toml
+-rw-r--r--   0        0        0      639 2024-04-16 12:48:01.843069 martin_binance-3.0.5/martin_binance/templates/trial_params.json
+-rw-r--r--   0        0        0     1425 2024-04-16 12:48:01.843069 martin_binance-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5155 1970-01-01 00:00:00.000000 martin_binance-3.0.5/PKG-INFO
```

### Comparing `martin_binance-3.0.4/LICENSE` & `martin_binance-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/README.md` & `martin_binance-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/__init__.py` & `martin_binance-3.0.5/martin_binance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.4"
+__version__ = "3.0.5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 
 from exchanges_wrapper.definitions import Interval
```

### Comparing `martin_binance-3.0.4/martin_binance/backtest/OoTSP.py` & `martin_binance-3.0.5/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/backtest/VCoSEL.py` & `martin_binance-3.0.5/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/backtest/exchange_simulator.py` & `martin_binance-3.0.5/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/backtest/optimizer.py` & `martin_binance-3.0.5/martin_binance/backtest/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 # -*- coding: utf-8 -*-
 """
 Searches for optimal parameters for a strategy under given conditions
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2024 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.4"
+__version__ = "3.0.5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 
-import asyncio
 import importlib.util as iu
 import logging.handlers
 import stat
 import sys
 from decimal import Decimal
 from pathlib import Path
```

### Comparing `martin_binance-3.0.4/martin_binance/client.py` & `martin_binance-3.0.5/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/db_utils.py` & `martin_binance-3.0.5/martin_binance/db_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/executor.py` & `martin_binance-3.0.5/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Cyclic grid strategy based on martingale
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.3"
+__version__ = "3.0.5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
+import logging
 import sys
 import gc
 import statistics
 import traceback
-from decimal import ROUND_HALF_EVEN, ROUND_FLOOR, ROUND_CEILING, ROUND_HALF_DOWN, ROUND_HALF_UP
+from decimal import Decimal, ROUND_HALF_EVEN, ROUND_FLOOR, ROUND_CEILING, ROUND_HALF_DOWN, ROUND_HALF_UP
 from threading import Thread
 import queue
 import math
 import sqlite3
 
 import ujson as json
 from datetime import datetime, timezone
@@ -128,15 +129,15 @@
         schedule.every().minute.at(":35").do(self.event_update_tp)
         schedule.every(2).seconds.do(self.event_exec_command)
         if MODE in ('T', 'TC'):
             schedule.every().minute.at(":15").do(self.event_export_operational_status)
             schedule.every(10).seconds.do(self.event_get_command_tlg)
             schedule.every(6).seconds.do(self.event_report)
 
-    def init(self, check_funds=True) -> None:  # skipcq: PYL-W0221
+    def init(self, check_funds=True) -> None:
         self.message_log('Start Init section')
         if COLLECT_ASSETS and GRID_ONLY:
             init_params_error = 'COLLECT_ASSETS and GRID_ONLY: one only allowed'
         elif PROFIT_MAX and PROFIT_MAX < PROFIT + FEE_TAKER:
             init_params_error = 'PROFIT_MAX'
         else:
             init_params_error = None
```

### Comparing `martin_binance-3.0.4/martin_binance/lib.py` & `martin_binance-3.0.5/martin_binance/lib.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/params.py` & `martin_binance-3.0.5/martin_binance/params.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 """
 martin-binance strategy parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "3.0.1"
+__version__ = "3.0.5"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import logging
 from decimal import Decimal
 from pathlib import Path
 
+__all__ = [
+    'SYMBOL', 'EXCHANGE', 'ID_EXCHANGE', 'FEE_MAKER', 'FEE_TAKER', 'FEE_FIRST', 'FEE_SECOND', 'GRID_MAX_COUNT',
+    'START_ON_BUY', 'AMOUNT_FIRST', 'USE_ALL_FUND', 'AMOUNT_SECOND', 'PRICE_SHIFT', 'PRICE_LIMIT_RULES',
+    'ROUND_BASE', 'ROUND_QUOTE', 'PROFIT', 'PROFIT_MAX', 'OVER_PRICE', 'ORDER_Q', 'MARTIN', 'SHIFT_GRID_DELAY',
+    'GRID_UPDATE_INTERVAL', 'STATUS_DELAY', 'GRID_ONLY', 'LOG_LEVEL', 'HOLD_TP_ORDER_TIMEOUT', 'COLLECT_ASSETS',
+    'GRID_ONLY_DELAY', 'ADAPTIVE_TRADE_CONDITION', 'BB_CANDLE_SIZE_IN_MINUTES', 'BB_NUMBER_OF_CANDLES', 'KBB',
+    'LINEAR_GRID_K', 'ADX_CANDLE_SIZE_IN_MINUTES', 'ADX_NUMBER_OF_CANDLES', 'ADX_PERIOD', 'ADX_THRESHOLD',
+    'ADX_PRICE_THRESHOLD', 'REVERSE', 'REVERSE_TARGET_AMOUNT', 'REVERSE_INIT_AMOUNT', 'REVERSE_STOP',
+    'HEAD_VERSION', 'LOAD_LAST_STATE', 'LAST_STATE_FILE', 'VPS_NAME', 'PARAMS', 'TELEGRAM_URL', 'TOKEN',
+    'CHANNEL_ID', 'STOP_TLG', 'INLINE_BOT', 'MODE', 'XTIME', 'SAVE_DS', 'SAVE_PERIOD', 'LOGGING', 'SELF_OPTIMIZATION',
+    'N_TRIALS', 'SESSION_RESULT'
+]
+
 SYMBOL = str()
 EXCHANGE = ()
 # Exchange setup
 ID_EXCHANGE = int()
 FEE_MAKER = Decimal()
 FEE_TAKER = Decimal()
 FEE_FIRST = False
```

### Comparing `martin_binance-3.0.4/martin_binance/service/funds_rate_exporter.py` & `martin_binance-3.0.5/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/service/grafana.json` & `martin_binance-3.0.5/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/service/relaunch.py` & `martin_binance-3.0.5/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/strategy_base.py` & `martin_binance-3.0.5/martin_binance/strategy_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1620,15 +1620,15 @@
                             self.message_log(
                                 f"Was restored order {_id}({_order.get('clientOrderId')}) from exchange data",
                                 log_level=logging.WARNING,
                                 color=Style.YELLOW
                             )
                     [self.trades.append(PrivateTrade(trade)) for trade in load_from_csv()]
                     #
-                    self.restore_strategy_state(last_state, restore=False)
+                    self.restore_strategy_state(strategy_state=last_state, restore=False)
                     #
                     self.init(check_funds=False)
                 else:
                     restore_state = False
 
             if not restore_state:
                 if prm.MODE in ('T', 'TC'):
@@ -1712,31 +1712,31 @@
         raise NotImplementedError
 
     @abstractmethod
     def get_sum_profit(self):
         raise NotImplementedError
 
     @abstractmethod
-    def get_free_assets(self, *args, **kwargs):
+    def get_free_assets(self, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def on_new_order_book(self, *args):
         raise NotImplementedError
 
     @abstractmethod
-    def restore_strategy_state(self, *args, **kwargs):
+    def restore_strategy_state(self, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def start(self, *args):
         raise NotImplementedError
 
     @abstractmethod
-    def init(self, *args, **kwargs):
+    def init(self, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def reset_vars_ex(self):
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `martin_binance-3.0.4/martin_binance/telegram_utils.py` & `martin_binance-3.0.5/martin_binance/telegram_utils.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/cli_0_BTCUSDT.py` & `martin_binance-3.0.5/martin_binance/templates/cli_0_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/cli_1_BTCUSDT.py` & `martin_binance-3.0.5/martin_binance/templates/cli_1_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py` & `martin_binance-3.0.5/martin_binance/templates/cli_2_TESTBTCTESTUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/cli_3_BTCUSDT.py` & `martin_binance-3.0.5/martin_binance/templates/cli_3_BTCUSDT.py`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/funds_rate.db` & `martin_binance-3.0.5/martin_binance/templates/funds_rate.db`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/ms_cfg.toml` & `martin_binance-3.0.5/martin_binance/templates/ms_cfg.toml`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/martin_binance/templates/trial_params.json` & `martin_binance-3.0.5/martin_binance/templates/trial_params.json`

 * *Files identical despite different names*

### Comparing `martin_binance-3.0.4/pyproject.toml` & `martin_binance-3.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "exchanges-wrapper==2.1.9",
+    "exchanges-wrapper==2.1.10",
     "jsonpickle==3.0.2",
     "psutil==5.9.6",
     "requests==2.31.0",
     "libtmux==0.23.2",
     "colorama==0.4.6",
     "prometheus-client==0.18.0",
     "optuna==3.4.0",
```

### Comparing `martin_binance-3.0.4/PKG-INFO` & `martin_binance-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 3.0.4
+Version: 3.0.5
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==2.1.9
+Requires-Dist: exchanges-wrapper==2.1.10
 Requires-Dist: jsonpickle==3.0.2
 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0
 Requires-Dist: libtmux==0.23.2
 Requires-Dist: colorama==0.4.6
 Requires-Dist: prometheus-client==0.18.0
 Requires-Dist: optuna==3.4.0
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 3.0.4 Summary: Free trading
+Metadata-Version: 2.1 Name: martin-binance Version: 3.0.5 Summary: Free trading
 system for Binance SPOT API Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: exchanges-
-wrapper==2.1.9 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
+wrapper==2.1.10 Requires-Dist: jsonpickle==3.0.2 Requires-Dist: psutil==5.9.6
 Requires-Dist: requests==2.31.0 Requires-Dist: libtmux==0.23.2 Requires-Dist:
 colorama==0.4.6 Requires-Dist: prometheus-client==0.18.0 Requires-Dist:
 optuna==3.4.0 Requires-Dist: plotly==5.18.0 Requires-Dist: pandas==2.1.2
 Requires-Dist: dash>=2.15.0 Requires-Dist: future==0.18.3 Requires-Dist:
 inquirer==3.1.3 Requires-Dist: scikit-learn==1.3.2 Requires-Dist: tqdm==4.66.1
 Requires-Dist: ujson~=5.9.0 Requires-Dist: orjson~=3.9.15 Requires-Dist:
 pyarrow~=14.0.2 Requires-Dist: shortuuid~=1.0.11 Requires-Dist: numpy~=1.23.4
```

