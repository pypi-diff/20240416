# Comparing `tmp/pytonconnect-0.3.0.tar.gz` & `tmp/pytonconnect-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytonconnect-0.3.0.tar", last modified: Mon Nov  6 01:18:11 2023, max compression
+gzip compressed data, was "pytonconnect-0.3.1.tar", last modified: Tue Apr 16 18:59:22 2024, max compression
```

## Comparing `pytonconnect-0.3.0.tar` & `pytonconnect-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.487013 pytonconnect-0.3.0/
--rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     4789 2023-11-06 01:18:11.487013 pytonconnect-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3740 2023-11-06 01:12:57.000000 pytonconnect-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.466949 pytonconnect-0.3.0/pytonconnect/
--rw-rw-rw-   0        0        0      181 2023-04-25 09:15:01.000000 pytonconnect-0.3.0/pytonconnect/__init__.py
--rw-rw-rw-   0        0        0     9924 2023-05-31 14:57:30.000000 pytonconnect-0.3.0/pytonconnect/_ton_connect.py
--rw-rw-rw-   0        0        0     5260 2023-11-06 01:05:21.000000 pytonconnect-0.3.0/pytonconnect/_wallets_list_manager.py
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.479013 pytonconnect-0.3.0/pytonconnect/crypto/
--rw-rw-rw-   0        0        0       84 2023-04-25 08:52:45.000000 pytonconnect-0.3.0/pytonconnect/crypto/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/pytonconnect/crypto/_session_crypto.py
--rw-rw-rw-   0        0        0     1928 2023-04-24 21:57:27.000000 pytonconnect-0.3.0/pytonconnect/exceptions.py
--rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/pytonconnect/logger.py
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.481013 pytonconnect-0.3.0/pytonconnect/parsers/
--rw-rw-rw-   0        0        0      293 2023-04-25 08:56:29.000000 pytonconnect-0.3.0/pytonconnect/parsers/__init__.py
--rw-rw-rw-   0        0        0     6329 2023-05-19 12:25:16.000000 pytonconnect-0.3.0/pytonconnect/parsers/_connect_event.py
--rw-rw-rw-   0        0        0      521 2023-04-19 17:56:13.000000 pytonconnect-0.3.0/pytonconnect/parsers/_rpc_parser.py
--rw-rw-rw-   0        0        0     1491 2023-04-25 08:54:29.000000 pytonconnect-0.3.0/pytonconnect/parsers/_send_transaction.py
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.484013 pytonconnect-0.3.0/pytonconnect/provider/
--rw-rw-rw-   0        0        0      153 2023-04-25 08:59:01.000000 pytonconnect-0.3.0/pytonconnect/provider/__init__.py
--rw-rw-rw-   0        0        0     4613 2023-09-28 06:37:01.000000 pytonconnect-0.3.0/pytonconnect/provider/_bridge_gateway.py
--rw-rw-rw-   0        0        0     9558 2023-11-06 01:05:21.000000 pytonconnect-0.3.0/pytonconnect/provider/_bridge_provider.py
--rw-rw-rw-   0        0        0      876 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/pytonconnect/provider/_bridge_session.py
--rw-rw-rw-   0        0        0      613 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/pytonconnect/provider/_provider.py
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.486014 pytonconnect-0.3.0/pytonconnect/storage/
--rw-rw-rw-   0        0        0      198 2023-10-06 19:28:18.000000 pytonconnect-0.3.0/pytonconnect/storage/__init__.py
--rw-rw-rw-   0        0        0      524 2023-04-25 09:00:27.000000 pytonconnect-0.3.0/pytonconnect/storage/_default_storage.py
--rw-rw-rw-   0        0        0     1401 2023-05-19 08:40:52.000000 pytonconnect-0.3.0/pytonconnect/storage/_file_storage.py
--rw-rw-rw-   0        0        0     1009 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/pytonconnect/storage/_interface.py
--rw-rw-rw-   0        0        0      567 2023-10-06 19:28:12.000000 pytonconnect-0.3.0/pytonconnect/storage/redis_storage.py
-drwxrwxrwx   0        0        0        0 2023-11-06 01:18:11.478013 pytonconnect-0.3.0/pytonconnect.egg-info/
--rw-rw-rw-   0        0        0     4789 2023-11-06 01:18:11.000000 pytonconnect-0.3.0/pytonconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-11-06 01:18:11.000000 pytonconnect-0.3.0/pytonconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-06 01:18:11.000000 pytonconnect-0.3.0/pytonconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.3.0/pytonconnect.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-11-06 01:18:11.000000 pytonconnect-0.3.0/pytonconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-06 01:18:11.000000 pytonconnect-0.3.0/pytonconnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1159 2023-11-06 01:18:11.491013 pytonconnect-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.256784 pytonconnect-0.3.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-04 12:05:05.000000 pytonconnect-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4847 2024-04-16 18:59:22.256784 pytonconnect-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3798 2024-04-16 18:47:30.000000 pytonconnect-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.175355 pytonconnect-0.3.1/pytonconnect/
+-rw-rw-rw-   0        0        0      181 2023-11-15 11:40:04.000000 pytonconnect-0.3.1/pytonconnect/__init__.py
+-rw-rw-rw-   0        0        0    10271 2024-04-16 18:11:51.000000 pytonconnect-0.3.1/pytonconnect/_ton_connect.py
+-rw-rw-rw-   0        0        0     5275 2024-04-16 16:46:26.000000 pytonconnect-0.3.1/pytonconnect/_wallets_list_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.248780 pytonconnect-0.3.1/pytonconnect/crypto/
+-rw-rw-rw-   0        0        0       84 2023-04-25 08:52:45.000000 pytonconnect-0.3.1/pytonconnect/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1328 2023-11-14 07:24:54.000000 pytonconnect-0.3.1/pytonconnect/crypto/_session_crypto.py
+-rw-rw-rw-   0        0        0     1998 2023-11-14 07:48:24.000000 pytonconnect-0.3.1/pytonconnect/exceptions.py
+-rw-rw-rw-   0        0        0       96 2023-04-19 17:53:09.000000 pytonconnect-0.3.1/pytonconnect/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.250780 pytonconnect-0.3.1/pytonconnect/parsers/
+-rw-rw-rw-   0        0        0      293 2024-04-16 16:41:14.000000 pytonconnect-0.3.1/pytonconnect/parsers/__init__.py
+-rw-rw-rw-   0        0        0     6363 2023-11-14 07:54:46.000000 pytonconnect-0.3.1/pytonconnect/parsers/_connect_event.py
+-rw-rw-rw-   0        0        0      515 2023-11-14 07:27:13.000000 pytonconnect-0.3.1/pytonconnect/parsers/_rpc_parser.py
+-rw-rw-rw-   0        0        0     1475 2024-04-16 16:41:14.000000 pytonconnect-0.3.1/pytonconnect/parsers/_send_transaction.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.252780 pytonconnect-0.3.1/pytonconnect/provider/
+-rw-rw-rw-   0        0        0      153 2023-04-25 08:59:01.000000 pytonconnect-0.3.1/pytonconnect/provider/__init__.py
+-rw-rw-rw-   0        0        0     5257 2024-04-16 18:05:32.000000 pytonconnect-0.3.1/pytonconnect/provider/_bridge_gateway.py
+-rw-rw-rw-   0        0        0     9641 2024-04-16 18:10:04.000000 pytonconnect-0.3.1/pytonconnect/provider/_bridge_provider.py
+-rw-rw-rw-   0        0        0      905 2023-11-14 07:59:26.000000 pytonconnect-0.3.1/pytonconnect/provider/_bridge_session.py
+-rw-rw-rw-   0        0        0      605 2023-11-14 07:21:31.000000 pytonconnect-0.3.1/pytonconnect/provider/_provider.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.255783 pytonconnect-0.3.1/pytonconnect/storage/
+-rw-rw-rw-   0        0        0      198 2023-10-06 19:28:18.000000 pytonconnect-0.3.1/pytonconnect/storage/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-11-14 07:23:44.000000 pytonconnect-0.3.1/pytonconnect/storage/_default_storage.py
+-rw-rw-rw-   0        0        0     1399 2023-11-14 07:30:30.000000 pytonconnect-0.3.1/pytonconnect/storage/_file_storage.py
+-rw-rw-rw-   0        0        0      983 2023-11-14 07:25:31.000000 pytonconnect-0.3.1/pytonconnect/storage/_interface.py
+-rw-rw-rw-   0        0        0      561 2023-11-14 07:25:37.000000 pytonconnect-0.3.1/pytonconnect/storage/redis_storage.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:59:22.255783 pytonconnect-0.3.1/pytonconnect.egg-info/
+-rw-rw-rw-   0        0        0     4847 2024-04-16 18:59:22.000000 pytonconnect-0.3.1/pytonconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2024-04-16 18:59:22.000000 pytonconnect-0.3.1/pytonconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:59:22.000000 pytonconnect-0.3.1/pytonconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-11 12:27:07.000000 pytonconnect-0.3.1/pytonconnect.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2024-04-16 18:59:22.000000 pytonconnect-0.3.1/pytonconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-16 18:59:22.000000 pytonconnect-0.3.1/pytonconnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1159 2024-04-16 18:59:22.257780 pytonconnect-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-04-19 17:53:09.000000 pytonconnect-0.3.1/setup.py
```

### Comparing `pytonconnect-0.3.0/LICENSE` & `pytonconnect-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.3.0/PKG-INFO` & `pytonconnect-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 4 - Beta
@@ -61,15 +61,18 @@
 If user connected his wallet before, connector will restore the connection
 
 ```python
 import asyncio
 from pytonconnect import TonConnect
 
 async def main():
-    connector = TonConnect(manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json')
+    connector = TonConnect(
+        manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json',
+        # api_tokens={'tonapi': 'key'},
+    )
     is_connected = await connector.restore_connection()
     print('is_connected:', is_connected)
 
 if __name__ == '__main__':
     asyncio.get_event_loop().run_until_complete(main())
 ```
```

### Comparing `pytonconnect-0.3.0/README.md` & `pytonconnect-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,18 @@
 If user connected his wallet before, connector will restore the connection
 
 ```python
 import asyncio
 from pytonconnect import TonConnect
 
 async def main():
-    connector = TonConnect(manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json')
+    connector = TonConnect(
+        manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json',
+        # api_tokens={'tonapi': 'key'},
+    )
     is_connected = await connector.restore_connection()
     print('is_connected:', is_connected)
 
 if __name__ == '__main__':
     asyncio.get_event_loop().run_until_complete(main())
 ```
```

### Comparing `pytonconnect-0.3.0/pytonconnect/_ton_connect.py` & `pytonconnect-0.3.1/pytonconnect/_ton_connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 import asyncio
+from typing import Dict
 
-from pytonconnect.exceptions import ManifestContentError, ManifestNotFoundError, WalletAlreadyConnectedError, WalletNotConnectedError, WalletNotSupportFeatureError
+from pytonconnect.exceptions import (
+    ManifestContentError,
+    ManifestNotFoundError,
+    WalletAlreadyConnectedError,
+    WalletNotConnectedError,
+    WalletNotSupportFeatureError,
+)
 from pytonconnect.logger import _LOGGER
 from pytonconnect.parsers import SendTransactionParser, ConnectEventParser, WalletInfo
 from pytonconnect.provider import BridgeProvider
 from pytonconnect.storage import IStorage, DefaultStorage
 
 from ._wallets_list_manager import WalletsListManager
 
@@ -12,14 +19,15 @@
 class TonConnect:
 
     _wallets_list = WalletsListManager()
 
     _provider: BridgeProvider
     _manifest_url: str
     _storage: IStorage
+    _api_tokens: Dict[str, str]
 
     _wallet: WalletInfo
 
     _status_change_subscriptions: list
     _status_change_error_subscriptions: list
 
     @property
@@ -33,37 +41,44 @@
         return self._wallet.account if self.connected else None
 
     @property
     def wallet(self):
         """Current connected wallet or None if no account is connected."""
         return self._wallet
 
-
-    def __init__(self, manifest_url: str, storage: IStorage=DefaultStorage(), wallets_list_source: str = None, wallets_list_cache_ttl: int = None):
+    def __init__(
+        self,
+        manifest_url: str,
+        storage: IStorage = DefaultStorage(),
+        wallets_list_source: str = None,
+        wallets_list_cache_ttl: int = None,
+        api_tokens: Dict[str, str] = {},
+    ):
         if wallets_list_source is not None or wallets_list_cache_ttl is not None:
-            self._wallets_list = WalletsListManager(wallets_list_source=wallets_list_source, cache_ttl=wallets_list_cache_ttl)
+            self._wallets_list = WalletsListManager(
+                wallets_list_source=wallets_list_source,
+                cache_ttl=wallets_list_cache_ttl)
 
         self._provider = None
         self._manifest_url = manifest_url
         self._storage = storage
+        self._api_tokens = api_tokens
 
         self._wallet = None
 
         self._status_change_subscriptions = []
         self._status_change_error_subscriptions = []
 
-
-    def get_wallets(self = None):
+    def get_wallets(self=None):
         """Return available wallets list."""
         return TonConnect._wallets_list.get_wallets() if self is None else self._wallets_list.get_wallets()
 
-
-    def on_status_change(self, callback, errors_handler = None):
+    def on_status_change(self, callback, errors_handler=None):
         """Allows to subscribe to connection status changes and handle connection errors.
-        
+
         :param callback: will be called after connections status changes with actual wallet or None
         :param errors_handler: will be called with some instance of TonConnectError when connect error is received
         :return: unsubscribe callback
         """
         self._status_change_subscriptions.append(callback)
         if errors_handler is not None:
             self._status_change_error_subscriptions.append(errors_handler)
@@ -72,54 +87,53 @@
             if callback in self._status_change_subscriptions:
                 self._status_change_subscriptions.remove(callback)
             if errors_handler is not None and errors_handler in self._status_change_error_subscriptions:
                 self._status_change_error_subscriptions.remove(errors_handler)
 
         return unsubscribe
 
-
-    async def connect(self, wallet, request = None):
-        """Generates universal link for an external wallet and subscribes to the wallet's bridge, or sends connect request to the injected wallet.
+    async def connect(self, wallet, request=None):
+        """Generates universal link for an external wallet and subscribes to the wallet's bridge,
+        or sends connect request to the injected wallet.
 
         :param wallet: wallet's bridge url and universal link for an external wallet.
         :param request: additional request to pass to the wallet while connect (currently only ton_proof is available).
         :return: universal link if external wallet was passed.
         """
         if self.connected:
             raise WalletAlreadyConnectedError()
 
         if self._provider:
             self._provider.close_connection()
-        
+
         self._provider = self._create_provider(wallet)
 
         return await self._provider.connect(self._create_connect_request(request))
 
-
     async def restore_connection(self):
-        """Try to restore existing session and reconnect to the corresponding wallet. Call it immediately when your app is loaded.
+        """Try to restore existing session and reconnect to the corresponding wallet.
+        Call it immediately when your app is loaded.
 
         :return: True if connection is restored
         """
         try:
-            self._provider = BridgeProvider(self._storage)
-        except:
+            self._provider = BridgeProvider(self._storage, api_tokens=self._api_tokens)
+        except Exception:
             await self._storage.remove_item(IStorage.KEY_CONNECTION)
             self._provider = None
-        
+
         if not self._provider:
             return False
 
         self._provider.listen(self._wallet_events_listener)
         return await self._provider.restore_connection()
 
-
     async def send_transaction(self, transaction: dict) -> dict:
         """Asks connected wallet to sign and send the transaction.
-        
+
         :param transaction: transaction to send.
         :return: signed transaction boc that allows you to find the transaction in the blockchain.
         If user rejects transaction, method will throw the corresponding error.
         """
         if not self.connected:
             raise WalletNotConnectedError()
 
@@ -136,34 +150,32 @@
         response = await self._provider.send_request(SendTransactionParser.convert_to_rpc_request(request))
 
         if SendTransactionParser.is_error(response):
             return SendTransactionParser.parse_and_throw_error(response)
 
         return SendTransactionParser.convert_from_rpc_response(response)
 
-
     async def disconnect(self):
         """Disconnect from wallet and drop current session."""
         if not self.connected:
             raise WalletNotConnectedError()
 
         await self._provider.disconnect()
         self._on_wallet_disconnected()
 
-
     def pause_connection(self):
-        """Pause bridge HTTP connection. Might be helpful, if you use SDK on backend and want to save server resources."""
+        """Pause bridge HTTP connection.
+        Might be helpful, if you use SDK on backend and want to save server resources.
+        """
         self._provider.pause()
 
-    
     async def unpause_connection(self):
         """Unpause bridge HTTP connection if it is paused."""
         await self._provider.unpause()
-    
-    
+
     def wait_for_connection(self):
         wait_resolve = asyncio.get_running_loop().create_future()
         if self.connected:
             wait_resolve.set_result(self.wallet)
             return wait_resolve
 
         def status_changed(wallet_info):
@@ -173,15 +185,14 @@
         def status_error(e):
             wait_resolve.set_result(e)
             unsubscribe()
 
         unsubscribe = self.on_status_change(status_changed, status_error)
 
         return wait_resolve
-    
 
     def _check_send_transaction_support(self, features, options):
         supports_deprecated_send_transaction_feature = 'SendTransaction' in features
         send_transaction_feature = None
         for feature in features:
             if isinstance(feature, dict) and feature.get('name', None) == 'SendTransaction':
                 send_transaction_feature = feature
@@ -190,59 +201,56 @@
         if not supports_deprecated_send_transaction_feature and not send_transaction_feature:
             raise WalletNotSupportFeatureError("Wallet doesn't support SendTransaction feature.")
 
         if send_transaction_feature:
             max_messages = send_transaction_feature.get('maxMessages', None)
             required_messages = options.get('required_messages_number')
             if max_messages and max_messages < required_messages:
-                raise WalletNotSupportFeatureError(f'Wallet is not able to handle such SendTransaction request. Max support messages number is {max_messages}, but {required_messages} is required.')
+                raise WalletNotSupportFeatureError(
+                    'Wallet is not able to handle such SendTransaction request. '
+                    f'Max support messages number is {max_messages}, but {required_messages} is required.')
         else:
-            _LOGGER.warning("Connected wallet didn't provide information about max allowed messages in the SendTransaction request. Request may be rejected by the wallet.")
-
+            _LOGGER.warning("Connected wallet didn't provide information about max allowed messages "
+                            "in the SendTransaction request. Request may be rejected by the wallet.")
 
     def _create_provider(self, wallet: dict) -> BridgeProvider:
-        provider = BridgeProvider(self._storage, wallet)
+        provider = BridgeProvider(self._storage, wallet, api_tokens=self._api_tokens)
         provider.listen(self._wallet_events_listener)
         return provider
 
-
     def _wallet_events_listener(self, data):
         if data['event'] == 'connect':
             self._on_wallet_connected(data['payload'])
 
         elif data['event'] == 'connect_error':
             self._on_wallet_connect_error(data['payload'])
 
         elif data['event'] == 'disconnect':
             self._on_wallet_disconnected()
 
-
     def _on_wallet_connected(self, payload):
         self._wallet = ConnectEventParser.parse_response(payload)
         for listener in self._status_change_subscriptions:
             listener(self._wallet)
 
-
     def _on_wallet_connect_error(self, payload):
         _LOGGER.debug('connect error %s', payload)
         error = ConnectEventParser.parse_error(payload)
         for listener in self._status_change_error_subscriptions:
             listener(error)
-        
+
         if isinstance(error, ManifestNotFoundError) or isinstance(error, ManifestContentError):
             _LOGGER.exception(error)
             raise error
 
-
     def _on_wallet_disconnected(self):
         self._wallet = None
         for listener in self._status_change_subscriptions:
             listener(None)
 
-
     def _create_connect_request(self, request):
         items = [
             {
                 'name': 'ton_addr'
             }
         ]
```

### Comparing `pytonconnect-0.3.0/pytonconnect/_wallets_list_manager.py` & `pytonconnect-0.3.1/pytonconnect/_wallets_list_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,22 @@
 
     _wallets_list_source = 'https://raw.githubusercontent.com/ton-blockchain/wallets-list/main/wallets-v2.json'
     _cache_ttl: int
 
     _wallets_list_cache: dict
     _wallets_list_cache_creation_timestamp: int
 
-
-    def __init__(self, wallets_list_source = None, cache_ttl = None):
+    def __init__(self, wallets_list_source=None, cache_ttl=None):
         if wallets_list_source:
             self._wallets_list_source = wallets_list_source
         self._cache_ttl = cache_ttl
 
         self._wallets_list_cache = None
         self._wallets_list_cache_creation_timestamp = None
 
-
     def get_wallets(self):
         if self._cache_ttl \
                 and self._wallets_list_cache_creation_timestamp \
                 and int(datetime.now().timestamp()) > self._wallets_list_cache_creation_timestamp + self._cache_ttl:
             self._wallets_list_cache = None
 
         if not self._wallets_list_cache:
@@ -97,26 +95,26 @@
                 if supported_wallet:
                     self._wallets_list_cache.append(supported_wallet)
 
             self._wallets_list_cache_creation_timestamp = int(datetime.now().timestamp())
 
         return self._wallets_list_cache
 
-
     def _get_supported_wallet_config(self, wallet):
         if not isinstance(wallet, dict):
             _LOGGER.warning(f'Not supported wallet: is not a dict -> {wallet}')
             return None
 
         containsName = 'name' in wallet
         containsImage = 'image' in wallet
         containsAbout = 'about_url' in wallet
 
         if not containsName or not containsImage or not containsAbout:
-            _LOGGER.warning(f'Not supported wallet: contains -> name({containsName}), image({containsImage}), about({containsAbout}), config -> {wallet}')
+            _LOGGER.warning(f'Not supported wallet: contains -> name({containsName}), image({containsImage}), '
+                            f'about({containsAbout}), config -> {wallet}')
             return None
 
         if 'bridge' not in wallet or not isinstance(wallet['bridge'], list) or not len(wallet['bridge']):
             _LOGGER.warning(f'Not supported wallet: bridge is not a list or len is equal 0, config -> {wallet}')
             return None
 
         walletConfig = {
@@ -132,15 +130,15 @@
                     _LOGGER.warning(f'Not supported wallet: bridge url not found, config -> {wallet}')
                     return None
 
                 walletConfig['bridge_url'] = bridge['url']
                 if 'universal_url' in wallet:
                     walletConfig['universal_url'] = wallet['universal_url']
                 break
-        
+
         if 'bridge_url' not in walletConfig:
             _LOGGER.warning(f'Not supported wallet: sse not found, config -> {wallet}')
             return None
 
         return walletConfig
```

### Comparing `pytonconnect-0.3.0/pytonconnect/crypto/_session_crypto.py` & `pytonconnect-0.3.1/pytonconnect/crypto/_session_crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,36 +5,32 @@
 
 
 class SessionCrypto:
 
     key_pair: PrivateKey
     session_id: str
 
-
     def __init__(self, private_key: str = None):
         self.key_pair = PrivateKey(private_key, HexEncoder) if private_key else PrivateKey.generate()
         self.session_id = self.key_pair.public_key.encode().hex()
-    
 
     def create_nonce(self):
         return random(Box.NONCE_SIZE)
 
-
     def encrypt(self, message: str, receiver_pub_key_hex: str):
         nonce = self.create_nonce()
 
         receiver_pk = PublicKey(receiver_pub_key_hex, HexEncoder)
         box = Box(self.key_pair, receiver_pk)
         encrypted = box.encrypt(message.encode('utf-8'), nonce)
 
         res = bytearray(nonce)
         res.extend(encrypted.ciphertext)
         return b64encode(bytes(res))
 
-
     def decrypt(self, message: bytes, sender_pub_key_hex: str):
         msg = b64decode(message)
         nonce = msg[:Box.NONCE_SIZE]
         internal_message = msg[Box.NONCE_SIZE:]
 
         sender_pk = PublicKey(sender_pub_key_hex, HexEncoder)
         box = Box(self.key_pair, sender_pk)
```

### Comparing `pytonconnect-0.3.0/pytonconnect/exceptions.py` & `pytonconnect-0.3.1/pytonconnect/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,16 @@
         super(TonConnectError, self).__init__(f'{self.prefix}'
                                               + (f': {self.info}' if self.info else '')
                                               + (f' {message}' if message is not None else '')
                                               )
 
 
 class WalletAlreadyConnectedError(TonConnectError):
-    info = 'Wallet connection called but wallet already connected. To avoid the error, disconnect the wallet before doing a new connection.'
+    info = ('Wallet connection called but wallet already connected. '
+            'To avoid the error, disconnect the wallet before doing a new connection.')
 
 
 class WalletNotConnectedError(TonConnectError):
     info = 'Send transaction or other protocol methods called while wallet is not connected.'
 
 
 class WalletNotSupportFeatureError(TonConnectError):
@@ -39,12 +40,15 @@
 
 
 class UserRejectsError(TonConnectError):
     info = 'User rejects the action in the wallet.'
 
 
 class ManifestNotFoundError(TonConnectError):
-    info = 'Manifest not found. Make sure you added `tonconnect-manifest.json` to the root of your app or passed correct manifest_url. See more https://github.com/ton-connect/docs/blob/main/requests-responses.md#app-manifest'
+    info = ('Manifest not found. Make sure you added `tonconnect-manifest.json` to the root of your app '
+            'or passed correct manifest_url. '
+            'See more https://github.com/ton-connect/docs/blob/main/requests-responses.md#app-manifest')
 
 
 class ManifestContentError(TonConnectError):
-    info = 'Passed `tonconnect-manifest.json` contains errors. Check format of your manifest. See more https://github.com/ton-connect/docs/blob/main/requests-responses.md#app-manifest'
+    info = ('Passed `tonconnect-manifest.json` contains errors. Check format of your manifest. '
+            'See more https://github.com/ton-connect/docs/blob/main/requests-responses.md#app-manifest')
```

### Comparing `pytonconnect-0.3.0/pytonconnect/parsers/_connect_event.py` & `pytonconnect-0.3.1/pytonconnect/parsers/_connect_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 from base64 import b64decode
 from enum import IntEnum
 from nacl.signing import VerifyKey
 from nacl.encoding import HexEncoder
 from typing import List
 
-from pytonconnect.exceptions import ManifestContentError, ManifestNotFoundError, TonConnectError, UnknownError, BadRequestError, UnknownAppError, UserRejectsError
+from pytonconnect.exceptions import (
+    BadRequestError,
+    ManifestContentError,
+    ManifestNotFoundError,
+    TonConnectError,
+    UnknownAppError,
+    UnknownError,
+    UserRejectsError,
+)
 from pytonconnect.logger import _LOGGER
 
 
 class CONNECT_EVENT_ERROR_CODES(IntEnum):
     UNKNOWN_ERROR = 0
     BAD_REQUEST_ERROR = 1
     MANIFEST_NOT_FOUND_ERROR = 2
@@ -33,17 +41,17 @@
 class CHAIN(IntEnum):
     MAINNET = '-239'
     TESTNET = '-3'
 
 
 class DeviceInfo():
 
-    platform: str # 'iphone' | 'ipad' | 'android' | 'windows' | 'mac' | 'linux' | 'browser'
-    app_name: str # e.g. "Tonkeeper"
-    app_version: str # e.g. "2.3.367"
+    platform: str  # 'iphone' | 'ipad' | 'android' | 'windows' | 'mac' | 'linux' | 'browser'
+    app_name: str  # e.g. "Tonkeeper"
+    app_version: str  # e.g. "2.3.367"
     max_protocol_version: int
     features: List[dict]
 
     def from_dict(device: dict):
         device_info = DeviceInfo()
         device_info.platform = device['platform']
         device_info.app_name = device['appName']
@@ -58,15 +66,16 @@
     # User's address in "hex" format: "<wc>:<hex>"
     address: str
 
     # User's selected chain
     chain: CHAIN
 
     # Base64 (not url safe) encoded wallet contract state_init.
-    # Can be used to get user's public key from the state_init if the wallet contract doesn't support corresponding method
+    # Can be used to get user's public key from the state_init
+    #   if the wallet contract doesn't support corresponding method
     wallet_state_init: str
 
     # Hex string without 0x prefix
     public_key: str
 
     def __repr__(self):
         return f'<Account "{self.address}">'
@@ -115,27 +124,24 @@
 
     # Selected account
     account: Account
 
     # Response for ton_proof item request
     ton_proof: TonProof
 
-
     def __repr__(self):
         return f'<WalletInfo {self.account}>'
 
-
     def __init__(self):
         self.device = None
-        self.provider = 'http' # only http supported
+        self.provider = 'http'  # only http supported
         self.account = None
         self.ton_proof = None
 
-
-    def check_proof(self, src_payload: str=None) -> bool:
+    def check_proof(self, src_payload: str = None) -> bool:
         if self.ton_proof is None:
             return False
 
         wc, whash = self.account.address.split(':', maxsplit=2)
 
         message = bytearray()
         message.extend('ton-proof-item-v2/'.encode())
@@ -156,16 +162,16 @@
 
         try:
             verify_key = VerifyKey(self.account.public_key, HexEncoder)
             verify_key.verify(hashlib.sha256(signature_message).digest(), self.ton_proof.signature)
             _LOGGER.debug('PROOF IS OK')
             return True
 
-        except Exception as e:
-            _LOGGER.exception(f'PROOF ERROR')
+        except Exception:
+            _LOGGER.exception('PROOF ERROR')
 
         return False
 
 
 class ConnectEventParser():
 
     def parse_response(payload: dict) -> WalletInfo:
@@ -184,17 +190,16 @@
         if wallet.account is None:
             raise TonConnectError('ton_addr not contains in items')
 
         wallet.device = DeviceInfo.from_dict(payload['device'])
 
         return wallet
 
-
     def parse_error(payload: dict) -> TonConnectError:
         error_constructor: TonConnectError = UnknownError
 
         code = payload.get('error', {}).get('code', None)
         if code is not None and code in CONNECT_EVENT_ERRORS:
             error_constructor = CONNECT_EVENT_ERRORS[code]
-        
+
         message = payload.get('error', {}).get('message', None)
         return error_constructor(message)
```

### Comparing `pytonconnect-0.3.0/pytonconnect/parsers/_rpc_parser.py` & `pytonconnect-0.3.1/pytonconnect/parsers/_rpc_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,17 @@
 
 class RpcParser(metaclass=ABCMeta):
 
     @abstractmethod
     def convert_to_rpc_request(*args, **kwargs) -> dict:
         raise NotImplementedError
 
-
     @abstractmethod
     def convert_from_rpc_response(rpc_response: dict) -> dict:
         raise NotImplementedError
 
-
     @abstractmethod
     def parse_and_throw_error(response: dict) -> None:
         raise NotImplementedError
 
-
     def is_error(response: dict) -> bool:
         return 'error' in response
```

### Comparing `pytonconnect-0.3.0/pytonconnect/parsers/_send_transaction.py` & `pytonconnect-0.3.1/pytonconnect/parsers/_send_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,28 @@
     SEND_TRANSACTION_ERROR_CODES.BAD_REQUEST_ERROR: BadRequestError,
     SEND_TRANSACTION_ERROR_CODES.UNKNOWN_APP_ERROR: UnknownAppError,
     SEND_TRANSACTION_ERROR_CODES.USER_REJECTS_ERROR: UserRejectsError,
 }
 
 
 class SendTransactionParser(RpcParser):
-    
+
     def convert_to_rpc_request(request: dict) -> dict:
         return {
             'method': 'sendTransaction',
             'params': [json.dumps(request)]
         }
 
-
     def convert_from_rpc_response(rpc_response: dict) -> dict:
         return {
             'boc': rpc_response['result']
         }
 
-
     def parse_and_throw_error(response: dict) -> None:
         error_constructor: TonConnectError = UnknownError
 
         code = response.get('error', {}).get('code', None)
         if code is not None and code in SEND_TRANSACTION_ERRORS:
             error_constructor = SEND_TRANSACTION_ERRORS[code]
-        
+
         message = response.get('error', {}).get('message', None)
         raise error_constructor(message)
```

### Comparing `pytonconnect-0.3.0/pytonconnect/provider/_bridge_gateway.py` & `pytonconnect-0.3.1/pytonconnect/provider/_bridge_gateway.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import json
+from typing import Dict
 
 from aiohttp import ClientSession
 from aiohttp.client_exceptions import ClientConnectionError
 from aiohttp_sse_client import client as sse_client
 
 from pytonconnect.exceptions import TonConnectError
 from pytonconnect.logger import _LOGGER
@@ -21,117 +22,130 @@
     _is_closed: bool
 
     _storage: IStorage
     _bridge_url: str
     _session_id: str
     _listener: any
     _errors_listener: any
+    _api_token: str
 
-
-    def __init__(self, storage: IStorage, bridge_url: str, session_id: str, listener, errors_listener):
+    def __init__(self, storage: IStorage, bridge_url: str, session_id: str, listener, errors_listener, api_tokens: Dict[str, str] = {}):
 
         self._handle_listen = None
         self._event_source = None
         self._is_closed = False
 
         self._storage = storage
         self._bridge_url = bridge_url
         self._session_id = session_id
         self._listener = listener
         self._errors_listener = errors_listener
-    
+
+        self._api_token = None
+        for api_name, api_token in api_tokens.items():
+            if api_name in self._bridge_url:
+                self._api_token = api_token
+                break
 
     async def listen_event_source(self, resolve: asyncio.Future):
         try:
             async with self._event_source:
                 resolve.set_result(True)
                 async for event in self._event_source:
                     await self._messages_handler(event)
 
         except asyncio.exceptions.TimeoutError:
-            _LOGGER.exception(f'Bridge error -> TimeoutError')
+            _LOGGER.exception('Bridge error -> TimeoutError')
         except asyncio.exceptions.CancelledError:
             pass
         except ClientConnectionError:
-            _LOGGER.exception(f'Bridge error -> ClientConnectionError')
+            _LOGGER.exception('Bridge error -> ClientConnectionError')
         except Exception:
-            _LOGGER.exception(f'Bridge error -> Unknown')
-        
+            _LOGGER.exception('Bridge error -> Unknown')
+
         if not resolve.done():
             resolve.set_result(False)
 
-
     async def register_session(self) -> bool:
         if self._is_closed:
             return False
 
         bridge_base = self._bridge_url.rstrip('/')
         bridge_url = f'{bridge_base}/{self.SSE_PATH}?client_id={self._session_id}'
-        
+
         last_event_id = await self._storage.get_item(IStorage.KEY_LAST_EVENT_ID)
         if last_event_id:
             bridge_url += f'&last_event_id={last_event_id}'
         _LOGGER.debug(f'Bridge url -> {bridge_url}')
 
         if self._handle_listen is not None:
             self._handle_listen.cancel()
 
         loop = asyncio.get_running_loop()
         resolve = loop.create_future()
 
-        self._event_source = sse_client.EventSource(bridge_url, timeout=-1, on_error=self._errors_handler)
+        headers = {}
+        if self._api_token is not None:
+            headers['Authorization'] = f'Bearer {self._api_token}'
+
+        session = ClientSession(headers=headers)
+        self._event_source = sse_client.EventSource(
+            bridge_url,
+            session=session,
+            timeout=-1,
+            on_error=self._errors_handler,
+        )
         self._handle_listen = asyncio.create_task(self.listen_event_source(resolve))
 
         return await resolve
 
-
     async def send(self, request: str, receiver_public_key: str, topic: str, ttl: int = None):
         bridge_base = self._bridge_url.rstrip('/')
         bridge_url = f'{bridge_base}/{self.POST_PATH}?client_id={self._session_id}'
         bridge_url += f'&to={receiver_public_key}'
         bridge_url += f'&ttl={ttl if ttl else self.DEFAULT_TTL}'
         bridge_url += f'&topic={topic}'
+        headers = {'Content-type': 'text/plain;charset=UTF-8'}
+
+        if self._api_token is not None:
+            headers['Authorization'] = f'Bearer {self._api_token}'
+
         async with ClientSession() as session:
-            async with session.post(bridge_url, data=request, headers={'Content-type': 'text/plain;charset=UTF-8'}):
+            async with session.post(bridge_url, data=request, headers=headers):
                 pass
 
-
     def pause(self):
         if self._handle_listen is not None:
             self._handle_listen.cancel()
             self._handle_listen = None
 
-
     async def unpause(self):
         await self.register_session()
 
-
     def close(self):
         self._is_closed = True
         self.pause()
 
-
     async def _messages_handler(self, event: sse_client.MessageEvent):
         await self._storage.set_item(IStorage.KEY_LAST_EVENT_ID, event.last_event_id)
 
         if not self._is_closed:
             try:
                 bridge_incoming_message = json.loads(event.data)
-            except:
+            except Exception:
                 raise TonConnectError(f'Bridge message parse failed, message {event.data}')
             else:
                 await self._listener(bridge_incoming_message)
 
-
     def _errors_handler(self):
         if not self._is_closed:
             if self._event_source.ready_state == sse_client.READY_STATE_CLOSED:
                 _LOGGER.error('Bridge error -> READY_STATE_CLOSED')
                 # TODO: reconnect
                 return
 
             elif self._event_source.ready_state == sse_client.READY_STATE_CONNECTING:
                 _LOGGER.error('Bridge error -> READY_STATE_CONNECTING')
                 return
-            
+
             if not self._errors_listener:
                 self._errors_listener()
```

### Comparing `pytonconnect-0.3.0/pytonconnect/provider/_bridge_provider.py` & `pytonconnect-0.3.1/pytonconnect/provider/_bridge_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 import json
+from typing import Dict
 from urllib.parse import quote_plus
 
 from pytonconnect.crypto import SessionCrypto
 from pytonconnect.exceptions import TonConnectError
 from pytonconnect.logger import _LOGGER
 from pytonconnect.storage import IStorage
 
@@ -20,124 +21,120 @@
     _storage: IStorage
     _wallet: dict
 
     _session: BridgeSession
     _gateway: BridgeGateway
     _pending_requests: dict
     _listeners: list
+    _api_tokens: Dict[str, str]
 
-
-    def __init__(self, storage: IStorage, wallet: dict = None):
+    def __init__(self, storage: IStorage, wallet: dict = None, api_tokens: Dict[str, str] = {}):
         self._storage = storage
         self._wallet = wallet
 
         self._session = BridgeSession()
         self._gateway = None
         self._pending_requests = {}
         self._listeners = []
-
+        self._api_tokens = api_tokens
 
     async def connect(self, request: dict):
         self._close_gateways()
         session_crypto = SessionCrypto()
-        
+
         bridge_url = ''
         universal_url = BridgeProvider.STANDART_UNIVERSAL_URL
 
         if isinstance(self._wallet, dict):
             bridge_url = self._wallet['bridge_url']
             if 'universal_url' in self._wallet:
                 universal_url = self._wallet['universal_url']
-            
+
             self._gateway = BridgeGateway(
                 self._storage,
                 bridge_url,
                 session_crypto.session_id,
                 self._gateway_listener,
-                self._gateway_errors_listener
+                self._gateway_errors_listener,
+                self._api_tokens,
             )
 
             await self._gateway.register_session()
-        
+
         self._session.session_crypto = session_crypto
         self._session.bridge_url = bridge_url
 
         return self._generate_universal_url(universal_url, request)
 
-
     async def restore_connection(self):
         self._close_gateways()
 
         connection = await self._storage.get_item(IStorage.KEY_CONNECTION)
         if not connection:
             return False
         connection = json.loads(connection)
 
         if 'session' not in connection:
             return False
         self._session = BridgeSession(connection['session'])
-        
+
         self._gateway = BridgeGateway(
             self._storage,
             self._session.bridge_url,
             self._session.session_crypto.session_id,
             self._gateway_listener,
-            self._gateway_errors_listener
+            self._gateway_errors_listener,
+            self._api_tokens,
         )
 
         await self._gateway.register_session()
 
         for listener in self._listeners:
             listener(connection['connect_event'])
-        
-        return True
 
+        return True
 
     def close_connection(self):
         self._close_gateways()
         self._session = BridgeSession()
         self._gateway = None
         self._pending_requests = {}
         self._listeners = []
 
-
     async def disconnect(self):
         loop = asyncio.get_running_loop()
         resolve = loop.create_future()
 
         def on_request_sent(request_future: asyncio.Future):
             asyncio.create_task(self._remove_session()) \
-                    .add_done_callback(lambda x: resolve.set_result(True) if not resolve.done() else None)
+                .add_done_callback(lambda x: resolve.set_result(True) if not resolve.done() else None)
             request_future.set_result(None)
 
         try:
             await asyncio.wait_for(self.send_request({'method': 'disconnect', 'params': []},
                                                      on_request_sent=on_request_sent),
-                                                     timeout=self.DISCONNECT_TIMEOUT)
+                                   timeout=self.DISCONNECT_TIMEOUT)
         except Exception:
-            _LOGGER.exception(f'Provider disconnect')
+            _LOGGER.exception('Provider disconnect')
         finally:
             if not resolve.done():
                 await self._remove_session()
                 resolve.set_result(True)
 
         return await resolve
 
-
     def pause(self):
         if self._gateway is not None:
             self._gateway.pause()
 
-
     async def unpause(self):
         if self._gateway is not None:
             await self._gateway.unpause()
 
-
-    async def send_request(self, request: dict, on_request_sent = None):
+    async def send_request(self, request: dict, on_request_sent=None):
         if not self._gateway or not self._session or not self._session.wallet_public_key:
             raise TonConnectError('Trying to send bridge request without session.')
 
         connection = json.loads(await self._storage.get_item(IStorage.KEY_CONNECTION, '{}'))
         id = connection.get('next_rpc_request_id', '0')
         connection['next_rpc_request_id'] = str(int(id)+1)
         await self._storage.set_item(IStorage.KEY_CONNECTION, json.dumps(connection))
@@ -157,88 +154,83 @@
 
         self._pending_requests[id] = resolve
         if on_request_sent is not None:
             on_request_sent(resolve)
 
         return await resolve
 
-
     def listen(self, callback):
         self._listeners.append(callback)
 
-
     async def _gateway_listener(self, bridge_incoming_message):
         wallet_message = json.loads(
             self._session.session_crypto.decrypt(bridge_incoming_message['message'], bridge_incoming_message['from'])
         )
 
         _LOGGER.debug(f'Wallet message received: {wallet_message}')
 
         if 'event' not in wallet_message:
             if 'id' in wallet_message:
                 id = wallet_message['id']
                 if id not in self._pending_requests:
                     _LOGGER.debug(f"Response id {id} doesn't match any request's id")
                     return
-                
+
                 self._pending_requests[id].set_result(wallet_message)
                 del self._pending_requests[id]
             return
 
         if 'id' in wallet_message:
             id = int(wallet_message['id'])
             connection = json.loads(await self._storage.get_item(IStorage.KEY_CONNECTION, '{}'))
             last_id = connection['last_wallet_event_id'] if 'last_wallet_event_id' in connection else 0
 
             if last_id and id <= last_id:
-                _LOGGER.error(f'Received event id (={id}) must be greater than stored last wallet event id (={last_id})')
+                _LOGGER.error(
+                    f'Received event id (={id}) must be greater than stored last wallet event id (={last_id})')
                 return
-            
+
             if 'event' in wallet_message and wallet_message['event'] != 'connect':
                 connection['last_wallet_event_id'] = id
                 await self._storage.set_item(IStorage.KEY_CONNECTION, json.dumps(connection))
 
         # self.listeners might be modified in the event handler
         listeners = self._listeners.copy()
 
         if wallet_message['event'] == 'connect':
             await self._update_session(wallet_message, bridge_incoming_message['from'])
 
         elif wallet_message['event'] == 'disconnect':
             await self._remove_session()
-        
+
         for listener in listeners:
             listener(wallet_message)
 
-
-    async def _gateway_errors_listener(self, e = None):
+    async def _gateway_errors_listener(self, e=None):
         raise TonConnectError(f'Bridge error {json.dumps(e or {})}')
 
-
     async def _update_session(self, connect_event: dict, wallet_public_key: str):
         self._session.wallet_public_key = wallet_public_key
 
         connection = {
             'type': 'http',
             'session': self._session.get_dict(),
             'last_wallet_event_id': connect_event['id'] if 'id' in connect_event else None,
             'connect_event': connect_event,
             'next_rpc_request_id': 0
         }
 
         await self._storage.set_item(IStorage.KEY_CONNECTION, json.dumps(connection))
 
-
     async def _remove_session(self):
         if self._gateway is not None:
             self.close_connection()
             await self._storage.remove_item(IStorage.KEY_CONNECTION)
             await self._storage.remove_item(IStorage.KEY_LAST_EVENT_ID)
 
-
     def _generate_universal_url(self, universal_url: str, request: dict):
         if 'tg://' in universal_url or 't.me/' in universal_url:
             return self._generate_tg_universal_url(universal_url, request)
         return self._generate_regular_universal_url(universal_url, request)
 
     def _generate_regular_universal_url(self, universal_url: str, request: dict):
         version = 2
@@ -261,11 +253,10 @@
                         .replace('=', '__')
                         .replace('%', '--')
                         .replace('+', '')
                         )
 
         return universal_url + '&startattach=' + start_attach
 
-
     def _close_gateways(self):
         if self._gateway:
             self._gateway.close()
```

### Comparing `pytonconnect-0.3.0/pytonconnect/provider/_bridge_session.py` & `pytonconnect-0.3.1/pytonconnect/provider/_bridge_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 
 class BridgeSession:
 
     session_crypto: SessionCrypto
     wallet_public_key: str
     bridge_url: str
 
-
     def __init__(self, stored: dict = None):
-        self.session_crypto = SessionCrypto(stored['session_private_key']) if stored and 'session_private_key' in stored else None
+        self.session_crypto = SessionCrypto(stored['session_private_key']) \
+                              if stored and 'session_private_key' in stored else None
         self.wallet_public_key = stored['wallet_public_key'] if stored and 'wallet_public_key' in stored else None
         self.bridge_url = stored['bridge_url'] if stored and 'bridge_url' in stored else None
 
-
     def __repr__(self):
         return json.dumps(self.get_dict())
 
-
     def get_dict(self):
         return {
             'session_private_key': self.session_crypto.key_pair.encode().hex(),
             'wallet_public_key': self.wallet_public_key,
             'bridge_url': self.bridge_url
-        }
+        }
```

### Comparing `pytonconnect-0.3.0/pytonconnect/provider/_provider.py` & `pytonconnect-0.3.1/pytonconnect/provider/_provider.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,26 +3,22 @@
 
 class BaseProvider(metaclass=ABCMeta):
 
     @abstractmethod
     async def restore_connection(self) -> None:
         raise NotImplementedError
 
-
     @abstractmethod
     def close_connection(self) -> None:
         raise NotImplementedError
 
-
     @abstractmethod
     async def disconnect(self) -> None:
         raise NotImplementedError
 
-
     @abstractmethod
     async def send_request(self, request) -> None:
         raise NotImplementedError
 
-
     @abstractmethod
     def listen(self, eventsCallback) -> None:
         raise NotImplementedError
```

### Comparing `pytonconnect-0.3.0/pytonconnect/storage/_default_storage.py` & `pytonconnect-0.3.1/pytonconnect/storage/_default_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 class DefaultStorage(IStorage):
 
     _cache: dict
 
     def __init__(self):
         self._cache = {}
 
-
     async def set_item(self, key: str, value: str):
         self._cache[key] = value
 
-
     async def get_item(self, key: str, default_value: str = None):
         if key not in self._cache:
             return default_value
         return self._cache[key]
 
-
     async def remove_item(self, key: str):
         if key in self._cache:
             del self._cache[key]
```

### Comparing `pytonconnect-0.3.0/pytonconnect/storage/_file_storage.py` & `pytonconnect-0.3.1/pytonconnect/storage/_file_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,48 +4,43 @@
 
 
 class FileStorage(IStorage):
 
     _cache: dict
     _file_path: str
 
-    def __init__(self, file_path: str, use_cache = True):
+    def __init__(self, file_path: str, use_cache=True):
         self._file_path = file_path
         if use_cache:
             self._cache = {}
             try:
                 with open(self._file_path, 'r') as f:
                     self._cache = json.loads(f.read())
-            except:
+            except Exception:
                 pass
         else:
             self._cache = None
 
-
     def _read_from_file(self):
         with open(self._file_path, 'r') as f:
             return json.loads(f.read())
 
-
     def _write_to_file(self, d: dict):
         with open(self._file_path, 'w') as f:
             f.write(json.dumps(d))
 
-
     async def set_item(self, key: str, value: str):
         data = self._read_from_file() if self._cache is None else self._cache
         data[key] = value
         self._write_to_file(data)
 
-
     async def get_item(self, key: str, default_value: str = None):
         data = self._read_from_file() if self._cache is None else self._cache
         if key not in data:
             return default_value
         return data[key]
 
-
     async def remove_item(self, key: str):
         data = self._read_from_file() if self._cache is None else self._cache
         if key in data:
             del data[key]
             self._write_to_file(data)
```

### Comparing `pytonconnect-0.3.0/pytonconnect.egg-info/PKG-INFO` & `pytonconnect-0.3.1/pytonconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytonconnect
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for TON Connect 2.0
 Author: XaBbl4
 Author-email: xabbl4@gmail.com
 License: Apache 2.0
 Project-URL: Github, https://github.com/XaBbl4/pytonconnect
 Keywords: TON,TON Connect,TON Connect SDK
 Classifier: Development Status :: 4 - Beta
@@ -61,15 +61,18 @@
 If user connected his wallet before, connector will restore the connection
 
 ```python
 import asyncio
 from pytonconnect import TonConnect
 
 async def main():
-    connector = TonConnect(manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json')
+    connector = TonConnect(
+        manifest_url='https://raw.githubusercontent.com/XaBbl4/pytonconnect/main/pytonconnect-manifest.json',
+        # api_tokens={'tonapi': 'key'},
+    )
     is_connected = await connector.restore_connection()
     print('is_connected:', is_connected)
 
 if __name__ == '__main__':
     asyncio.get_event_loop().run_until_complete(main())
 ```
```

### Comparing `pytonconnect-0.3.0/pytonconnect.egg-info/SOURCES.txt` & `pytonconnect-0.3.1/pytonconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytonconnect-0.3.0/setup.cfg` & `pytonconnect-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7974 6f6e 636f 6e6e 6563 740d   = pytonconnect.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 2e30  .version = 0.3.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 2e31  .version = 0.3.1
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 5079 7468 6f6e 2053 444b 2066 6f72 2054  Python SDK for T
 00000050: 4f4e 2043 6f6e 6e65 6374 2032 2e30 0d0a  ON Connect 2.0..
 00000060: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000070: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000080: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 00000090: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

