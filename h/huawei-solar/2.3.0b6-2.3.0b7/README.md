# Comparing `tmp/huawei-solar-2.3.0b6.tar.gz` & `tmp/huawei_solar-2.3.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.3.0b6.tar", last modified: Mon Apr  1 08:53:28 2024, max compression
+gzip compressed data, was "huawei_solar-2.3.0b7.tar", last modified: Tue Apr 16 18:59:36 2024, max compression
```

## Comparing `huawei-solar-2.3.0b6.tar` & `huawei_solar-2.3.0b7.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:53:28.659236 huawei-solar-2.3.0b6/
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)    34273 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     8218 2024-04-01 08:53:28.659236 huawei-solar-2.3.0b6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7163 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-04-01 08:53:28.660236 huawei-solar-2.3.0b6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:53:28.649237 huawei-solar-2.3.0b6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:53:28.655236 huawei-solar-2.3.0b6/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18820 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11326 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    25878 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    21070 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22488 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    46878 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:53:28.658236 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8218 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-01 08:53:28.000000 huawei-solar-2.3.0b6/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3578 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:53:28.658236 huawei-solar-2.3.0b6/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      818 2024-04-01 08:53:16.000000 huawei-solar-2.3.0b6/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:59:36.492495 huawei_solar-2.3.0b7/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)    34273 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-04-16 18:59:36.492495 huawei_solar-2.3.0b7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3869 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-16 18:59:36.493495 huawei_solar-2.3.0b7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:59:36.482495 huawei_solar-2.3.0b7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:59:36.488495 huawei_solar-2.3.0b7/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18911 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11324 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    25883 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     7077 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    21900 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22488 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    47109 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:59:36.491495 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-16 18:59:36.000000 huawei_solar-2.3.0b7/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 18:59:36.491495 huawei_solar-2.3.0b7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test_bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    16244 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-04-16 18:59:24.000000 huawei_solar-2.3.0b7/tox.ini
```

### Comparing `huawei-solar-2.3.0b6/.gitignore` & `huawei_solar-2.3.0b7/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/.gitlab-ci.yml` & `huawei_solar-2.3.0b7/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -60,8 +60,14 @@
 python310:
   stage: test
   image: python:3.10
   script: tox -e py310
 
 python311:
   stage: test
+  image: python:3.11
   script: tox -e py311
+
+python312:
+  stage: test
+  image: python:3.12
+  script: tox -e py312
```

### Comparing `huawei-solar-2.3.0b6/.pre-commit-config.yaml` & `huawei_solar-2.3.0b7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/LICENSE.md` & `huawei_solar-2.3.0b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/bridge_tst.py` & `huawei_solar-2.3.0b7/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/pyproject.toml` & `huawei_solar-2.3.0b7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/setup.cfg` & `huawei_solar-2.3.0b7/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 author = Emil Vanherp
 author_email = emil@vanherp.me
 license = MIT License
 license_file = LICENSE.md
 classifiers = 
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	=src
 packages = find:
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/__init__.py` & `huawei_solar-2.3.0b7/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/bridge.py` & `huawei_solar-2.3.0b7/src/huawei_solar/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     def __init__(
         self,
         client: AsyncHuaweiSolar,
         update_lock: asyncio.Lock,
         primary: bool,
         slave_id: t.Optional[int] = None,
     ):
+        """DO NOT USE THIS CONSTRUCTOR DIRECTLY. Use HuaweiSolarBridge.create() instead"""
         self.client = client
         self.update_lock = update_lock
 
         self._primary = primary
         self.slave_id = slave_id or 0
 
     @classmethod
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/exceptions.py` & `huawei_solar-2.3.0b7/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/files.py` & `huawei_solar-2.3.0b7/src/huawei_solar/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,8 +313,8 @@
 
 
 def _to_string(data: bytes):
     try:
         return data.decode("ascii").rstrip("\x00")
     except ValueError:
         _LOGGER.exception("Could not decode '%s'. Ignoring.", binascii.hexlify(data))
-        return None
+        return ""
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/huawei_solar.py` & `huawei_solar-2.3.0b7/src/huawei_solar/huawei_solar.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
     @classmethod
     async def create(
         cls,
         host,
         port: int = DEFAULT_TCP_PORT,
         slave: int = DEFAULT_SLAVE,
         timeout: int = DEFAULT_TIMEOUT,
-        cooldown_time: int = DEFAULT_COOLDOWN_TIME,
+        cooldown_time: float = DEFAULT_COOLDOWN_TIME,
     ):  # pylint: disable=too-many-arguments
         """Creates an AsyncHuaweiSolar instance."""
 
         client = None
         try:
             client = AsyncHuaweiSolarModbusTcpClient(host, port, timeout)
             await client.connect()
@@ -191,15 +191,15 @@
     @classmethod
     async def create_rtu(
         cls,
         port,
         baudrate: int = DEFAULT_BAUDRATE,
         slave: int = DEFAULT_SLAVE,
         timeout: int = DEFAULT_TIMEOUT,
-        cooldown_time: int = DEFAULT_COOLDOWN_TIME,
+        cooldown_time: float = DEFAULT_COOLDOWN_TIME,
         **serial_kwargs,
     ):
         """Create a serial client"""
         client = None
         try:
             client = AsyncHuaweiSolarModbusSerialClient(port, baudrate, timeout, **serial_kwargs)
             await client.connect()
@@ -428,15 +428,15 @@
                 if response.exception_code == PERMISSION_DENIED_EXCEPTION_CODE:
                     raise PermissionDenied("Permission denied")
                 if response.exception_code == ModbusExceptions.SlaveBusy:
                     raise SlaveBusyException()
                 if response.exception_code == ModbusExceptions.SlaveFailure:
                     raise SlaveFailureException()
                 raise ReadException(
-                    f"Exception occured while trying to read file {hex(file_type)}: {hex(response.exception_code)}",
+                    f"Exception occurred while trying to read file {hex(file_type)}: {hex(response.exception_code)}",
                     modbus_exception_code=response.exception_code,
                 )
 
             return response_type(response.content)
 
         async def _do_read_file():
             # Start the upload
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/modbus.py` & `huawei_solar-2.3.0b7/src/huawei_solar/modbus.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,21 @@
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 
 RECONNECT_DELAY = 1000  # in milliseconds
 WAIT_ON_CONNECT = 1500  # in milliseconds
 
 LOGGER = logging.getLogger(__name__)
 
+if t.TYPE_CHECKING:
+    _Base = AsyncModbusSerialClient | AsyncModbusTcpClient
+else:
+    _Base = object
 
-class ModbusConnectionMixin:
+
+class ModbusConnectionMixin(_Base):
     """Mixin that adds support for custom Huawei modbus messages and delays upon reconnect"""
 
     connected_event = asyncio.Event()
 
     def __init__(self, *args, **kwargs) -> None:
         """Add support for the custom Huawei modbus messages"""
         super().__init__(*args, **kwargs)
@@ -31,31 +36,31 @@
         async def _made_connection_task():
             LOGGER.debug("Waiting for %d milliseconds after connection before performing operations", WAIT_ON_CONNECT)
             await asyncio.sleep(WAIT_ON_CONNECT / 1000)
             self.connected_event.set()
 
         asyncio.create_task(_made_connection_task())
 
-    def connection_lost(self, exc):
+    def connection_lost(self, reason):
         """Register that a connection has been lost in an asyncio Event"""
-        super().connection_lost(exc)
+        super().connection_lost(reason)
         self.connected_event.clear()
 
 
 class AsyncHuaweiSolarModbusSerialClient(ModbusConnectionMixin, AsyncModbusSerialClient):
     """Custom SerialClient with support for custom Huawei modbus messages"""
 
     def __init__(self, port, baudrate, timeout: int, **serial_kwargs):
         super().__init__(port, **serial_kwargs, baudrate=baudrate, reconnect_delay=RECONNECT_DELAY, timeout=timeout)
 
 
 class AsyncHuaweiSolarModbusTcpClient(ModbusConnectionMixin, AsyncModbusTcpClient):
     """Custom TcpClient that supports wait after connect and custom Huawei modbus messages"""
 
-    def __init__(self, host, port, timeout) -> AsyncModbusTcpClient:
+    def __init__(self, host, port, timeout):
         super().__init__(host, port, timeout=timeout, reconnect_delay=RECONNECT_DELAY)
 
 
 class PrivateHuaweiModbusResponse(ModbusResponse):
     """Response with the private Huawei Solar function code"""
 
     function_code = 0x41
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/register_names.py` & `huawei_solar-2.3.0b7/src/huawei_solar/register_names.py`

 * *Files 10% similar despite different names*

```diff
@@ -302,14 +302,26 @@
 STORAGE_UNIT_2_BATTERY_PACK_1_MINIMUM_TEMPERATURE = "storage_unit_2_battery_pack_1_minimum_temperature"
 STORAGE_UNIT_2_BATTERY_PACK_2_MAXIMUM_TEMPERATURE = "storage_unit_2_battery_pack_2_maximum_temperature"
 STORAGE_UNIT_2_BATTERY_PACK_2_MINIMUM_TEMPERATURE = "storage_unit_2_battery_pack_2_minimum_temperature"
 STORAGE_UNIT_2_BATTERY_PACK_3_MAXIMUM_TEMPERATURE = "storage_unit_2_battery_pack_3_maximum_temperature"
 STORAGE_UNIT_2_BATTERY_PACK_3_MINIMUM_TEMPERATURE = "storage_unit_2_battery_pack_3_minimum_temperature"
 SYSTEM_TIME = "system_time"
 SYSTEM_TIME_RAW = "system_time_raw"
+Q_U_CHARACTERISTIC_CURVE_MODEL = "q_u_characteristic_curve_model"
+Q_U_SCHEDULING_TRIGGER_POWER_PERCENTAGE = "q_u_scheduling_trigger_power_percentage"
+POWER_FACTOR_2 = "power_factor_2"
+REACTIVE_POWER_COMPENSATION = "reactive_power_compensation"
+REACTIVE_POWER_ADJUSTMENT_TIME = "reactive_power_adjustment_time"
+ACTIVE_POWER_PERCENTAGE_DERATING = "active_power_percentage_derating"
+ACTIVE_POWER_FIXED_VALUE_DERATING = "active_power_fixed_value_derating"
+REACTIVE_POWER_COMPENSATION_AT_NIGHT = "reactive_power_compensation_at_night"
+FIXED_REACTIVE_POWER_AT_NIGHT = "fixed_reactive_power_at_night"
+CHARACTERISTIC_CURVE_REACTIVE_POWER_ADJUSTMENT_TIME = "characteristic_curve_reactive_power_adjustment_time"
+PERCENT_APPARENT_POWER = "percent_apparent_power"
+Q_U_SCHEDULING_EXIT_POWER_PERCENTAGE = "q_u_scheduling_exit_power_percentage"
 STARTUP = "startup"
 SHUTDOWN = "shutdown"
 GRID_CODE = "grid_code"
 MPPT_MULTIMODAL_SCANNING = "mppt_multimodal_scanning"
 MPPT_SCANNING_INTERVAL = "mppt_scanning_interval"
 MPPT_PREDICTED_POWER = "mppt_predicted_power"
 TIME_ZONE = "time_zone"
@@ -346,15 +358,15 @@
 STORAGE_TIME_OF_USE_CHARGING_AND_DISCHARGING_PERIODS = "storage_time_of_use_charging_and_discharging_periods"
 STORAGE_EXCESS_PV_ENERGY_USE_IN_TOU = "storage_excess_pv_energy_use_in_tou"
 ACTIVE_POWER_CONTROL_MODE = "active_power_control_mode"
 MAXIMUM_FEED_GRID_POWER_WATT = "maximum_feed_grid_power_watt"
 MAXIMUM_FEED_GRID_POWER_PERCENT = "maximum_feed_grid_power_percent"
 DONGLE_PLANT_MAXIMUM_CHARGE_FROM_GRID_POWER = "dongle_plant_maximum_charge_from_grid_power"
 BACKUP_SWITCH_TO_OFF_GRID = "backup_switch_to_off_grid"
-BACKUP_VOLTAGE_INDEPENDEND_OPERATION = "backup_voltage_independend_operation"
+BACKUP_VOLTAGE_INDEPENDENT_OPERATION = "backup_voltage_independent_operation"
 STORAGE_UNIT_1_PACK_1_NO = "storage_unit_1_pack_1_no"
 STORAGE_UNIT_1_PACK_2_NO = "storage_unit_1_pack_2_no"
 STORAGE_UNIT_1_PACK_3_NO = "storage_unit_1_pack_3_no"
 STORAGE_UNIT_2_PACK_1_NO = "storage_unit_2_pack_1_no"
 STORAGE_UNIT_2_PACK_2_NO = "storage_unit_2_pack_2_no"
 STORAGE_UNIT_2_PACK_3_NO = "storage_unit_2_pack_3_no"
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/register_values.py` & `huawei_solar-2.3.0b7/src/huawei_solar/register_values.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar/registers.py` & `huawei_solar-2.3.0b7/src/huawei_solar/registers.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,69 +121,69 @@
 
         getattr(builder, self._encode_function_name)(data)
 
 
 class U16Register(NumberRegister):
     """Unsigned 16-bit register"""
 
-    def __init__(self, unit, gain, register, length, writeable=False, readable=True, ignore_invalid=False):
+    def __init__(self, unit, gain, register, writeable=False, readable=True, ignore_invalid=False):
         super().__init__(
             unit,
             gain,
             register,
-            length,
+            1,
             "decode_16bit_uint",
             "add_16bit_uint",
             writeable=writeable,
             readable=readable,
             invalid_value=2**16 - 1 if not ignore_invalid else None,
         )
 
 
 class U32Register(NumberRegister):
     """Unsigned 32-bit register"""
 
-    def __init__(self, unit, gain, register, length, writeable=False):
+    def __init__(self, unit, gain, register, writeable=False):
         super().__init__(
             unit,
             gain,
             register,
-            length,
+            2,
             "decode_32bit_uint",
             "add_32bit_uint",
             writeable=writeable,
             invalid_value=2**32 - 1,
         )
 
 
 class I16Register(NumberRegister):
     """Signed 16-bit register"""
 
-    def __init__(self, unit, gain, register, length, writeable=False):
+    def __init__(self, unit, gain, register, writeable=False):
         super().__init__(
             unit,
             gain,
             register,
-            length,
+            1,
             "decode_16bit_int",
             "add_16bit_int",
             writeable=writeable,
             invalid_value=2**15 - 1,
         )
 
 
 class I32Register(NumberRegister):
     """Signed 32-bit register."""
 
-    def __init__(self, unit, gain, register, length, writeable=False):
+    def __init__(self, unit, gain, register, writeable=False):
         super().__init__(
             unit,
             gain,
             register,
-            length,
+            2,
             "decode_32bit_int",
             "add_32bit_int",
             writeable=writeable,
             invalid_value=2**31 - 1,
         )
 
 
@@ -194,20 +194,20 @@
      as a positive number, but are (in some cases) being reported as a
      negative number.
 
     cfr. https://github.com/wlcrs/huawei_solar/issues/54
 
     """
 
-    def __init__(self, unit, gain, register, length, writeable=False):
+    def __init__(self, unit, gain, register, writeable=False):
         super().__init__(
             unit,
             gain,
             register,
-            length,
+            2,
             "decode_32bit_int",
             "add_32bit_int",
             writeable=writeable,
             invalid_value=2**31 - 1,
         )
 
     def decode(self, decoder: BinaryPayloadDecoder, inverter: "AsyncHuaweiSolar"):
@@ -229,16 +229,16 @@
 
     return result
 
 
 class TimestampRegister(U32Register):
     """Timestamp register."""
 
-    def __init__(self, register, length, writeable=False):
-        super().__init__(None, 1, register, length, writeable=writeable)
+    def __init__(self, register, writeable=False):
+        super().__init__(None, 1, register, writeable=writeable)
 
     def decode(self, decoder: BinaryPayloadDecoder, inverter: "AsyncHuaweiSolar"):
         value = super().decode(decoder, inverter)
 
         if value is None:
             return None
 
@@ -257,16 +257,16 @@
             return datetime.fromtimestamp(value, timezone.utc)
         except OverflowError as err:
             raise DecodeError(f"Received invalid timestamp {value}") from err
 
 
 @dataclass
 class LG_RESU_TimeOfUsePeriod:  # pylint: disable=invalid-name
-    start_time: int  # minutes sinds midnight
-    end_time: int  # minutes sinds midnight
+    start_time: int  # minutes since midnight
+    end_time: int  # minutes since midnight
     electricity_price: float
 
 
 class ChargeFlag(IntEnum):
     CHARGE = 0
     DISCHARGE = 1
 
@@ -322,17 +322,17 @@
                 raise TimeOfUsePeriodsException("TOU period is invalid (Below zero)")
             if tou_period.start_time > 24 * 60 or tou_period.end_time > 24 * 60:
                 raise TimeOfUsePeriodsException("TOU period is invalid (Spans over more than one day)")
             if tou_period.start_time >= tou_period.end_time:
                 raise TimeOfUsePeriodsException("TOU period is invalid (start-time is greater than end-time)")
 
         if isinstance(data[0], HUAWEI_LUNA2000_TimeOfUsePeriod):
-            return self._validate_huawei_luna2000(data)
+            return self._validate_huawei_luna2000(t.cast(list[HUAWEI_LUNA2000_TimeOfUsePeriod], data))
         elif isinstance(data[0], LG_RESU_TimeOfUsePeriod):
-            return self._validate_lg_resu(data)
+            return self._validate_lg_resu(t.cast(list[LG_RESU_TimeOfUsePeriod], data))
         else:
             raise TimeOfUsePeriodsException("TOU period is of an unexpected type")
 
     def _validate_huawei_luna2000(self, data: list[HUAWEI_LUNA2000_TimeOfUsePeriod]):
         # Sanity checks between periods
 
         for day_idx in range(0, 7):
@@ -348,19 +348,19 @@
                 prev_period = active_periods[period_idx - 1]
                 if (
                     prev_period.start_time <= current_period.start_time < prev_period.end_time
                     or prev_period.start_time < current_period.end_time <= prev_period.end_time
                 ):
                     raise TimeOfUsePeriodsException("TOU periods are overlapping")
 
-    def _validate_lg_resu(self, data: list[HUAWEI_LUNA2000_TimeOfUsePeriod]):
+    def _validate_lg_resu(self, data: list[LG_RESU_TimeOfUsePeriod]):
         # Sanity checks between periods
 
         # make a copy of the data to sort
-        sorted_periods: list[HUAWEI_LUNA2000_TimeOfUsePeriod] = data.copy()
+        sorted_periods: list[LG_RESU_TimeOfUsePeriod] = data.copy()
 
         sorted_periods.sort(key=lambda a: a.start_time)
 
         for period_idx in range(1, len(sorted_periods)):
             current_period = sorted_periods[period_idx]
             prev_period = sorted_periods[period_idx - 1]
             if (
@@ -373,27 +373,29 @@
         self,
         data: t.Union[list[HUAWEI_LUNA2000_TimeOfUsePeriod], list[LG_RESU_TimeOfUsePeriod]],
         builder: BinaryPayloadBuilder,
     ):
         self._validate(data)
 
         if len(data) == 0 or isinstance(data[0], HUAWEI_LUNA2000_TimeOfUsePeriod):
-            return self.encode_huawei_luna2000(data=data, builder=builder)
+            return self.encode_huawei_luna2000(
+                data=t.cast(list[HUAWEI_LUNA2000_TimeOfUsePeriod], data), builder=builder
+            )
         elif isinstance(data[0], LG_RESU_TimeOfUsePeriod):
-            return self.encode_lg_resu(data=data, builder=builder)
+            return self.encode_lg_resu(data=t.cast(list[LG_RESU_TimeOfUsePeriod], data), builder=builder)
         else:
             raise EncodeError(f"Invalid dataclass to encode for TOU Registers: {type(data[0])}")
 
     def encode_lg_resu(self, data: list[LG_RESU_TimeOfUsePeriod], builder: BinaryPayloadBuilder):
         assert len(data) <= LG_RESU_TOU_PERIODS
         builder.add_16bit_uint(len(data))
 
         for period in data:
-            builder.add_16bit_uint(period.start_time),
-            builder.add_16bit_uint(period.end_time),
+            builder.add_16bit_uint(period.start_time)
+            builder.add_16bit_uint(period.end_time)
             builder.add_32bit_uint(int(period.electricity_price * 1000))
 
         # pad with empty periods
         for _ in range(len(data), LG_RESU_TOU_PERIODS):
             builder.add_16bit_uint(0)
             builder.add_16bit_uint(0)
             builder.add_32bit_uint(0)
@@ -435,30 +437,30 @@
                 if days_tuple[i]:
                     result += mask
                 mask = mask << 1
 
             return result
 
         for period in data:
-            builder.add_16bit_uint(period.start_time),
-            builder.add_16bit_uint(period.end_time),
+            builder.add_16bit_uint(period.start_time)
+            builder.add_16bit_uint(period.end_time)
             builder.add_8bit_uint(int(period.charge_flag))
             builder.add_8bit_uint(_days_effective_builder(period.days_effective))
 
         # pad with empty periods
         for _ in range(len(data), HUAWEI_LUNA2000_TOU_PERIODS):
             builder.add_16bit_uint(0)
             builder.add_16bit_uint(0)
             builder.add_16bit_uint(0)
 
 
 @dataclass
 class ChargeDischargePeriod:
-    start_time: int  # minutes sinds midnight
-    end_time: int  # minutes sinds midnight
+    start_time: int  # minutes since midnight
+    end_time: int  # minutes since midnight
     power: int  # power in watts
 
 
 CHARGE_DISCHARGE_PERIODS = 10
 
 
 class ChargeDischargePeriodRegisters(RegisterDefinition):
@@ -479,29 +481,29 @@
         return periods[:number_of_periods]
 
     def encode(self, data: list[ChargeDischargePeriod], builder: BinaryPayloadBuilder):
         assert len(data) <= CHARGE_DISCHARGE_PERIODS
         builder.add_16bit_uint(len(data))
 
         for period in data:
-            builder.add_16bit_uint(period.start_time),
-            builder.add_16bit_uint(period.end_time),
+            builder.add_16bit_uint(period.start_time)
+            builder.add_16bit_uint(period.end_time)
             builder.add_32bit_uint(period.power)
 
         # pad with empty periods
         for _ in range(len(data), CHARGE_DISCHARGE_PERIODS):
             builder.add_16bit_uint(0)
             builder.add_16bit_uint(0)
             builder.add_32bit_uint(0)
 
 
 @dataclass
 class PeakSettingPeriod:
-    start_time: int  # minutes sinds midnight
-    end_time: int  # minutes sinds midnight
+    start_time: int  # minutes since midnight
+    end_time: int  # minutes since midnight
     power: int  # power in watts
     days_effective: t.Tuple[bool, bool, bool, bool, bool, bool, bool]  # Valid on days Sunday to
 
 
 PEAK_SETTING_PERIODS = 14
 
 
@@ -577,16 +579,16 @@
     def encode(self, data: list[PeakSettingPeriod], builder: BinaryPayloadBuilder):
         if len(data) > PEAK_SETTING_PERIODS:
             data = data[:PEAK_SETTING_PERIODS]
 
         builder.add_16bit_uint(len(data))
 
         for period in data:
-            builder.add_16bit_uint(period.start_time),
-            builder.add_16bit_uint(period.end_time),
+            builder.add_16bit_uint(period.start_time)
+            builder.add_16bit_uint(period.end_time)
             builder.add_32bit_uint(period.power)
             builder.add_8bit_uint(_days_effective_builder(period.days_effective))
 
         # pad with empty periods
         for _ in range(len(data), PEAK_SETTING_PERIODS):
             builder.add_16bit_uint(0)
             builder.add_16bit_uint(0)
@@ -596,39 +598,39 @@
 
 REGISTERS: dict[str, RegisterDefinition] = {
     rn.MODEL_NAME: StringRegister(30000, 15),
     rn.SERIAL_NUMBER: StringRegister(30015, 10),
     rn.PN: StringRegister(30025, 10),
     rn.FIRMWARE_VERSION: StringRegister(30035, 15),
     rn.SOFTWARE_VERSION: StringRegister(30050, 15),
-    rn.PROTOCOL_VERSION_MODBUS: U32Register(None, 1, 30068, 2),
-    rn.MODEL_ID: U16Register(None, 1, 30070, 1),
-    rn.NB_PV_STRINGS: U16Register(None, 1, 30071, 1),
-    rn.NB_MPP_TRACKS: U16Register(None, 1, 30072, 1),
-    rn.RATED_POWER: U32Register("W", 1, 30073, 2),
-    rn.P_MAX: U32Register("W", 1, 30075, 2),
-    rn.S_MAX: U32Register("VA", 1, 30077, 2),
-    rn.Q_MAX_OUT: I32Register("VAr", 1, 30079, 2),
-    rn.Q_MAX_IN: I32Register("VAr", 1, 30081, 2),
-    rn.P_MAX_REAL: U32Register("W", 1, 30083, 2),
-    rn.S_MAX_REAL: U32Register("VA", 1, 30085, 2),
+    rn.PROTOCOL_VERSION_MODBUS: U32Register(None, 1, 30068),
+    rn.MODEL_ID: U16Register(None, 1, 30070),
+    rn.NB_PV_STRINGS: U16Register(None, 1, 30071),
+    rn.NB_MPP_TRACKS: U16Register(None, 1, 30072),
+    rn.RATED_POWER: U32Register("W", 1, 30073),
+    rn.P_MAX: U32Register("W", 1, 30075),
+    rn.S_MAX: U32Register("VA", 1, 30077),
+    rn.Q_MAX_OUT: I32Register("VAr", 1, 30079),
+    rn.Q_MAX_IN: I32Register("VAr", 1, 30081),
+    rn.P_MAX_REAL: U32Register("W", 1, 30083),
+    rn.S_MAX_REAL: U32Register("VA", 1, 30085),
     rn.PRODUCT_SALES_AREA: StringRegister(30105, 2),
-    rn.PRODUCT_SOFTWARE_NUMBER: U16Register(None, 1, 30107, 1),
-    rn.PRODUCT_SOFTWARE_VERSION_NUMBER: U16Register(None, 1, 30108, 1),
-    rn.GRID_STANDARD_CODE_PROTOCOL_VERSION: U16Register(None, 1, 30110, 1),
-    rn.NUMBER_OF_PACKAGES_TO_BE_UPGRADED: U16Register(None, 1, 30111, 1),
-    rn.HARDWARE_FUNCTIONAL_UNIT_CONF_ID: U16Register(None, 1, 30206, 1),
-    rn.SUBDEVICE_SUPPORT_FLAG: U32Register(None, 1, 30207, 2),
-    rn.SUBDEVICE_IN_POSITION_FLAG: U32Register(None, 1, 30209, 2),
-    rn.FEATURE_MASK_1: U32Register(None, 1, 30211, 2),
-    rn.FEATURE_MASK_2: U32Register(None, 1, 30213, 2),
-    rn.FEATURE_MASK_3: U32Register(None, 1, 30215, 2),
-    rn.FEATURE_MASK_4: U32Register(None, 1, 30217, 2),
-    rn.REALTIME_MAX_ACTIVE_CAPABILITY: I32Register(None, 1, 30366, 2),
-    rn.REALTIME_MAX_INDUCTIVE_REACTIVE_CAPACITY: I32Register(None, 1, 30368, 2),
+    rn.PRODUCT_SOFTWARE_NUMBER: U16Register(None, 1, 30107),
+    rn.PRODUCT_SOFTWARE_VERSION_NUMBER: U16Register(None, 1, 30108),
+    rn.GRID_STANDARD_CODE_PROTOCOL_VERSION: U16Register(None, 1, 30110),
+    rn.NUMBER_OF_PACKAGES_TO_BE_UPGRADED: U16Register(None, 1, 30111),
+    rn.HARDWARE_FUNCTIONAL_UNIT_CONF_ID: U16Register(None, 1, 30206),
+    rn.SUBDEVICE_SUPPORT_FLAG: U32Register(None, 1, 30207),
+    rn.SUBDEVICE_IN_POSITION_FLAG: U32Register(None, 1, 30209),
+    rn.FEATURE_MASK_1: U32Register(None, 1, 30211),
+    rn.FEATURE_MASK_2: U32Register(None, 1, 30213),
+    rn.FEATURE_MASK_3: U32Register(None, 1, 30215),
+    rn.FEATURE_MASK_4: U32Register(None, 1, 30217),
+    rn.REALTIME_MAX_ACTIVE_CAPABILITY: I32Register(None, 1, 30366),
+    rn.REALTIME_MAX_INDUCTIVE_REACTIVE_CAPACITY: I32Register(None, 1, 30368),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_1: StringRegister(30561, 15),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_2: StringRegister(30576, 15),
     rn.OFFERING_NAME_OF_SOUTHBOUND_DEVICE_3: StringRegister(30591, 15),
     rn.HARDWARE_VERSION: StringRegister(31000, 15),
     rn.MONITORING_BOARD_SN: StringRegister(31015, 10),
     rn.MONITORING_SOFTWARE_VERSION: StringRegister(31025, 15),
     rn.MASTER_DSP_VERSION: StringRegister(31040, 15),
@@ -636,359 +638,371 @@
     rn.CPLD_VERSION: StringRegister(31070, 15),
     rn.AFCI_VERSION: StringRegister(31085, 15),
     rn.BUILTIN_PID_VERSION: StringRegister(31100, 15),
     rn.DC_MBUS_VERSION: StringRegister(31115, 15),
     rn.EL_MODULE_VERSION: StringRegister(31130, 15),
     rn.AFCI_2_VERSION: StringRegister(31145, 15),
     rn.REGKEY: StringRegister(31200, 10),
-    rn.STATE_1: U16Register(partial(bitfield_decoder, rv.STATE_CODES_1), 1, 32000, 1),
-    rn.STATE_2: U16Register(partial(bitfield_decoder, rv.STATE_CODES_2), 1, 32002, 1),
-    rn.STATE_3: U32Register(partial(bitfield_decoder, rv.STATE_CODES_3), 1, 32003, 2),
-    rn.ALARM_1: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_1), 1, 32008, 1, ignore_invalid=True),
-    rn.ALARM_2: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_2), 1, 32009, 1, ignore_invalid=True),
-    rn.ALARM_3: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_3), 1, 32010, 1),
-    rn.INPUT_POWER: I32Register("W", 1, 32064, 2),
-    rn.GRID_VOLTAGE: U16Register("V", 10, 32066, 1),
-    rn.LINE_VOLTAGE_A_B: U16Register("V", 10, 32066, 1),
-    rn.LINE_VOLTAGE_B_C: U16Register("V", 10, 32067, 1),
-    rn.LINE_VOLTAGE_C_A: U16Register("V", 10, 32068, 1),
-    rn.PHASE_A_VOLTAGE: U16Register("V", 10, 32069, 1),
-    rn.PHASE_B_VOLTAGE: U16Register("V", 10, 32070, 1),
-    rn.PHASE_C_VOLTAGE: U16Register("V", 10, 32071, 1),
-    rn.GRID_CURRENT: I32Register("A", 1000, 32072, 2),
-    rn.PHASE_A_CURRENT: I32Register("A", 1000, 32072, 2),
-    rn.PHASE_B_CURRENT: I32Register("A", 1000, 32074, 2),
-    rn.PHASE_C_CURRENT: I32Register("A", 1000, 32076, 2),
-    rn.DAY_ACTIVE_POWER_PEAK: I32Register("W", 1, 32078, 2),
-    rn.ACTIVE_POWER: I32Register("W", 1, 32080, 2),
-    rn.REACTIVE_POWER: I32Register("VA", 1, 32082, 2),
-    rn.POWER_FACTOR: I16Register(None, 1000, 32084, 1),
-    rn.GRID_FREQUENCY: U16Register("Hz", 100, 32085, 1),
-    rn.EFFICIENCY: U16Register("%", 100, 32086, 1),
-    rn.INTERNAL_TEMPERATURE: I16Register("°C", 10, 32087, 1),
-    rn.INSULATION_RESISTANCE: U16Register("MOhm", 100, 32088, 1),
-    rn.DEVICE_STATUS: U16Register(rv.DEVICE_STATUS_DEFINITIONS, 1, 32089, 1),
-    rn.FAULT_CODE: U16Register(None, 1, 32090, 1),
-    rn.STARTUP_TIME: TimestampRegister(32091, 2),
-    rn.SHUTDOWN_TIME: TimestampRegister(32093, 2),
-    rn.ACTIVE_POWER_FAST: I32Register("W", 1, 32095, 2),
-    rn.ACCUMULATED_YIELD_ENERGY: U32Register("kWh", 100, 32106, 2),
-    rn.TOTAL_DC_INPUT_POWER: U32Register("kWh", 100, 32108, 2),
-    rn.CURRENT_ELECTRICITY_GENERATION_STATISTICS_TIME: TimestampRegister(32110, 2),
-    rn.HOURLY_YIELD_ENERGY: U32Register("kWh", 100, 32112, 2),
-    rn.DAILY_YIELD_ENERGY: U32Register("kWh", 100, 32114, 2),
-    rn.MONTHLY_YIELD_ENERGY: U32Register("kWh", 100, 32116, 2),
-    rn.YEARLY_YIELD_ENERGY: U32Register("kWh", 100, 32118, 2),
-    rn.LATEST_ACTIVE_ALARM_SN: U32Register(None, 1, 32172, 2),
-    rn.LATEST_HISTORICAL_ALARM_SN: U32Register(None, 1, 32174, 2),
-    rn.TOTAL_BUS_VOLTAGE: I16Register("V", 10, 32176, 1),
-    rn.MAX_PV_VOLTAGE: I16Register("V", 10, 32177, 1),
-    rn.MIN_PV_VOLTAGE: I16Register("V", 10, 32178, 1),
-    rn.AVERAGE_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32179, 1),
-    rn.MIN_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32180, 1),
-    rn.MAX_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32181, 1),
-    rn.INVERTER_TO_PE_VOLTAGE_TOLERANCE: U16Register("V", 1, 32182, 1),
-    rn.ISO_FEATURE_INFORMATION: U16Register(None, 1, 32183, 1),
-    rn.BUILTIN_PID_RUNNING_STATUS: U16Register(None, 1, 32190, 1),
-    rn.PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32191, 1),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT1: U32Register("kWh", 100, 32212, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT2: U32Register("kWh", 100, 32214, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT3: U32Register("kWh", 100, 32216, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT4: U32Register("kWh", 100, 32218, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT5: U32Register("kWh", 100, 32220, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT6: U32Register("kWh", 100, 32222, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT7: U32Register("kWh", 100, 32224, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT8: U32Register("kWh", 100, 32226, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT9: U32Register("kWh", 100, 32228, 2),
-    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT10: U32Register("kWh", 100, 32230, 2),
-    rn.CAPBANK_RUNNING_TIME: U32Register("hour", 10, 35000, 2),  # SUN2000MA-only register
-    rn.INTERNAL_FAN_1_RUNNING_TIME: U32Register("hour", 10, 35002, 2),  # SUN2000MA-only register
-    rn.INV_MODULE_A_TEMP: I16Register("°C", 10, 35021, 1),  # SUN2000MA-only register
-    rn.INV_MODULE_B_TEMP: I16Register("°C", 10, 35022, 1),  # SUN2000MA-only register
-    rn.INV_MODULE_C_TEMP: I16Register("°C", 10, 35023, 1),  # SUN2000MA-only register
-    rn.ANTI_REVERSE_MODULE_1_TEMP: I16Register("°C", 10, 35024, 1),  # SUN2000MA-only register
-    rn.OUTPUT_BOARD_RELAY_AMBIENT_TEMP_MAX: I16Register("°C", 10, 35025, 1),  # SUN2000MA-only register
-    rn.ANTI_REVERSE_MODULE_2_TEMP: I16Register("°C", 10, 35027, 1),  # SUN2000MA-only register
-    rn.DC_TERMINAL_1_2_MAX_TEMP: I16Register("°C", 10, 35028, 1),  # SUN2000MA-only register
-    rn.AC_TERMINAL_1_2_3_MAX_TEMP: I16Register("°C", 10, 35029, 1),  # SUN2000MA-only register
-    rn.PHASE_A_DC_COMPONENT_DCI: I16Register("A", 1000, 35038, 1),  # SUN2000MA-only register
-    rn.PHASE_B_DC_COMPONENT_DCI: I16Register("A", 1000, 35039, 1),  # SUN2000MA-only register
-    rn.PHASE_C_DC_COMPONENT_DCI: I16Register("A", 1000, 35040, 1),  # SUN2000MA-only register
-    rn.LEAKAGE_CURRENT_RCD: I16Register("mA", 1, 35041, 1),  # SUN2000MA-only register
-    rn.POSITIVE_BUS_VOLTAGE: I16Register("V", 10, 35042, 1),  # SUN2000MA-only register
-    rn.NEGATIVE_BUS_VOLTAGE: I16Register("V", 10, 35043, 1),  # SUN2000MA-only register
-    rn.BUS_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 35044, 1),  # SUN2000MA-only register
-    rn.NB_OPTIMIZERS: U16Register(None, 1, 37200, 1),
-    rn.NB_ONLINE_OPTIMIZERS: U16Register(None, 1, 37201, 1),
-    rn.SYSTEM_TIME: TimestampRegister(40000, 2),
-    rn.SYSTEM_TIME_RAW: U32Register("seconds", 1, 40000, 2),
-    rn.STARTUP: U16Register(None, 1, 40200, 1, writeable=True, readable=False),
-    rn.SHUTDOWN: U16Register(None, 1, 40201, 1, writeable=True, readable=False),
-    rn.GRID_CODE: U16Register(rv.GRID_CODES, 1, 42000, 1),
-    rn.MPPT_MULTIMODAL_SCANNING: U16Register(bool, 1, 42054, 1, writeable=True),
-    rn.MPPT_SCANNING_INTERVAL: U16Register("minutes", 1, 42055, 1, writeable=True),
-    rn.MPPT_PREDICTED_POWER: U32Register("W", 1, 42056, 2),
-    rn.TIME_ZONE: I16Register("min", 1, 43006, 1, writeable=True),
-    rn.WLAN_WAKEUP: I16Register(rv.WlanWakeup, 1, 45052, 1, writeable=True),
+    rn.STATE_1: U16Register(partial(bitfield_decoder, rv.STATE_CODES_1), 1, 32000),
+    rn.STATE_2: U16Register(partial(bitfield_decoder, rv.STATE_CODES_2), 1, 32002),
+    rn.STATE_3: U32Register(partial(bitfield_decoder, rv.STATE_CODES_3), 1, 32003),
+    rn.ALARM_1: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_1), 1, 32008, ignore_invalid=True),
+    rn.ALARM_2: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_2), 1, 32009, ignore_invalid=True),
+    rn.ALARM_3: U16Register(partial(bitfield_decoder, rv.ALARM_CODES_3), 1, 32010),
+    rn.INPUT_POWER: I32Register("W", 1, 32064),
+    rn.GRID_VOLTAGE: U16Register("V", 10, 32066),
+    rn.LINE_VOLTAGE_A_B: U16Register("V", 10, 32066),
+    rn.LINE_VOLTAGE_B_C: U16Register("V", 10, 32067),
+    rn.LINE_VOLTAGE_C_A: U16Register("V", 10, 32068),
+    rn.PHASE_A_VOLTAGE: U16Register("V", 10, 32069),
+    rn.PHASE_B_VOLTAGE: U16Register("V", 10, 32070),
+    rn.PHASE_C_VOLTAGE: U16Register("V", 10, 32071),
+    rn.GRID_CURRENT: I32Register("A", 1000, 32072),
+    rn.PHASE_A_CURRENT: I32Register("A", 1000, 32072),
+    rn.PHASE_B_CURRENT: I32Register("A", 1000, 32074),
+    rn.PHASE_C_CURRENT: I32Register("A", 1000, 32076),
+    rn.DAY_ACTIVE_POWER_PEAK: I32Register("W", 1, 32078),
+    rn.ACTIVE_POWER: I32Register("W", 1, 32080),
+    rn.REACTIVE_POWER: I32Register("VA", 1, 32082),
+    rn.POWER_FACTOR: I16Register(None, 1000, 32084),
+    rn.GRID_FREQUENCY: U16Register("Hz", 100, 32085),
+    rn.EFFICIENCY: U16Register("%", 100, 32086),
+    rn.INTERNAL_TEMPERATURE: I16Register("°C", 10, 32087),
+    rn.INSULATION_RESISTANCE: U16Register("MOhm", 100, 32088),
+    rn.DEVICE_STATUS: U16Register(rv.DEVICE_STATUS_DEFINITIONS, 1, 32089),
+    rn.FAULT_CODE: U16Register(None, 1, 32090),
+    rn.STARTUP_TIME: TimestampRegister(32091),
+    rn.SHUTDOWN_TIME: TimestampRegister(32093),
+    rn.ACTIVE_POWER_FAST: I32Register("W", 1, 32095),
+    rn.ACCUMULATED_YIELD_ENERGY: U32Register("kWh", 100, 32106),
+    rn.TOTAL_DC_INPUT_POWER: U32Register("kWh", 100, 32108),
+    rn.CURRENT_ELECTRICITY_GENERATION_STATISTICS_TIME: TimestampRegister(32110),
+    rn.HOURLY_YIELD_ENERGY: U32Register("kWh", 100, 32112),
+    rn.DAILY_YIELD_ENERGY: U32Register("kWh", 100, 32114),
+    rn.MONTHLY_YIELD_ENERGY: U32Register("kWh", 100, 32116),
+    rn.YEARLY_YIELD_ENERGY: U32Register("kWh", 100, 32118),
+    rn.LATEST_ACTIVE_ALARM_SN: U32Register(None, 1, 32172),
+    rn.LATEST_HISTORICAL_ALARM_SN: U32Register(None, 1, 32174),
+    rn.TOTAL_BUS_VOLTAGE: I16Register("V", 10, 32176),
+    rn.MAX_PV_VOLTAGE: I16Register("V", 10, 32177),
+    rn.MIN_PV_VOLTAGE: I16Register("V", 10, 32178),
+    rn.AVERAGE_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32179),
+    rn.MIN_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32180),
+    rn.MAX_PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32181),
+    rn.INVERTER_TO_PE_VOLTAGE_TOLERANCE: U16Register("V", 1, 32182),
+    rn.ISO_FEATURE_INFORMATION: U16Register(None, 1, 32183),
+    rn.BUILTIN_PID_RUNNING_STATUS: U16Register(None, 1, 32190),
+    rn.PV_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 32191),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT1: U32Register("kWh", 100, 32212),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT2: U32Register("kWh", 100, 32214),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT3: U32Register("kWh", 100, 32216),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT4: U32Register("kWh", 100, 32218),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT5: U32Register("kWh", 100, 32220),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT6: U32Register("kWh", 100, 32222),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT7: U32Register("kWh", 100, 32224),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT8: U32Register("kWh", 100, 32226),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT9: U32Register("kWh", 100, 32228),
+    rn.CUMULATIVE_DC_ENERGY_YIELD_MPPT10: U32Register("kWh", 100, 32230),
+    rn.CAPBANK_RUNNING_TIME: U32Register("hour", 10, 35000),  # SUN2000MA-only register
+    rn.INTERNAL_FAN_1_RUNNING_TIME: U32Register("hour", 10, 35002),  # SUN2000MA-only register
+    rn.INV_MODULE_A_TEMP: I16Register("°C", 10, 35021),  # SUN2000MA-only register
+    rn.INV_MODULE_B_TEMP: I16Register("°C", 10, 35022),  # SUN2000MA-only register
+    rn.INV_MODULE_C_TEMP: I16Register("°C", 10, 35023),  # SUN2000MA-only register
+    rn.ANTI_REVERSE_MODULE_1_TEMP: I16Register("°C", 10, 35024),  # SUN2000MA-only register
+    rn.OUTPUT_BOARD_RELAY_AMBIENT_TEMP_MAX: I16Register("°C", 10, 35025),  # SUN2000MA-only register
+    rn.ANTI_REVERSE_MODULE_2_TEMP: I16Register("°C", 10, 35027),  # SUN2000MA-only register
+    rn.DC_TERMINAL_1_2_MAX_TEMP: I16Register("°C", 10, 35028),  # SUN2000MA-only register
+    rn.AC_TERMINAL_1_2_3_MAX_TEMP: I16Register("°C", 10, 35029),  # SUN2000MA-only register
+    rn.PHASE_A_DC_COMPONENT_DCI: I16Register("A", 1000, 35038),  # SUN2000MA-only register
+    rn.PHASE_B_DC_COMPONENT_DCI: I16Register("A", 1000, 35039),  # SUN2000MA-only register
+    rn.PHASE_C_DC_COMPONENT_DCI: I16Register("A", 1000, 35040),  # SUN2000MA-only register
+    rn.LEAKAGE_CURRENT_RCD: I16Register("mA", 1, 35041),  # SUN2000MA-only register
+    rn.POSITIVE_BUS_VOLTAGE: I16Register("V", 10, 35042),  # SUN2000MA-only register
+    rn.NEGATIVE_BUS_VOLTAGE: I16Register("V", 10, 35043),  # SUN2000MA-only register
+    rn.BUS_NEGATIVE_VOLTAGE_TO_GROUND: I16Register("V", 10, 35044),  # SUN2000MA-only register
+    rn.NB_OPTIMIZERS: U16Register(None, 1, 37200),
+    rn.NB_ONLINE_OPTIMIZERS: U16Register(None, 1, 37201),
+    rn.SYSTEM_TIME: TimestampRegister(40000),
+    rn.SYSTEM_TIME_RAW: U32Register("seconds", 1, 40000),
+    rn.Q_U_CHARACTERISTIC_CURVE_MODEL: U16Register(
+        None, 1, 40037, writeable=True
+    ),  # Documented as 'E16' instead of 'U16'
+    rn.Q_U_SCHEDULING_TRIGGER_POWER_PERCENTAGE: I16Register(None, 1, 40038, writeable=True),
+    rn.POWER_FACTOR_2: I16Register(None, 1000, 40122, writeable=True),
+    rn.REACTIVE_POWER_COMPENSATION: I16Register(None, 1000, 40123, writeable=True),
+    rn.REACTIVE_POWER_ADJUSTMENT_TIME: U16Register("seconds", 1, 40124, writeable=True),
+    rn.ACTIVE_POWER_PERCENTAGE_DERATING: I16Register("%", 10, 40125, writeable=True),
+    rn.ACTIVE_POWER_FIXED_VALUE_DERATING: U32Register("W", 1, 40126, writeable=True),
+    rn.REACTIVE_POWER_COMPENSATION_AT_NIGHT: I16Register(None, 1000, 40128, writeable=True),
+    rn.FIXED_REACTIVE_POWER_AT_NIGHT: I32Register("Var", 1000, 40129, writeable=True),
+    rn.CHARACTERISTIC_CURVE_REACTIVE_POWER_ADJUSTMENT_TIME: U16Register("seconds", 1, 40196, writeable=True),
+    rn.PERCENT_APPARENT_POWER: U16Register("%", 10, 40197, writeable=True),
+    rn.Q_U_SCHEDULING_EXIT_POWER_PERCENTAGE: I16Register("%", 1, 40198, writeable=True),
+    rn.STARTUP: U16Register(None, 1, 40200, writeable=True, readable=False),
+    rn.SHUTDOWN: U16Register(None, 1, 40201, writeable=True, readable=False),
+    rn.GRID_CODE: U16Register(rv.GRID_CODES, 1, 42000),
+    rn.MPPT_MULTIMODAL_SCANNING: U16Register(bool, 1, 42054, writeable=True),
+    rn.MPPT_SCANNING_INTERVAL: U16Register("minutes", 1, 42055, writeable=True),
+    rn.MPPT_PREDICTED_POWER: U32Register("W", 1, 42056),
+    rn.TIME_ZONE: I16Register("min", 1, 43006, writeable=True),
+    rn.WLAN_WAKEUP: I16Register(rv.WlanWakeup, 1, 45052, writeable=True),
 }
 
 
 PV_REGISTERS = {
-    rn.PV_01_VOLTAGE: I16Register("V", 10, 32016, 1),
-    rn.PV_01_CURRENT: I16Register("A", 100, 32017, 1),
-    rn.PV_02_VOLTAGE: I16Register("V", 10, 32018, 1),
-    rn.PV_02_CURRENT: I16Register("A", 100, 32019, 1),
-    rn.PV_03_VOLTAGE: I16Register("V", 10, 32020, 1),
-    rn.PV_03_CURRENT: I16Register("A", 100, 32021, 1),
-    rn.PV_04_VOLTAGE: I16Register("V", 10, 32022, 1),
-    rn.PV_04_CURRENT: I16Register("A", 100, 32023, 1),
-    rn.PV_05_VOLTAGE: I16Register("V", 10, 32024, 1),
-    rn.PV_05_CURRENT: I16Register("A", 100, 32025, 1),
-    rn.PV_06_VOLTAGE: I16Register("V", 10, 32026, 1),
-    rn.PV_06_CURRENT: I16Register("A", 100, 32027, 1),
-    rn.PV_07_VOLTAGE: I16Register("V", 10, 32028, 1),
-    rn.PV_07_CURRENT: I16Register("A", 100, 32029, 1),
-    rn.PV_08_VOLTAGE: I16Register("V", 10, 32030, 1),
-    rn.PV_08_CURRENT: I16Register("A", 100, 32031, 1),
-    rn.PV_09_VOLTAGE: I16Register("V", 10, 32032, 1),
-    rn.PV_09_CURRENT: I16Register("A", 100, 32033, 1),
-    rn.PV_10_VOLTAGE: I16Register("V", 10, 32034, 1),
-    rn.PV_10_CURRENT: I16Register("A", 100, 32035, 1),
-    rn.PV_11_VOLTAGE: I16Register("V", 10, 32036, 1),
-    rn.PV_11_CURRENT: I16Register("A", 100, 32037, 1),
-    rn.PV_12_VOLTAGE: I16Register("V", 10, 32038, 1),
-    rn.PV_12_CURRENT: I16Register("A", 100, 32039, 1),
-    rn.PV_13_VOLTAGE: I16Register("V", 10, 32040, 1),
-    rn.PV_13_CURRENT: I16Register("A", 100, 32041, 1),
-    rn.PV_14_VOLTAGE: I16Register("V", 10, 32042, 1),
-    rn.PV_14_CURRENT: I16Register("A", 100, 32043, 1),
-    rn.PV_15_VOLTAGE: I16Register("V", 10, 32044, 1),
-    rn.PV_15_CURRENT: I16Register("A", 100, 32045, 1),
-    rn.PV_16_VOLTAGE: I16Register("V", 10, 32046, 1),
-    rn.PV_16_CURRENT: I16Register("A", 100, 32047, 1),
-    rn.PV_17_VOLTAGE: I16Register("V", 10, 32048, 1),
-    rn.PV_17_CURRENT: I16Register("A", 100, 32049, 1),
-    rn.PV_18_VOLTAGE: I16Register("V", 10, 32050, 1),
-    rn.PV_18_CURRENT: I16Register("A", 100, 32051, 1),
-    rn.PV_19_VOLTAGE: I16Register("V", 10, 32052, 1),
-    rn.PV_19_CURRENT: I16Register("A", 100, 32053, 1),
-    rn.PV_20_VOLTAGE: I16Register("V", 10, 32054, 1),
-    rn.PV_20_CURRENT: I16Register("A", 100, 32055, 1),
-    rn.PV_21_VOLTAGE: I16Register("V", 10, 32056, 1),
-    rn.PV_21_CURRENT: I16Register("A", 100, 32057, 1),
-    rn.PV_22_VOLTAGE: I16Register("V", 10, 32058, 1),
-    rn.PV_22_CURRENT: I16Register("A", 100, 32059, 1),
-    rn.PV_23_VOLTAGE: I16Register("V", 10, 32060, 1),
-    rn.PV_23_CURRENT: I16Register("A", 100, 32061, 1),
-    rn.PV_24_VOLTAGE: I16Register("V", 10, 32062, 1),
-    rn.PV_24_CURRENT: I16Register("A", 100, 32063, 1),
+    rn.PV_01_VOLTAGE: I16Register("V", 10, 32016),
+    rn.PV_01_CURRENT: I16Register("A", 100, 32017),
+    rn.PV_02_VOLTAGE: I16Register("V", 10, 32018),
+    rn.PV_02_CURRENT: I16Register("A", 100, 32019),
+    rn.PV_03_VOLTAGE: I16Register("V", 10, 32020),
+    rn.PV_03_CURRENT: I16Register("A", 100, 32021),
+    rn.PV_04_VOLTAGE: I16Register("V", 10, 32022),
+    rn.PV_04_CURRENT: I16Register("A", 100, 32023),
+    rn.PV_05_VOLTAGE: I16Register("V", 10, 32024),
+    rn.PV_05_CURRENT: I16Register("A", 100, 32025),
+    rn.PV_06_VOLTAGE: I16Register("V", 10, 32026),
+    rn.PV_06_CURRENT: I16Register("A", 100, 32027),
+    rn.PV_07_VOLTAGE: I16Register("V", 10, 32028),
+    rn.PV_07_CURRENT: I16Register("A", 100, 32029),
+    rn.PV_08_VOLTAGE: I16Register("V", 10, 32030),
+    rn.PV_08_CURRENT: I16Register("A", 100, 32031),
+    rn.PV_09_VOLTAGE: I16Register("V", 10, 32032),
+    rn.PV_09_CURRENT: I16Register("A", 100, 32033),
+    rn.PV_10_VOLTAGE: I16Register("V", 10, 32034),
+    rn.PV_10_CURRENT: I16Register("A", 100, 32035),
+    rn.PV_11_VOLTAGE: I16Register("V", 10, 32036),
+    rn.PV_11_CURRENT: I16Register("A", 100, 32037),
+    rn.PV_12_VOLTAGE: I16Register("V", 10, 32038),
+    rn.PV_12_CURRENT: I16Register("A", 100, 32039),
+    rn.PV_13_VOLTAGE: I16Register("V", 10, 32040),
+    rn.PV_13_CURRENT: I16Register("A", 100, 32041),
+    rn.PV_14_VOLTAGE: I16Register("V", 10, 32042),
+    rn.PV_14_CURRENT: I16Register("A", 100, 32043),
+    rn.PV_15_VOLTAGE: I16Register("V", 10, 32044),
+    rn.PV_15_CURRENT: I16Register("A", 100, 32045),
+    rn.PV_16_VOLTAGE: I16Register("V", 10, 32046),
+    rn.PV_16_CURRENT: I16Register("A", 100, 32047),
+    rn.PV_17_VOLTAGE: I16Register("V", 10, 32048),
+    rn.PV_17_CURRENT: I16Register("A", 100, 32049),
+    rn.PV_18_VOLTAGE: I16Register("V", 10, 32050),
+    rn.PV_18_CURRENT: I16Register("A", 100, 32051),
+    rn.PV_19_VOLTAGE: I16Register("V", 10, 32052),
+    rn.PV_19_CURRENT: I16Register("A", 100, 32053),
+    rn.PV_20_VOLTAGE: I16Register("V", 10, 32054),
+    rn.PV_20_CURRENT: I16Register("A", 100, 32055),
+    rn.PV_21_VOLTAGE: I16Register("V", 10, 32056),
+    rn.PV_21_CURRENT: I16Register("A", 100, 32057),
+    rn.PV_22_VOLTAGE: I16Register("V", 10, 32058),
+    rn.PV_22_CURRENT: I16Register("A", 100, 32059),
+    rn.PV_23_VOLTAGE: I16Register("V", 10, 32060),
+    rn.PV_23_CURRENT: I16Register("A", 100, 32061),
+    rn.PV_24_VOLTAGE: I16Register("V", 10, 32062),
+    rn.PV_24_CURRENT: I16Register("A", 100, 32063),
 }
 
 REGISTERS.update(PV_REGISTERS)
 
 BATTERY_REGISTERS = {
-    rn.STORAGE_UNIT_1_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37000, 1),
-    rn.STORAGE_UNIT_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37001, 2),
-    rn.STORAGE_UNIT_1_BUS_VOLTAGE: U16Register("V", 10, 37003, 1),
-    rn.STORAGE_UNIT_1_STATE_OF_CAPACITY: U16Register("%", 10, 37004, 1),
-    rn.STORAGE_UNIT_1_WORKING_MODE_B: U16Register(rv.StorageWorkingModesB, 1, 37006, 1),
-    rn.STORAGE_UNIT_1_RATED_CHARGE_POWER: U32Register("W", 1, 37007, 2),
-    rn.STORAGE_UNIT_1_RATED_DISCHARGE_POWER: U32Register("W", 1, 37009, 2),
-    rn.STORAGE_UNIT_1_FAULT_ID: U16Register(None, 1, 37014, 1),
-    rn.STORAGE_UNIT_1_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37015, 2),
-    rn.STORAGE_UNIT_1_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37017, 2),
-    rn.STORAGE_UNIT_1_BUS_CURRENT: I16Register("A", 10, 37021, 1),
-    rn.STORAGE_UNIT_1_BATTERY_TEMPERATURE: I16Register("°C", 10, 37022, 1),
-    rn.STORAGE_UNIT_1_REMAINING_CHARGE_DIS_CHARGE_TIME: U16Register("min", 1, 37025, 1),
+    rn.STORAGE_UNIT_1_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37000),
+    rn.STORAGE_UNIT_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37001),
+    rn.STORAGE_UNIT_1_BUS_VOLTAGE: U16Register("V", 10, 37003),
+    rn.STORAGE_UNIT_1_STATE_OF_CAPACITY: U16Register("%", 10, 37004),
+    rn.STORAGE_UNIT_1_WORKING_MODE_B: U16Register(rv.StorageWorkingModesB, 1, 37006),
+    rn.STORAGE_UNIT_1_RATED_CHARGE_POWER: U32Register("W", 1, 37007),
+    rn.STORAGE_UNIT_1_RATED_DISCHARGE_POWER: U32Register("W", 1, 37009),
+    rn.STORAGE_UNIT_1_FAULT_ID: U16Register(None, 1, 37014),
+    rn.STORAGE_UNIT_1_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37015),
+    rn.STORAGE_UNIT_1_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37017),
+    rn.STORAGE_UNIT_1_BUS_CURRENT: I16Register("A", 10, 37021),
+    rn.STORAGE_UNIT_1_BATTERY_TEMPERATURE: I16Register("°C", 10, 37022),
+    rn.STORAGE_UNIT_1_REMAINING_CHARGE_DIS_CHARGE_TIME: U16Register("min", 1, 37025),
     rn.STORAGE_UNIT_1_DCDC_VERSION: StringRegister(37026, 10),
     rn.STORAGE_UNIT_1_BMS_VERSION: StringRegister(37036, 10),
-    rn.STORAGE_MAXIMUM_CHARGE_POWER: U32Register("W", 1, 37046, 2),
-    rn.STORAGE_MAXIMUM_DISCHARGE_POWER: U32Register("W", 1, 37048, 2),
+    rn.STORAGE_MAXIMUM_CHARGE_POWER: U32Register("W", 1, 37046),
+    rn.STORAGE_MAXIMUM_DISCHARGE_POWER: U32Register("W", 1, 37048),
     rn.STORAGE_UNIT_1_SERIAL_NUMBER: StringRegister(37052, 10),
-    rn.STORAGE_UNIT_1_TOTAL_CHARGE: U32Register("kWh", 100, 37066, 2),
-    rn.STORAGE_UNIT_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 37068, 2),
+    rn.STORAGE_UNIT_1_TOTAL_CHARGE: U32Register("kWh", 100, 37066),
+    rn.STORAGE_UNIT_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 37068),
     rn.STORAGE_UNIT_2_SERIAL_NUMBER: StringRegister(37700, 10),
-    rn.STORAGE_UNIT_2_STATE_OF_CAPACITY: U16Register("%", 10, 37738, 1),
-    rn.STORAGE_UNIT_2_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37741, 1),
-    rn.STORAGE_UNIT_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37743, 2),
-    rn.STORAGE_UNIT_2_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37746, 2),
-    rn.STORAGE_UNIT_2_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37748, 2),
-    rn.STORAGE_UNIT_2_BUS_VOLTAGE: U16Register("V", 10, 37750, 1),
-    rn.STORAGE_UNIT_2_BUS_CURRENT: I16Register("A", 10, 37751, 1),
-    rn.STORAGE_UNIT_2_BATTERY_TEMPERATURE: I16Register("°C", 10, 37752, 1),
-    rn.STORAGE_UNIT_2_TOTAL_CHARGE: U32Register("kWh", 100, 37753, 2),
-    rn.STORAGE_UNIT_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 37755, 2),
-    rn.STORAGE_RATED_CAPACITY: U32Register("Wh", 1, 37758, 2),
-    rn.STORAGE_STATE_OF_CAPACITY: U16Register("%", 10, 37760, 1),
-    rn.STORAGE_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37762, 1),
-    rn.STORAGE_BUS_VOLTAGE: U16Register("V", 10, 37763, 1),
-    rn.STORAGE_BUS_CURRENT: I16Register("A", 10, 37764, 1),
-    rn.STORAGE_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37765, 2),
-    rn.STORAGE_TOTAL_CHARGE: U32Register("kWh", 100, 37780, 2),
-    rn.STORAGE_TOTAL_DISCHARGE: U32Register("kWh", 100, 37782, 2),
-    rn.STORAGE_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37784, 2),
-    rn.STORAGE_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37786, 2),
+    rn.STORAGE_UNIT_2_STATE_OF_CAPACITY: U16Register("%", 10, 37738),
+    rn.STORAGE_UNIT_2_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37741),
+    rn.STORAGE_UNIT_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37743),
+    rn.STORAGE_UNIT_2_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37746),
+    rn.STORAGE_UNIT_2_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37748),
+    rn.STORAGE_UNIT_2_BUS_VOLTAGE: U16Register("V", 10, 37750),
+    rn.STORAGE_UNIT_2_BUS_CURRENT: I16Register("A", 10, 37751),
+    rn.STORAGE_UNIT_2_BATTERY_TEMPERATURE: I16Register("°C", 10, 37752),
+    rn.STORAGE_UNIT_2_TOTAL_CHARGE: U32Register("kWh", 100, 37753),
+    rn.STORAGE_UNIT_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 37755),
+    rn.STORAGE_RATED_CAPACITY: U32Register("Wh", 1, 37758),
+    rn.STORAGE_STATE_OF_CAPACITY: U16Register("%", 10, 37760),
+    rn.STORAGE_RUNNING_STATUS: U16Register(rv.StorageStatus, 1, 37762),
+    rn.STORAGE_BUS_VOLTAGE: U16Register("V", 10, 37763),
+    rn.STORAGE_BUS_CURRENT: I16Register("A", 10, 37764),
+    rn.STORAGE_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 37765),
+    rn.STORAGE_TOTAL_CHARGE: U32Register("kWh", 100, 37780),
+    rn.STORAGE_TOTAL_DISCHARGE: U32Register("kWh", 100, 37782),
+    rn.STORAGE_CURRENT_DAY_CHARGE_CAPACITY: U32Register("kWh", 100, 37784),
+    rn.STORAGE_CURRENT_DAY_DISCHARGE_CAPACITY: U32Register("kWh", 100, 37786),
     rn.STORAGE_UNIT_2_SOFTWARE_VERSION: StringRegister(37799, 15),
     rn.STORAGE_UNIT_1_SOFTWARE_VERSION: StringRegister(37814, 15),
     rn.STORAGE_UNIT_1_BATTERY_PACK_1_SERIAL_NUMBER: StringRegister(38200, 10),
     rn.STORAGE_UNIT_1_BATTERY_PACK_1_FIRMWARE_VERSION: StringRegister(38210, 15),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_WORKING_STATUS: U16Register(None, 1, 38228, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_STATE_OF_CAPACITY: U16Register("%", 10, 38229, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38233, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_VOLTAGE: U16Register("V", 10, 38235, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_CURRENT: I16Register("A", 10, 38236, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_TOTAL_CHARGE: U32Register("kWh", 100, 38238, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 38240, 2),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_WORKING_STATUS: U16Register(None, 1, 38228),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_STATE_OF_CAPACITY: U16Register("%", 10, 38229),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38233),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_VOLTAGE: U16Register("V", 10, 38235),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_CURRENT: I16Register("A", 10, 38236),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_TOTAL_CHARGE: U32Register("kWh", 100, 38238),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 38240),
     rn.STORAGE_UNIT_1_BATTERY_PACK_2_SERIAL_NUMBER: StringRegister(38242, 10),
     rn.STORAGE_UNIT_1_BATTERY_PACK_2_FIRMWARE_VERSION: StringRegister(38252, 15),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_WORKING_STATUS: U16Register(None, 1, 38270, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_STATE_OF_CAPACITY: U16Register("%", 10, 38271, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38275, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_VOLTAGE: U16Register("V", 10, 38277, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_CURRENT: I16Register("A", 10, 38278, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_TOTAL_CHARGE: U32Register("kWh", 100, 38280, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 38282, 2),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_WORKING_STATUS: U16Register(None, 1, 38270),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_STATE_OF_CAPACITY: U16Register("%", 10, 38271),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38275),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_VOLTAGE: U16Register("V", 10, 38277),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_CURRENT: I16Register("A", 10, 38278),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_TOTAL_CHARGE: U32Register("kWh", 100, 38280),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 38282),
     rn.STORAGE_UNIT_1_BATTERY_PACK_3_SERIAL_NUMBER: StringRegister(38284, 10),
     rn.STORAGE_UNIT_1_BATTERY_PACK_3_FIRMWARE_VERSION: StringRegister(38294, 15),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_WORKING_STATUS: U16Register(None, 1, 38312, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_STATE_OF_CAPACITY: U16Register("%", 10, 38313, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38317, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_VOLTAGE: U16Register("V", 10, 38319, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_CURRENT: I16Register("A", 10, 38320, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_TOTAL_CHARGE: U32Register("kWh", 100, 38322, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_TOTAL_DISCHARGE: U32Register("kWh", 100, 38324, 2),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_WORKING_STATUS: U16Register(None, 1, 38312),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_STATE_OF_CAPACITY: U16Register("%", 10, 38313),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38317),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_VOLTAGE: U16Register("V", 10, 38319),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_CURRENT: I16Register("A", 10, 38320),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_TOTAL_CHARGE: U32Register("kWh", 100, 38322),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_TOTAL_DISCHARGE: U32Register("kWh", 100, 38324),
     rn.STORAGE_UNIT_2_BATTERY_PACK_1_SERIAL_NUMBER: StringRegister(38326, 10),
     rn.STORAGE_UNIT_2_BATTERY_PACK_1_FIRMWARE_VERSION: StringRegister(38336, 15),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_WORKING_STATUS: U16Register(None, 1, 38354, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_STATE_OF_CAPACITY: U16Register("%", 10, 38355, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38359, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_VOLTAGE: U16Register("V", 10, 38361, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_CURRENT: I16Register("A", 10, 38362, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_TOTAL_CHARGE: U32Register("kWh", 100, 38364, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 38366, 2),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_WORKING_STATUS: U16Register(None, 1, 38354),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_STATE_OF_CAPACITY: U16Register("%", 10, 38355),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38359),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_VOLTAGE: U16Register("V", 10, 38361),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_CURRENT: I16Register("A", 10, 38362),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_TOTAL_CHARGE: U32Register("kWh", 100, 38364),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_TOTAL_DISCHARGE: U32Register("kWh", 100, 38366),
     rn.STORAGE_UNIT_2_BATTERY_PACK_2_SERIAL_NUMBER: StringRegister(38368, 10),
     rn.STORAGE_UNIT_2_BATTERY_PACK_2_FIRMWARE_VERSION: StringRegister(38378, 15),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_WORKING_STATUS: U16Register(None, 1, 38396, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_STATE_OF_CAPACITY: U16Register("%", 10, 38397, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38401, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_VOLTAGE: U16Register("V", 10, 38403, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_CURRENT: I16Register("A", 10, 38404, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_TOTAL_CHARGE: U32Register("kWh", 100, 38406, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 38408, 2),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_WORKING_STATUS: U16Register(None, 1, 38396),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_STATE_OF_CAPACITY: U16Register("%", 10, 38397),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38401),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_VOLTAGE: U16Register("V", 10, 38403),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_CURRENT: I16Register("A", 10, 38404),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_TOTAL_CHARGE: U32Register("kWh", 100, 38406),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_TOTAL_DISCHARGE: U32Register("kWh", 100, 38408),
     rn.STORAGE_UNIT_2_BATTERY_PACK_3_SERIAL_NUMBER: StringRegister(38410, 10),
     rn.STORAGE_UNIT_2_BATTERY_PACK_3_FIRMWARE_VERSION: StringRegister(38420, 15),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_WORKING_STATUS: U16Register(None, 1, 38438, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_STATE_OF_CAPACITY: U16Register("%", 10, 38439, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38443, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_VOLTAGE: U16Register("V", 10, 38445, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_CURRENT: I16Register("A", 10, 38446, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_TOTAL_CHARGE: U32Register("kWh", 100, 38448, 2),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_TOTAL_DISCHARGE: U32Register("kWh", 100, 38450, 2),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38452, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_1_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38453, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38454, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_2_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38455, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38456, 1),
-    rn.STORAGE_UNIT_1_BATTERY_PACK_3_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38457, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38458, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_1_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38459, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38460, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_2_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38461, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38462, 1),
-    rn.STORAGE_UNIT_2_BATTERY_PACK_3_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38463, 1),
-    rn.STORAGE_UNIT_1_PRODUCT_MODEL: U16Register(rv.StorageProductModel, 1, 47000, 1),
-    rn.STORAGE_WORKING_MODE_A: I16Register(rv.StorageWorkingModesA, 1, 47004, 1),
-    rn.STORAGE_TIME_OF_USE_PRICE: I16Register(bool, 1, 47027, 1),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_WORKING_STATUS: U16Register(None, 1, 38438),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_STATE_OF_CAPACITY: U16Register("%", 10, 38439),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_CHARGE_DISCHARGE_POWER: I32Register("W", 1, 38443),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_VOLTAGE: U16Register("V", 10, 38445),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_CURRENT: I16Register("A", 10, 38446),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_TOTAL_CHARGE: U32Register("kWh", 100, 38448),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_TOTAL_DISCHARGE: U32Register("kWh", 100, 38450),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38452),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_1_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38453),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38454),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_2_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38455),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38456),
+    rn.STORAGE_UNIT_1_BATTERY_PACK_3_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38457),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38458),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_1_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38459),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38460),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_2_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38461),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_MAXIMUM_TEMPERATURE: I16Register("°C", 10, 38462),
+    rn.STORAGE_UNIT_2_BATTERY_PACK_3_MINIMUM_TEMPERATURE: I16Register("°C", 10, 38463),
+    rn.STORAGE_UNIT_1_PRODUCT_MODEL: U16Register(rv.StorageProductModel, 1, 47000),
+    rn.STORAGE_WORKING_MODE_A: I16Register(rv.StorageWorkingModesA, 1, 47004),
+    rn.STORAGE_TIME_OF_USE_PRICE: I16Register(bool, 1, 47027),
     rn.STORAGE_TIME_OF_USE_PRICE_PERIODS: TimeOfUseRegisters(47028, 41, writeable=True),
-    rn.STORAGE_LCOE: U32Register(None, 1000, 47069, 2),
-    rn.STORAGE_MAXIMUM_CHARGING_POWER: U32Register("W", 1, 47075, 2, writeable=True),
-    rn.STORAGE_MAXIMUM_DISCHARGING_POWER: U32Register("W", 1, 47077, 2, writeable=True),
-    rn.STORAGE_POWER_LIMIT_GRID_TIED_POINT: I32Register("W", 1, 47079, 2),
-    rn.STORAGE_CHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47081, 1, writeable=True),
-    rn.STORAGE_DISCHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47082, 1, writeable=True),
-    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_PERIOD: U16Register("min", 1, 47083, 1, writeable=True),
-    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_POWER: I32Register("W", 1, 47084, 2),
-    rn.STORAGE_WORKING_MODE_SETTINGS: U16Register(rv.StorageWorkingModesC, 1, 47086, 1, writeable=True),
-    rn.STORAGE_CHARGE_FROM_GRID_FUNCTION: U16Register(bool, 1, 47087, 1, writeable=True),
-    rn.STORAGE_GRID_CHARGE_CUTOFF_STATE_OF_CHARGE: U16Register("%", 10, 47088, 1, writeable=True),
-    rn.STORAGE_UNIT_2_PRODUCT_MODEL: U16Register(rv.StorageProductModel, 1, 47089, 1),
+    rn.STORAGE_LCOE: U32Register(None, 1000, 47069),
+    rn.STORAGE_MAXIMUM_CHARGING_POWER: U32Register("W", 1, 47075, writeable=True),
+    rn.STORAGE_MAXIMUM_DISCHARGING_POWER: U32Register("W", 1, 47077, writeable=True),
+    rn.STORAGE_POWER_LIMIT_GRID_TIED_POINT: I32Register("W", 1, 47079),
+    rn.STORAGE_CHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47081, writeable=True),
+    rn.STORAGE_DISCHARGING_CUTOFF_CAPACITY: U16Register("%", 10, 47082, writeable=True),
+    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_PERIOD: U16Register("min", 1, 47083, writeable=True),
+    rn.STORAGE_FORCED_CHARGING_AND_DISCHARGING_POWER: I32Register("W", 1, 47084),
+    rn.STORAGE_WORKING_MODE_SETTINGS: U16Register(rv.StorageWorkingModesC, 1, 47086, writeable=True),
+    rn.STORAGE_CHARGE_FROM_GRID_FUNCTION: U16Register(bool, 1, 47087, writeable=True),
+    rn.STORAGE_GRID_CHARGE_CUTOFF_STATE_OF_CHARGE: U16Register("%", 10, 47088, writeable=True),
+    rn.STORAGE_UNIT_2_PRODUCT_MODEL: U16Register(rv.StorageProductModel, 1, 47089),
     rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_WRITE: U16Register(
-        rv.StorageForcibleChargeDischarge, 1, 47100, 1, writeable=True
+        rv.StorageForcibleChargeDischarge, 1, 47100, writeable=True
     ),
-    rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_SOC: U16Register("%", 10, 47101, 1, writeable=True),
-    rn.STORAGE_BACKUP_POWER_STATE_OF_CHARGE: U16Register("%", 10, 47102, 1, writeable=True),
-    rn.STORAGE_UNIT_1_NO: U16Register(None, 1, 47107, 1),
-    rn.STORAGE_UNIT_2_NO: U16Register(None, 1, 47108, 1),
+    rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_SOC: U16Register("%", 10, 47101, writeable=True),
+    rn.STORAGE_BACKUP_POWER_STATE_OF_CHARGE: U16Register("%", 10, 47102, writeable=True),
+    rn.STORAGE_UNIT_1_NO: U16Register(None, 1, 47107),
+    rn.STORAGE_UNIT_2_NO: U16Register(None, 1, 47108),
     rn.STORAGE_FIXED_CHARGING_AND_DISCHARGING_PERIODS: ChargeDischargePeriodRegisters(47200, 41, writeable=True),
-    rn.STORAGE_POWER_OF_CHARGE_FROM_GRID: U32Register("W", 1, 47242, 2, writeable=True),
-    rn.STORAGE_MAXIMUM_POWER_OF_CHARGE_FROM_GRID: U32Register("W", 1, 47244, 2, writeable=True),
-    rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_SETTING_MODE: U16Register(None, 1, 47246, 1, writeable=True),
-    rn.STORAGE_FORCIBLE_CHARGE_POWER: U32Register(None, 1, 47247, 2, writeable=True),
-    rn.STORAGE_FORCIBLE_DISCHARGE_POWER: U32Register(None, 1, 47249, 2, writeable=True),
+    rn.STORAGE_POWER_OF_CHARGE_FROM_GRID: U32Register("W", 1, 47242, writeable=True),
+    rn.STORAGE_MAXIMUM_POWER_OF_CHARGE_FROM_GRID: U32Register("W", 1, 47244, writeable=True),
+    rn.STORAGE_FORCIBLE_CHARGE_DISCHARGE_SETTING_MODE: U16Register(None, 1, 47246, writeable=True),
+    rn.STORAGE_FORCIBLE_CHARGE_POWER: U32Register(None, 1, 47247, writeable=True),
+    rn.STORAGE_FORCIBLE_DISCHARGE_POWER: U32Register(None, 1, 47249, writeable=True),
     rn.STORAGE_TIME_OF_USE_CHARGING_AND_DISCHARGING_PERIODS: TimeOfUseRegisters(47255, 43, writeable=True),
-    rn.STORAGE_EXCESS_PV_ENERGY_USE_IN_TOU: U16Register(rv.StorageExcessPvEnergyUseInTOU, 1, 47299, 1, writeable=True),
-    rn.ACTIVE_POWER_CONTROL_MODE: U16Register(rv.ActivePowerControlMode, 1, 47415, 1, writeable=True),
-    rn.MAXIMUM_FEED_GRID_POWER_WATT: I32Register("W", 1, 47416, 2, writeable=True),
-    rn.MAXIMUM_FEED_GRID_POWER_PERCENT: I16Register("%", 10, 47418, 1, writeable=True),
-    rn.DONGLE_PLANT_MAXIMUM_CHARGE_FROM_GRID_POWER: U32Register("W", 1, 47590, 2, writeable=True),
-    rn.BACKUP_SWITCH_TO_OFF_GRID: U16Register(None, 1, 47604, 1, writeable=True),
-    rn.BACKUP_VOLTAGE_INDEPENDEND_OPERATION: U16Register(
-        rv.BackupVoltageIndependentOperation, 1, 47605, 1, writeable=True
-    ),
-    rn.REMOTE_CHARGE_DISCHARGE_CONTROL_MODE: I16Register(
-        rv.RemoteChargeDischargeControlMode, 1, 47589, 1, writeable=True
+    rn.STORAGE_EXCESS_PV_ENERGY_USE_IN_TOU: U16Register(rv.StorageExcessPvEnergyUseInTOU, 1, 47299, writeable=True),
+    rn.ACTIVE_POWER_CONTROL_MODE: U16Register(rv.ActivePowerControlMode, 1, 47415, writeable=True),
+    rn.MAXIMUM_FEED_GRID_POWER_WATT: I32Register("W", 1, 47416, writeable=True),
+    rn.MAXIMUM_FEED_GRID_POWER_PERCENT: I16Register("%", 10, 47418, writeable=True),
+    rn.REMOTE_CHARGE_DISCHARGE_CONTROL_MODE: I16Register(rv.RemoteChargeDischargeControlMode, 1, 47589, writeable=True),
+    rn.DONGLE_PLANT_MAXIMUM_CHARGE_FROM_GRID_POWER: U32Register("W", 1, 47590, writeable=True),
+    rn.BACKUP_SWITCH_TO_OFF_GRID: U16Register(None, 1, 47604, writeable=True),
+    rn.BACKUP_VOLTAGE_INDEPENDENT_OPERATION: U16Register(
+        rv.BackupVoltageIndependentOperation, 1, 47605, writeable=True
     ),
-    rn.DEFAULT_MAXIMUM_FEED_IN_POWER: I32Register("W", 1, 47675, 2, writeable=True),
-    rn.DEFAULT_ACTIVE_POWER_CHANGE_GRADIENT: U32Register("%/s", 1000, 47677, 2),
-    rn.STORAGE_UNIT_1_PACK_1_NO: U16Register(None, 1, 47750, 1),
-    rn.STORAGE_UNIT_1_PACK_2_NO: U16Register(None, 1, 47751, 1),
-    rn.STORAGE_UNIT_1_PACK_3_NO: U16Register(None, 1, 47752, 1),
-    rn.STORAGE_UNIT_2_PACK_1_NO: U16Register(None, 1, 47753, 1),
-    rn.STORAGE_UNIT_2_PACK_2_NO: U16Register(None, 1, 47754, 1),
-    rn.STORAGE_UNIT_2_PACK_3_NO: U16Register(None, 1, 47755, 1),
+    rn.DEFAULT_MAXIMUM_FEED_IN_POWER: I32Register("W", 1, 47675, writeable=True),
+    rn.DEFAULT_ACTIVE_POWER_CHANGE_GRADIENT: U32Register("%/s", 1000, 47677),
+    rn.STORAGE_UNIT_1_PACK_1_NO: U16Register(None, 1, 47750),
+    rn.STORAGE_UNIT_1_PACK_2_NO: U16Register(None, 1, 47751),
+    rn.STORAGE_UNIT_1_PACK_3_NO: U16Register(None, 1, 47752),
+    rn.STORAGE_UNIT_2_PACK_1_NO: U16Register(None, 1, 47753),
+    rn.STORAGE_UNIT_2_PACK_2_NO: U16Register(None, 1, 47754),
+    rn.STORAGE_UNIT_2_PACK_3_NO: U16Register(None, 1, 47755),
 }
 REGISTERS.update(BATTERY_REGISTERS)
 
 CAPACITY_CONTROL_REGISTERS = {
     # We must check if we can read from these registers to know if this feature is supported
     # by the inverter/battery firmware
-    rn.STORAGE_CAPACITY_CONTROL_MODE: U16Register(rv.StorageCapacityControlMode, 1, 47954, 1, writeable=True),
-    rn.STORAGE_CAPACITY_CONTROL_SOC_PEAK_SHAVING: U16Register("%", 10, 47955, 1, writeable=True),
+    rn.STORAGE_CAPACITY_CONTROL_MODE: U16Register(rv.StorageCapacityControlMode, 1, 47954, writeable=True),
+    rn.STORAGE_CAPACITY_CONTROL_SOC_PEAK_SHAVING: U16Register("%", 10, 47955, writeable=True),
     rn.STORAGE_CAPACITY_CONTROL_PERIODS: PeakSettingPeriodRegisters(47956, 64, writeable=True),
 }
 
 REGISTERS.update(CAPACITY_CONTROL_REGISTERS)
 
 EMMA_REGISTERS = {
-    rn.EMMA: U16Register(bool, 1, 48020, 1, writeable=True),
+    rn.EMMA: U16Register(bool, 1, 48020, writeable=True),
 }
 
 REGISTERS.update(EMMA_REGISTERS)
 
 
 METER_REGISTERS = {
-    rn.METER_STATUS: U16Register(rv.MeterStatus, 1, 37100, 1),
-    rn.GRID_A_VOLTAGE: I32Register("V", 10, 37101, 2),
-    rn.GRID_B_VOLTAGE: I32Register("V", 10, 37103, 2),
-    rn.GRID_C_VOLTAGE: I32Register("V", 10, 37105, 2),
-    rn.ACTIVE_GRID_A_CURRENT: I32Register("I", 100, 37107, 2),
-    rn.ACTIVE_GRID_B_CURRENT: I32Register("I", 100, 37109, 2),
-    rn.ACTIVE_GRID_C_CURRENT: I32Register("I", 100, 37111, 2),
-    rn.POWER_METER_ACTIVE_POWER: I32Register("W", 1, 37113, 2),
-    rn.POWER_METER_REACTIVE_POWER: I32Register("Var", 1, 37115, 2),
-    rn.ACTIVE_GRID_POWER_FACTOR: I16Register(None, 1000, 37117, 1),
-    rn.ACTIVE_GRID_FREQUENCY: I16Register("Hz", 100, 37118, 1),
+    rn.METER_STATUS: U16Register(rv.MeterStatus, 1, 37100),
+    rn.GRID_A_VOLTAGE: I32Register("V", 10, 37101),
+    rn.GRID_B_VOLTAGE: I32Register("V", 10, 37103),
+    rn.GRID_C_VOLTAGE: I32Register("V", 10, 37105),
+    rn.ACTIVE_GRID_A_CURRENT: I32Register("I", 100, 37107),
+    rn.ACTIVE_GRID_B_CURRENT: I32Register("I", 100, 37109),
+    rn.ACTIVE_GRID_C_CURRENT: I32Register("I", 100, 37111),
+    rn.POWER_METER_ACTIVE_POWER: I32Register("W", 1, 37113),
+    rn.POWER_METER_REACTIVE_POWER: I32Register("Var", 1, 37115),
+    rn.ACTIVE_GRID_POWER_FACTOR: I16Register(None, 1000, 37117),
+    rn.ACTIVE_GRID_FREQUENCY: I16Register("Hz", 100, 37118),
     # cfr. https://github.com/wlcrs/huawei_solar/issues/54
-    rn.GRID_EXPORTED_ENERGY: I32AbsoluteValueRegister("kWh", 100, 37119, 2),
-    rn.GRID_ACCUMULATED_ENERGY: I32Register("kWh", 100, 37121, 2),
-    rn.GRID_ACCUMULATED_REACTIVE_POWER: I32Register("kVarh", 100, 37123, 2),
-    rn.METER_TYPE: U16Register(rv.MeterType, 1, 37125, 1),
-    rn.ACTIVE_GRID_A_B_VOLTAGE: I32Register("V", 10, 37126, 2),
-    rn.ACTIVE_GRID_B_C_VOLTAGE: I32Register("V", 10, 37128, 2),
-    rn.ACTIVE_GRID_C_A_VOLTAGE: I32Register("V", 10, 37130, 2),
-    rn.ACTIVE_GRID_A_POWER: I32Register("W", 1, 37132, 2),
-    rn.ACTIVE_GRID_B_POWER: I32Register("W", 1, 37134, 2),
-    rn.ACTIVE_GRID_C_POWER: I32Register("W", 1, 37136, 2),
-    rn.METER_TYPE_CHECK: U16Register(rv.MeterTypeCheck, 1, 37125, 2),
+    rn.GRID_EXPORTED_ENERGY: I32AbsoluteValueRegister("kWh", 100, 37119),
+    rn.GRID_ACCUMULATED_ENERGY: I32Register("kWh", 100, 37121),
+    rn.GRID_ACCUMULATED_REACTIVE_POWER: I32Register("kVarh", 100, 37123),
+    rn.METER_TYPE: U16Register(rv.MeterType, 1, 37125),
+    rn.ACTIVE_GRID_A_B_VOLTAGE: I32Register("V", 10, 37126),
+    rn.ACTIVE_GRID_B_C_VOLTAGE: I32Register("V", 10, 37128),
+    rn.ACTIVE_GRID_C_A_VOLTAGE: I32Register("V", 10, 37130),
+    rn.ACTIVE_GRID_A_POWER: I32Register("W", 1, 37132),
+    rn.ACTIVE_GRID_B_POWER: I32Register("W", 1, 37134),
+    rn.ACTIVE_GRID_C_POWER: I32Register("W", 1, 37136),
+    rn.METER_TYPE_CHECK: U16Register(rv.MeterTypeCheck, 1, 37138),
 }
 
 REGISTERS.update(METER_REGISTERS)
```

### Comparing `huawei-solar-2.3.0b6/src/huawei_solar.egg-info/SOURCES.txt` & `huawei_solar-2.3.0b7/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,9 +29,11 @@
 src/huawei_solar.egg-info/dependency_links.txt
 src/huawei_solar.egg-info/requires.txt
 src/huawei_solar.egg-info/top_level.txt
 tests/conftest.py
 tests/mock_huawei_solar.py
 tests/test__registers__peak_periods.py
 tests/test__registers__time_of_use.py
+tests/test_bridge.py
+tests/test_config.py
 tests/test_huawei_solar.py
 tests/test_registers.py
```

### Comparing `huawei-solar-2.3.0b6/test.py` & `huawei_solar-2.3.0b7/test.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/tests/mock_huawei_solar.py` & `huawei_solar-2.3.0b7/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/tests/test__registers__peak_periods.py` & `huawei_solar-2.3.0b7/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/tests/test__registers__time_of_use.py` & `huawei_solar-2.3.0b7/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/tests/test_huawei_solar.py` & `huawei_solar-2.3.0b7/tests/test_huawei_solar.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,36 +90,36 @@
 async def test_get_rated_power(huawei_solar):
     result = await huawei_solar.get("rated_power")
     assert result.value == 3000
     assert result.unit == "W"
 
 
 @pytest.mark.asyncio
-async def test_get_P_max(huawei_solar):
+async def test_get_p_max(huawei_solar):
     result = await huawei_solar.get("P_max")
     assert result.value == 3300
     assert result.unit == "W"
 
 
 @pytest.mark.asyncio
-async def test_get_S_max(huawei_solar):
+async def test_get_s_max(huawei_solar):
     result = await huawei_solar.get("S_max")
     assert result.value == 3300
     assert result.unit == "VA"
 
 
 @pytest.mark.asyncio
-async def test_get_Q_max_out(huawei_solar):
+async def test_get_q_max_out(huawei_solar):
     result = await huawei_solar.get("Q_max_out")
     assert result.value == 1980
     assert result.unit == "VAr"
 
 
 @pytest.mark.asyncio
-async def test_get_Q_max_in(huawei_solar):
+async def test_get_q_max_in(huawei_solar):
     result = await huawei_solar.get("Q_max_in")
     assert result.value == -1980
     assert result.unit == "VAr"
 
 
 @pytest.mark.asyncio
 async def test_get_state_1(huawei_solar):
@@ -152,15 +152,14 @@
     with patch.object(
         huawei_solar,
         "_read_registers",
         return_value=ReadHoldingRegistersResponse([0b0111_1111_1111_1000]),
     ):
         result = await huawei_solar.get(rn.STATE_2)
 
-        result.value == ["Locked", "PV disconnected", "No DSP data collection"]
         assert result.unit is None
 
 
 @pytest.mark.asyncio
 async def test_get_state_3(huawei_solar):
     result = await huawei_solar.get(rn.STATE_3)
     assert result.value == ["On-grid", "Off-grid switch disabled"]
@@ -352,78 +351,78 @@
 async def test_get_grid_voltage(huawei_solar):
     result = await huawei_solar.get(rn.GRID_VOLTAGE)
     assert result.value == 0.0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_voltage_A_B(huawei_solar):
+async def test_get_line_voltage_a_b(huawei_solar):
     result = await huawei_solar.get(rn.LINE_VOLTAGE_A_B)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_voltage_B_C(huawei_solar):
+async def test_get_line_voltage_b_c(huawei_solar):
     result = await huawei_solar.get(rn.LINE_VOLTAGE_B_C)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_voltage_C_A(huawei_solar):
+async def test_get_line_voltage_c_a(huawei_solar):
     result = await huawei_solar.get(rn.LINE_VOLTAGE_C_A)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_phase_A_voltage(huawei_solar):
+async def test_get_line_phase_a_voltage(huawei_solar):
     result = await huawei_solar.get(rn.PHASE_A_VOLTAGE)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_phase_B_voltage(huawei_solar):
+async def test_get_line_phase_b_voltage(huawei_solar):
     result = await huawei_solar.get(rn.PHASE_B_VOLTAGE)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
-async def test_get_line_phase_C_voltage(huawei_solar):
+async def test_get_line_phase_c_voltage(huawei_solar):
     result = await huawei_solar.get(rn.PHASE_C_VOLTAGE)
     assert result.value == 0
     assert result.unit == "V"
 
 
 @pytest.mark.asyncio
 async def test_get_grid_current(huawei_solar):
     result = await huawei_solar.get("grid_current")
     assert result.value == 0
     assert result.unit == "A"
 
 
 @pytest.mark.asyncio
-async def test_get_phase_A_current(huawei_solar):
+async def test_get_phase_a_current(huawei_solar):
     result = await huawei_solar.get("phase_A_current")
     assert result.value == 0
     assert result.unit == "A"
 
 
 @pytest.mark.asyncio
-async def test_get_phase_B_current(huawei_solar):
+async def test_get_phase_b_current(huawei_solar):
     result = await huawei_solar.get("phase_B_current")
     assert result.value == 0
     assert result.unit == "A"
 
 
 @pytest.mark.asyncio
-async def test_get_phase_C_current(huawei_solar):
+async def test_get_phase_c_current(huawei_solar):
     result = await huawei_solar.get("phase_C_current")
     assert result.value == 0
     assert result.unit == "A"
 
 
 @pytest.mark.asyncio
 async def test_get_day_active_power_peak(huawei_solar):
```

### Comparing `huawei-solar-2.3.0b6/tests/test_registers.py` & `huawei_solar-2.3.0b7/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.3.0b6/tox.ini` & `huawei_solar-2.3.0b7/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# content of: tox.ini , put in same dir as setup.py
+# content of: tox.ini, put in same dir as setup.py
 [tox]
-envlist = py310, py311, flake8, pylint, codecov, yamllint
+envlist = py310, py311, py312, flake8, pylint, codecov, yamllint
 skip_missing_interpreters = True
 
 [testenv]
 # install the test-dependencies mentioned in pyproject.toml
 extras = test
 
 #changedir = tests
```

