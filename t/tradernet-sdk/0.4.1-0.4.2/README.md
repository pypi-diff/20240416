# Comparing `tmp/tradernet_sdk-0.4.1.tar.gz` & `tmp/tradernet_sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_sdk-0.4.1.tar", max compression
+gzip compressed data, was "tradernet_sdk-0.4.2.tar", max compression
```

## Comparing `tradernet_sdk-0.4.1.tar` & `tradernet_sdk-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1178 2024-03-08 12:26:04.858908 tradernet_sdk-0.4.1/LICENSE
--rw-r--r--   0        0        0     4066 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/README.md
--rw-r--r--   0        0        0     1031 2024-03-08 13:12:14.425063 tradernet_sdk-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1296 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/PublicApiClient.py
--rw-r--r--   0        0        0      583 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/__init__.py
--rw-r--r--   0        0        0    34159 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/client.py
--rw-r--r--   0        0        0      212 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/common/__init__.py
--rw-r--r--   0        0        0     2222 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/common/netutils.py
--rw-r--r--   0        0        0     7361 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/common/string_utils.py
--rw-r--r--   0        0        0     3249 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/common/ws_utils.py
--rw-r--r--   0        0        0    12198 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/core.py
--rw-r--r--   0        0        0        0 2024-03-08 13:11:40.976843 tradernet_sdk-0.4.1/tradernet/py.typed
--rw-r--r--   0        0        0        0 2024-03-08 13:11:40.976843 tradernet_sdk-0.4.1/tradernet/symbols/__init__.py
--rw-r--r--   0        0        0     5295 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/base_market_symbol.py
--rw-r--r--   0        0        0     4134 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/base_option_symbol.py
--rw-r--r--   0        0        0     2488 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/das_option.py
--rw-r--r--   0        0        0      290 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/option_properties.py
--rw-r--r--   0        0        0     1515 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/tradernet_option.py
--rw-r--r--   0        0        0     1838 2024-03-08 12:24:39.786352 tradernet_sdk-0.4.1/tradernet/symbols/tradernet_symbol.py
--rw-r--r--   0        0        0     2998 2024-03-08 12:24:39.790352 tradernet_sdk-0.4.1/tradernet/tradernet_wsapi.py
--rw-r--r--   0        0        0     8234 2024-03-08 12:24:39.790352 tradernet_sdk-0.4.1/tradernet/trading.py
--rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 tradernet_sdk-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1178 2024-04-16 14:08:11.956390 tradernet_sdk-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4066 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/README.md
+-rw-r--r--   0        0        0     1031 2024-04-16 14:21:28.797634 tradernet_sdk-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1296 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/PublicApiClient.py
+-rw-r--r--   0        0        0      583 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/__init__.py
+-rw-r--r--   0        0        0    34159 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/client.py
+-rw-r--r--   0        0        0      212 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/common/__init__.py
+-rw-r--r--   0        0        0     2222 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/common/netutils.py
+-rw-r--r--   0        0        0     7361 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/common/string_utils.py
+-rw-r--r--   0        0        0     3249 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/common/ws_utils.py
+-rw-r--r--   0        0        0    12198 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/core.py
+-rw-r--r--   0        0        0        0 2024-04-16 14:20:51.961392 tradernet_sdk-0.4.2/tradernet/py.typed
+-rw-r--r--   0        0        0        0 2024-04-16 14:20:51.961392 tradernet_sdk-0.4.2/tradernet/symbols/__init__.py
+-rw-r--r--   0        0        0     5295 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/base_market_symbol.py
+-rw-r--r--   0        0        0     4134 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/base_option_symbol.py
+-rw-r--r--   0        0        0     2488 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/das_option.py
+-rw-r--r--   0        0        0      290 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/option_properties.py
+-rw-r--r--   0        0        0     1515 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/tradernet_option.py
+-rw-r--r--   0        0        0     1838 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/symbols/tradernet_symbol.py
+-rw-r--r--   0        0        0     2998 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/tradernet_wsapi.py
+-rw-r--r--   0        0        0     8648 2024-04-16 14:08:11.960389 tradernet_sdk-0.4.2/tradernet/trading.py
+-rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 tradernet_sdk-0.4.2/PKG-INFO
```

### Comparing `tradernet_sdk-0.4.1/LICENSE` & `tradernet_sdk-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/README.md` & `tradernet_sdk-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/pyproject.toml` & `tradernet_sdk-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tradernet-sdk"
-version = "0.4.1"
+version = "0.4.2"
 description = "Public API for TraderNet"
 authors = ["Anton Kudelin <a.kudelin@freedomfinance.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://tradernet.ru/tradernet-api/python-sdk"
 packages = [
     {include = "tradernet"}
```

### Comparing `tradernet_sdk-0.4.1/tradernet/PublicApiClient.py` & `tradernet_sdk-0.4.2/tradernet/PublicApiClient.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/__init__.py` & `tradernet_sdk-0.4.2/tradernet/__init__.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/client.py` & `tradernet_sdk-0.4.2/tradernet/client.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/common/netutils.py` & `tradernet_sdk-0.4.2/tradernet/common/netutils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/common/string_utils.py` & `tradernet_sdk-0.4.2/tradernet/common/string_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/common/ws_utils.py` & `tradernet_sdk-0.4.2/tradernet/common/ws_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/core.py` & `tradernet_sdk-0.4.2/tradernet/core.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/symbols/base_market_symbol.py` & `tradernet_sdk-0.4.2/tradernet/symbols/base_market_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/symbols/base_option_symbol.py` & `tradernet_sdk-0.4.2/tradernet/symbols/base_option_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/symbols/das_option.py` & `tradernet_sdk-0.4.2/tradernet/symbols/das_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/symbols/tradernet_option.py` & `tradernet_sdk-0.4.2/tradernet/symbols/tradernet_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/symbols/tradernet_symbol.py` & `tradernet_sdk-0.4.2/tradernet/symbols/tradernet_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/tradernet_wsapi.py` & `tradernet_sdk-0.4.2/tradernet/tradernet_wsapi.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.4.1/tradernet/trading.py` & `tradernet_sdk-0.4.2/tradernet/trading.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
     def buy(
         self,
         symbol: str,
         quantity: int = 1,
         price: float = 0.0,
         duration: str = 'day',
-        use_margin: bool = True
+        use_margin: bool = True,
+        custom_order_id: int | None = None
     ) -> dict[str, Any]:
         """
         Placing a new buy order.
 
         Parameters
         ----------
         symbol : str
@@ -51,36 +52,41 @@
             Units of the symbol, by default 1.
         price : float, optional
             Limit price, by default 0.0 that means market order.
         duration : str, optional
             Time to order expiration, by default 'day'.
         use_margin : bool, optional
             If margin credit might be used, by default True.
+        custom_order_id : int, optional
+            Custom order ID, by default None meaning that it will be generated
+            by Tradernet.
 
         Returns
         -------
         dict[str, Any]
             Order information.
         """
         return self.__trade(
             'buy',
             symbol,
             quantity,
             price,
             duration,
-            use_margin
+            use_margin,
+            custom_order_id
         )
 
     def sell(
         self,
         symbol: str,
         quantity: int = 1,
         price: float = 0.0,
         duration: str = 'day',
-        use_margin: bool = True
+        use_margin: bool = True,
+        custom_order_id: int | None = None
     ) -> dict[str, Any]:
         """
         Placing a new sell order.
 
         Parameters
         ----------
         symbol : str
@@ -96,15 +102,16 @@
         """
         return self.__trade(
             'sell',
             symbol,
             quantity,
             price,
             duration,
-            use_margin
+            use_margin,
+            custom_order_id
         )
 
     def stop(self, symbol: str, price: float) -> dict[str, Any]:
         """
         Placing a new stop order on a certain open position.
 
         Parameters
@@ -254,29 +261,31 @@
     def __trade(
         self,
         direction: str,
         symbol: str,
         quantity: int = 1,
         price: float = 0.0,
         duration: str = 'day',
-        use_margin: bool = True
+        use_margin: bool = True,
+        custom_order_id: int | None = None
     ) -> dict[str, Any]:
         duration = duration.lower()
 
         # IOC emulation is much slower than the real IOC, because emulation
         # requires two sent and two received FIX messages instead of only one
         # pair, so total execution time is about 0.5 sec.
         if duration == 'ioc':
             order = self.__trade(
                 direction,
                 symbol,
                 quantity,
                 price,
                 'day',
-                use_margin
+                use_margin,
+                custom_order_id
             )
             if 'order_id' in order:
                 self.cancel(order['order_id'])
             return order
 
         if duration not in self.DURATION:
             raise ValueError(f'Unknown duration {duration}')
@@ -294,11 +303,12 @@
         cmd = 'putTradeOrder'
         params = {
             'instr_name': symbol,
             'action_id': action_id,
             'order_type_id': 2 if price else 1,
             'qty': quantity,
             'limit_price': price,
-            'expiration_id': self.DURATION[duration]
+            'expiration_id': self.DURATION[duration],
+            'user_order_id': custom_order_id
         }
 
         return self.authorized_request(cmd, params, version=2)
```

### Comparing `tradernet_sdk-0.4.1/PKG-INFO` & `tradernet_sdk-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradernet-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: Public API for TraderNet
 Home-page: https://tradernet.ru/tradernet-api/python-sdk
 License: MIT
 Author: Anton Kudelin
 Author-email: a.kudelin@freedomfinance.eu
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

