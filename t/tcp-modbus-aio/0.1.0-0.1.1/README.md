# Comparing `tmp/tcp_modbus_aio-0.1.0.tar.gz` & `tmp/tcp_modbus_aio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.1.0.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.1.1.tar", max compression
```

## Comparing `tcp_modbus_aio-0.1.0.tar` & `tcp_modbus_aio-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/LICENSE
--rw-r--r--   0        0        0     1649 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/README.md
--rw-r--r--   0        0        0      825 2024-04-16 18:58:50.786280 tcp_modbus_aio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-16 18:58:50.802281 tcp_modbus_aio-0.1.0/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    18747 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/tcp_modbus_aio/connection.py
--rw-r--r--   0        0        0      267 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1140 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-04-16 18:58:50.058270 tcp_modbus_aio-0.1.0/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-04-16 18:58:50.062270 tcp_modbus_aio-0.1.0/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1649 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/README.md
+-rw-r--r--   0        0        0      825 2024-04-16 19:16:29.307997 tcp_modbus_aio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-16 19:16:29.311997 tcp_modbus_aio-0.1.1/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    18586 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/connection.py
+-rw-r--r--   0        0        0      267 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1140 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-04-16 19:16:28.451996 tcp_modbus_aio-0.1.1/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.1.1/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.1.0/LICENSE` & `tcp_modbus_aio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.0/README.md` & `tcp_modbus_aio-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.0/pyproject.toml` & `tcp_modbus_aio-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.1.0"
+version = "0.1.1"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tcp_modbus_aio-0.1.0/tcp_modbus_aio/connection.py` & `tcp_modbus_aio-0.1.1/tcp_modbus_aio/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,28 @@
     task: asyncio.Task | None = None
 
 
 TEST_CONNECTION_MESSAGE = ReadCoils()
 TEST_CONNECTION_MESSAGE.starting_address = 0
 TEST_CONNECTION_MESSAGE.quantity = 1
 
+DEFAULT_MODBUS_TIMEOUT_SEC = 0.1
+MAX_TRANSACTION_ID = 2**16 - 1  # maximum number that fits in 2 bytes
+MODBUS_MBAP_SIZE = 7
+MBAP_HEADER_STRUCT_FORMAT = ">HHHB"
+
 
 @dataclass
 class TCPModbusClient:
     KEEPALIVE_AFTER_IDLE_SEC: ClassVar = 10
     KEEPALIVE_INTERVAL_SEC: ClassVar = 10
     KEEPALIVE_MAX_FAILS: ClassVar = 5
 
     PING_LOOP_PERIOD: ClassVar = 1
 
-    DEFAULT_MODBUS_TIMEOUT_SEC: ClassVar = 0.1
-    MAX_TRANSACTION_ID: ClassVar = 2**16 - 1  # maximum number that fits in 2 bytes
-    MODBUS_MBAP_SIZE: ClassVar = 7
-    MBAP_HEADER_STRUCT_FORMAT: ClassVar = ">HHHB"
-
     def __init__(
         self,
         host: str,
         port: int = 502,
         slave_id: int = 1,
         logger: logging.Logger | None = None,
     ) -> None:
@@ -100,15 +100,15 @@
 
         # If we succesfully write a request but the response times out, we cache the transaction ID here
         # so we know to throw it away if we see it again.
         self._lost_transaction_ids = TTLCache[int, bool](maxsize=1000, ttl=60)
 
         # Instead of randomly sampling transaction IDs, we can use a global counter with random seed.
         # This way, we can avoid duplicate transaction IDs via birthday paradox.
-        self._next_transaction_id = random.randint(0, self.MAX_TRANSACTION_ID)
+        self._next_transaction_id = random.randint(0, MAX_TRANSACTION_ID)
 
     def __repr__(self) -> str:
         last_ping_msg = (
             f"{self._last_ping*1000:.1f}ms ping"
             if self._last_ping is not None
             else "no ping"
         )
@@ -319,22 +319,20 @@
 
         :param adu: Request ADU.
         :param sock: Socket instance.
         :return: Parsed response from server.
         """
 
         request_transaction_id = self._next_transaction_id
-        self._next_transaction_id = (
-            self._next_transaction_id + 1
-        ) % self.MAX_TRANSACTION_ID
+        self._next_transaction_id = (self._next_transaction_id + 1) % MAX_TRANSACTION_ID
 
         msg_str = f"{request_function.__class__.__name__}[{request_transaction_id}]"
 
         request_mbap_header = struct.pack(
-            self.MBAP_HEADER_STRUCT_FORMAT,
+            MBAP_HEADER_STRUCT_FORMAT,
             request_transaction_id,
             0,
             len(request_function.request_pdu) + 1,
             self.slave_id,
         )
 
         request_adu = request_mbap_header + request_function.request_pdu
@@ -376,35 +374,33 @@
                     )
 
                 raise ModbusCommunicationFailureError(
                     f"Failed to write request {msg_str} to modbus device {self.host}"
                 )
 
             expected_response_size = (
-                request_function.expected_response_pdu_size + self.MODBUS_MBAP_SIZE
+                request_function.expected_response_pdu_size + MODBUS_MBAP_SIZE
             )
 
             try:
                 seen_response_transaction_ids = []
                 while True:
                     response_adu = await asyncio.wait_for(
                         reader.read(expected_response_size), timeout=timeout
                     )
 
-                    response_pdu = response_adu[self.MODBUS_MBAP_SIZE :]
-                    response_mbap_header = response_adu[: self.MODBUS_MBAP_SIZE]
+                    response_pdu = response_adu[MODBUS_MBAP_SIZE:]
+                    response_mbap_header = response_adu[:MODBUS_MBAP_SIZE]
 
                     (
                         response_transaction_id,
                         _,
                         mbap_asserted_pdu_length_plus_one,
                         response_asserted_slave_id,
-                    ) = struct.unpack(
-                        self.MBAP_HEADER_STRUCT_FORMAT, response_mbap_header
-                    )
+                    ) = struct.unpack(MBAP_HEADER_STRUCT_FORMAT, response_mbap_header)
 
                     seen_response_transaction_ids.append(response_transaction_id)
 
                     if response_transaction_id in self._lost_transaction_ids:
                         self._lost_transaction_ids.pop(response_transaction_id)
                         if self.logger is not None:
                             self.logger.warning(
```

### Comparing `tcp_modbus_aio-0.1.0/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.1.1/tcp_modbus_aio/ping.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.0/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.1.1/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.1.0/PKG-INFO` & `tcp_modbus_aio-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.1.0
+Version: 0.1.1
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

