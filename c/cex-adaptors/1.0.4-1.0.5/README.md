# Comparing `tmp/cex-adaptors-1.0.4.tar.gz` & `tmp/cex-adaptors-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cex-adaptors-1.0.4.tar", last modified: Fri Apr  5 14:30:04 2024, max compression
+gzip compressed data, was "cex-adaptors-1.0.5.tar", last modified: Tue Apr 16 10:38:25 2024, max compression
```

## Comparing `cex-adaptors-1.0.4.tar` & `cex-adaptors-1.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.675141 cex-adaptors-1.0.4/
--rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-04-05 14:30:04.674839 cex-adaptors-1.0.4/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)     8155 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/README.md
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.667493 cex-adaptors-1.0.4/cex_adaptors/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     8394 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     6355 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)     8292 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/bybit.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.671153 cex-adaptors-1.0.4/cex_adaptors/exchanges/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     2945 2024-03-27 02:40:55.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/auth.py
--rw-r--r--   0 davidding   (501) staff       (20)     2098 2024-03-27 02:40:55.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/base.py
--rw-r--r--   0 davidding   (501) staff       (20)     4656 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     2034 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)      129 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)     2873 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/bybit.py
--rw-r--r--   0 davidding   (501) staff       (20)     2572 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)     3032 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     2284 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)     6356 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/okx.py
--rw-r--r--   0 davidding   (501) staff       (20)      336 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/exchanges/woo.py
--rw-r--r--   0 davidding   (501) staff       (20)     5101 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)     5986 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     4562 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)    15548 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/okx.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.674452 cex-adaptors-1.0.4/cex_adaptors/parsers/
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/__init__.py
--rw-r--r--   0 davidding   (501) staff       (20)     4457 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/base.py
--rw-r--r--   0 davidding   (501) staff       (20)     9183 2024-04-05 14:26:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/binance.py
--rw-r--r--   0 davidding   (501) staff       (20)     8230 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bitget.py
--rw-r--r--   0 davidding   (501) staff       (20)        0 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bitmex.py
--rw-r--r--   0 davidding   (501) staff       (20)    10000 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/bybit.py
--rw-r--r--   0 davidding   (501) staff       (20)    10967 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/gateio.py
--rw-r--r--   0 davidding   (501) staff       (20)    15223 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/htx.py
--rw-r--r--   0 davidding   (501) staff       (20)     9404 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/kucoin.py
--rw-r--r--   0 davidding   (501) staff       (20)    16864 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/okx.py
--rw-r--r--   0 davidding   (501) staff       (20)     2464 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/parsers/woo.py
--rw-r--r--   0 davidding   (501) staff       (20)     1532 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/cex_adaptors/utils.py
--rw-r--r--   0 davidding   (501) staff       (20)      441 2024-03-27 03:36:43.000000 cex-adaptors-1.0.4/cex_adaptors/woo.py
-drwxr-xr-x   0 davidding   (501) staff       (20)        0 2024-04-05 14:30:04.668383 cex-adaptors-1.0.4/cex_adaptors.egg-info/
--rw-r--r--   0 davidding   (501) staff       (20)     8252 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/PKG-INFO
--rw-r--r--   0 davidding   (501) staff       (20)     1174 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/SOURCES.txt
--rw-r--r--   0 davidding   (501) staff       (20)        1 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/dependency_links.txt
--rw-r--r--   0 davidding   (501) staff       (20)      384 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/requires.txt
--rw-r--r--   0 davidding   (501) staff       (20)       13 2024-04-05 14:30:04.000000 cex-adaptors-1.0.4/cex_adaptors.egg-info/top_level.txt
--rw-r--r--   0 davidding   (501) staff       (20)      614 2024-03-21 09:58:13.000000 cex-adaptors-1.0.4/pyproject.toml
--rw-r--r--   0 davidding   (501) staff       (20)       38 2024-04-05 14:30:04.675200 cex-adaptors-1.0.4/setup.cfg
--rw-r--r--   0 davidding   (501) staff       (20)      380 2024-04-05 14:27:29.000000 cex-adaptors-1.0.4/setup.py
+drwxr-xr-x   0 davidding  (1085) research-group   (500)        0 2024-04-16 10:38:25.350824 cex-adaptors-1.0.5/
+-rw-r--r--   0 davidding  (1085) research-group   (500)     5936 2024-04-16 10:38:25.350824 cex-adaptors-1.0.5/PKG-INFO
+-rw-r--r--   0 davidding  (1085) research-group   (500)     5838 2024-04-16 10:38:04.000000 cex-adaptors-1.0.5/README.md
+drwxr-xr-x   0 davidding  (1085) research-group   (500)        0 2024-04-16 10:38:25.342824 cex-adaptors-1.0.5/cex_adaptors/
+-rw-r--r--   0 davidding  (1085) research-group   (500)        0 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/__init__.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    13698 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/binance.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    13814 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/bitget.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)        0 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/bitmex.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    10339 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/bybit.py
+drwxr-xr-x   0 davidding  (1085) research-group   (500)        0 2024-04-16 10:38:25.346824 cex-adaptors-1.0.5/cex_adaptors/exchanges/
+-rw-r--r--   0 davidding  (1085) research-group   (500)        0 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/__init__.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     2945 2024-03-26 03:23:56.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/auth.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     2098 2024-03-26 03:23:56.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/base.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     8104 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/binance.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     4345 2024-04-16 10:02:14.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/bitget.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)      129 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/bitmex.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     2881 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/bybit.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     3131 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/gateio.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     4327 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/htx.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     4813 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/kucoin.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     6356 2024-03-26 08:51:55.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/okx.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)      336 2024-03-26 08:51:55.000000 cex-adaptors-1.0.5/cex_adaptors/exchanges/woo.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     8652 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/gateio.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    10885 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/htx.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    12267 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/kucoin.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    15267 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/okx.py
+drwxr-xr-x   0 davidding  (1085) research-group   (500)        0 2024-04-16 10:38:25.350824 cex-adaptors-1.0.5/cex_adaptors/parsers/
+-rw-r--r--   0 davidding  (1085) research-group   (500)        0 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/__init__.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     4566 2024-04-16 10:02:14.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/base.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    12976 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/binance.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    10994 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/bitget.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)        0 2024-03-19 10:09:11.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/bitmex.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    12206 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/bybit.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    11541 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/gateio.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    18348 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/htx.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    13646 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/kucoin.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)    17807 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/okx.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     2464 2024-03-26 08:51:55.000000 cex-adaptors-1.0.5/cex_adaptors/parsers/woo.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)     1043 2024-04-16 10:06:24.000000 cex-adaptors-1.0.5/cex_adaptors/utils.py
+-rw-r--r--   0 davidding  (1085) research-group   (500)      441 2024-03-26 08:51:55.000000 cex-adaptors-1.0.5/cex_adaptors/woo.py
+drwxr-xr-x   0 davidding  (1085) research-group   (500)        0 2024-04-16 10:38:25.342824 cex-adaptors-1.0.5/cex_adaptors.egg-info/
+-rw-r--r--   0 davidding  (1085) research-group   (500)     5936 2024-04-16 10:38:25.000000 cex-adaptors-1.0.5/cex_adaptors.egg-info/PKG-INFO
+-rw-r--r--   0 davidding  (1085) research-group   (500)     1174 2024-04-16 10:38:25.000000 cex-adaptors-1.0.5/cex_adaptors.egg-info/SOURCES.txt
+-rw-r--r--   0 davidding  (1085) research-group   (500)        1 2024-04-16 10:38:25.000000 cex-adaptors-1.0.5/cex_adaptors.egg-info/dependency_links.txt
+-rw-r--r--   0 davidding  (1085) research-group   (500)      384 2024-04-16 10:38:25.000000 cex-adaptors-1.0.5/cex_adaptors.egg-info/requires.txt
+-rw-r--r--   0 davidding  (1085) research-group   (500)       13 2024-04-16 10:38:25.000000 cex-adaptors-1.0.5/cex_adaptors.egg-info/top_level.txt
+-rw-r--r--   0 davidding  (1085) research-group   (500)      615 2024-04-16 10:02:14.000000 cex-adaptors-1.0.5/pyproject.toml
+-rw-r--r--   0 davidding  (1085) research-group   (500)       38 2024-04-16 10:38:25.350824 cex-adaptors-1.0.5/setup.cfg
+-rw-r--r--   0 davidding  (1085) research-group   (500)      380 2024-04-16 10:10:29.000000 cex-adaptors-1.0.5/setup.py
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/binance.py` & `cex-adaptors-1.0.5/cex_adaptors/gateio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,216 +1,224 @@
-import tracemalloc
-from typing import Literal, Optional
+from .exchanges.gateio import GateioUnified
+from .parsers.gateio import GateioParser
 
-from .exchanges.binance import BinanceInverse, BinanceLinear, BinanceSpot
-from .parsers.binance import BinanceParser
-from .utils import sort_dict
 
-tracemalloc.start()
+class Gateio(GateioUnified):
+    name = "gateio"
 
+    PERP_SETTLE = ["btc", "usdt", "usd"]
 
-class Binance(object):
-    name = "binance"
-
-    def __init__(self, api_key: str = None, api_secret: str = None):
-        self.spot = BinanceSpot(api_key=api_key, api_secret=api_secret)
-        self.linear = BinanceLinear()
-        self.inverse = BinanceInverse()
-        self.parser = BinanceParser()
-
+    def __init__(self):
+        super().__init__()
+        self.parser = GateioParser()
         self.exchange_info = {}
 
-    async def close(self):
-        await self.spot.close()
-        await self.linear.close()
-        await self.inverse.close()
-
-    @classmethod
-    async def create(cls):
-        instance = cls()
-        instance.exchange_info = await instance.get_exchange_info()
-        return instance
-
-    async def sync_exchange_info(self) -> None:
+    async def sync_exchange_info(self):
         self.exchange_info = await self.get_exchange_info()
 
-    async def get_exchange_info(self, market_type: Optional[Literal["spot", "margin", "futures", "perp"]] = None):
-        spot = self.parser.parse_exchange_info(
-            await self.spot._get_exchange_info(), self.parser.spot_exchange_info_parser
-        )
-        linear = self.parser.parse_exchange_info(
-            await self.linear._get_exchange_info(), self.parser.futures_exchange_info_parser("linear")
-        )
-        inverse = self.parser.parse_exchange_info(
-            await self.inverse._get_exchange_info(), self.parser.futures_exchange_info_parser("inverse")
+    async def get_exchange_info(self):
+        spot = self.parser.parse_exchange_info(await self._get_currency_pairs(), self.parser.spot_exchange_info_parser)
+
+        perps = {}
+        for settle in self.PERP_SETTLE:
+            perp = self.parser.parse_exchange_info(
+                await self._get_perp_info(settle),
+                self.parser.perp_exchange_info_parser,
+                settle=settle.upper(),
+            )
+            perps.update(perp)
+
+        settle = "usdt"
+        futures = self.parser.parse_exchange_info(
+            await self._get_futures_info(settle),
+            self.parser.futures_exchange_info_parser,
+            settle=settle.upper(),
         )
-        result = {**spot, **linear, **inverse}
-        return result if not market_type else self.parser.query_dict(result, {f"is_{market_type}": True})
 
-    async def get_ticker(self, instrument_id: str):
-        _symbol = self.exchange_info[instrument_id]["raw_data"]["symbol"]
-        info = self.exchange_info[instrument_id]
-        market_type = self.parser.get_market_type(info)
+        return {**spot, **perps, **futures}
 
+    async def get_tickers(self, market_type: str = None) -> dict:
         if market_type == "spot":
-            return {instrument_id: self.parser.parse_ticker(await self.spot._get_ticker(_symbol), info)}
-        elif market_type == "linear":
-            return {instrument_id: self.parser.parse_ticker(await self.linear._get_ticker(_symbol), info)}
-        elif market_type == "inverse":
-            return {instrument_id: self.parser.parse_ticker(await self.inverse._get_ticker(_symbol), info)}
-
-    async def get_tickers(self, market_type: Optional[Literal["spot", "margin", "futures", "perp"]] = None) -> dict:
-        results = {}
-
-        tickers = [(self.spot, "spot"), (self.linear, "linear"), (self.inverse, "inverse")]
-
-        for exchange, _market_type in tickers:
-            parsed_tickers = self.parser.parse_tickers(await exchange._get_tickers(), _market_type, self.exchange_info)
-            results.update(parsed_tickers)
-
-        if market_type:
-            ids = list(self.parser.query_dict(self.exchange_info, {f"is_{market_type}": True}).keys())
-            return self.parser.query_dict_by_keys(results, ids)
+            return self.parser.parse_tickers(await self._get_spot_tickers(), self.exchange_info, "spot")
+        elif market_type == "futures":
+            return self.parser.parse_tickers(
+                await self._get_futures_tickers(settle="usdt"), self.exchange_info, "futures"
+            )
+        elif market_type == "perp":
+            perps = {}
+            for settle in self.PERP_SETTLE:
+                perp = self.parser.parse_tickers(await self._get_perp_tickers(settle), self.exchange_info, "perp")
+                perps.update(perp)
+            return perps
         else:
-            return results
-
-    async def get_klines(self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = 500):
-        _symbol = self.exchange_info[instrument_id]["raw_data"]["symbol"]
-        _interval = self.parser.get_interval(interval)
-        limit = 1000
-        market_type = self.parser.get_market_type(self.exchange_info[instrument_id])
-
-        params = {
-            "symbol": _symbol,
-            "interval": _interval,
-            "limit": limit,
-        }
+            spot = self.parser.parse_tickers(await self._get_spot_tickers(), self.exchange_info, "spot")
+            futures = self.parser.parse_tickers(
+                await self._get_futures_tickers(settle="usdt"), self.exchange_info, "futures"
+            )
+            perps = {}
+            for settle in self.PERP_SETTLE:
+                perp = self.parser.parse_tickers(await self._get_perp_tickers(settle), self.exchange_info, "perp")
+                perps.update(perp)
+            return {**spot, **futures, **perps}
 
+    async def get_ticker(self, instrument_id: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not found in {self.name} exchange info")
+        info = self.exchange_info[instrument_id]
+        market_type = self.parser.get_market_type(info)
         method_map = {
-            "spot": self.spot._get_klines,
-            "linear": self.linear._get_klines,
-            "inverse": self.inverse._get_klines,
+            "spot": self._get_spot_tickers,
+            "futures": self._get_futures_tickers,
+            "perp": self._get_perp_tickers,
         }
+        # prepare request params
+        if market_type == "spot":
+            params = {"currency_pair": info["raw_data"]["id"]}
+        elif market_type == "futures":
+            params = {"contract": info["raw_data"]["name"], "settle": info["settle"].lower()}
+        else:  # perp
+            params = {"contract": info["raw_data"]["name"], "settle": info["settle"].lower()}
 
-        query_end = None
+        return {instrument_id: self.parser.parse_raw_ticker(await method_map[market_type](**params), market_type, info)}
 
-        results = {}
-        if start and end:
-            query_end = end
-            while True:
-                params["endTime"] = query_end
-                klines = self.parser.parse_klines(await method_map[market_type](**params), market_type)
-                if not klines:
-                    break
+    async def get_current_candlestick(self, instrument_id: str, interval: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not found in {self.name} exchange info")
 
-                results.update(klines)
-                query_end = sorted(list(klines.keys()))[0]
-                if len(klines) < limit or query_end <= start:
-                    break
-                continue
-            return sort_dict({k: v for k, v in results.items() if end >= k >= start}, ascending=True)
+        info = self.exchange_info[instrument_id]
+        market_type = self.parser.get_market_type(info)
+        _interval = self.parser.get_interval(interval)
 
-        elif num:
-            while True:
-                params.update({"endTime": query_end} if query_end else {})
-                klines = self.parser.parse_klines(
-                    await method_map[market_type](**params),
-                    market_type,
-                )
-                results.update(klines)
-                if len(klines) < limit or len(results) >= num:
-                    break
-                query_end = sorted(list(klines.keys()))[0]
-                continue
+        method_map = {
+            "spot": self._get_spot_klines,
+            "futures": self._get_futures_klines,
+            "perp": self._get_perp_klines,
+        }
+        params = {
+            "symbol": info["raw_data"]["id" if market_type == "spot" else "name"],
+            "interval": _interval,
+            "limit": 1,
+        }
 
-            return sort_dict(results, ascending=True, num=num)
+        if market_type in ["futures", "perp"]:
+            params["settle"] = info["settle"].lower()
 
-    async def get_history_funding_rate(
-        self, instrument_id: str, start: int = None, end: int = None, num: int = 30
+        return {
+            instrument_id: self.parser.parse_candlesticks(
+                await method_map[market_type](**params), info, market_type, interval
+            )
+        }
+
+    async def get_history_candlesticks(
+        self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = None
     ) -> list:
         if instrument_id not in self.exchange_info:
-            raise ValueError(f"{instrument_id} not found in exchange info")
+            raise ValueError(f"{instrument_id} not found in exchange_info")
 
         info = self.exchange_info[instrument_id]
         market_type = self.parser.get_market_type(info)
-        limit = 1000
-        symbol = info["raw_data"]["symbol"]
+        _interval = self.parser.get_interval(interval)
+        limit_map = {"spot": 1000, "futures": 2000, "perp": 2000}
+
+        symbol_map = {
+            "spot": "id",
+            "futures": "name",
+            "perp": "name",
+        }
 
         method_map = {
-            "linear": self.linear._get_funding_rate_history,
-            "inverse": self.inverse._get_funding_rate_history,
+            "spot": self._get_spot_klines,
+            "futures": self._get_futures_klines,
+            "perp": self._get_perp_klines,
         }
 
         params = {
-            "symbol": symbol,
-            "limit": limit,
+            "symbol": info["raw_data"][symbol_map[market_type]],
+            "interval": _interval,
+            "limit": limit_map[market_type],
         }
 
+        # handle special market type params
+        if market_type in ["futures", "perp"]:
+            params["settle"] = info["settle"].lower()
+
         results = []
         query_end = None
         if start and end:
-            query_start = start - 1
-            query_end = end + 1
+            query_end = str(int(str(end)[:10]) + 1)
             while True:
-                params.update({"startTime": query_start, "endTime": query_end})
-                result = self.parser.parse_history_funding_rate(await method_map[market_type](**params), info)
+                params.update({"end": query_end})
+                result = self.parser.parse_candlesticks(
+                    await method_map[market_type](**params), info, market_type, interval
+                )
                 results.extend(result)
-                results = list({v["timestamp"]: v for v in results}.values())
 
-                if len(result) < limit:
+                if len(result) < limit_map[market_type]:
                     break
 
-                query_start = max([v["timestamp"] for v in result]) - 1
+                query_end = min([v["timestamp"] for v in result])
 
-                if query_start < end:
+                if query_end < start:
                     break
 
+                query_end = str(int(str(query_end)[:10]) + 1)
                 continue
+
             return sorted(
-                [v for v in results if end >= v["timestamp"] >= start], key=lambda x: x["timestamp"], reverse=False
+                [v for v in results if start <= v["timestamp"] <= end], key=lambda x: x["timestamp"], reverse=False
             )
 
         elif num:
             while True:
-                params.update({"endTime": query_end} if query_end else {})
-                result = self.parser.parse_history_funding_rate(await method_map[market_type](**params), info)
+                params.update({"end": query_end} if query_end else {})
+                result = self.parser.parse_candlesticks(
+                    await method_map[market_type](**params), info, market_type, interval
+                )
                 results.extend(result)
 
-                # exclude the datas with same timestamp
-                results = list({v["timestamp"]: v for v in results}.values())
-
-                if len(result) < limit or len(results) >= num:
+                if len(result) < limit_map[market_type] or len(results) >= num:
                     break
-                query_end = min([v["timestamp"] for v in result]) + 1
+                query_end = str(int(str(min([v["timestamp"] for v in result]))[:10]) + 1)
+
                 continue
             return sorted(results, key=lambda x: x["timestamp"], reverse=False)[-num:]
         else:
             raise ValueError("(start, end) or num must be provided")
 
-    # Private function
-    async def get_spot_account_info(self) -> dict:
-        return self.parser.parse_spot_account_info(await self.spot._get_account_info())
+    async def get_current_funding_rate(self, instrument_id: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not in {self.name} exchange info")
 
-    async def get_margin_account_info(self) -> dict:
-        return self.parser.parse_margin_account_info(await self.spot._get_margin_account_info())
+        info = self.exchange_info[instrument_id]
+        market_type = self.parser.get_market_type(info)
 
-    async def get_margin_balance(self, currency: str = None) -> dict:
-        return self.parser.parse_margin_balance(await self.spot._get_margin_account_info(), currency=currency)
+        method_map = {
+            "futures": self._get_futures_tickers,
+            "perp": self._get_perp_tickers,
+        }
 
-    async def get_margin_account_value(self, in_currency: str = None):
-        info = await self.get_margin_account_info()
+        params = {
+            "contract": info["raw_data"]["name"],
+            "settle": info["settle"].lower(),
+        }
+        return {instrument_id: self.parser.parse_current_funding_rate(await method_map[market_type](**params), info)}
 
-        net_btc_value = self.parser.parse_str(info["raw_data"]["totalNetAssetOfBtc"], float)
+    async def get_history_funding_rate(
+        self, instrument_id: str, start: int = None, end: int = None, num: int = None
+    ) -> list:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not in {self.name} exchange info")
 
-        instrument_id = "BTC/USDT:USDT"
-        ticker = await self.get_ticker(instrument_id)
-        btc_price = ticker[instrument_id]["last_price"]
+        info = self.exchange_info[instrument_id]
 
-        if in_currency:
-            instrument_id = f"{in_currency}/USDT:USDT"
-            ccy_ticker = await self.get_ticker(instrument_id)
-            ccy_price = ccy_ticker[instrument_id]["last_price"]
+        params = {"contract": info["raw_data"]["name"], "settle": info["settle"].lower(), "limit": 1000}
 
-            return net_btc_value * btc_price / ccy_price
+        results = self.parser.parse_history_funding_rate(await self._get_futures_funding_rate_history(**params), info)
 
+        if start and end:
+            return sorted(
+                [v for v in results if start <= v["timestamp"] <= end], key=lambda x: x["timestamp"], reverse=False
+            )
+        elif num:
+            return sorted(results, key=lambda x: x["timestamp"], reverse=False)[-num:]
         else:
-            return net_btc_value * btc_price
+            raise ValueError("(start, end) or num must be provided")
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/bybit.py` & `cex-adaptors-1.0.5/cex_adaptors/bybit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Literal, Optional
 
 from .exchanges.bybit import BybitUnified
 from .parsers.bybit import BybitParser
-from .utils import sort_dict
 
 
 class Bybit(BybitUnified):
     name = "bybit"
 
     def __init__(self):
         super().__init__()
@@ -32,71 +31,122 @@
     async def get_tickers(self, market_type: Optional[Literal["spot", "margin", "futures", "perp"]] = None):
 
         results = {}
 
         tickers = ["spot", "linear", "inverse"]
 
         for _market_type in tickers:
-            parsed_tickers = self.parser.parse_tickers(await self._get_tickers(_market_type), _market_type)
-            id_map = self.parser.get_id_symbol_map(self.exchange_info, _market_type)
-
-            for ticker in parsed_tickers:
-                symbol = ticker["symbol"]
-                if symbol not in id_map:
-                    print(symbol)
-                    continue
-                id = id_map[symbol]
-
-                results[id] = ticker
+            parsed_tickers = self.parser.parse_tickers(
+                await self._get_tickers(_market_type), _market_type, self.exchange_info
+            )
+            results.update(parsed_tickers)
 
         if market_type:
             ids = list(self.parser.query_dict(self.exchange_info, {f"is_{market_type}": True}).keys())
             return self.parser.query_dict_by_keys(results, ids)
         else:
             return results
 
-    async def get_klines(self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = 30):
-        _category = self.parser.get_category(self.exchange_info[instrument_id])
-        _symbol = self.exchange_info[instrument_id]["raw_data"]["symbol"]
+    async def get_ticker(self, instrument_id: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} is not found in {self.name} exchange info.")
+
+        info = self.exchange_info[instrument_id]
+        _symbol = info["raw_data"]["symbol"]
+        _market_type = self.parser.get_market_type(info)
+        _category = self.parser.get_category(info)
+
+        return {
+            instrument_id: self.parser.parse_raw_ticker(
+                await self._get_ticker(symbol=_symbol, category=_category), _market_type, info
+            )
+        }
+
+    async def get_current_candlestick(self, instrument_id: str, interval: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} is not found in {self.name} exchange info.")
+
+        info = self.exchange_info[instrument_id]
+        _symbol = info["raw_data"]["symbol"]
+        _interval = self.parser.get_interval(interval)
+        _category = self.parser.get_category(info)
+        limit = 1
+
+        params = {"symbol": _symbol, "interval": _interval, "limit": limit, "category": _category}
+
+        return {
+            instrument_id: self.parser.parse_candlesticks(await self._get_klines(**params), info, _category, interval)
+        }
+
+    async def get_history_candlesticks(
+        self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = 30
+    ) -> list:
+
+        info = self.exchange_info[instrument_id]
+        _category = self.parser.get_category(info)
+        _symbol = info["raw_data"]["symbol"]
         _interval = self.parser.get_interval(interval)
         limit = 1000
 
         params = {"symbol": _symbol, "interval": _interval, "limit": limit, "category": _category}
 
-        results = {}
+        results = []
         query_end = None
         if start and end:
-            query_end = end
+            query_end = end + 1
             while True:
                 params["end"] = query_end
-                klines = self.parser.parse_klines(await self._get_klines(**params))
+                klines = self.parser.parse_candlesticks(await self._get_klines(**params), info, _category, interval)
                 if not klines:
                     break
-                results.update(klines)
-                query_end = sorted(list(klines.keys()))[0]
+                results.extend(klines)
+
+                # exclude data with same timestamp
+                results = list({v["timestamp"]: v for v in results}.values())
+
+                query_end = min([v["timestamp"] for v in klines]) + 1
                 if len(klines) < limit or query_end <= start:
                     break
                 continue
-            return sort_dict({k: v for k, v in results.items() if end >= k >= start}, ascending=True)
+            return sorted(
+                [v for v in results if end >= v["timestamp"] >= start], key=lambda x: x["timestamp"], reverse=False
+            )
 
         elif num:
             while True:
                 params.update({"end": query_end} if query_end else {})
-                klines = self.parser.parse_klines(await self._get_klines(**params))
-                results.update(klines)
+                klines = self.parser.parse_candlesticks(await self._get_klines(**params), info, _category, interval)
+
+                results.extend(klines)
+                # exclude data with same timestamp
+                results = list({v["timestamp"]: v for v in results}.values())
 
                 if len(klines) < limit or len(results) >= num:
                     break
-                query_end = sorted(list(klines.keys()))[0]
+                query_end = min([v["timestamp"] for v in klines]) + 1
                 continue
 
-            return sort_dict(results, ascending=True, num=num)
+            return sorted(results, key=lambda x: x["timestamp"], reverse=False)[-num:]
         else:
             raise ValueError("(start, end) or num must be provided")
 
+    async def get_current_funding_rate(self, instrument_id: str):
+        if instrument_id not in self.exchange_info:
+            raise ValueError(f"{instrument_id} not in {self.name} exchange info")
+
+        info = self.exchange_info[instrument_id]
+        _symbol = info["raw_data"]["symbol"]
+        _category = self.parser.get_category(info)
+
+        params = {
+            "symbol": _symbol,
+            "category": _category,
+        }
+        return {instrument_id: self.parser.parse_current_funding_rate(await self._get_ticker(**params), info)}
+
     async def get_history_funding_rate(self, instrument_id: str, start: int = None, end: int = None, num: int = 30):
         if instrument_id not in self.exchange_info:
             raise ValueError(f"{instrument_id} is not supported")
 
         info = self.exchange_info[instrument_id]
         _category = self.parser.get_category(info)
         _symbol = info["raw_data"]["symbol"]
@@ -106,15 +156,15 @@
 
         results = []
         query_end = None
         if start and end:
             query_end = end + 1
             while True:
                 params["endTime"] = query_end
-                result = self.parser.parse_funding_rate(await self._get_funding_rate(**params), info)
+                result = self.parser.parse_funding_rate(await self._get_funding_rate_history(**params), info)
                 results.extend(result)
 
                 # exclude data with same timestamp
                 results = list({v["timestamp"]: v for v in results}.values())
 
                 if len(result) < limit:
                     break
@@ -127,15 +177,15 @@
             return sorted(
                 [v for v in results if end >= v["timestamp"] >= start], key=lambda x: x["timestamp"], reverse=False
             )
 
         elif num:
             while True:
                 params.update({"endTime": query_end} if query_end else {})
-                result = self.parser.parse_funding_rate(await self._get_funding_rate(**params), info)
+                result = self.parser.parse_funding_rate(await self._get_funding_rate_history(**params), info)
 
                 results.extend(result)
                 # exclude data with same timestamp
                 results = list({v["timestamp"]: v for v in results}.values())
 
                 if len(result) < limit or len(results) >= num:
                     break
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/auth.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/auth.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/base.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/base.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/binance.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/kucoin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,129 @@
 from .base import BaseClient
 
 
-class BinanceSpot(BaseClient):
-    BASE_ENDPOINT = "https://api{}.binance.com"
-    name = "binance"
+class KucoinSpot(BaseClient):
+    BASE_ENDPOINT = "https://api.kucoin.com"
 
-    def __init__(self, api_key: str, api_secret: str, api_version: int = 3):
+    def __init__(self) -> None:
         super().__init__()
-        self.base_endpoint = self.BASE_ENDPOINT.format(api_version)
+        self.spot_base_endpoint = self.BASE_ENDPOINT
+
+    async def _get_currency_list(self):
+        return await self._get(self.spot_base_endpoint + "/api/v3/currencies")
+
+    async def _get_symbol_list(self):
+        return await self._get(self.spot_base_endpoint + "/api/v2/symbols")
+
+    async def _get_tickers(self):
+        return await self._get(self.spot_base_endpoint + "/api/v1/market/allTickers")
+
+    async def _get_24hr_ticker(self, symbol: str):
+        params = {"symbol": symbol}
+        return await self._get(self.spot_base_endpoint + "/api/v1/market/stats", params=params)
 
-        self.auth_data = {
-            "api_key": api_key,
-            "api_secret": api_secret,
+    async def _get_24hr_stats(self, symbol: str):
+        return await self._get(self.spot_base_endpoint + f"/api/v1/market/stats?symbol={symbol}")
+
+    async def _get_klines(self, symbol: str, type: str, start: int = None, end: int = None):
+        params = {
+            "symbol": symbol,
+            "type": type,
         }
+        if start:
+            params["startAt"] = start
 
-    async def _get_exchange_info(self):
-        return await self._get(self.base_endpoint + "/api/v3/exchangeInfo")
+        if end:
+            params["endAt"] = end
 
-    async def _get_ticker(self, symbol: str):
-        return await self._get(self.base_endpoint + "/api/v3/ticker/24hr", params={"symbol": symbol})
+        return await self._get(self.spot_base_endpoint + "/api/v1/market/candles", params=params)
 
-    async def _get_tickers(self):
-        return await self._get(self.base_endpoint + "/api/v3/ticker/24hr")
+    async def _get_margin_mark_price(self, symbol: str):
+        return await self._get(self.spot_base_endpoint + f"/api/v1/mark-price/{symbol}/current")
 
-    async def _get_klines(
-        self,
-        symbol: str,
-        interval: str,
-        startTime: int = None,
-        endTime: int = None,
-        limit: int = 500,
-        timeZone: str = "0",
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit, "timeZone": timeZone}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.base_endpoint + "/api/v3/klines", params=params)
-
-    # Private endpoint
-    async def _get_account_info(self):
-        return await self._get(self.base_endpoint + "/api/v3/account", auth_data=self.auth_data)
+    async def _get_part_orderbook(self, symbol: str, depth: int):
+        if depth not in [20, 100]:
+            raise ValueError("Depth must be 20 or 100 in KucoinSpot")
+        return await self._get(
+            self.spot_base_endpoint + f"/api/v1/market/orderbook/level2_{depth}", params={"symbol": symbol}
+        )
 
-    async def _get_margin_account_info(self):
-        return await self._get(self.base_endpoint + "/sapi/v1/margin/account", auth_data=self.auth_data)
+    async def _get_full_orderbook(self, symbol: str):
+        return await self._get(self.spot_base_endpoint + f"/api/v3/market/orderbook/level2", params={"symbol": symbol})
 
 
-class BinanceLinear(BaseClient):
-    BASE_ENDPOINT = "https://fapi.binance.com"
+class KucoinFutures(BaseClient):
+    BASE_ENDPOINT = "https://api-futures.kucoin.com"
 
     def __init__(self) -> None:
         super().__init__()
-        self.linear_base_endpoint = self.BASE_ENDPOINT
+        self.futures_base_endpoint = self.BASE_ENDPOINT
 
-    async def _get_exchange_info(self):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/exchangeInfo")
+    async def _get_symbol_list(self):
+        return await self._get(self.futures_base_endpoint + "/api/v1/contracts/active")
 
     async def _get_ticker(self, symbol: str):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/ticker/24hr", params={"symbol": symbol})
+        params = {"symbol": symbol}
+        return await self._get(self.futures_base_endpoint + f"/api/v1/ticker", params=params)
 
-    async def _get_tickers(self):
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/ticker/24hr")
+    async def _get_symbol_detail(self, symbol: str):
+        return await self._get(self.futures_base_endpoint + f"/api/v1/contracts/{symbol}")
 
-    async def _get_klines(
-        self, symbol: str, interval: str, startTime: int = None, endTime: int = None, limit: int = 500
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/klines", params=params)
+    async def _get_klines(self, symbol: str, granularity: int, start: int = None, end: int = None):
 
-    async def _get_funding_rate_history(
-        self, symbol: str, startTime: int = None, endTime: int = None, limit: int = 1000
-    ):
         params = {
-            k: v
-            for k, v in {
-                "symbol": symbol,
-                "startTime": startTime,
-                "endTime": endTime,
-                "limit": limit,
-            }.items()
-            if v
+            "symbol": symbol,
+            "granularity": granularity,
         }
-        return await self._get(self.linear_base_endpoint + "/fapi/v1/fundingRate", params=params)
+        if start:
+            params["from"] = start
+        if end:
+            params["to"] = end
 
+        return await self._get(self.futures_base_endpoint + "/api/v1/kline/query", params=params)
 
-class BinanceInverse(BaseClient):
-    BASE_ENDPOINT = "https://dapi.binance.com"
+    async def _get_current_mark_price(self, symbol: str):
+        return await self._get(self.futures_base_endpoint + f"/api/v1/mark-price/{symbol}/current")
 
-    def __init__(self) -> None:
-        super().__init__()
-        self.inverse_base_endpoint = self.BASE_ENDPOINT
+    async def _get_part_orderbook(self, symbol: str, depth: int):
+        if depth not in [20, 100]:
+            raise ValueError("Depth must be 20 or 100 in KucoinSpot")
+        return await self._get(self.futures_base_endpoint + f"/api/v1/level2/depth{depth}", params={"symbol": symbol})
 
-    async def _get_exchange_info(self):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/exchangeInfo")
+    async def _get_full_orderbook(self, symbol: str):
+        return await self._get(self.futures_base_endpoint + "/api/v1/level2/snapshot", params={"symbol": symbol})
 
-    async def _get_ticker(self, symbol: str):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/ticker/24hr", params={"symbol": symbol})
+    async def _get_current_funding_rate(self, symbol: str):
+        return await self._get(self.futures_base_endpoint + f"/api/v1/funding-rate/{symbol}/current")
 
-    async def _get_tickers(self):
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/ticker/24hr")
-
-    async def _get_klines(
-        self, symbol: str, interval: str, startTime: int = None, endTime: int = None, limit: int = 500
-    ):
-        params = {"symbol": symbol, "interval": interval, "limit": limit}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/klines", params=params)
+    async def _get_public_funding_history(self, symbol: str, _from: int, to: int):
+        params = {
+            "symbol": symbol,
+            "from": _from,
+            "to": to,
+        }
+        return await self._get(self.futures_base_endpoint + "/api/v1/contract/funding-rates", params=params)
 
-    async def _get_funding_rate_history(
-        self, symbol: str, startTime: int = None, endTime: int = None, limit: int = 1000
+    async def _get_private_funding_history(
+        self,
+        symbol: str,
+        startAt: int = None,
+        endAt: int = None,
+        reverse: bool = None,
+        offset: int = None,
+        forward: bool = None,
+        maxCount: int = None,
     ):
         params = {
             k: v
             for k, v in {
                 "symbol": symbol,
-                "startTime": startTime,
-                "endTime": endTime,
-                "limit": limit,
+                "startAt": startAt,
+                "endAt": endAt,
+                "reverse": reverse,
+                "offset": offset,
+                "forward": forward,
+                "maxCount": maxCount,
             }.items()
-            if v
+            if v is not None
         }
-        return await self._get(self.inverse_base_endpoint + "/dapi/v1/fundingRate", params=params)
+        return await self._get(self.futures_base_endpoint + "/api/v1/funding-history", params=params)
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/bitget.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/gateio.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,73 @@
 from .base import BaseClient
 
 
-class BitgetUnified(BaseClient):
-    BASE_URL = "https://api.bitget.com"
+class GateioUnified(BaseClient):
+    BASE_URL = "https://api.gateio.ws/api/v4"
 
     def __init__(self) -> None:
         super().__init__()
-        self.base_endpoint = self.BASE_URL
+        self.base_url = self.BASE_URL
 
-    async def _get_spot_exchange_info(self):
-        return await self._get(self.base_endpoint + "/api/v2/spot/public/symbols")
+    async def _get_currency_pairs(self):
+        return await self._get(self.base_url + "/spot/currency_pairs")
 
-    async def _get_derivative_exchange_info(self, product_type: str):
-        params = {"productType": product_type}
-        return await self._get(self.base_endpoint + "/api/v2/mix/market/contracts", params=params)
-
-    async def _get_spot_tickers(self):
-        return await self._get(self.base_endpoint + "/api/v2/spot/market/tickers")
+    async def _get_perp_info(self, settle: str, contract: str = None):
+        params = {k: v for k, v in {"contract": contract}.items() if v}
+        return await self._get(self.base_url + f"/futures/{settle}/contracts", params=params)
+
+    async def _get_futures_info(self, settle: str = "usdt"):
+        return await self._get(self.base_url + f"/delivery/{settle}/contracts")
+
+    async def _get_spot_tickers(self, currency_pair: str = None, timezone: str = None):
+        params = {k: v for k, v in {"currency_pair": currency_pair, "timezone": timezone}.items() if v}
+        return await self._get(self.base_url + "/spot/tickers", params=params)
+
+    async def _get_perp_tickers(self, settle: str, contract: str = None):
+        params = {k: v for k, v in {"contract": contract}.items() if v}
+        return await self._get(self.base_url + f"/futures/{settle}/tickers", params=params)
+
+    async def _get_futures_tickers(self, settle: str = "usdt", contract: str = None):
+        params = {k: v for k, v in {"contract": contract}.items() if v}
+        return await self._get(self.base_url + f"/delivery/{settle}/tickers", params=params)
+
+    async def _get_spot_klines(self, symbol: str, interval: str, start: int = None, end: int = None, limit: int = None):
+        params = {"currency_pair": symbol, "interval": interval}
+        if start:
+            params["from"] = start
+        if end:
+            params["to"] = end
+        if limit:
+            params["limit"] = limit
 
-    async def _get_derivative_tickers(self, product_type: str):
-        params = {"productType": product_type}
-        return await self._get(self.base_endpoint + "/api/v2/mix/market/tickers", params=params)
+        return await self._get(self.base_url + "/spot/candlesticks", params=params)
 
-    async def _get_spot_candlesticks(
-        self, symbol: str, granularity: str, startTime: str = None, endTime: str = None, limit: str = None
+    async def _get_perp_klines(
+        self, symbol: str, settle: str, interval: str, start: int = None, end: int = None, limit: int = None
     ):
-        params = {"symbol": symbol, "granularity": granularity}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
+        params = {"contract": symbol, "interval": interval}
+        if start:
+            params["from"] = start
+        if end:
+            params["to"] = end
         if limit:
             params["limit"] = limit
-        return await self._get(self.base_endpoint + "/api/v2/spot/market/candles", params=params)
 
-    async def _get_derivative_candlesticks(
-        self,
-        symbol: str,
-        productType: str,
-        granularity: str,
-        startTime: str = None,
-        endTime: str = None,
-        kLineType: str = "MARKET",
-        limit: str = None,
+        return await self._get(self.base_url + f"/futures/{settle}/candlesticks", params=params)
+
+    async def _get_futures_klines(
+        self, symbol: str, settle: str, interval: str, start: int = None, end: int = None, limit: int = None
     ):
-        params = {"symbol": symbol, "productType": productType, "granularity": granularity, "kLineType": kLineType}
-        if startTime:
-            params["startTime"] = startTime
-        if endTime:
-            params["endTime"] = endTime
-        if limit:
+        params = {"contract": symbol, "interval": interval}
+        if start:
+            params["from"] = start
+        if end:
+            params["to"] = end
+
+        if not start and not end and limit:
             params["limit"] = limit
-        return await self._get(self.base_endpoint + "/api/v2/mix/market/candles", params=params)
+
+        return await self._get(self.base_url + f"/delivery/{settle}/candlesticks", params=params)
+
+    async def _get_futures_funding_rate_history(self, settle: str, contract: str, limit: int = None):
+        params = {k: v for k, v in {"contract": contract, "limit": limit}.items() if v}
+        return await self._get(self.base_url + f"/futures/{settle}/funding_rate", params=params)
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/bybit.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/bybit.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 "limit": limit,
             }.items()
             if v is not None
         }
 
         return await self._get(self.base_endpoint + "/v5/market/kline", params=params)
 
-    async def _get_funding_rate(
+    async def _get_funding_rate_history(
         self, category: str, symbol: str, startTime: int = None, endTime: int = None, limit: int = None
     ):
         params = {
             k: v
             for k, v in {
                 "category": category,
                 "symbol": symbol,
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/htx.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/bitget.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,95 @@
 from .base import BaseClient
 
 
-class HtxUnified(BaseClient):
-    BASE_URL = "https://api.huobi.pro"
+class BitgetUnified(BaseClient):
+    BASE_URL = "https://api.bitget.com"
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.base_endpoint = self.BASE_URL
 
-    async def _get_exchange_info(self):
-        return await self._get(self.base_endpoint + "/v2/settings/common/symbols")
+    async def _get_spot_exchange_info(self):
+        return await self._get(self.base_endpoint + "/api/v2/spot/public/symbols")
 
-    async def _get_tickers(self):
-        return await self._get(self.base_endpoint + "/market/tickers")
+    async def _get_derivative_exchange_info(self, product_type: str):
+        params = {"productType": product_type}
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/contracts", params=params)
+
+    async def _get_spot_tickers(self, symbol: str = None):
+        params = {k: v for k, v in {"symbol": symbol}.items() if v}
+        return await self._get(self.base_endpoint + "/api/v2/spot/market/tickers", params=params)
+
+    async def _get_derivative_tickers(self, productType: str):
+        params = {"productType": productType}
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/tickers", params=params)
+
+    async def _get_derivative_ticker(self, symbol: str, productType: str):
+        params = {"symbol": symbol, "productType": productType}
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/ticker", params=params)
 
-    async def _get_klines(self, symbol: str, period: str, limit: int):
-        params = {"symbol": symbol, "period": period, "size": limit}
-
-        return await self._get(self.base_endpoint + "/market/history/kline", params=params)
-
-
-class HtxFutures(BaseClient):
-    BASE_URL = "https://api.hbdm.com"
-
-    def __init__(self):
-        super().__init__()
-        self.base_endpoint = self.BASE_URL
-
-    async def _get_linear_contract_info(self):
-        return await self._get(self.base_endpoint + "/linear-swap-api/v1/swap_contract_info")
-
-    async def _get_inverse_futures_info(self):
-        return await self._get(self.base_endpoint + "/api/v1/contract_contract_info")
-
-    async def _get_inverse_perp_info(self):
-        return await self._get(self.base_endpoint + "/swap-api/v1/swap_contract_info")
-
-    async def _get_linear_contract_tickers(self):
-        return await self._get(self.base_endpoint + "/v2/linear-swap-ex/market/detail/batch_merged")
-
-    async def _get_inverse_perp_tickers(self):
-        return await self._get(self.base_endpoint + "/v2/swap-ex/market/detail/batch_merged")
-
-    async def _get_inverse_futures_tickers(self):
-        return await self._get(self.base_endpoint + "/v2/market/detail/batch_merged")
-
-    async def _get_linear_contract_klines(
-        self, symbol: str, period: str, start: int = None, end: int = None, limit: int = None
+    async def _get_spot_candlesticks(
+        self, symbol: str, granularity: str, startTime: str = None, endTime: str = None, limit: str = None
     ):
-        params = {"contract_code": symbol, "period": period}
-        if start:
-            params["from"] = start
-        if end:
-            params["to"] = end
+        params = {"symbol": symbol, "granularity": granularity}
+        if startTime:
+            params["startTime"] = startTime
+        if endTime:
+            params["endTime"] = endTime
         if limit:
-            params["size"] = limit
-
-        return await self._get(self.base_endpoint + "/linear-swap-ex/market/history/kline", params=params)
+            params["limit"] = limit
+        return await self._get(self.base_endpoint + "/api/v2/spot/market/candles", params=params)
 
-    async def _get_inverse_perp_klines(
-        self, symbol: str, period: str, start: int = None, end: int = None, limit: int = None
+    async def _get_derivative_candlesticks(
+        self,
+        symbol: str,
+        productType: str,
+        granularity: str,
+        startTime: str = None,
+        endTime: str = None,
+        kLineType: str = "MARKET",
+        limit: str = None,
     ):
-        params = {"contract_code": symbol, "period": period}
-        if start:
-            params["from"] = start
-        if end:
-            params["to"] = end
+        params = {"symbol": symbol, "productType": productType, "granularity": granularity, "kLineType": kLineType}
+        if startTime:
+            params["startTime"] = startTime
+        if endTime:
+            params["endTime"] = endTime
         if limit:
-            params["size"] = limit
+            params["limit"] = limit
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/candles", params=params)
 
-        return await self._get(self.base_endpoint + "/swap-ex/market/history/kline", params=params)
+    async def _get_derivative_mark_index_price(self, symbol: str, productType: str):
+        params = {"symbol": symbol, "productType": productType}
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/symbol-price", params=params)
+
+    async def _get_spot_orderbook(self, symbol: str, type: str = None, limit: int = None):
+        params = {k: v for k, v in {"symbol": symbol, "type": type, "limit": limit}.items() if v}
+        return await self._get(self.base_endpoint + "/api/v2/spot/market/orderbook", params=params)
+
+    async def _get_spot_merge_depth(self, symbol: str, precision: str = None, limit: str = None):
+        params = {k: v for k, v in {"symbol": symbol, "precision": precision, "limit": limit}.items() if v}
+        return await self._get(self.base_endpoint + "/api/v2/spot/market/merge-depth", params=params)
 
-    async def _get_inverse_futures_klines(
-        self, symbol: str, period: str, start: int = None, end: int = None, limit: int = None
+    async def _get_derivative_merge_market_depth(
+        self, symbol: str, productType: str, precision: str = None, limit: str = None
     ):
-        params = {"symbol": symbol, "period": period}
-        if start:
-            params["from"] = start
-        if end:
-            params["to"] = end
-        if limit:
-            params["size"] = limit
+        params = {
+            k: v
+            for k, v in {"symbol": symbol, "productType": productType, "precision": precision, "limit": limit}.items()
+            if v
+        }
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/merge-depth", params=params)
+
+    async def _get_derivative_current_funding_rate(self, symbol: str, productType: str):
+        params = {"symbol": symbol, "productType": productType}
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/current-fund-rate", params=params)
 
-        return await self._get(self.base_endpoint + "/market/history/kline", params=params)
+    async def _get_derivative_history_funding_rate(
+        self, symbol: str, productType: str, pageSize: str = None, pageNo: str = None
+    ):
+        params = {
+            k: v
+            for k, v in {"symbol": symbol, "productType": productType, "pageSize": pageSize, "pageNo": pageNo}.items()
+            if v
+        }
+        return await self._get(self.base_endpoint + "/api/v2/mix/market/history-fund-rate", params=params)
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/exchanges/okx.py` & `cex-adaptors-1.0.5/cex_adaptors/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.4/cex_adaptors/okx.py` & `cex-adaptors-1.0.5/cex_adaptors/okx.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,91 +63,80 @@
                     await self._get_tickers(_market_type), market_type, self.exchange_info
                 )
                 results.update(parsed_tickers)
 
             return results
 
     async def get_ticker(self, instrument_id: str):
+        if instrument_id not in self.exchange_info:
+            raise Exception(f"{instrument_id} not found in {self.name} exchange_info")
         _instrument_id = self.exchange_info[instrument_id]["raw_data"]["instId"]
         market_type = self._market_type_map[self.exchange_info[instrument_id]["raw_data"]["instType"]]
-        return {instrument_id: self.parser.parse_ticker(await self._get_ticker(_instrument_id), market_type)}
+        info = self.exchange_info[instrument_id]
+        return {instrument_id: self.parser.parse_ticker(await self._get_ticker(_instrument_id), market_type, info)}
+
+    async def get_current_candlestick(self, instrument_id: str, interval: str) -> dict:
+        if instrument_id not in self.exchange_info:
+            raise Exception(f"{instrument_id} not found in exchange_info")
+
+        info = self.exchange_info[instrument_id]
+        _symbol = info["raw_data"]["instId"]
+        _interval = self.parser.get_interval(interval)
+        limit = 1
+
+        params = {"instId": _symbol, "bar": _interval, "limit": limit}
 
-    async def get_klines(self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = None):
+        return {instrument_id: self.parser.parse_candlesticks(await self._get_klines(**params), info, interval)}
+
+    async def get_history_candlesticks(
+        self, instrument_id: str, interval: str, start: int = None, end: int = None, num: int = None
+    ) -> list:
         info = self.exchange_info[instrument_id]
-        market_type = self._market_type_map[info["raw_data"]["instType"]]
         _instrument_id = info["raw_data"]["instId"]
         _interval = self.parser.get_interval(interval)
         limit = 300
 
         params = {"instId": _instrument_id, "bar": _interval, "limit": limit}
 
-        results = {}
+        results = []
         if start and end:
-            query_end = end
+            query_end = end + 1
             while True:
                 params.update({"after": query_end})
-                datas = self.parser.parse_klines(
-                    await self._get_klines(**params),
-                    market_type,
-                )
-                results.update(datas)
+                datas = self.parser.parse_candlesticks(await self._get_klines(**params), info, interval)
+                results.extend(datas)
 
-                if not datas or len(datas) < limit:
-                    break
-                query_end = sorted(datas.keys())[0]
-                if query_end < start:
-                    break
-            results = {k: v for k, v in results.items() if start <= k <= end}
+                # exclude same timestamp datas
+                results = list({v["timestamp"]: v for v in results}.values())
 
-        elif start:
-            query_end = end
-            while True:
-                params.update({"after": query_end} if query_end else {})
-                datas = self.parser.parse_klines(
-                    await self._get_klines(**params),
-                    market_type,
-                )
-                results.update(datas)
                 if not datas or len(datas) < limit:
                     break
-                query_end = sorted(datas.keys())[0]
+                query_end = min([v["timestamp"] for v in datas]) + 1
                 if query_end < start:
                     break
-            results = {k: v for k, v in results.items() if k >= start}
-        elif end and num:
-            query_end = end
-            query_num = min(num, limit)
-            while True:
-                params.update({"after": query_end, "limit": query_num})
-                datas = self.parser.parse_klines(
-                    await self._get_klines(**params),
-                    market_type,
-                )
-                results.update(datas)
-                if not datas or len(datas) < limit:
-                    break
-                query_num = min(num - len(results), limit)
-                query_end = sorted(datas.keys())[0]
-            results = {k: v for k, v in results.items() if k <= end}
+            results = sorted(
+                [v for v in results if start <= v["timestamp"] <= end], key=lambda x: x["timestamp"], reverse=False
+            )
         elif num:
             query_end = end
-            query_num = min(num, limit)
             while True:
-                params.update({"after": query_end, "limit": query_num} if query_end else {"limit": query_num})
-                datas = self.parser.parse_klines(
-                    await self._get_klines(**params),
-                    market_type,
-                )
-                results.update(datas)
+                params.update({"after": query_end} if query_end else {})
+                datas = self.parser.parse_candlesticks(await self._get_klines(**params), info, interval)
+                results.extend(datas)
+
+                # exclude same timestamp datas
+                results = list({v["timestamp"]: v for v in results}.values())
+
                 if not datas or len(datas) < limit:
                     break
-                query_num = min(num - len(results), limit)
-                query_end = sorted(datas.keys())[0]
 
-            results = dict(sorted(results.items(), key=lambda x: x[0])[-num:])
+                query_end = min([v["timestamp"] for v in datas])
+                continue
+
+            results = sorted(results, key=lambda x: x["timestamp"], reverse=False)[-num:]
         else:
             raise Exception("invalid params")
 
         return results
 
     async def get_history_funding_rate(
         self, instrument_id: str, start: int = None, end: int = None, num: int = 30
@@ -203,15 +192,19 @@
             raise Exception("(start, end) or num must be provided")
 
     async def get_current_funding_rate(self, instrument_id: str) -> dict:
         if instrument_id not in self.exchange_info:
             raise Exception(f"{instrument_id} not found in exchange_info")
         info = self.exchange_info[instrument_id]
         _instrument_id = info["raw_data"]["instId"]
-        return self.parser.parse_current_funding_rate(await self._get_current_funding_rate(_instrument_id), info)
+        return {
+            instrument_id: self.parser.parse_current_funding_rate(
+                await self._get_current_funding_rate(_instrument_id), info
+            )
+        }
 
     async def get_last_price(self, instrument_id: str) -> dict:
         if instrument_id not in self.exchange_info:
             raise Exception(f"{instrument_id} not found in exchange_info")
         info = self.exchange_info[instrument_id]
         _instrument_id = info["raw_data"]["instId"]
         return self.parser.parse_last_price(await self._get_ticker(_instrument_id), instrument_id=instrument_id)
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/base.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     LINEAR_TYPES = ["LinearFutures", "LinearPerpetual", "linear"]
     INVERSE_TYPES = ["InverseFutures", "InversePerpetual", "inverse"]
     STABLE_CURRENCY = ["USDT", "USDC"]
     FIAT_CURRENCY = ["USD"]
 
     @staticmethod
     def parse_str(data: str, method: callable):
-        if not data:
+        if data is None:
             return None
         return method(data)
 
     def get_result_with_parser(self, data: dict, parser: dict) -> dict:
         results = {}
         for key in parser:
             if callable(parser[key]):
@@ -122,7 +122,11 @@
             if any(value.get(k) == v for k, v in query.items()):
                 filtered_data[key] = value
         return filtered_data
 
     @staticmethod
     def query_dict_by_keys(datas: dict, keys: list) -> dict:
         return {key: datas[key] for key in keys if key in datas}
+
+    @staticmethod
+    def get_timestamp() -> int:
+        return int(datetime.now().timestamp() * 1000)
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/binance.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/bitget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,231 +1,275 @@
+from ..utils import query_dict
 from .base import Parser
 
 
-class BinanceParser(Parser):
-    @staticmethod
-    def check_response(response: dict):
-        return {"code": 200, "status": "success", "data": response}
+class BitgetParser(Parser):
+    LINEAR_FUTURES_SETTLE = ["USDT", "USDC"]
+
+    INTERVAL_MAP = {
+        "spot": {
+            "1m": "1min",
+            "5m": "5min",
+            "15m": "15min",
+            "30m": "30min",
+            "1h": "1h",
+            "4h": "4h",
+            "6h": "6h",
+            "12h": "12h",
+            "1d": "1day",
+            "3d": "3day",
+            "1w": "1week",
+            "1M": "1M",
+        },
+        "derivative": {
+            "1m": "1m",
+            "3m": "3m",
+            "5m": "5m",
+            "15m": "15m",
+            "30m": "30m",
+            "1h": "1H",
+            "4h": "4H",
+            "6h": "6H",
+            "12h": "12H",
+            "1d": "1D",
+            "1w": "1W",
+            "1M": "1M",
+        },
+    }
+
+    def __init__(self):
+        super().__init__()
+
+    def check_response(self, response: dict):
+        if response["code"] == "00000":
+            return {
+                "code": 200,
+                "status": "success",
+                "data": response["data"],
+                "timestamp": self.parse_str(response["requestTime"], int),
+            }
+        else:
+            raise ValueError(f"Error in parsing Bitget response: {response}")
 
     @property
     def spot_exchange_info_parser(self):
         return {
-            "active": (lambda x: x["status"] == "TRADING"),
+            "active": (lambda x: x["status"] == "online"),
             "is_spot": True,
-            "is_margin": (lambda x: x["isMarginTradingAllowed"]),
+            "is_margin": False,
             "is_futures": False,
             "is_perp": False,
             "is_linear": True,
             "is_inverse": False,
-            "symbol": (lambda x: self.parse_unified_symbol(x["baseAsset"], x["quoteAsset"])),
-            "base": (lambda x: str(x["baseAsset"])),
-            "quote": (lambda x: str(x["quoteAsset"])),
-            "settle": (lambda x: str(x["quoteAsset"])),
+            "symbol": (lambda x: self.parse_unified_symbol(x["baseCoin"], x["quoteCoin"])),
+            "base": (lambda x: str(x["baseCoin"])),
+            "quote": (lambda x: str(x["quoteCoin"])),
+            "settle": (lambda x: str(x["quoteCoin"])),
             "multiplier": 1,  # spot multiplier default 1
             "leverage": 1,  # spot leverage default 1
             "listing_time": None,  # api not support this field
             "expiration_time": None,  # spot not support this field
             "contract_size": 1,  # spot contract size default 1
             "tick_size": None,  # Not yet implemented
-            "min_order_size": None,  # Not yet implemented
-            "max_order_size": None,  # Not yet implemented
+            "min_order_size": (lambda x: float(x["minTradeAmount"])),
+            "max_order_size": (lambda x: float(x["maxTradeAmount"])),
             "raw_data": (lambda x: x),
         }
 
-    def futures_exchange_info_parser(self, market_type: str):
+    @property
+    def derivative_exchange_info_parser(self):
         return {
-            "active": (lambda x: (x["status"] if market_type != "inverse" else x["contractStatus"]) == "TRADING"),
+            "active": (lambda x: x["symbolStatus"] == "normal"),
             "is_spot": False,
             "is_margin": False,
-            "is_futures": (lambda x: self.parse_is_futures(x["contractType"])),
-            "is_perp": (lambda x: self.parse_is_perpetual(x["contractType"])),
-            "is_linear": True if market_type == "linear" else False,
-            "is_inverse": True if market_type == "inverse" else False,
-            "symbol": (lambda x: self.parse_unified_symbol(self.parse_base_currency(x["baseAsset"]), x["quoteAsset"])),
-            "base": (lambda x: self.parse_base_currency(x["baseAsset"])),
-            "quote": (lambda x: x["quoteAsset"]),
-            "settle": (lambda x: x["marginAsset"]),
-            "multiplier": (lambda x: self.parse_multiplier(x["baseAsset"])),
-            "leverage": 1,  # need to find another way to get the leverage data
-            "listing_time": (lambda x: int(x["onboardDate"])),
-            "expiration_time": (lambda x: int(x["deliveryDate"])),
-            "contract_size": (
-                lambda x: 1 if "contractSize" not in x else float(x["contractSize"])
-            ),  # binance only have contract size to inverse perp and futures
+            "is_futures": (lambda x: self.parse_is_futures(x["symbolType"])),
+            "is_perp": (lambda x: self.parse_is_perpetual(x["symbolType"])),
+            "is_linear": (lambda x: False if x["quoteCoin"] in self.FIAT_CURRENCY else True),
+            "is_inverse": (lambda x: True if x["quoteCoin"] in self.FIAT_CURRENCY else False),
+            "symbol": (lambda x: self.parse_unified_symbol(x["baseCoin"], x["quoteCoin"])),
+            "base": (lambda x: self.parse_base_currency(x["baseCoin"])),
+            "quote": (lambda x: str(x["quoteCoin"])),
+            "settle": (lambda x: str(x["baseCoin"]) if x["quoteCoin"] in self.FIAT_CURRENCY else x["quoteCoin"]),
+            "multiplier": (lambda x: self.parse_multiplier(x["baseCoin"])),
+            "leverage": (lambda x: int(x["maxLever"])),
+            "listing_time": (lambda x: int(x["launchTime"]) if x["launchTime"] else None),
+            "expiration_time": (lambda x: int(x["deliveryTime"]) if x["deliveryTime"] else None),
+            "contract_size": (lambda x: float(x["sizeMultiplier"])),
             "tick_size": None,  # not yet implemented
-            "min_order_size": None,  # not yet implemented
-            "max_order_size": None,  # not yet implemented
+            "min_order_size": None,  # API not support this field
+            "max_order_size": None,  # API not support this field
             "raw_data": (lambda x: x),
         }
 
-    def parse_exchange_info(self, response: dict, parser: dict) -> dict:
+    def parse_exchange_info(self, response: dict, parser: callable):
         response = self.check_response(response)
-        if response["code"] != 200:
-            return response
 
-        datas = response["data"]["symbols"]
+        datas = response["data"]
         results = {}
         for data in datas:
             result = self.get_result_with_parser(data, parser)
-            id = self.parse_unified_id(result)
-            results[id] = result
-
+            instrument_id = self.parse_unified_id(result)
+            results[instrument_id] = result
         return results
 
-    def parse_ticker(self, response: dict, info: dict) -> dict:
-        if isinstance(response, list):
-            response = response[0]
-
-        base_volume = float(response["volume"] if info["is_linear"] else response["baseVolume"])
-        quote_volume = float(response["quoteVolume"] if info["is_linear"] else response["volume"])
-
-        quote_volume *= info["contract_size"] if info["is_perp"] or info["is_futures"] else 1
-
-        return {
-            "symbol": response["symbol"],
-            "open_time": int(response["openTime"]),
-            "close_time": int(response["closeTime"]),
-            "open": float(response["openPrice"]),
-            "high": float(response["highPrice"]),
-            "low": float(response["lowPrice"]),
-            "last_price": float(response["lastPrice"]),
-            "base_volume": base_volume,
-            "quote_volume": quote_volume,
-            "price_change": float(response["priceChange"]),
-            "price_change_percent": float(response["priceChangePercent"]) / 100,
+    def get_bitget_id_map(self, exchange_info: dict, market_type: str) -> dict:
+        if market_type == "derivative":
+            infos = query_dict(exchange_info, "is_perp == True or is_futures == True")
+        else:
+            infos = query_dict(exchange_info, f"is_{market_type} == True")
+
+        return {v["raw_data"]["symbol"]: k for k, v in infos.items()}
+
+    def parse_ticker(self, response: dict, info: dict, market_type: str):
+        return {
+            "timestamp": self.parse_str(response["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": None,  # API not support
+            "close_time": self.parse_str(response["ts"], int),
+            "open": self.parse_str(response["open" if market_type == "spot" else "open24h"], float),
+            "high": self.parse_str(response["high24h"], float),
+            "low": self.parse_str(response["low24h"], float),
+            "last": self.parse_str(response["lastPr"], float),
+            "base_volume": self.parse_str(response["baseVolume"], float),
+            "quote_volume": self.parse_str(response["quoteVolume"], float),
+            "price_change": None,  # API not support
+            "price_change_percent": self.parse_str(response["change24h"], float),
             "raw_data": response,
         }
 
-    def get_id_map(self, infos: dict, market_type: str) -> dict:
-        infos = self.query_dict(infos, {f"is_{market_type}": True})
-        return {v["raw_data"]["symbol"]: k for k, v in infos.items()}
+    def parse_raw_ticker(self, response: dict, info: dict, market_type: str):
+        response = self.check_response(response)
+        data = response["data"][0]
+        return self.parse_ticker(data, info, market_type)
 
-    def parse_tickers(self, response: dict, market_type: str, infos: dict) -> dict:
+    def parse_tickers(self, response: dict, exchange_info: dict, market_type: str) -> dict:
         response = self.check_response(response)
-        if response["code"] != 200:
-            return response
 
         datas = response["data"]
-        id_map = self.get_id_map(infos, market_type)
+
+        id_map = self.get_bitget_id_map(exchange_info, market_type)
         results = {}
         for data in datas:
             if data["symbol"] not in id_map:
-                print(data["symbol"])
+                print(f"Unmapped symbol: {data['symbol']} in {market_type} in Bitget")
                 continue
             instrument_id = id_map[data["symbol"]]
-            results[instrument_id] = self.parse_ticker(data, infos[instrument_id])
+            results[instrument_id] = self.parse_ticker(data, exchange_info[instrument_id], market_type)
         return results
 
-    def parse_kline(self, response: list, market_type: str) -> dict:
-        """
-        # spot
-        [
-            [
-                1499040000000,      // Kline open time
-                "0.01634790",       // Open price
-                "0.80000000",       // High price
-                "0.01575800",       // Low price
-                "0.01577100",       // Close price
-                "148976.11427815",  // Volume
-                1499644799999,      // Kline Close time
-                "2434.19055334",    // Quote asset volume
-                308,                // Number of trades
-                "1756.87402397",    // Taker buy base asset volume
-                "28.46694368",      // Taker buy quote asset volume
-                "0"                 // Unused field, ignore.
-            ]
-        ]
+    def parse_mark_index_price(self, response: dict, info: dict, query_type: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"][0]
 
-        # linear
-        # inverse
-        """
-        return {
-            int(response[0]): {
-                "open": float(response[1]),
-                "high": float(response[2]),
-                "low": float(response[3]),
-                "close": float(response[4]),
-                "base_volume": float(response[7]),
-                "quote_volume": float(response[5]),
-                "close_time": int(response[6]),
-                "raw_data": response,
-            }
+        return {
+            "timestamp": self.parse_str(data["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "index_price": self.parse_str(data["indexPrice" if query_type == "index" else "markPrice"], float),
+            "raw_data": data,
         }
 
-    def parse_klines(self, response: list, market_type: str) -> dict:
+    @staticmethod
+    def get_market_type(response: dict) -> str:
+        if response["is_spot"]:
+            return "spot"
+        elif response["is_futures"] or response["is_perp"]:
+            return "derivative"
+        else:
+            raise ValueError("Unknown market type")
+
+    @staticmethod
+    def get_product_type(response: dict) -> str:
+        if response["is_linear"]:
+            return f"{response['settle']}-FUTURES"
+        else:
+            return "COIN-FUTURES"
+
+    def get_interval(self, interval: str, market_type: str) -> str:
+        if interval not in self.INTERVAL_MAP[market_type]:
+            raise ValueError(f"Invalid interval {interval}")
+        return self.INTERVAL_MAP[market_type][interval]
+
+    def parse_candlesticks(self, response: dict, info: dict, market_type: str, interval: str) -> any:
         response = self.check_response(response)
         datas = response["data"]
-
-        results = {}
+        update_ = {
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "interval": interval,
+        }
+        results = []
         for data in datas:
-            result = self.parse_kline(data, market_type)
-            results.update(result)
-        return results
+            result = self.parse_candlestick(data, info, market_type)
+            result.update(update_)
+            results.append(result)
+        return results if len(results) > 1 else results[0]
 
-    def parse_spot_account_info(self, response: dict) -> dict:
-        response = self.check_response(response)
-        data = response["data"]
+    def parse_candlestick(self, data: list, info: dict, market_type: str):
         return {
-            "timestamp": data["updateTime"],
-            "account_id": data["uid"],
-            "account_type": data["accountType"],
+            "timestamp": self.parse_str(data[0], int),
+            "open": self.parse_str(data[1], float),
+            "high": self.parse_str(data[2], float),
+            "low": self.parse_str(data[3], float),
+            "close": self.parse_str(data[4], float),
+            "base_volume": self.parse_str(data[5], float),
+            "quote_volume": self.parse_str(data[6], float),
+            "contract_volume": self.parse_str(data[5], float) / (1 if market_type == "spot" else info["contract_size"]),
             "raw_data": data,
         }
 
-    def parse_margin_account_info(self, response: dict) -> dict:
-        response = self.check_response(response)
-
-        data = response["data"]
-        return {"raw_data": data}
-
-    def parse_margin_balance(self, response: dict, currency: str = None) -> dict:
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
         response = self.check_response(response)
-        datas = response["data"]["userAssets"]
-        query_currency = currency
+        data = response["data"][0]
 
-        results = {}
-        for data in datas:
-            if data["netAsset"] == "0":
-                continue
-
-            result = {
-                "currency": data["asset"],
-                "balance": self.parse_str(data["netAsset"], float),
-                "available": self.parse_str(data["free"], float),
-                "raw_data": data,
-            }
-            currency = result["currency"]
-            results[currency] = result
-        return results if not query_currency else {query_currency: results[query_currency]}
+        return {
+            "timestamp": response["timestamp"],
+            "next_funding_time": None,
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "funding_rate": self.parse_str(data["fundingRate"], float),
+            "raw_data": data,
+        }
 
-    def parse_history_funding_rate(self, response: dict, info: dict) -> list:
+    def parse_history_funding_rate(self, response: dict, info: dict) -> dict:
         response = self.check_response(response)
         datas = response["data"]
 
-        results = []
-        for data in datas:
-            result = {
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
+
+        return [
+            {
                 "timestamp": self.parse_str(data["fundingTime"], int),
-                "instrument_id": self.parse_unified_id(info),
-                "market": self.parse_unified_market_type(info),
+                "instrument_id": instrument_id,
+                "market_type": market_type,
                 "funding_rate": self.parse_str(data["fundingRate"], float),
-                "realized_rate": None,
+                "realized_rate": self.parse_str(data["fundingRate"], float),
                 "raw_data": data,
             }
-            results.append(result)
-        return results
-
-    def get_symbol(self, info: dict) -> str:
-        return f'{info["base"]}{info["quote"]}'
+            for data in datas
+        ]
 
-    def get_interval(self, interval: str) -> str:
-        return interval
+    def parse_orderbook(self, response: dict, info: dict) -> dict:
+        response = self.check_response(response)
+        datas = response["data"]
 
-    def get_market_type(self, info: dict):
-        if info["is_spot"]:
-            return "spot"
-        elif info["is_linear"]:
-            return "linear"
-        elif info["is_inverse"]:
-            return "inverse"
-        else:
-            raise Exception("market type not found")
+        return {
+            "timestamp": self.parse_str(datas["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "asks": [
+                {
+                    "price": self.parse_str(ask[0], float),
+                    "volume": self.parse_str(ask[1], float),
+                    "order_number": None,
+                }
+                for ask in datas["asks"]
+            ],
+            "bids": [
+                {
+                    "price": self.parse_str(bid[0], float),
+                    "volume": self.parse_str(bid[1], float),
+                    "order_number": None,
+                }
+                for bid in datas["bids"]
+            ],
+            "raw_data": datas,
+        }
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/bitget.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/bybit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,213 +1,301 @@
-from ..utils import query_dict
 from .base import Parser
 
 
-class BitgetParser(Parser):
-    LINEAR_FUTURES_SETTLE = ["USDT", "USDC"]
-
+class BybitParser(Parser):
     INTERVAL_MAP = {
-        "spot": {
-            "1m": "1min",
-            "5m": "5min",
-            "15m": "15min",
-            "30m": "30min",
-            "1h": "1h",
-            "4h": "4h",
-            "6h": "6h",
-            "12h": "12h",
-            "1d": "1day",
-            "3d": "3day",
-            "1w": "1week",
-            "1M": "1M",
-        },
-        "derivative": {
-            "1m": "1m",
-            "3m": "3m",
-            "5m": "5m",
-            "15m": "15m",
-            "30m": "30m",
-            "1h": "1H",
-            "4h": "4H",
-            "6h": "6H",
-            "12h": "12H",
-            "1d": "1D",
-            "1w": "1W",
-            "1M": "1M",
-        },
+        "1m": "1",
+        "3m": "3",
+        "5m": "5",
+        "15m": "15",
+        "30m": "30",
+        "1h": "60",
+        "2h": "120",
+        "4h": "240",
+        "6h": "360",
+        "12h": "720",
+        "1d": "D",
+        "1M": "M",
+        "1w": "W",
     }
 
-    def __init__(self):
-        super().__init__()
-
     def check_response(self, response: dict):
-        if response["code"] != "00000":
-            return {"code": 400, "status": "error", "data": response}
+        if response["retCode"] != 0:
+            raise ValueError(f"Error in parsing Bybit response: {response}")
+        else:
+            return {
+                "code": 200,
+                "status": "success",
+                "data": response["result"]["list"] if "list" in response["result"] else response["result"],
+                "timestamp": self.parse_str(response["time"], int),
+            }
+
+    @staticmethod
+    def get_market_type(info: dict) -> str:
+        if info["is_spot"]:
+            return "spot"
+        elif info["is_linear"]:
+            return "linear"
+        elif info["is_inverse"]:
+            return "inverse"
         else:
-            return {"code": 200, "status": "success", "data": response["data"]}
+            raise ValueError(f"Invalid market type: {info}")
 
     @property
-    def spot_exchange_info_parser(self):
+    def spot_exchange_info_parser(self) -> dict:
         return {
-            "active": (lambda x: x["status"] == "online"),
+            "active": (lambda x: x["status"] == "Trading"),
             "is_spot": True,
-            "is_margin": False,
+            "is_margin": (lambda x: self.parse_is_margin(x["marginTrading"])),
             "is_futures": False,
             "is_perp": False,
             "is_linear": True,
             "is_inverse": False,
             "symbol": (lambda x: self.parse_unified_symbol(x["baseCoin"], x["quoteCoin"])),
             "base": (lambda x: str(x["baseCoin"])),
             "quote": (lambda x: str(x["quoteCoin"])),
             "settle": (lambda x: str(x["quoteCoin"])),
             "multiplier": 1,  # spot multiplier default 1
             "leverage": 1,  # spot leverage default 1
             "listing_time": None,  # api not support this field
             "expiration_time": None,  # spot not support this field
             "contract_size": 1,  # spot contract size default 1
-            "tick_size": None,  # Not yet implemented
-            "min_order_size": (lambda x: float(x["minTradeAmount"])),
-            "max_order_size": (lambda x: float(x["maxTradeAmount"])),
+            "tick_size": (lambda x: float(x["priceFilter"]["tickSize"])),
+            "min_order_size": (lambda x: float(x["lotSizeFilter"]["minOrderQty"])),
+            "max_order_size": (lambda x: float(x["lotSizeFilter"]["maxOrderQty"])),
             "raw_data": (lambda x: x),
         }
 
     @property
-    def derivative_exchange_info_parser(self):
+    def perp_futures_exchange_info_parser(self) -> dict:
         return {
-            "active": (lambda x: x["symbolStatus"] == "normal"),
+            "active": (lambda x: x["status"] == "Trading"),
             "is_spot": False,
             "is_margin": False,
-            "is_futures": (lambda x: self.parse_is_futures(x["symbolType"])),
-            "is_perp": (lambda x: self.parse_is_perpetual(x["symbolType"])),
-            "is_linear": (lambda x: False if x["quoteCoin"] in self.FIAT_CURRENCY else True),
-            "is_inverse": (lambda x: True if x["quoteCoin"] in self.FIAT_CURRENCY else False),
-            "symbol": (lambda x: self.parse_unified_symbol(x["baseCoin"], x["quoteCoin"])),
+            "is_futures": (lambda x: self.parse_is_futures(x["contractType"])),
+            "is_perp": (lambda x: self.parse_is_perpetual(x["contractType"])),
+            "is_linear": (lambda x: self.parse_is_linear(x["contractType"])),
+            "is_inverse": (lambda x: self.parse_is_inverse(x["contractType"])),
+            "symbol": (lambda x: self.parse_unified_symbol(self.parse_base_currency(x["baseCoin"]), x["quoteCoin"])),
             "base": (lambda x: self.parse_base_currency(x["baseCoin"])),
             "quote": (lambda x: str(x["quoteCoin"])),
-            "settle": (lambda x: str(x["quoteCoin"])),
+            "settle": (lambda x: str(x["settleCoin"])),
             "multiplier": (lambda x: self.parse_multiplier(x["baseCoin"])),
-            "leverage": (lambda x: int(x["maxLever"])),
-            "listing_time": (lambda x: int(x["launchTime"]) if x["launchTime"] else None),
-            "expiration_time": (lambda x: int(x["deliveryTime"]) if x["deliveryTime"] else None),
-            "contract_size": (lambda x: float(x["sizeMultiplier"])),
-            "tick_size": None,  # not yet implemented
-            "min_order_size": None,  # API not support this field
-            "max_order_size": None,  # API not support this field
+            "leverage": (lambda x: float(x["leverageFilter"]["maxLeverage"])),
+            "listing_time": (lambda x: int(x["launchTime"])),
+            "expiration_time": (lambda x: int(x["deliveryTime"])),
+            "contract_size": (lambda x: float(x["lotSizeFilter"]["qtyStep"])),
+            "tick_size": (lambda x: float(x["priceFilter"]["tickSize"])),
+            "min_order_size": (lambda x: float(x["lotSizeFilter"]["minOrderQty"])),
+            "max_order_size": (lambda x: float(x["lotSizeFilter"]["maxOrderQty"])),
             "raw_data": (lambda x: x),
         }
 
-    def parse_exchange_info(self, response: dict, parser: callable):
+    def parse_exchange_info(self, response: dict, parser: dict) -> dict:
         response = self.check_response(response)
-        if response["code"] != 200:
-            return response
-
         datas = response["data"]
+
         results = {}
         for data in datas:
             result = self.get_result_with_parser(data, parser)
-            instrument_id = self.parse_unified_id(result)
-            results[instrument_id] = result
+            id = self.parse_unified_id(result)
+            results[id] = result
         return results
 
-    def get_bitget_id_map(self, exchange_info: dict, market_type: str) -> dict:
-        if market_type == "derivative":
-            infos = query_dict(exchange_info, "is_perp == True or is_futures == True")
-        else:
-            infos = query_dict(exchange_info, f"is_{market_type} == True")
+    def parse_tickers(self, response: dict, market_type: str, infos: dict) -> dict:
+        response = self.check_response(response)
+        datas = response["data"]
 
-        return {v["raw_data"]["symbol"]: k for k, v in infos.items()}
+        id_map = self.get_id_symbol_map(infos, market_type)
+        results = {}
+        for data in datas:
+            symbol = data["symbol"]
+            if symbol not in id_map:
+                print(f"Symbol {symbol} not found in Bybit exchange info.")
+                continue
+            instrument_id = id_map[symbol]
+            results[instrument_id] = self.parse_ticker(
+                data, market_type, infos[instrument_id], timestamp=response["timestamp"]
+            )
+        return results
 
-    def parse_spot_ticker(self, response: dict, info: dict):
-        return {
-            "symbol": response["symbol"],
-            "open_time": None,  # API not support
-            "close_time": int(response["ts"]),
-            "open": float(response["open"]),
-            "high": float(response["high24h"]),
-            "low": float(response["low24h"]),
-            "last_price": float(response["lastPr"]),
-            "base_volume": float(response["baseVolume"]),
-            "quote_volume": float(response["quoteVolume"]),
-            "price_change": float(response["change24h"]),
-            "price_change_percent": None,  # API not support
-            "raw_data": response,
-        }
+    def parse_raw_ticker(self, response: dict, market_type: str, info: dict):
+        response = self.check_response(response)
+        data = response["data"][0]
+        return self.parse_ticker(data, market_type, info, timestamp=response["timestamp"])
 
-    def parse_derivative_ticker(self, response: dict, info: dict):
+    def parse_ticker(self, response: dict, market_type: str, info: dict, **kwargs) -> dict:
         return {
-            "symbol": response["symbol"],
-            "open_time": None,  # API not support
-            "close_time": int(response["ts"]),
-            "open": float(response["open24h"]),
-            "high": float(response["high24h"]),
-            "low": float(response["low24h"]),
-            "last_price": float(response["lastPr"]),
-            "base_volume": float(response["baseVolume"]),
-            "quote_volume": float(response["quoteVolume"]),
-            "price_change": float(response["change24h"]),
-            "price_change_percent": None,  # API not support
+            "timestamp": self.parse_str(kwargs["timestamp"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": None,
+            "close_time": self.parse_str(kwargs["timestamp"], int),
+            "open": self.parse_str(response["prevPrice24h"], float),
+            "high": self.parse_str(response["highPrice24h"], float),
+            "low": self.parse_str(response["lowPrice24h"], float),
+            "last": self.parse_str(response["lastPrice"], float),
+            "base_volume": self.parse_str(response["volume24h" if market_type != "inverse" else "turnover24h"], float),
+            "quote_volume": self.parse_str(response["turnover24h" if market_type != "inverse" else "volume24h"], float),
+            "price_change": (
+                self.parse_str(response["prevPrice24h"], float) - self.parse_str(response["lastPrice"], float)
+            ),
+            "price_change_percent": self.parse_str(response["price24hPcnt"], float),
             "raw_data": response,
         }
 
-    def parse_tickers(self, response: dict, exchange_info: dict, market_type: str) -> dict:
+    def get_interval(self, interval: str) -> str:
+        if interval not in self.INTERVAL_MAP:
+            raise ValueError(f"Invalid interval: {interval}")
+        return self.INTERVAL_MAP[interval]
+
+    def parse_candlesticks(self, response: dict, info: dict, market_type: str, interval: str) -> any:
         response = self.check_response(response)
-        if response["code"] != 200:
-            return response
+        datas = response["data"]
+
+        market = self.parse_unified_market_type(info)
+        instrument_id = self.parse_unified_id(info)
+
+        results = [
+            {
+                "timestamp": self.parse_str(data[0], int),
+                "instrument_id": instrument_id,
+                "market_type": market,
+                "interval": interval,
+                "open": self.parse_str(data[1], float),
+                "high": self.parse_str(data[2], float),
+                "low": self.parse_str(data[3], float),
+                "close": self.parse_str(data[4], float),
+                "base_volume": self.parse_str(data[5], float),
+                "quote_volume": self.parse_str(data[6], float),
+                "contract_volume": (
+                    self.parse_str(data[5], float) / (1 if market_type == "spot" else info["contract_size"])
+                ),
+                "raw_data": data,
+            }
+            for data in datas
+        ]
+
+        return results if len(results) > 1 else results[0]
 
+    def get_category(self, info: dict) -> str:
+        if info["is_spot"] or info["is_margin"]:
+            return "spot"
+        elif info["is_linear"]:
+            return "linear"
+        elif info["is_inverse"]:
+            return "inverse"
+        else:
+            raise ValueError(f"Invalid market type: {info}")
+
+    def parse_funding_rate(self, response: dict, info: dict) -> list:
+        response = self.check_response(response)
         datas = response["data"]
 
-        method_map = {"spot": self.parse_spot_ticker, "derivative": self.parse_derivative_ticker}
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
 
-        id_map = self.get_bitget_id_map(exchange_info, market_type)
-        results = {}
+        results = []
         for data in datas:
-            if data["symbol"] not in id_map:
-                print(f"Unmapped symbol: {data['symbol']} in {market_type}")
-                continue
-            instrument_id = id_map[data["symbol"]]
-            results[instrument_id] = method_map[market_type](data, exchange_info[instrument_id])
+            results.append(
+                {
+                    "timestamp": self.parse_str(data["fundingRateTimestamp"], int),
+                    "instrument_id": instrument_id,
+                    "market_type": market_type,
+                    "funding_rate": self.parse_str(data["fundingRate"], float),
+                    "realized_rate": self.parse_str(data["fundingRate"], float),
+                    "raw_data": data,
+                }
+            )
         return results
 
     @staticmethod
-    def get_market_type(response: dict) -> str:
-        if response["is_spot"]:
-            return "spot"
-        elif response["is_futures"] or response["is_perp"]:
-            return "derivative"
-        else:
-            raise ValueError("Unknown market type")
+    def get_open_interest_interval(interval: str) -> str:
+        interval_map = {
+            "5m": "5min",
+            "15m": "15min",
+            "30m": "30min",
+            "1h": "1h",
+            "4h": "4h",
+            "1d": "1d",
+        }
+        if interval not in interval_map:
+            raise ValueError(f"Invalid interval: {interval}, should be one of {list(interval_map.keys())}")
+        return interval_map[interval]
 
-    @staticmethod
-    def get_product_type(response: dict) -> str:
-        if response["is_linear"]:
-            return f"{response['settle']}-FUTURES"
-        else:
-            return "COIN-FUTURES"
+    def parse_open_interest(self, response: dict, info: dict) -> dict | list:
+        response = self.check_response(response)
 
-    def get_interval(self, interval: str, market_type: str) -> str:
-        if interval not in self.INTERVAL_MAP[market_type]:
-            raise ValueError(f"Invalid interval {interval}")
-        return self.INTERVAL_MAP[market_type][interval]
+        results = []
+        datas = response["data"]
+        for datas in datas:
+            results.append(
+                {
+                    "timestamp": self.parse_str(datas["timestamp"], int),
+                    "instrument_id": self.parse_unified_id(info),
+                    "open_interest": self.parse_str(datas["openInterest"], float),
+                    "raw_data": datas,
+                }
+            )
+        return results[0] if len(results) == 1 else results
 
-    def parse_klines(self, response: dict, market_type: str) -> dict:
+    def parse_orderbook(self, response: dict, info: dict) -> dict:
         response = self.check_response(response)
-        if response["code"] != 200:
-            return response
-
         datas = response["data"]
-        results = {}
-        for data in datas:
-            timestamp = int(data[0])
-            results[timestamp] = self.parse_kline(data, market_type)
-        return results
 
-    def parse_kline(self, response: list, market_type: str) -> dict:
+        asks = datas["a"]
+        bids = datas["b"]
+
         return {
-            "open": float(response[1]),
-            "high": float(response[2]),
-            "low": float(response[3]),
-            "close": float(response[4]),
-            "base_volume": float(response[5]),
-            "quote_volume": float(response[6]),
-            "close_time": None,
-            "raw_data": response,
+            "timestamp": self.parse_str(datas["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "asks": [
+                {"price": self.parse_str(ask[0], float), "volume": self.parse_str(ask[1], float), "order_number": None}
+                for ask in asks
+            ],
+            "bids": [
+                {"price": self.parse_str(bid[0], float), "volume": self.parse_str(bid[1], float), "order_number": None}
+                for bid in bids
+            ],
+            "raw_data": datas,
+        }
+
+    def parse_last_price(self, response: dict, instrument_id: str) -> dict:
+        response = self.check_response(response)
+        datas = response["data"][0]
+        return {
+            "timestamp": response["timestamp"],
+            "instrument_id": instrument_id,
+            "last_price": float(datas["lastPrice"]),
+            "raw_data": datas,
+        }
+
+    def parse_index_price(self, response: dict, instrument_id: str) -> dict:
+        response = self.check_response(response)
+        datas = response["data"][0]
+        return {
+            "timestamp": response["timestamp"],
+            "instrument_id": instrument_id,
+            "index_price": float(datas["indexPrice"]),
+            "raw_data": datas,
+        }
+
+    def parse_mark_price(self, response: dict, instrument_id: str) -> dict:
+        response = self.check_response(response)
+        datas = response["data"][0]
+        return {
+            "timestamp": response["timestamp"],
+            "instrument_id": instrument_id,
+            "mark_price": float(datas["markPrice"]),
+            "raw_data": datas,
+        }
+
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
+        response = self.check_response(response)
+        data = response["data"][0]
+        return {
+            "timestamp": response["timestamp"],
+            "next_funding_time": self.parse_str(data["nextFundingTime"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "funding_rate": self.parse_str(data["fundingRate"], float),
+            "raw_data": data,
         }
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/bybit.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/binance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,262 +1,321 @@
-from datetime import datetime as dt
-from datetime import timedelta as td
-
 from .base import Parser
 
 
-class BybitParser(Parser):
-    INTERVAL_MAP = {
-        "1m": "1",
-        "3m": "3",
-        "5m": "5",
-        "15m": "15",
-        "30m": "30",
-        "1h": "60",
-        "2h": "120",
-        "4h": "240",
-        "6h": "360",
-        "12h": "720",
-        "1d": "D",
-        "1M": "M",
-        "1w": "W",
-    }
-
-    def check_response(self, response: dict):
-        if response["retCode"] != 0:
-            raise ValueError(f"Error in parsing Bybit response: {response}")
-        else:
-            return {
-                "code": 200,
-                "status": "success",
-                "data": response["result"]["list"] if "list" in response["result"] else response["result"],
-                "timestamp": self.parse_str(response["time"], int),
-            }
+class BinanceParser(Parser):
+    @staticmethod
+    def check_response(response: dict):
+        return {"code": 200, "status": "success", "data": response}
 
     @property
-    def spot_exchange_info_parser(self) -> dict:
+    def spot_exchange_info_parser(self):
         return {
-            "active": (lambda x: x["status"] == "Trading"),
+            "active": (lambda x: x["status"] == "TRADING"),
             "is_spot": True,
-            "is_margin": (lambda x: self.parse_is_margin(x["marginTrading"])),
+            "is_margin": (lambda x: x["isMarginTradingAllowed"]),
             "is_futures": False,
             "is_perp": False,
             "is_linear": True,
             "is_inverse": False,
-            "symbol": (lambda x: self.parse_unified_symbol(x["baseCoin"], x["quoteCoin"])),
-            "base": (lambda x: str(x["baseCoin"])),
-            "quote": (lambda x: str(x["quoteCoin"])),
-            "settle": (lambda x: str(x["quoteCoin"])),
+            "symbol": (lambda x: self.parse_unified_symbol(x["baseAsset"], x["quoteAsset"])),
+            "base": (lambda x: str(x["baseAsset"])),
+            "quote": (lambda x: str(x["quoteAsset"])),
+            "settle": (lambda x: str(x["quoteAsset"])),
             "multiplier": 1,  # spot multiplier default 1
             "leverage": 1,  # spot leverage default 1
             "listing_time": None,  # api not support this field
             "expiration_time": None,  # spot not support this field
             "contract_size": 1,  # spot contract size default 1
-            "tick_size": (lambda x: float(x["priceFilter"]["tickSize"])),
-            "min_order_size": (lambda x: float(x["lotSizeFilter"]["minOrderQty"])),
-            "max_order_size": (lambda x: float(x["lotSizeFilter"]["maxOrderQty"])),
+            "tick_size": None,  # Not yet implemented
+            "min_order_size": None,  # Not yet implemented
+            "max_order_size": None,  # Not yet implemented
             "raw_data": (lambda x: x),
         }
 
-    @property
-    def perp_futures_exchange_info_parser(self) -> dict:
+    def futures_exchange_info_parser(self, market_type: str):
         return {
-            "active": (lambda x: x["status"] == "Trading"),
+            "active": (lambda x: (x["status"] if market_type != "inverse" else x["contractStatus"]) == "TRADING"),
             "is_spot": False,
             "is_margin": False,
             "is_futures": (lambda x: self.parse_is_futures(x["contractType"])),
             "is_perp": (lambda x: self.parse_is_perpetual(x["contractType"])),
-            "is_linear": (lambda x: self.parse_is_linear(x["contractType"])),
-            "is_inverse": (lambda x: self.parse_is_inverse(x["contractType"])),
-            "symbol": (lambda x: self.parse_unified_symbol(self.parse_base_currency(x["baseCoin"]), x["quoteCoin"])),
-            "base": (lambda x: self.parse_base_currency(x["baseCoin"])),
-            "quote": (lambda x: str(x["quoteCoin"])),
-            "settle": (lambda x: str(x["settleCoin"])),
-            "multiplier": (lambda x: self.parse_multiplier(x["baseCoin"])),
-            "leverage": (lambda x: float(x["leverageFilter"]["maxLeverage"])),
-            "listing_time": (lambda x: int(x["launchTime"])),
-            "expiration_time": (lambda x: int(x["deliveryTime"])),
-            "contract_size": (lambda x: float(x["lotSizeFilter"]["qtyStep"])),
-            "tick_size": (lambda x: float(x["priceFilter"]["tickSize"])),
-            "min_order_size": (lambda x: float(x["lotSizeFilter"]["minOrderQty"])),
-            "max_order_size": (lambda x: float(x["lotSizeFilter"]["maxOrderQty"])),
+            "is_linear": True if market_type == "linear" else False,
+            "is_inverse": True if market_type == "inverse" else False,
+            "symbol": (lambda x: self.parse_unified_symbol(self.parse_base_currency(x["baseAsset"]), x["quoteAsset"])),
+            "base": (lambda x: self.parse_base_currency(x["baseAsset"])),
+            "quote": (lambda x: x["quoteAsset"]),
+            "settle": (lambda x: x["marginAsset"]),
+            "multiplier": (lambda x: self.parse_multiplier(x["baseAsset"])),
+            "leverage": 1,  # need to find another way to get the leverage data
+            "listing_time": (lambda x: int(x["onboardDate"])),
+            "expiration_time": (lambda x: int(x["deliveryDate"])),
+            "contract_size": (
+                lambda x: 1 if "contractSize" not in x else float(x["contractSize"])
+            ),  # binance only have contract size to inverse perp and futures
+            "tick_size": None,  # not yet implemented
+            "min_order_size": None,  # not yet implemented
+            "max_order_size": None,  # not yet implemented
             "raw_data": (lambda x: x),
         }
 
     def parse_exchange_info(self, response: dict, parser: dict) -> dict:
         response = self.check_response(response)
-        datas = response["data"]
+        if response["code"] != 200:
+            return response
 
+        datas = response["data"]["symbols"]
         results = {}
         for data in datas:
             result = self.get_result_with_parser(data, parser)
             id = self.parse_unified_id(result)
             results[id] = result
+
         return results
 
-    def parse_tickers(self, response: dict, market_type: str) -> list:
-        response = self.check_response(response)
-        datas = response["data"]
+    def parse_ticker(self, response: dict, info: dict) -> dict:
+        if isinstance(response, list):
+            response = response[0]
 
-        results = []
-        for data in datas:
-            result = self.parse_ticker(data, market_type)
-            results.append(result)
-        return results
+        base_volume = float(response["volume"] if info["is_linear"] else response["baseVolume"])
+        quote_volume = float(response["quoteVolume"] if info["is_linear"] else response["volume"])
+
+        quote_volume *= info["contract_size"] if info["is_perp"] or info["is_futures"] else 1
 
-    def parse_ticker(self, response: dict, market_type: str) -> dict:
         return {
-            "symbol": response["symbol"],
-            "open_time": int((dt.now() - td(days=1)).timestamp() * 1000),
-            "close_time": int(dt.now().timestamp() * 1000),
-            "open": float(response["prevPrice24h"]),
-            "high": float(response["highPrice24h"]),
-            "low": float(response["lowPrice24h"]),
-            "last_price": float(response["lastPrice"]),
-            "base_volume": float(response["volume24h"]) if market_type != "inverse" else float(response["turnover24h"]),
-            "quote_volume": float(response["turnover24h"])
-            if market_type != "inverse"
-            else float(response["volume24h"]),
-            "price_change": float(response["prevPrice24h"]) - float(response["lastPrice"]),
-            "price_change_percent": float(response["price24hPcnt"]),
+            "timestamp": self.parse_str(response["closeTime"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": self.parse_str(response["openTime"], int),
+            "close_time": self.parse_str(response["closeTime"], int),
+            "open": self.parse_str(response["openPrice"], float),
+            "high": self.parse_str(response["highPrice"], float),
+            "low": self.parse_str(response["lowPrice"], float),
+            "last": self.parse_str(response["lastPrice"], float),
+            "base_volume": base_volume,
+            "quote_volume": quote_volume,
+            "price_change": self.parse_str(response["priceChange"], float),
+            "price_change_percent": self.parse_str(response["priceChangePercent"], float) / 100,
             "raw_data": response,
         }
 
-    def get_interval(self, interval: str) -> str:
-        if interval not in self.INTERVAL_MAP:
-            raise ValueError(f"Invalid interval: {interval}")
-        return self.INTERVAL_MAP[interval]
+    def get_id_map(self, infos: dict, market_type: str) -> dict:
+        infos = self.query_dict(infos, {f"is_{market_type}": True})
+        return {v["raw_data"]["symbol"]: k for k, v in infos.items()}
 
-    def parse_klines(self, response: dict) -> dict:
+    def parse_tickers(self, response: dict, market_type: str, infos: dict) -> dict:
         response = self.check_response(response)
+        if response["code"] != 200:
+            return response
 
-        results = {}
         datas = response["data"]
+        id_map = self.get_id_map(infos, market_type)
+        results = {}
         for data in datas:
-            result = self.parse_kline(data)
-            timestamp = int(data[0])
-            results[timestamp] = result
+            if data["symbol"] not in id_map:
+                print(data["symbol"])
+                continue
+            instrument_id = id_map[data["symbol"]]
+            results[instrument_id] = self.parse_ticker(data, infos[instrument_id])
         return results
 
-    def get_category(self, info: dict) -> str:
-        if info["is_spot"] or info["is_margin"]:
-            return "spot"
-        elif info["is_linear"]:
-            return "linear"
-        elif info["is_inverse"]:
-            return "inverse"
-        else:
-            raise ValueError(f"Invalid market type: {info}")
-
-    def parse_kline(self, response: dict) -> dict:
+    def parse_spot_account_info(self, response: dict) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
         return {
-            "open": float(response[1]),
-            "high": float(response[2]),
-            "low": float(response[3]),
-            "close": float(response[4]),
-            "base_volume": float(response[5]),
-            "quote_volume": float(response[6]),
-            "raw_data": response,
+            "timestamp": data["updateTime"],
+            "account_id": data["uid"],
+            "account_type": data["accountType"],
+            "raw_data": data,
         }
 
-    def parse_funding_rate(self, response: dict, info: dict) -> list:
+    def parse_margin_account_info(self, response: dict) -> dict:
+        response = self.check_response(response)
+
+        data = response["data"]
+        return {"raw_data": data}
+
+    def parse_margin_balance(self, response: dict, currency: str = None) -> dict:
+        response = self.check_response(response)
+        datas = response["data"]["userAssets"]
+        query_currency = currency
+
+        results = {}
+        for data in datas:
+            if data["netAsset"] == "0":
+                continue
+
+            result = {
+                "currency": data["asset"],
+                "balance": self.parse_str(data["netAsset"], float),
+                "available": self.parse_str(data["free"], float),
+                "raw_data": data,
+            }
+            currency = result["currency"]
+            results[currency] = result
+        return results if not query_currency else {query_currency: results[query_currency]}
+
+    def parse_history_funding_rate(self, response: dict, info: dict) -> list:
         response = self.check_response(response)
         datas = response["data"]
 
         results = []
         for data in datas:
-            results.append(
-                {
-                    "timestamp": self.parse_str(data["fundingRateTimestamp"], int),
-                    "instrument_id": self.parse_unified_id(info),
-                    "funding_rate": self.parse_str(data["fundingRate"], float),
-                    "raw_data": data,
-                }
-            )
+            result = {
+                "timestamp": int(round(self.parse_str(data["fundingTime"], int) / 1000)) * 1000,
+                "instrument_id": self.parse_unified_id(info),
+                "market_type": self.parse_unified_market_type(info),
+                "funding_rate": self.parse_str(data["fundingRate"], float),
+                "realized_rate": None,
+                "raw_data": data,
+            }
+            results.append(result)
         return results
 
-    @staticmethod
-    def get_open_interest_interval(interval: str) -> str:
-        interval_map = {
-            "5m": "5min",
-            "15m": "15min",
-            "30m": "30min",
-            "1h": "1h",
-            "4h": "4h",
-            "1d": "1d",
+    def parse_last_price(self, response: dict, instrument_id: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"][instrument_id]
+
+        return {
+            "timestamp": data["close_time"],
+            "instrument_id": instrument_id,
+            "last_price": self.parse_str(data["last_price"], float),
+            "raw_data": data,
         }
-        if interval not in interval_map:
-            raise ValueError(f"Invalid interval: {interval}, should be one of {list(interval_map.keys())}")
-        return interval_map[interval]
 
-    def parse_open_interest(self, response: dict, info: dict) -> dict | list:
+    def parse_index_price(self, response: dict, info: dict, market_type: str) -> dict:
         response = self.check_response(response)
+        data = response["data"]
 
-        results = []
-        datas = response["data"]
-        for datas in datas:
-            results.append(
-                {
-                    "timestamp": self.parse_str(datas["timestamp"], int),
-                    "instrument_id": self.parse_unified_id(info),
-                    "open_interest": self.parse_str(datas["openInterest"], float),
-                    "raw_data": datas,
-                }
-            )
-        return results[0] if len(results) == 1 else results
+        if not isinstance(data, dict):
+            data = data[0]
+
+        if market_type == "spot":
+            return {
+                "timestamp": self.parse_str(data["calcTime"], int),
+                "instrument_id": self.parse_unified_id(info),
+                "index_price": self.parse_str(data["price"], float),
+                "raw_data": data,
+            }
+        else:  # linear, inverse
+            return {
+                "timestamp": self.parse_str(data["time"], int),
+                "instrument_id": self.parse_unified_id(info),
+                "index_price": self.parse_str(data["indexPrice"], float),
+                "raw_data": data,
+            }
 
-    def parse_orderbook(self, response: dict, info: dict) -> dict:
+    def parse_mark_price(self, response: dict, info: dict, market_type: str) -> dict:
         response = self.check_response(response)
-        datas = response["data"]
+        data = response["data"]
+
+        if not isinstance(data, dict):
+            data = data[0]
+
+        return {
+            "timestamp": self.parse_str(data["time"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "mark_price": self.parse_str(data["markPrice"], float),
+            "raw_data": data,
+        }
 
-        asks = datas["a"]
-        bids = datas["b"]
+    def parse_open_interest(self, response: dict, info: dict, market_type: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
 
         return {
-            "timestamp": self.parse_str(datas["ts"], int),
+            "timestamp": self.parse_str(data["time"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "oi_contract": self.parse_str(data["openInterest"], float),
+            "oi_currency": None,
+            "raw_data": data,
+        }
+
+    def parse_orderbook(self, response: dict, info: dict, market_type: str, depth: int) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
+
+        results = {
+            "timestamp": self.get_timestamp(),
             "instrument_id": self.parse_unified_id(info),
             "asks": [
                 {
                     "price": self.parse_str(ask[0], float),
                     "volume": self.parse_str(ask[1], float),
+                    "order_number": None,
                 }
-                for ask in asks
+                for ask in data["asks"]
             ],
             "bids": [
                 {
                     "price": self.parse_str(bid[0], float),
                     "volume": self.parse_str(bid[1], float),
+                    "order_number": None,
                 }
-                for bid in bids
+                for bid in data["bids"]
             ],
-            "raw_data": datas,
+            "raw_data": data,
         }
 
-    def parse_last_price(self, response: dict, instrument_id: str) -> dict:
-        response = self.check_response(response)
-        datas = response["data"][0]
-        return {
-            "timestamp": response["timestamp"],
-            "instrument_id": instrument_id,
-            "last_price": float(datas["lastPrice"]),
-            "raw_data": datas,
-        }
+        results["bids"] = sorted(results["bids"], key=lambda x: x["price"], reverse=True)
+        results["asks"] = sorted(results["asks"], key=lambda x: x["price"])
+
+        if depth:
+            results["bids"] = results["bids"][:depth]
+            results["asks"] = results["asks"][:depth]
+
+        return results
 
-    def parse_index_price(self, response: dict, instrument_id: str) -> dict:
+    def get_symbol(self, info: dict) -> str:
+        return f'{info["base"]}{info["quote"]}'
+
+    def get_interval(self, interval: str) -> str:
+        return interval
+
+    def get_market_type(self, info: dict):
+        if info["is_spot"]:
+            return "spot"
+        elif info["is_linear"]:
+            return "linear"
+        elif info["is_inverse"]:
+            return "inverse"
+        else:
+            raise Exception("market type not found")
+
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
         response = self.check_response(response)
-        datas = response["data"][0]
+        data = response["data"]
+
         return {
-            "timestamp": response["timestamp"],
-            "instrument_id": instrument_id,
-            "index_price": float(datas["indexPrice"]),
-            "raw_data": datas,
+            "timestamp": self.parse_str(data["time"], int),
+            "next_funding_time": self.parse_str(data["nextFundingTime"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "funding_rate": self.parse_str(data["lastFundingRate"], float),
+            "raw_data": data,
         }
 
-    def parse_mark_price(self, response: dict, instrument_id: str) -> dict:
+    def parse_candlesticks(self, response: dict, info: dict, market_type: str, interval: str) -> any:
         response = self.check_response(response)
-        datas = response["data"][0]
-        return {
-            "timestamp": response["timestamp"],
-            "instrument_id": instrument_id,
-            "mark_price": float(datas["markPrice"]),
-            "raw_data": datas,
-        }
+        datas = response["data"]
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
+
+        results = []
+
+        for data in datas:
+            results.append(
+                {
+                    "timestamp": self.parse_str(data[0], int),
+                    "instrument_id": instrument_id,
+                    "market_type": market_type,
+                    "interval": interval,
+                    "open": self.parse_str(data[1], float),
+                    "high": self.parse_str(data[2], float),
+                    "low": self.parse_str(data[3], float),
+                    "close": self.parse_str(data[4], float),
+                    "base_volume": self.parse_str(data[5], float),
+                    "quote_volume": self.parse_str(data[7], float),
+                    "contract_volume": self.parse_str(data[5], float),
+                    "raw_data": data,
+                }
+            )
+        return results[0] if len(results) == 1 else results
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/gateio.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/kucoin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,278 +1,349 @@
+from ..utils import query_dict
 from .base import Parser
 
 
-class GateioParser(Parser):
-
-    INTERVAL_MAP = {
-        "1m": "1m",
-        "5m": "5m",
-        "15m": "15m",
-        "30m": "30m",
-        "1h": "1h",
-        "4h": "4h",
-        "8h": "8h",
-        "1d": "1d",
-        "7d": "7d",
-        "1M": "30d",
+class KucoinParser(Parser):
+    SPOT_INTERVAL_MAP = {
+        "1m": "1min",
+        "3m": "3min",
+        "5m": "5min",
+        "15m": "15min",
+        "30m": "30min",
+        "1h": "1hour",
+        "2h": "2hour",
+        "4h": "4hour",
+        "6h": "6hour",
+        "8h": "8hour",
+        "12h": "12hour",
+        "1d": "1day",
+        "1w": "1week",
     }
 
-    def __init__(self):
-        super().__init__()
+    DERIVATIVE_INTERVAL_MAP = {
+        "1m": 1,
+        "5m": 5,
+        "15m": 15,
+        "30m": 30,
+        "1h": 60,
+        "2h": 120,
+        "4h": 240,
+        "8h": 480,
+        "12h": 720,
+        "1d": 1440,
+        "1w": 10080,
+    }
 
     @staticmethod
     def check_response(response: dict):
-        return {"code": 200, "status": "success", "data": response}
+        if response.get("code") == "200000":
+            return {"code": 200, "status": "success", "data": response["data"]}
+        else:
+            raise ValueError(f"Error when checking response: {response} in KucoinParser")
+
+    def parse_kucoin_base_currency(self, base: str) -> str:
+        base = base.replace("XBT", "BTC")
+        return self.parse_base_currency(base)
 
     @property
     def spot_exchange_info_parser(self) -> dict:
         return {
-            "active": (lambda x: x["trade_status"] == "tradable"),
+            "active": (lambda x: x["enableTrading"]),
             "is_spot": True,
-            "is_margin": False,
+            "is_margin": (lambda x: x["isMarginEnabled"]),
             "is_futures": False,
             "is_perp": False,
             "is_linear": True,
             "is_inverse": False,
-            "symbol": (lambda x: self.parse_unified_symbol(x["base"], x["quote"])),
-            "base": (lambda x: str(x["base"])),
-            "quote": (lambda x: str(x["quote"])),
-            "settle": (lambda x: str(x["quote"])),
+            "symbol": (lambda x: self.parse_unified_symbol(x["baseCurrency"], x["quoteCurrency"])),
+            "base": (lambda x: self.parse_kucoin_base_currency(x["baseCurrency"])),
+            "quote": (lambda x: str(x["quoteCurrency"])),
+            "settle": (lambda x: str(x["quoteCurrency"])),
             "multiplier": 1,  # spot multiplier default 1
             "leverage": 1,  # spot leverage default 1
-            "listing_time": (lambda x: min([int(x["sell_start"]), int(x["buy_start"])]) * 1000),
+            "listing_time": None,  # api not support this field
             "expiration_time": None,  # spot not support this field
             "contract_size": 1,  # spot contract size default 1
-            "tick_size": 1,
-            "min_order_size": (lambda x: float(x["min_quote_amount"]) if "min_quote_amount" in x else 0),
-            "max_order_size": (lambda x: float(x["max_quote_amount"]) if "max_quote_amount" in x else 0),
-            "raw_data": (lambda x: x),
-        }
-
-    @property
-    def perp_exchange_info_parser(self) -> dict:
-        return {
-            "active": True,
-            "is_spot": False,
-            "is_margin": False,
-            "is_futures": False,
-            "is_perp": True,
-            "is_linear": (lambda x: True if x["settle"] in self.STABLE_CURRENCY else False),
-            "is_inverse": (lambda x: False if x["settle"] in self.STABLE_CURRENCY else True),
-            "symbol": (
-                lambda x: self.parse_unified_symbol(
-                    self.parse_perp_name(x["name"])["base"], self.parse_perp_name(x["name"])["quote"]
-                )
-            ),
-            "base": (lambda x: self.parse_perp_name(x["name"])["base"]),
-            "quote": (lambda x: self.parse_perp_name(x["name"])["quote"]),
-            "settle": (lambda x: str(x["settle"])),
-            "multiplier": None,
-            "leverage": (lambda x: float(x["leverage_max"])),
-            "listing_time": None,
-            "expiration_time": None,
-            "contract_size": None,
-            "tick_size": None,
-            "min_order_size": None,
-            "max_order_size": None,
+            "tick_size": None,  # Not yet implemented
+            "min_order_size": None,  # Not yet implemented
+            "max_order_size": None,  # Not yet implemented
             "raw_data": (lambda x: x),
         }
 
     @property
     def futures_exchange_info_parser(self) -> dict:
         return {
-            "active": (lambda x: not x["in_delisting"]),
+            "active": (lambda x: x["status"] == "Open"),
             "is_spot": False,
             "is_margin": False,
-            "is_futures": True,
-            "is_perp": False,
-            "is_linear": (lambda x: True if x["settle"] in self.STABLE_CURRENCY else False),
-            "is_inverse": (lambda x: False if x["settle"] in self.STABLE_CURRENCY else True),
-            "symbol": (
-                lambda x: self.parse_unified_symbol(
-                    self.parse_futures_name(x["name"])["base"], self.parse_futures_name(x["name"])["quote"]
-                )
-            ),
-            "base": (lambda x: self.parse_base_currency(self.parse_futures_name(x["name"])["base"])),
-            "quote": (lambda x: self.parse_futures_name(x["name"])["quote"]),
-            "settle": (lambda x: str(x["settle"])),
-            "multiplier": (lambda x: self.parse_multiplier(self.parse_futures_name(x["name"])["base"])),
-            "leverage": 1,  # Not yet implemented
-            "listing_time": None,
-            "expiration_time": (lambda x: int(x["expire_time"]) * 1000),
-            "contract_size": None,
-            "tick_size": None,
-            "min_order_size": None,
-            "max_order_size": None,
+            "is_futures": (lambda x: True if x["expireDate"] else False),
+            "is_perp": (lambda x: False if x["expireDate"] else True),
+            "is_linear": (lambda x: True),  # Not yet implemented
+            "is_inverse": (lambda x: False),  # Not yet implemented
+            "symbol": (lambda x: self.parse_unified_symbol(x["baseCurrency"], x["quoteCurrency"])),
+            "base": (lambda x: self.parse_kucoin_base_currency(x["baseCurrency"])),
+            "quote": (lambda x: str(x["quoteCurrency"])),
+            "settle": (lambda x: str(x["quoteCurrency"])),
+            "multiplier": (lambda x: self.parse_multiplier(x["baseCurrency"])),
+            "leverage": (lambda x: x["maxLeverage"]),
+            "listing_time": (lambda x: x["firstOpenDate"] if x["firstOpenDate"] else None),
+            "expiration_time": (lambda x: x["expireDate"] if x["expireDate"] else None),
+            "contract_size": (lambda x: abs(int(x["multiplier"]))),
+            "tick_size": None,  # Not yet implemented
+            "min_order_size": None,  # Not yet implemented
+            "max_order_size": None,  # Not yet implemented
             "raw_data": (lambda x: x),
         }
 
-    def parse_perp_name(self, name: str) -> dict:
-        return {
-            "base": name.split("_")[0],
-            "quote": name.split("_")[1],
-        }
-
-    def parse_futures_name(self, name: str) -> dict:
-        return {
-            "base": name.split("_")[0],
-            "quote": name.split("_")[1],
-            "datetime": name.split("_")[2],
-        }
-
-    def parse_exchange_info(self, response: dict, parser: dict, **kwargs) -> dict:
+    def parse_exchange_info(self, response: dict, parser: dict) -> dict:
         response = self.check_response(response)
-        datas = response["data"]
 
+        datas = response["data"]
         results = {}
         for data in datas:
-            data.update(kwargs)
             result = self.get_result_with_parser(data, parser)
             id = self.parse_unified_id(result)
             results[id] = result
         return results
 
-    def get_id_map(self, exchange_info: dict, market_type: str) -> dict:
-        raw_id = {
-            "spot": "id",
-            "futures": "name",
-            "perp": "name",
-        }
-        infos = self.query_dict(exchange_info, {f"is_{market_type}": True})
-        return {v["raw_data"][raw_id[market_type]]: k for k, v in infos.items()}
+    def get_id_map(self, infos: dict, market_type: str) -> dict:
+        if market_type == "derivative":
+            infos = query_dict(infos, f"is_futures == True or is_perp == True")
+        else:
+            infos = query_dict(infos, f"is_{market_type} == True")
+        return {v["raw_data"]["symbol"]: k for k, v in infos.items()}
 
-    def parse_tickers(self, response: dict, exchange_info: dict, market_type: str) -> dict:
+    def parse_spot_tickers(self, response: dict, infos: dict) -> dict:
         response = self.check_response(response)
-        datas = response["data"]
+        id_map = self.get_id_map(infos, "spot")
 
-        id_map = self.get_id_map(exchange_info, market_type)
-        method_map = {
-            "spot": self.parse_spot_ticker,
-            "futures": self.parse_futures_ticker,
-            "perp": self.parse_perp_ticker,
-        }
+        datas = response["data"]["ticker"]
+        results = {}
+        for data in datas:
+            id = id_map[data["symbol"]]
+            result = self.parse_spot_ticker(data, infos[id])
+            results[id] = result
+        return results
 
-        key_map = {
-            "spot": "currency_pair",
-            "futures": "contract",
-            "perp": "contract",
-        }
+    def parse_derivative_tickers(self, response: dict, infos: dict) -> dict:
+        datas = response
 
         results = {}
+        id_map = self.get_id_map(infos, "derivative")
         for data in datas:
-            instrument_id = id_map[data[key_map[market_type]]]
-            results[instrument_id] = method_map[market_type](data, exchange_info[instrument_id])
+            data = data["data"]
+            instrument_id = id_map[data["symbol"]]
+            result = self.parse_derivative_ticker(data, infos[instrument_id])
+            results[instrument_id] = result
         return results
 
+    def get_interval(self, interval: str, market: str) -> str:
+        if market == "spot":
+            if interval not in self.SPOT_INTERVAL_MAP:
+                raise ValueError(f"Invalid interval: {interval}. Must be one of {list(self.SPOT_INTERVAL_MAP.keys())}")
+            return self.SPOT_INTERVAL_MAP[interval]
+        else:
+            if interval not in self.DERIVATIVE_INTERVAL_MAP:
+                raise ValueError(
+                    f"Invalid interval: {interval}. Must be one of {list(self.DERIVATIVE_INTERVAL_MAP.keys())}"
+                )
+            return self.DERIVATIVE_INTERVAL_MAP[interval]
+
+    def parse_kucoin_timestamp(self, timestamp: int, market_type: str) -> int:
+        timestamp_str = str(timestamp)
+
+        if market_type == "spot":
+            if len(timestamp_str) == 13:
+                return int(timestamp_str[:-3])
+            elif len(timestamp_str) == 10:
+                return timestamp
+            else:
+                raise ValueError(f"Invalid timestamp: {timestamp}. Must be in seconds or milliseconds.")
+        else:
+            if len(timestamp_str) == 10:
+                return int(timestamp_str + "000")
+            elif len(timestamp_str) == 13:
+                return timestamp
+            else:
+                raise ValueError(f"Invalid timestamp: {timestamp}. Must be in seconds or milliseconds.")
+
+    def parse_ticker(self, response: dict, info: dict, market_type: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
+        if market_type == "spot":
+            return self.parse_spot_ticker(data, info)
+        else:
+            return self.parse_derivative_ticker(data, info)
+
     def parse_spot_ticker(self, response: dict, info: dict) -> dict:
+        data = response
+
+        last = self.parse_str(data["last"], float)
+        change_price = self.parse_str(data["changePrice"], float)
+        open = last - change_price
+
+        timestamp = self.parse_str(data["time"], int) if "time" in data else self.get_timestamp()
+
         return {
-            "symbol": response["currency_pair"],
-            "open_time": None,  # Not yet implemented
-            "close_time": None,  # Not yet implemented
-            "open": None,  # Not yet implemented
-            "high": float(response["high_24h"]),
-            "low": float(response["low_24h"]),
-            "last_price": float(response["last"]),
-            "base_volume": float(response["base_volume"]),
-            "quote_volume": float(response["quote_volume"]),
-            "price_change": float(response["change_utc8"]),
-            "price_change_percent": float(response["change_percentage"]) / 100,
+            "timestamp": timestamp,
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": None,
+            "close_time": timestamp,
+            "open": open,
+            "high": self.parse_str(data["high"], float),
+            "low": self.parse_str(data["low"], float),
+            "last": last,
+            "base_volume": None,  # not yet implemented
+            "quote_volume": self.parse_str(data["volValue"], float),
+            "price_change": change_price,
+            "price_change_percent": self.parse_str(data["changeRate"], float),
             "raw_data": response,
         }
 
-    def parse_futures_ticker(self, response: dict, info: dict) -> dict:
+    def parse_derivative_ticker(self, response: dict, info: dict) -> dict:
+        data = response
+
+        last = self.parse_str(data["lastTradePrice"], float)
+        change_price = self.parse_str(data["priceChg"], float)
+        open = last - change_price
+
         return {
-            "symbol": response["contract"],
-            "open_time": None,  # Not yet implemented
-            "close_time": None,  # Not yet implemented
-            "open": None,  # Not yet implemented
-            "high": float(response["high_24h"]),
-            "low": float(response["low_24h"]),
-            "last_price": float(response["last"]),
-            "base_volume": float(response["volume_24h_base"]),
-            "quote_volume": float(response["volume_24h_quote"]),
-            "price_change": None,  # Not yet implemented
-            "price_change_percent": float(response["change_percentage"]) / 100,
+            "timestamp": self.get_timestamp(),
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": None,
+            "close_time": self.get_timestamp(),
+            "open": open,
+            "high": self.parse_str(data["highPrice"], float),
+            "low": self.parse_str(data["lowPrice"], float),
+            "last": last,
+            "base_volume": self.parse_str(data["volumeOf24h"], float),
+            "quote_volume": self.parse_str(data["turnoverOf24h"], float),
+            "price_change": change_price,
+            "price_change_percent": self.parse_str(data["priceChgPct"], float),
             "raw_data": response,
         }
 
-    def parse_perp_ticker(self, response: dict, info: dict) -> dict:
+    def parse_mark_price(self, response: dict, info: dict, market_type: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
+
         return {
-            "symbol": response["contract"],
-            "open_time": None,  # Not yet implemented
-            "close_time": None,  # Not yet implemented
-            "open": None,  # Not yet implemented
-            "high": float(response["high_24h"]),
-            "low": float(response["low_24h"]),
-            "last_price": float(response["last"]),
-            "base_volume": float(response["volume_24h_base"]),
-            "quote_volume": float(response["volume_24h_quote"]),
-            "price_change": None,  # Not yet implemented
-            "price_change_percent": float(response["change_percentage"]) / 100,
-            "raw_data": response,
+            "timestamp": self.parse_str(data["timePoint"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "mark_price": self.parse_str(data["value"], float),
+            "raw_data": data,
         }
 
-    def get_market_type(self, info: str) -> str:
-        if info["is_spot"]:
-            return "spot"
-        elif info["is_futures"]:
-            return "futures"
-        elif info["is_perp"]:
-            return "perp"
-        else:
-            raise ValueError(f"Invalid market type. {info}")
+    def parse_index_price(self, response: dict, info: dict, market_type: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
+
+        return {
+            "timestamp": self.parse_str(data["timePoint"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "index_price": self.parse_str(data["indexPrice"], float),
+            "raw_data": data,
+        }
 
-    def parse_klines(self, response: dict, market_type: str, info: dict):
+    def parse_orderbook(self, response: dict, info: dict, market_type: str) -> dict:
         response = self.check_response(response)
+        data = response["data"]
+
+        return {
+            "timestamp": self.parse_str(data["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "bids": [
+                {
+                    "price": self.parse_str(bid[0], float),
+                    "volume": self.parse_str(bid[1], float),
+                    "order_number": None,
+                }
+                for bid in data["bids"]
+            ],
+            "asks": [
+                {
+                    "price": self.parse_str(ask[0], float),
+                    "volume": self.parse_str(ask[1], float),
+                    "order_number": None,
+                }
+                for ask in data["asks"]
+            ],
+            "raw_data": data,
+        }
 
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
+        response = self.check_response(response)
+        data = response["data"]
+        return {
+            "timestamp": self.parse_str(data["timePoint"], int),
+            "next_funding_time": None,
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "funding_rate": self.parse_str(data["value"], float),
+            "raw_data": data,
+        }
+
+    def parse_history_funding_rate(self, response: dict, info: dict) -> list:
+        response = self.check_response(response)
         datas = response["data"]
-        results = {}
-        for data in datas:
-            timestamp = self.parse_kline_timestamp(data, market_type)
-            results[timestamp] = self.parse_kline(data, market_type, info)
-        return results
 
-    def parse_kline_timestamp(self, response: any, market_type: str) -> int:
-        if market_type == "spot":
-            return int(response[0]) * 1000
-        else:
-            return response["t"] * 1000
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
 
-    def parse_kline(self, response: any, market_type: str, info: dict) -> dict:
-        if market_type == "spot":
-            return {
-                "open": float(response[5]),
-                "high": float(response[3]),
-                "low": float(response[4]),
-                "close": float(response[2]),
-                "base_volume": float(response[6]),
-                "quote_volume": float(response[1]),
-                "close_time": None,
-                "raw_data": response,
-            }
-        elif market_type == "futures":
-            return {
-                "open": float(response["o"]),
-                "high": float(response["h"]),
-                "low": float(response["l"]),
-                "close": float(response["c"]),
-                "base_volume": float(response["v"]),  # need to convert into base volume, currently is contract number
-                "quote_volume": None,  # not supported
-                "close_time": None,
-                "raw_data": response,
+        results = [
+            {
+                "timestamp": self.parse_str(data["timepoint"], int),
+                "instrument_id": instrument_id,
+                "market_type": market_type,
+                "funding_rate": self.parse_str(data["fundingRate"], float),
+                "realized_rate": self.parse_str(data["fundingRate"], float),
+                "raw_data": data,
             }
-        else:  # perp
-            return {
-                "open": float(response["o"]),
-                "high": float(response["h"]),
-                "low": float(response["l"]),
-                "close": float(response["c"]),
-                "base_volume": float(response["v"]),  # need to convert into base volume, currently is contract number
-                "quote_volume": float(response["sum"]),
-                "close_time": None,
-                "raw_data": response,
+            for data in datas
+        ]
+
+        return results
+
+    def parse_current_candlestick(self, response: dict, info: dict, market_type: str, interval: str) -> dict:
+        response = self.check_response(response)
+        data = response["data"][0]
+
+        result = self.parse_candlestick(data, info, market_type)
+        result.update(
+            {
+                "instrument_id": self.parse_unified_id(info),
+                "market_type": self.parse_unified_market_type(info),
+                "interval": interval,
             }
+        )
+        return result
 
-    def get_interval(self, interval: str) -> str:
-        if interval not in self.INTERVAL_MAP:
-            raise ValueError(f"Invalid interval. {interval}. Must be one of {list(self.INTERVAL_MAP.keys())}")
-        return self.INTERVAL_MAP[interval]
+    def parse_history_candlesticks(self, response: dict, info: dict, market_type: str, interval: str) -> list:
+        response = self.check_response(response)
+        datas = response["data"]
+
+        update_ = {
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "interval": interval,
+        }
+        results = []
+        for data in datas:
+
+            result = self.parse_candlestick(data, info, market_type)
+            result.update(update_)
+            results.append(result)
+
+        return results
+
+    def parse_candlestick(self, data: dict, info: dict, market_type) -> dict:
+        return {
+            "timestamp": self.parse_str(data[0], int) * (1000 if len(str(data[0])) == 10 else 1),
+            "open": self.parse_str(data[1], float),
+            "high": self.parse_str(data[3], float),
+            "low": self.parse_str(data[4], float),
+            "close": self.parse_str(data[2], float),
+            "base_volume": self.parse_str(data[5], float) if market_type == "spot" else None,
+            "quote_volume": self.parse_str(data[6 if market_type == "spot" else 5], float),
+            "contract_volume": self.parse_str(data[5], float) if market_type == "spot" else None,
+            "raw_data": data,
+        }
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/htx.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/htx.py`

 * *Files 19% similar despite different names*

```diff
@@ -51,20 +51,22 @@
         },
     }
 
     def __init__(self):
         super().__init__()
 
     def check_htx_response(self, response: dict):
-        if response["status"] != "ok":
-            return {"code": 400, "status": "error", "data": response}
-        else:
+        if response["status"] == "ok":
             for _key in self.response_keys:
                 if _key in response:
-                    return {"code": 200, "status": "success", "data": response[_key]}
+                    results = {"code": 200, "status": "success", "data": response[_key]}
+                    results.update({"timestamp": response["ts"]} if "ts" in response else {})
+                    return results
+        else:
+            raise ValueError(f"Error when parsing HTX response: {response}")
 
     @property
     def spot_exchange_info_parser(self) -> dict:
         return {
             "active": (lambda x: x["state"] == "online"),
             "is_spot": True,
             "is_margin": False,
@@ -176,16 +178,14 @@
             return {
                 "base": response["pair"].split("-")[0],
                 "quote": response["pair"].split("-")[1],
             }
 
     def parse_exchange_info(self, response: dict, parser: dict):
         response = self.check_htx_response(response)
-        if response["code"] != 200:
-            return response
 
         results = {}
         datas = response["data"]
         for data in datas:
             result = self.get_result_with_parser(data, parser)
             id = self.parse_unified_id(result)
             results[id] = result
@@ -215,16 +215,14 @@
             "next_week": "NW",
             "quarter": "CQ",
         }
         return f"{datas['symbol']}_{contract_type_map[datas['contract_type']]}"
 
     def parse_tickers(self, response: dict, exchange_infos: dict, market_type: str) -> dict:
         response = self.check_htx_response(response)
-        if response["code"] != 200:
-            return response
 
         method_map = {
             "spot": self.parse_spot_ticker,
             "linear": self.parse_linear_ticker,
             "inverse_perp": self.parse_inverse_perp_ticker,
             "inverse_futures": self.parse_inverse_futures_ticker,
         }
@@ -241,77 +239,102 @@
         results = {}
         datas = response["data"]
         for data in datas:
             if data[keys_map[market_type]] not in id_map:
                 print(f"Unmapped symbol: {data[keys_map[market_type]]} in {market_type}")
                 continue
             instrument_id = id_map[data[keys_map[market_type]]]
-            results[instrument_id] = method_map[market_type](data, exchange_infos[instrument_id])
+            params = {
+                "response": data,
+                "info": exchange_infos[instrument_id],
+            }
+            if market_type == "spot":
+                params["timestamp"] = response["timestamp"]
+            results[instrument_id] = method_map[market_type](**params)
         return results
 
-    def parse_spot_ticker(self, response: dict, info: dict):
+    def parse_ticker(self, response: dict, market_type: str, info: dict) -> dict:
+        method_map = {
+            "spot": self.parse_spot_ticker,
+            "linear": self.parse_linear_ticker,
+            "inverse_perp": self.parse_inverse_perp_ticker,
+            "inverse_futures": self.parse_inverse_futures_ticker,
+        }
+        params = {
+            "response": response,
+            "info": info,
+        }
+        if market_type == "spot":
+            params["timestamp"] = response["ts"]
+        return method_map[market_type](**params)
+
+    def parse_spot_ticker(self, response: dict, info: dict, timestamp: str):
         return {
-            "symbol": response["symbol"],
+            "timestamp": self.parse_str(timestamp, int),
+            "instrument_id": self.parse_unified_id(info),
             "open_time": None,
             "close_time": None,
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "last_price": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]),
-            "price_change": float(response["close"]) - float(response["open"]),
+            "open": self.parse_str(response["open"], float),
+            "high": self.parse_str(response["high"], float),
+            "low": self.parse_str(response["low"], float),
+            "last": self.parse_str(response["close"], float),
+            "base_volume": self.parse_str(response["amount"], float),
+            "quote_volume": self.parse_str(response["vol"], float),
+            "price_change": self.parse_str(response["close"], float) - self.parse_str(response["open"], float),
             "price_change_percent": None,
             "raw_data": response,
         }
 
     def parse_linear_ticker(self, response: dict, info: dict):
         return {
-            "symbol": response["contract_code"],
+            "timestamp": self.parse_str(response["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
             "open_time": None,
-            "close_time": int(response["ts"]),
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "last_price": float(response["close"]),
-            "base_volume": float(response["amount"]) * info["contract_size"],
-            "quote_volume": float(response["vol"]),
-            "price_change": float(response["close"]) - float(response["open"]),
+            "close_time": self.parse_str(response["ts"], int),
+            "open": self.parse_str(response["open"], float),
+            "high": self.parse_str(response["high"], float),
+            "low": self.parse_str(response["low"], float),
+            "last": self.parse_str(response["close"], float),
+            "base_volume": self.parse_str(response["amount"], float) * info["contract_size"],
+            "quote_volume": self.parse_str(response["vol"], float),
+            "price_change": self.parse_str(response["close"], float) - self.parse_str(response["open"], float),
             "price_change_percent": None,
             "raw_data": response,
         }
 
     def parse_inverse_perp_ticker(self, response: dict, info: dict):
         return {
-            "symbol": response["contract_code"],
+            "timestamp": self.parse_str(response["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
             "open_time": None,
-            "close_time": int(response["ts"]),
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "last_price": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]),
-            "price_change": float(response["close"]) - float(response["open"]),
+            "close_time": self.parse_str(response["ts"], int),
+            "open": self.parse_str(response["open"], float),
+            "high": self.parse_str(response["high"], float),
+            "low": self.parse_str(response["low"], float),
+            "last": self.parse_str(response["close"], float),
+            "base_volume": self.parse_str(response["amount"], float),
+            "quote_volume": self.parse_str(response["vol"], float),
+            "price_change": self.parse_str(response["close"], float) - self.parse_str(response["open"], float),
             "price_change_percent": None,
             "raw_data": response,
         }
 
     def parse_inverse_futures_ticker(self, response: dict, info: dict):
         return {
-            "symbol": response["symbol"],
+            "timestamp": self.parse_str(response["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
             "open_time": None,
-            "close_time": int(response["ts"]),
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "last_price": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]),
-            "price_change": float(response["close"]) - float(response["open"]),
+            "close_time": self.parse_str(response["ts"], int),
+            "open": self.parse_str(response["open"], float),
+            "high": self.parse_str(response["high"], float),
+            "low": self.parse_str(response["low"], float),
+            "last": self.parse_str(response["close"], float),
+            "base_volume": self.parse_str(response["amount"], float),
+            "quote_volume": self.parse_str(response["vol"], float),
+            "price_change": self.parse_str(response["close"], float) - self.parse_str(response["open"], float),
             "price_change_percent": None,
             "raw_data": response,
         }
 
     def get_market_type(self, info: dict) -> str:
         if info["is_spot"]:
             return "spot"
@@ -320,68 +343,122 @@
         elif info["is_inverse"] and info["is_futures"]:
             return "inverse_futures"
         elif info["is_inverse"] and info["is_perp"]:
             return "inverse_perp"
         else:
             raise ValueError("Unknown market type")
 
-    def parse_klines(self, response: dict, market_type: str, info: dict) -> dict:
+    def get_interval(self, interval: str, market_type: str) -> str:
+        if interval not in self.INTERVAL_MAP[market_type]:
+            raise ValueError(
+                f"Invalid interval: {interval} in {market_type}, must be one of {list(self.INTERVAL_MAP[market_type])}"
+            )
+        return self.INTERVAL_MAP[market_type][interval]
+
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
         response = self.check_htx_response(response)
-        if response["code"] != 200:
-            return response
+        data = response["data"]
+        return {
+            "timestamp": response["timestamp"],
+            "next_funding_time": self.parse_str(data["funding_time"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "funding_rate": self.parse_str(data["funding_rate"], float),
+            "raw_data": data,
+        }
 
-        method_map = {
-            "spot": self.parse_spot_and_linear_kline,
-            "linear": self.parse_spot_and_linear_kline,
-            "inverse_perp": self.parse_inverse_perp_kline,
-            "inverse_futures": self.parse_inverse_futures_kline,
+    def parse_history_funding_rate(self, response: dict, info: dict) -> list:
+        response = self.check_htx_response(response)
+        datas = response["data"]["data"]
+
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
+
+        return [
+            {
+                "timestamp": self.parse_str(data["funding_time"], int),
+                "instrument_id": instrument_id,
+                "market_type": market_type,
+                "funding_rate": self.parse_str(data["funding_rate"], float),
+                "realized_rate": self.parse_str(data["realized_rate"], float),
+                "raw_data": data,
+            }
+            for data in datas
+        ]
+
+    def parse_candlesticks(self, response: dict, info: dict, market_type: str, interval: str) -> any:
+        """
+        - spot :
+        [
+            {
+                'id': 1713110400,
+                'open': 64186.51,
+                'close': 66184.98,
+                'low': 62578.94,
+                'high': 66566.0,
+                'amount': 1187.8846778540208,
+                'vol': 77002399.88436274,
+                'count': 86506
+            }
+        ]
+
+        - linear :
+        {
+            "amount":0.004
+            "close":13076.8
+            "count":1
+            "high":13076.8
+            "id":1603695060
+            "low":13076.8
+            "open":13076.8
+            "trade_turnover":52.3072
+            "vol":4
+        }
+
+        - inverse:
+        {
+            "id":1628652420
+            "open":45875.02
+            "close":45851
+            "low":45850.93
+            "high":45880.01
+            "amount":2.6471133153472475
+            "vol":1214
+            "count":50
         }
 
-        results = {}
+        """
+
+        response = self.check_htx_response(response)
         datas = response["data"]
-        for data in datas:
-            timestamp = int(int(data["id"]) * 1000)
-            results[timestamp] = method_map[market_type](data, info=info)
-        return results
 
-    def parse_spot_and_linear_kline(self, response: dict, info: dict) -> dict:
-        return {
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "close": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]),
-            "close_time": None,
-            "raw_data": response,
+        update_ = {
+            "instrument_id": self.parse_unified_id(info),
+            "market_type": self.parse_unified_market_type(info),
+            "interval": interval,
         }
 
-    def parse_inverse_perp_kline(self, response: dict, info: dict) -> dict:
-        return {
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "close": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]) * info["contract_size"],
-            "close_time": None,
-            "raw_data": response,
-        }
+        results = []
 
-    def parse_inverse_futures_kline(self, response: dict, info: dict) -> dict:
-        return {
-            "open": float(response["open"]),
-            "high": float(response["high"]),
-            "low": float(response["low"]),
-            "close": float(response["close"]),
-            "base_volume": float(response["amount"]),
-            "quote_volume": float(response["vol"]) * info["contract_size"],
-            "close_time": None,
-            "raw_data": response,
+        for data in datas:
+            result = self.parse_candlestick(data, info, market_type)
+            result.update(update_)
+            results.append(result)
+
+        return results if len(results) > 1 else results[0]
+
+    def parse_candlestick(self, data: dict, info: dict, market_type: str) -> dict:
+
+        return {
+            "timestamp": self.parse_str(data["id"], int) * 1000,
+            "open": self.parse_str(data["open"], float),
+            "high": self.parse_str(data["high"], float),
+            "low": self.parse_str(data["low"], float),
+            "close": self.parse_str(data["close"], float),
+            "base_volume": self.parse_str(data["amount"], float),
+            "quote_volume": (
+                self.parse_str(data["vol" if market_type != "linear" else "trade_turnover"], float)
+                * (1 if info["is_linear"] else info["contract_size"])
+            ),
+            "contract_volume": self.parse_str(data["amount" if market_type == "spot" else "vol"], float),
+            "raw_data": data,
         }
-
-    def get_interval(self, interval: str, market_type: str) -> str:
-        if interval not in self.INTERVAL_MAP[market_type]:
-            raise ValueError(
-                f"Invalid interval: {interval} in {market_type}, must be one of {list(self.INTERVAL_MAP[market_type])}"
-            )
-        return self.INTERVAL_MAP[market_type][interval]
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/okx.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/okx.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from datetime import timedelta as td
-
 from .base import Parser
 
 
 class OkxParser(Parser):
     interval_map = {
         "1m": "1m",
         "3m": "3m",
@@ -130,33 +128,34 @@
 
                 if spot["tick_size"] != margin["tick_size"]:
                     print(f"tick_size of {instrument_id} is different between spot and margin")
 
                 spots[instrument_id] = spot
         return spots
 
-    def parse_ticker(self, response: any, market_type: str) -> dict:
+    def parse_ticker(self, response: any, market_type: str, info: dict) -> dict:
         if "data" in response:
             response = response["data"][0]
 
         if market_type == "spot":
             base_volume = float(response["vol24h"])
             quote_volume = float(response["volCcy24h"])
         else:
             base_volume = float(response["volCcy24h"])
             quote_volume = float(response["volCcy24h"]) * (float(response["last"]) + float(response["open24h"])) / 2
 
         return {
-            "symbol": response["instId"],
-            "open_time": self.adjust_timestamp(int(response["ts"]), td(days=-1)),
-            "close_time": int(response["ts"]),
-            "open": float(response["open24h"]),
-            "high": float(response["high24h"]),
-            "low": float(response["low24h"]),
-            "last_price": float(response["last"]),
+            "timestamp": self.parse_str(response["ts"], int),
+            "instrument_id": self.parse_unified_id(info),
+            "open_time": None,
+            "close_time": self.parse_str(response["ts"], int),
+            "open": self.parse_str(response["open24h"], float),
+            "high": self.parse_str(response["high24h"], float),
+            "low": self.parse_str(response["low24h"], float),
+            "last": self.parse_str(response["last"], float),
             "base_volume": base_volume,
             "quote_volume": quote_volume,
             "price_change": None,
             "price_change_percent": None,
             "raw_data": response,
         }
 
@@ -169,69 +168,45 @@
         response = self.check_response(response)
         datas = response["data"]
 
         id_map = self.get_id_map(infos, market_type)
         results = {}
         for data in datas:
             instrument_id = id_map[data["instId"]]
-            results[instrument_id] = self.parse_ticker(data, market_type)
-        return results
-
-    @staticmethod
-    def parse_kline(response: dict, market_type: str) -> dict:
-        return {
-            "open": float(response[1]),
-            "high": float(response[2]),
-            "low": float(response[3]),
-            "close": float(response[4]),
-            "base_volume": float(response[6] if market_type != "spot" else response[5]),
-            "quote_volume": float(response[7]),
-            "raw_data": response,
-        }
-
-    def parse_klines(self, response: dict, market_type: str) -> dict:
-        response = self.check_response(response)
-
-        datas = response["data"]
-        results = {}
-        for data in datas:
-            result = self.parse_kline(data, market_type)
-            timestamp = int(data[0])
-            results[timestamp] = result
+            info = infos[instrument_id]
+            results[instrument_id] = self.parse_ticker(data, market_type, info)
         return results
 
     def parse_funding_rates(self, response: dict, info: dict) -> list:
         response = self.check_response(response)
         datas = response["data"]
 
         results = []
         for data in datas:
             results.append(
                 {
-                    "timestamp": int(data["fundingTime"]),
+                    "timestamp": self.parse_str(data["fundingTime"], int),
                     "instrument_id": self.parse_unified_id(info),
-                    "market": self._market_type_map[data["instType"]],
-                    "funding_rate": float(data["fundingRate"]),
-                    "realized_rate": float(data["realizedRate"]),
+                    "market_type": self.parse_unified_market_type(info),
+                    "funding_rate": self.parse_str(data["fundingRate"], float),
+                    "realized_rate": self.parse_str(data["realizedRate"], float),
                     "raw_data": data,
                 }
             )
         return results
 
-    def parse_current_funding_rate(self, resposne: dict, info: dict) -> dict:
-        response = self.check_response(resposne)
+    def parse_current_funding_rate(self, response: dict, info: dict) -> dict:
+        response = self.check_response(response)
         data = response["data"][0]
         return {
-            "timestamp": int(data["ts"]),
+            "timestamp": self.parse_str(data["ts"], int),
+            "next_funding_time": self.parse_str(data["nextFundingTime"], int),
             "instrument_id": self.parse_unified_id(info),
-            "market": self._market_type_map[data["instType"]],
-            "funding_time": int(data["fundingTime"]),
-            "funding_rate": float(data["fundingRate"]),
-            "next_funding_time": int(data["nextFundingTime"]),
-            "next_funding_rate": float(data["nextFundingRate"]) if data["nextFundingRate"] else None,
+            "market_type": self._market_type_map[data["instType"]],
+            "funding_rate": self.parse_str(data["fundingRate"], float),
             "raw_data": data,
         }
 
     def parse_balance(self, response: dict) -> dict:
         response = self.check_response(response)
 
         datas = response["data"][0]["details"]
@@ -265,14 +240,16 @@
             "main_account_id": data["mainUid"],
             "key_name": data["label"],
             "permission": data["perm"].split(","),
             "raw_data": data,
         }
 
     def get_interval(self, interval: str) -> str:
+        if interval not in self.interval_map:
+            raise ValueError(f"{interval} is not supported. Must be one of {list(self.interval_map.keys())}")
         return self.interval_map[interval]
 
     def parse_order_id(self, response: dict) -> str:
         response = self.check_response(response)
         data = response["data"][0]
         return str(data["ordId"])
 
@@ -428,7 +405,43 @@
                     "volume": self.parse_str(bid[1], float),
                     "order_number": self.parse_str(bid[3], int),
                 }
                 for bid in bids
             ],
             "raw_data": datas,
         }
+
+    def parse_candlesticks(self, response: dict, info: dict, interval: str) -> any:
+        def parse_volumes(data: list, market_type: str) -> dict:
+            return {
+                "base_volume": self.parse_str(data[5 if market_type == "spot" else 6], float),
+                "quote_volume": self.parse_str(data[7], float),
+                "contract_volume": self.parse_str(data[5], float),
+            }
+
+        response = self.check_response(response)
+        datas = response["data"]
+
+        instrument_id = self.parse_unified_id(info)
+        market_type = self.parse_unified_market_type(info)
+
+        results = []
+        for data in datas:
+            volumes = parse_volumes(data, market_type)
+            results.append(
+                {
+                    "timestamp": self.parse_str(data[0], int),
+                    "instrument_id": instrument_id,
+                    "market_type": market_type,
+                    "interval": interval,
+                    "open": self.parse_str(data[1], float),
+                    "high": self.parse_str(data[2], float),
+                    "low": self.parse_str(data[3], float),
+                    "close": self.parse_str(data[4], float),
+                    "base_volume": volumes["base_volume"],
+                    "quote_volume": volumes["quote_volume"],
+                    "contract_volume": volumes["contract_volume"],
+                    "raw_data": data,
+                }
+            )
+
+        return results if len(results) > 1 else results[0]
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors/parsers/woo.py` & `cex-adaptors-1.0.5/cex_adaptors/parsers/woo.py`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.4/cex_adaptors/utils.py` & `cex-adaptors-1.0.5/cex_adaptors/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -32,21 +32,7 @@
     if not query:
         return dictionary
 
     new_dict = {outer: inner[key] for outer, inner in dictionary.items() if key in inner}
 
     queried_dict = query_dict(new_dict, query)
     return {key: dictionary[key] for key in queried_dict.keys()}
-
-
-def sort_dict(dictionary: dict, ascending: bool = True, num: int = None) -> dict:
-    """
-    Sort a dictionary by its values
-    :param dictionary: dictionary to sort
-    :param ascending: ascending or descending
-    :param num: number of items to return
-    :return: sorted dictionary
-    """
-    df = pd.DataFrame(dictionary).T.reset_index().sort_values(by="index", ascending=ascending).set_index("index")
-    if num:
-        df = df.iloc[-num:]
-    return df.to_dict(orient="index")
```

### Comparing `cex-adaptors-1.0.4/cex_adaptors.egg-info/SOURCES.txt` & `cex-adaptors-1.0.5/cex_adaptors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cex-adaptors-1.0.4/pyproject.toml` & `cex-adaptors-1.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 profile = "black"
 # cuctom section
 sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "LOCALFOLDER"]
 known_third_party = []
 known_local_folder = []
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.10"
 warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
```

