# Comparing `tmp/fennel_invest_api-1.0.0.tar.gz` & `tmp/fennel_invest_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fennel_invest_api-1.0.0.tar", last modified: Wed Apr 10 19:15:44 2024, max compression
+gzip compressed data, was "fennel_invest_api-1.0.1.tar", last modified: Tue Apr 16 19:56:41 2024, max compression
```

## Comparing `fennel_invest_api-1.0.0.tar` & `fennel_invest_api-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:44.101162 fennel_invest_api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 19:15:44.101162 fennel_invest_api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-10 19:15:35.000000 fennel_invest_api-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:44.101162 fennel_invest_api-1.0.0/fennel_invest_api/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 19:15:35.000000 fennel_invest_api-1.0.0/fennel_invest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-10 19:15:35.000000 fennel_invest_api-1.0.0/fennel_invest_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-10 19:15:35.000000 fennel_invest_api-1.0.0/fennel_invest_api/fennel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:15:44.101162 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 19:15:44.000000 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-10 19:15:44.000000 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:15:44.000000 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 19:15:44.000000 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 19:15:44.000000 fennel_invest_api-1.0.0/fennel_invest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:15:44.101162 fennel_invest_api-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-10 19:15:35.000000 fennel_invest_api-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.298024 fennel_invest_api-1.0.1/fennel_invest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/fennel_invest_api/fennel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 19:56:41.000000 fennel_invest_api-1.0.1/fennel_invest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:56:41.302024 fennel_invest_api-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-16 19:56:37.000000 fennel_invest_api-1.0.1/setup.py
```

### Comparing `fennel_invest_api-1.0.0/PKG-INFO` & `fennel_invest_api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

### Comparing `fennel_invest_api-1.0.0/README.md` & `fennel_invest_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fennel_invest_api-1.0.0/fennel_invest_api/endpoints.py` & `fennel_invest_api-1.0.1/fennel_invest_api/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 import json
 
 
 class Endpoints:
     def __init__(self):
         self.accounts = "https://accounts.fennel.com"
         self.graphql = "https://fennel-api.prod.fennel.com/graphql/"
-    
+
     def retrieve_bearer_url(self):
         return f"{self.accounts}/passwordless/start"
 
     def oauth_url(self):
         return f"{self.accounts}/oauth/token"
 
-    def build_graphql_payload(self, query, variables={}):
-        return {
-            "operationName": None,
-            "variables": variables,
-            "query": query
-        }
+    @staticmethod
+    def build_graphql_payload(query, variables=None):
+        if variables is None:
+            variables = {}
+        return {"operationName": None, "variables": variables, "query": query}
 
     def portfolio_query(self):
         query = """
             query GetPortfolioSummary {
                 portfolio {
                     cash {
                         balance {
@@ -37,15 +36,15 @@
                         currency
                     }
                     totalEquityValue
                 }
             }
         """
         return json.dumps(self.build_graphql_payload(query))
-    
+
     def stock_holdings_query(self):
         query = """
             query MinimumPortfolioData {
                 portfolio {
                     totalEquityValue
                     bulbs {
                         isin
@@ -82,18 +81,15 @@
                 searchSearch {
                     searchSecurities(query: $query, count: $count) {
                         isin
                     }
                 }
             }
         """
-        variables = {
-            "query": symbol,
-            "count": count
-        }
+        variables = {"query": symbol, "count": count}
         return json.dumps(self.build_graphql_payload(query, variables))
 
     def stock_order_query(self, symbol, quantity, isin, side, priceRule):
         query = """
             mutation CreateOrder($order_details: OrderDetailsInput__!){
                 orderCreateOrder(order: $order_details)
             }
@@ -107,21 +103,20 @@
                 "priceRule": priceRule,
                 "timeInForce": "day",
                 "routingOption": "exchange_ats_sdp",
             }
         }
         return json.dumps(self.build_graphql_payload(query, variables))
 
-
     @staticmethod
     def build_headers(Bearer, graphql=True):
         headers = {
-            'accept': '*/*',
-            'accept-encoding': 'gzip',
-            'authorization': f"Bearer {Bearer}",
-            'content-type': 'application/json',
-            'host': 'fennel-api.prod.fennel.com',
-            'user-agent': 'Dart/3.3 (dart:io)',
+            "accept": "*/*",
+            "accept-encoding": "gzip",
+            "authorization": f"Bearer {Bearer}",
+            "content-type": "application/json",
+            "host": "fennel-api.prod.fennel.com",
+            "user-agent": "Dart/3.3 (dart:io)",
         }
         if not graphql:
-            headers['host'] = 'accounts.fennel.com'
+            headers["host"] = "accounts.fennel.com"
         return headers
```

### Comparing `fennel_invest_api-1.0.0/fennel_invest_api/fennel.py` & `fennel_invest_api-1.0.1/fennel_invest_api/fennel.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,81 +7,92 @@
 
 
 def check_login(func):
     def wrapper(self, *args, **kwargs):
         if self.Bearer is None:
             raise Exception("Bearer token is not set. Please login first.")
         return func(self, *args, **kwargs)
+
     return wrapper
 
 
 class Fennel:
     def __init__(self, filename="fennel_credentials.pkl", path=None) -> None:
         self.session = requests.Session()
         self.endpoints = Endpoints()
         self.Bearer = None
         self.Refresh = None
         self.ID_Token = None
         self.timeout = 10
-        self.account_number = "00000000" # Fennel only has 1 account which they don't share
+        self.account_number = (
+            "00000000"  # Fennel only has 1 account which they don't share
+        )
         self.client_id = "FXGlhcVdamwozAFp8BZ2MWl6coPl6agX"
         self.filename = filename
         self.path = None
         if path is not None:
             self.path = path
         self._load_credentials()
 
-    def _verify_filepath(self):
+    def _load_credentials(self):
+        filename = self.filename
         if self.path is not None:
-            self.filename = os.path.join(self.path, self.filename)
-            if not os.path.exists(self.filename):
+            filename = os.path.join(self.path, filename)
+            if not os.path.exists(self.path):
                 os.makedirs(self.path)
-        
-    def _load_credentials(self):
-        self._verify_filepath()
-        if os.path.exists(self.filename):
-            with open(self.filename, "rb") as f:
+        if os.path.exists(filename):
+            with open(filename, "rb") as f:
                 credentials = pickle.load(f)
             self.Bearer = credentials.get("Bearer")
             self.Refresh = credentials.get("Refresh")
             self.ID_Token = credentials.get("ID_Token")
             self.client_id = credentials.get("client_id", self.client_id)
-        
+
     def _save_credentials(self):
-        self._verify_filepath()
-        with open(self.filename, "wb") as f:
-            pickle.dump({
-                "Bearer": self.Bearer,
-                "Refresh": self.Refresh,
-                "ID_Token": self.ID_Token,
-                "client_id": self.client_id
-            }, f)
+        filename = self.filename
+        if self.path is not None:
+            filename = os.path.join(self.path, filename)
+            if not os.path.exists(self.path):
+                os.makedirs(self.path)
+        with open(filename, "wb") as f:
+            pickle.dump(
+                {
+                    "Bearer": self.Bearer,
+                    "Refresh": self.Refresh,
+                    "ID_Token": self.ID_Token,
+                    "client_id": self.client_id,
+                },
+                f,
+            )
 
     def _clear_credentials(self):
-        self._verify_filepath()
-        if os.path.exists(self.filename):
-            os.remove(self.filename)
+        filename = self.filename
+        if self.path is not None:
+            filename = os.path.join(self.path, filename)
+            if not os.path.exists(self.path):
+                os.makedirs(self.path)
+        if os.path.exists(filename):
+            os.remove(filename)
         self.Bearer = None
         self.Refresh = None
         self.ID_Token = None
 
     def login(self, email, wait_for_code=True, code=None):
         # If creds exist, then see if they are valid
         if self.Bearer is not None:
             if self._verify_login():
                 return True
-            else:
-                self._clear_credentials()
+            self._clear_credentials()
         if code is None:
             url = self.endpoints.retrieve_bearer_url()
             payload = {
                 "email": email,
                 "client_id": self.client_id,
                 "connection": "email",
-                "send": "code"
+                "send": "code",
             }
             response = self.session.post(url, json=payload)
             if response.status_code != 200:
                 raise Exception(f"Failed to start passwordless login: {response.text}")
             if not wait_for_code:
                 raise Exception("2FA required. Please provide the code.")
             print("2FA code sent to email")
@@ -90,100 +101,119 @@
         payload = {
             "grant_type": "http://auth0.com/oauth/grant-type/passwordless/otp",
             "client_id": self.client_id,
             "otp": code,
             "username": email,
             "scope": "openid profile offline_access email",
             "audience": "https://meta.api.fennel.com/graphql",
-            "realm": "email"
+            "realm": "email",
         }
         response = self.session.post(url, json=payload)
         if response.status_code != 200:
             raise Exception(f"Failed to login: {response.text}")
         response = response.json()
-        self.Bearer = response['access_token']
-        self.Refresh = response['refresh_token']
-        self.ID_Token = response['id_token']
-        # refresh_token() # Refresh token after login?
+        self.Bearer = response["access_token"]
+        self.Refresh = response["refresh_token"]
+        self.ID_Token = response["id_token"]
         self._save_credentials()
         return True
 
     def refresh_token(self):
         url = self.endpoints.oauth_url()
         payload = {
             "grant_type": "refresh_token",
             "client_id": self.client_id,
             "refresh_token": self.Refresh,
-            "scope": "openid profile offline_access email"
+            "scope": "openid profile offline_access email",
         }
         response = self.session.post(url, json=payload)
         if response.status_code != 200:
             raise Exception(f"Failed to refresh bearer token: {response.text}")
         response = response.json()
         self.Bearer = f"{response['access_token']}"
-        self.Refresh = response['refresh_token']
-        self.ID_Token = response['id_token']
+        self.Refresh = response["refresh_token"]
+        self.ID_Token = response["id_token"]
         return response
 
     def _verify_login(self):
         # Test login by getting portfolio summary
         try:
             self.get_portfolio_summary()
             return True
-        except Exception as e:
+        except Exception:
             self.refresh_token()
             try:
                 self.get_portfolio_summary()
                 return True
-            except Exception as e:
+            except Exception:
                 return False
 
     @check_login
     def get_portfolio_summary(self):
         query = self.endpoints.portfolio_query()
         headers = self.endpoints.build_headers(self.Bearer)
-        response = self.session.post(self.endpoints.graphql, headers=headers, data=query)
+        response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
         if response.status_code != 200:
-            raise Exception(f"Portfolio Request failed with status code {response.status_code}: {response.text}")
+            raise Exception(
+                f"Portfolio Request failed with status code {response.status_code}: {response.text}"
+            )
         return response.json()
-    
+
     @check_login
     def get_stock_holdings(self):
         query = self.endpoints.stock_holdings_query()
         headers = self.endpoints.build_headers(self.Bearer)
-        response = self.session.post(self.endpoints.graphql, headers=headers, data=query)
+        response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
         if response.status_code != 200:
-            raise Exception(f"Stock Holdings Request failed with status code {response.status_code}: {response.text}")
+            raise Exception(
+                f"Stock Holdings Request failed with status code {response.status_code}: {response.text}"
+            )
         response = response.json()
-        return response['data']['portfolio']['bulbs']
+        return response["data"]["portfolio"]["bulbs"]
 
     @check_login
     def is_market_open(self):
         query = self.endpoints.is_market_open_query()
         headers = self.endpoints.build_headers(self.Bearer)
-        response = self.session.post(self.endpoints.graphql, headers=headers, data=query)
+        response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
         if response.status_code != 200:
-            raise Exception(f"Market Open Request failed with status code {response.status_code}: {response.text}")
+            raise Exception(
+                f"Market Open Request failed with status code {response.status_code}: {response.text}"
+            )
         response = response.json()
-        return response['data']['securityMarketInfo']['isOpen']
+        return response["data"]["securityMarketInfo"]["isOpen"]
 
     @check_login
     def place_order(self, ticker, quantity, side, price="market"):
         if side.lower() not in ["buy", "sell"]:
             raise Exception("Side must be either 'buy' or 'sell'")
         # Check if market is open
         if not self.is_market_open():
             raise Exception("Market is closed. Cannot place order.")
         # Search for stock "isin"
         query = self.endpoints.stock_search_query(ticker)
         headers = self.endpoints.build_headers(self.Bearer)
-        search_response = self.session.post(self.endpoints.graphql, headers=headers, data=query)
+        search_response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
         if search_response.status_code != 200:
-            raise Exception(f"Stock Search Request failed with status code {search_response.status_code}: {search_response.text}")
+            raise Exception(
+                f"Stock Search Request failed with status code {search_response.status_code}: {search_response.text}"
+            )
         search_response = search_response.json()
-        isin = search_response['data']['searchSearch']['searchSecurities'][0]['isin']
+        isin = search_response["data"]["searchSearch"]["searchSecurities"][0]["isin"]
         # Place order
         query = self.endpoints.stock_order_query(ticker, quantity, isin, side, price)
-        order_response = self.session.post(self.endpoints.graphql, headers=headers, data=query)
+        order_response = self.session.post(
+            self.endpoints.graphql, headers=headers, data=query
+        )
         if order_response.status_code != 200:
-            raise Exception(f"Order Request failed with status code {order_response.status_code}: {order_response.text}")
-        return order_response.json()
+            raise Exception(
+                f"Order Request failed with status code {order_response.status_code}: {order_response.text}"
+            )
+        return order_response.json()
```

### Comparing `fennel_invest_api-1.0.0/fennel_invest_api.egg-info/PKG-INFO` & `fennel_invest_api-1.0.1/fennel_invest_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fennel_invest_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial Fennel.com Invest API written in Python Requests
 Home-page: https://github.com/NelsonDane/fennel-invest-api
 Author: Nelson Dane
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: python-dotenv
```

