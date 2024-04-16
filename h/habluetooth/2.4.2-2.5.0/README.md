# Comparing `tmp/habluetooth-2.4.2.tar.gz` & `tmp/habluetooth-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habluetooth-2.4.2.tar", max compression
+gzip compressed data, was "habluetooth-2.5.0.tar", max compression
```

## Comparing `habluetooth-2.4.2.tar` & `habluetooth-2.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11345 2024-02-29 19:43:20.762752 habluetooth-2.4.2/LICENSE
--rw-r--r--   0        0        0     3805 2024-02-29 19:43:20.762752 habluetooth-2.4.2/README.md
--rw-r--r--   0        0        0     1496 2024-02-29 19:43:20.762752 habluetooth-2.4.2/build_ext.py
--rw-r--r--   0        0        0     3730 2024-02-29 19:43:29.042777 habluetooth-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     1457 2024-02-29 19:43:29.042777 habluetooth-2.4.2/src/habluetooth/__init__.py
--rw-r--r--   0        0        0      395 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/advertisement_tracker.pxd
--rw-r--r--   0        0        0     2809 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/advertisement_tracker.py
--rw-r--r--   0        0        0     1917 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/base_scanner.pxd
--rw-r--r--   0        0        0    16704 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/base_scanner.py
--rw-r--r--   0        0        0      650 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/central_manager.py
--rw-r--r--   0        0        0     1692 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/const.py
--rw-r--r--   0        0        0     2214 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/manager.pxd
--rw-r--r--   0        0        0    28056 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/manager.py
--rw-r--r--   0        0        0      726 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/models.pxd
--rw-r--r--   0        0        0     7310 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/models.py
--rw-r--r--   0        0        0        0 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/py.typed
--rw-r--r--   0        0        0      542 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/scanner.pxd
--rw-r--r--   0        0        0    15722 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/scanner.py
--rw-r--r--   0        0        0      530 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/scanner_device.py
--rw-r--r--   0        0        0     1733 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/usage.py
--rw-r--r--   0        0        0      544 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/util.py
--rw-r--r--   0        0        0    14651 2024-02-29 19:43:20.766752 habluetooth-2.4.2/src/habluetooth/wrappers.py
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 habluetooth-2.4.2/setup.py
--rw-r--r--   0        0        0     5143 1970-01-01 00:00:00.000000 habluetooth-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-04-16 20:35:09.313703 habluetooth-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3805 2024-04-16 20:35:09.313703 habluetooth-2.5.0/README.md
+-rw-r--r--   0        0        0     1496 2024-04-16 20:35:09.313703 habluetooth-2.5.0/build_ext.py
+-rw-r--r--   0        0        0     3791 2024-04-16 20:35:10.081710 habluetooth-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1457 2024-04-16 20:35:10.081710 habluetooth-2.5.0/src/habluetooth/__init__.py
+-rw-r--r--   0        0        0      395 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/advertisement_tracker.pxd
+-rw-r--r--   0        0        0     2809 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/advertisement_tracker.py
+-rw-r--r--   0        0        0     1917 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/base_scanner.pxd
+-rw-r--r--   0        0        0    16704 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/base_scanner.py
+-rw-r--r--   0        0        0      650 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/central_manager.py
+-rw-r--r--   0        0        0     1709 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/const.py
+-rw-r--r--   0        0        0     2214 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/manager.pxd
+-rw-r--r--   0        0        0    28056 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/manager.py
+-rw-r--r--   0        0        0      726 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/models.pxd
+-rw-r--r--   0        0        0     7310 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/py.typed
+-rw-r--r--   0        0        0      542 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/scanner.pxd
+-rw-r--r--   0        0        0    18257 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/scanner.py
+-rw-r--r--   0        0        0      530 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/scanner_device.py
+-rw-r--r--   0        0        0     1733 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/usage.py
+-rw-r--r--   0        0        0      544 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/util.py
+-rw-r--r--   0        0        0    14651 2024-04-16 20:35:09.317703 habluetooth-2.5.0/src/habluetooth/wrappers.py
+-rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 habluetooth-2.5.0/setup.py
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 habluetooth-2.5.0/PKG-INFO
```

### Comparing `habluetooth-2.4.2/LICENSE` & `habluetooth-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/README.md` & `habluetooth-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/build_ext.py` & `habluetooth-2.5.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/pyproject.toml` & `habluetooth-2.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "habluetooth"
-version = "2.4.2"
+version = "2.5.0"
 description = "High availability Bluetooth"
 authors = ["J. Nick Koston <bluetooth@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/habluetooth"
 documentation = "https://habluetooth.readthedocs.io"
 classifiers = [
@@ -23,24 +23,25 @@
 script = "build_ext.py"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bluetooth-devices/habluetooth/issues"
 "Changelog" = "https://github.com/bluetooth-devices/habluetooth/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.13"
+python = ">=3.11,<3.13"
 bleak = ">=0.21.1"
 bleak-retry-connector = ">=3.3.0"
 bluetooth-data-tools = ">=1.16.0"
 bluetooth-adapters = ">=0.16.1"
 bluetooth-auto-recovery = ">=1.2.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
@@ -70,14 +71,16 @@
 [tool.semantic_release.branches.noop]
 match = "(?!main$)"
 prerelease = true
 
 [tool.pytest.ini_options]
 addopts = "-v -Wdefault --cov=habluetooth --cov-report=term-missing:skip-covered"
 pythonpath = ["src"]
+log_cli="true"
+log_level="NOTSET"
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
```

### Comparing `habluetooth-2.4.2/src/habluetooth/__init__.py` & `habluetooth-2.5.0/src/habluetooth/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.4.2"
+__version__ = "2.5.0"
 
 from .advertisement_tracker import (
     TRACKER_BUFFERING_WOBBLE_SECONDS,
     AdvertisementTracker,
 )
 from .base_scanner import BaseHaRemoteScanner, BaseHaScanner
 from .central_manager import get_manager, set_manager
```

### Comparing `habluetooth-2.4.2/src/habluetooth/advertisement_tracker.py` & `habluetooth-2.5.0/src/habluetooth/advertisement_tracker.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/base_scanner.pxd` & `habluetooth-2.5.0/src/habluetooth/base_scanner.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/base_scanner.py` & `habluetooth-2.5.0/src/habluetooth/base_scanner.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/central_manager.py` & `habluetooth-2.5.0/src/habluetooth/central_manager.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/const.py` & `habluetooth-2.5.0/src/habluetooth/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import Callable, Final
 
 CALLBACK_TYPE = Callable[[], None]
 
 SOURCE_LOCAL: Final = "local"
 
 START_TIMEOUT = 15
+STOP_TIMEOUT = 5
 
 # The maximum time between advertisements for a device to be considered
 # stale when the advertisement tracker cannot determine the interval.
 #
 # We have to set this quite high as we don't know
 # when devices fall out of the ESPHome device (and other non-local scanners)'s
 # stack like we do with BlueZ so its safer to assume its available
```

### Comparing `habluetooth-2.4.2/src/habluetooth/manager.pxd` & `habluetooth-2.5.0/src/habluetooth/manager.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/manager.py` & `habluetooth-2.5.0/src/habluetooth/manager.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/models.pxd` & `habluetooth-2.5.0/src/habluetooth/models.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/models.py` & `habluetooth-2.5.0/src/habluetooth/models.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/scanner.pxd` & `habluetooth-2.5.0/src/habluetooth/scanner.pxd`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/scanner.py` & `habluetooth-2.5.0/src/habluetooth/scanner.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,21 +19,24 @@
 from .base_scanner import BaseHaScanner
 from .const import (
     CALLBACK_TYPE,
     SCANNER_WATCHDOG_INTERVAL,
     SCANNER_WATCHDOG_TIMEOUT,
     SOURCE_LOCAL,
     START_TIMEOUT,
+    STOP_TIMEOUT,
 )
 from .models import BluetoothScanningMode, BluetoothServiceInfoBleak
 from .util import async_reset_adapter, is_docker_env
 
 SYSTEM = platform.system()
+IS_LINUX = SYSTEM == "Linux"
+IS_MACOS = SYSTEM == "Darwin"
 
-if SYSTEM == "Linux":
+if IS_LINUX:
     from bleak.backends.bluezdbus.advertisement_monitor import OrPattern
     from bleak.backends.bluezdbus.scanner import BlueZScannerArgs
 
     # or_patterns is a workaround for the fact that passive scanning
     # needs at least one matcher to be set. The below matcher
     # will match all devices.
     PASSIVE_SCANNER_ARGS = BlueZScannerArgs(
@@ -59,15 +62,15 @@
 ]
 
 # When the adapter is still initializing, the scanner will raise an exception
 # with org.freedesktop.DBus.Error.UnknownObject
 WAIT_FOR_ADAPTER_TO_INIT_ERRORS = ["org.freedesktop.DBus.Error.UnknownObject"]
 ADAPTER_INIT_TIME = 1.5
 
-START_ATTEMPTS = 3
+START_ATTEMPTS = 4
 
 SCANNING_MODE_TO_BLEAK = {
     BluetoothScanningMode.ACTIVE: "active",
     BluetoothScanningMode.PASSIVE: "passive",
 }
 
 # The minimum number of seconds to know
@@ -90,31 +93,45 @@
     adapter: str | None,
 ) -> bleak.BleakScanner:
     """Create a Bleak scanner."""
     scanner_kwargs: dict[str, Any] = {
         "detection_callback": detection_callback,
         "scanning_mode": SCANNING_MODE_TO_BLEAK[scanning_mode],
     }
-    if SYSTEM == "Linux":
+    if IS_LINUX:
         # Only Linux supports multiple adapters
         if adapter:
             scanner_kwargs["adapter"] = adapter
         if scanning_mode == BluetoothScanningMode.PASSIVE:
             scanner_kwargs["bluez"] = PASSIVE_SCANNER_ARGS
-    elif SYSTEM == "Darwin":
+    elif IS_MACOS:
         # We want mac address on macOS
         scanner_kwargs["cb"] = {"use_bdaddr": True}
     _LOGGER.debug("Initializing bluetooth scanner with %s", scanner_kwargs)
 
     try:
         return OriginalBleakScanner(**scanner_kwargs)
     except (FileNotFoundError, BleakError) as ex:
         raise RuntimeError(f"Failed to initialize Bluetooth: {ex}") from ex
 
 
+def _error_indicates_reset_needed(error_str: str) -> bool:
+    """Return if the error indicates a reset is needed."""
+    return any(
+        needs_reset_error in error_str for needs_reset_error in NEED_RESET_ERRORS
+    )
+
+
+def _error_indicates_wait_for_adapter_to_init(error_str: str) -> bool:
+    """Return if the error indicates the adapter is still initializing."""
+    return any(
+        wait_error in error_str for wait_error in WAIT_FOR_ADAPTER_TO_INIT_ERRORS
+    )
+
+
 class HaScanner(BaseHaScanner):
     """
     Operate and automatically recover a BleakScanner.
 
     Multiple BleakScanner can be used at the same time
     if there are multiple adapters. This is only useful
     if the adapters are not located physically next to each other.
@@ -172,17 +189,14 @@
     ) -> tuple[BLEDevice, AdvertisementData] | None:
         """Return the advertisement data for a discovered device."""
         return self.discovered_devices_and_advertisement_data.get(address)
 
     def async_setup(self) -> CALLBACK_TYPE:
         """Set up the scanner."""
         super().async_setup()
-        self.scanner = create_bleak_scanner(
-            self._async_detection_callback, self.mode, self.adapter
-        )
         return self._unsetup
 
     async def async_diagnostics(self) -> dict[str, Any]:
         """Return diagnostic information about the scanner."""
         base_diag = await super().async_diagnostics()
         return base_diag | {
             "adapter": self.adapter,
@@ -232,119 +246,187 @@
     async def async_start(self) -> None:
         """Start bluetooth scanner."""
         async with self._start_stop_lock:
             await self._async_start()
 
     async def _async_start(self) -> None:
         """Start bluetooth scanner under the lock."""
-        if TYPE_CHECKING:
-            assert self.scanner is not None
-        for attempt in range(START_ATTEMPTS):
-            _LOGGER.debug(
-                "%s: Starting bluetooth discovery attempt: (%s/%s)",
+        for attempt in range(1, START_ATTEMPTS + 1):
+            if await self._async_start_attempt(attempt):
+                # Everything is fine, break out of the loop
+                break
+        await self._async_on_successful_start()
+
+    async def _async_on_successful_start(self) -> None:
+        """Run when the scanner has successfully started."""
+        self.scanning = True
+        self._async_setup_scanner_watchdog()
+        await restore_discoveries(self.scanner, self.adapter)
+
+    async def _async_start_attempt(self, attempt: int) -> bool:
+        """Start the scanner and handle errors."""
+        mode = self.mode
+        # 1st attempt - no auto reset
+        # 2nd attempt - try to reset the adapter and wait a bit
+        # 3th attempt - no auto reset
+        # 4th attempt - fallback to passive if available
+
+        if (
+            IS_LINUX
+            and attempt == START_ATTEMPTS
+            and mode is BluetoothScanningMode.ACTIVE
+        ):
+            mode = BluetoothScanningMode.PASSIVE
+            _LOGGER.warning(
+                "%s: Falling back to passive scanning mode "
+                "after active scanning failed (%s/%s)",
                 self.name,
-                attempt + 1,
+                attempt,
                 START_ATTEMPTS,
             )
-            try:
-                async with asyncio.timeout(START_TIMEOUT):
-                    await self.scanner.start()
-            except InvalidMessageError as ex:
-                _LOGGER.debug(
-                    "%s: Invalid DBus message received: %s",
-                    self.name,
-                    ex,
-                    exc_info=True,
-                )
-                raise ScannerStartError(
-                    f"{self.name}: Invalid DBus message received: {ex}; "
-                    "try restarting `dbus`"
-                ) from ex
-            except BrokenPipeError as ex:
-                _LOGGER.debug(
-                    "%s: DBus connection broken: %s", self.name, ex, exc_info=True
-                )
-                if is_docker_env():
-                    raise ScannerStartError(
-                        f"{self.name}: DBus connection broken: {ex}; try restarting "
-                        "`bluetooth`, `dbus`, and finally the docker container"
-                    ) from ex
-                raise ScannerStartError(
-                    f"{self.name}: DBus connection broken: {ex}; try restarting "
-                    "`bluetooth` and `dbus`"
-                ) from ex
-            except FileNotFoundError as ex:
-                _LOGGER.debug(
-                    "%s: FileNotFoundError while starting bluetooth: %s",
-                    self.name,
-                    ex,
-                    exc_info=True,
-                )
-                if is_docker_env():
-                    raise ScannerStartError(
-                        f"{self.name}: DBus service not found; docker config may "
-                        "be missing `-v /run/dbus:/run/dbus:ro`: {ex}"
-                    ) from ex
-                raise ScannerStartError(
-                    f"{self.name}: DBus service not found; make sure the DBus socket "
-                    f"is available to Home Assistant: {ex}"
-                ) from ex
-            except asyncio.TimeoutError as ex:
-                if attempt == 0:
-                    await self._async_reset_adapter()
-                    continue
-                raise ScannerStartError(
-                    f"{self.name}: Timed out starting Bluetooth after"
-                    f" {START_TIMEOUT} seconds; "
-                    "Try power cycling the Bluetooth hardware."
-                ) from ex
-            except BleakError as ex:
-                error_str = str(ex)
-                if attempt == 0:
-                    if any(
-                        needs_reset_error in error_str
-                        for needs_reset_error in NEED_RESET_ERRORS
-                    ):
-                        await self._async_reset_adapter()
-                    continue
-                if attempt != START_ATTEMPTS - 1:
-                    # If we are not out of retry attempts, and the
-                    # adapter is still initializing, wait a bit and try again.
-                    if any(
-                        wait_error in error_str
-                        for wait_error in WAIT_FOR_ADAPTER_TO_INIT_ERRORS
-                    ):
-                        _LOGGER.debug(
-                            "%s: Waiting for adapter to initialize; attempt (%s/%s)",
-                            self.name,
-                            attempt + 1,
-                            START_ATTEMPTS,
-                        )
-                        await asyncio.sleep(ADAPTER_INIT_TIME)
-                        continue
 
-                _LOGGER.debug(
-                    "%s: BleakError while starting bluetooth; attempt: (%s/%s): %s",
-                    self.name,
-                    attempt + 1,
-                    START_ATTEMPTS,
-                    ex,
-                    exc_info=True,
-                )
-                raise ScannerStartError(
-                    f"{self.name}: Failed to start Bluetooth: {ex}; "
-                    "Try power cycling the Bluetooth hardware."
-                ) from ex
+        self.scanner = create_bleak_scanner(
+            self._async_detection_callback, mode, self.adapter
+        )
+        self._log_start_attempt(attempt)
+        try:
+            async with asyncio.timeout(START_TIMEOUT):
+                await self.scanner.start()
+        except InvalidMessageError as ex:
+            await self._async_stop_scanner()
+            self._raise_for_invalid_dbus_message(ex)
+        except BrokenPipeError as ex:
+            await self._async_stop_scanner()
+            self._raise_for_broken_pipe_error(ex)
+        except FileNotFoundError as ex:
+            await self._async_stop_scanner()
+            self._raise_for_file_not_found_error(ex)
+        except asyncio.TimeoutError as ex:
+            await self._async_stop_scanner()
+            if attempt == 2:
+                await self._async_reset_adapter()
+            if attempt < START_ATTEMPTS:
+                self._log_start_timeout(attempt)
+                return False
+            raise ScannerStartError(
+                f"{self.name}: Timed out starting Bluetooth after"
+                f" {START_TIMEOUT} seconds; "
+                "Try power cycling the Bluetooth hardware."
+            ) from ex
+        except BleakError as ex:
+            await self._async_stop_scanner()
+            error_str = str(ex)
+            if attempt == 2 and _error_indicates_reset_needed(error_str):
+                await self._async_reset_adapter()
+            elif (
+                attempt != START_ATTEMPTS
+                and _error_indicates_wait_for_adapter_to_init(error_str)
+            ):
+                # If we are not out of retry attempts, and the
+                # adapter is still initializing, wait a bit and try again.
+                self._log_adapter_init_wait(attempt)
+                await asyncio.sleep(ADAPTER_INIT_TIME)
+            if attempt < START_ATTEMPTS:
+                self._log_start_failed(ex, attempt)
+                return False
+            raise ScannerStartError(
+                f"{self.name}: Failed to start Bluetooth: {ex}; "
+                "Try power cycling the Bluetooth hardware."
+            ) from ex
+
+        self._log_start_success(attempt)
+        return True
+
+    def _log_adapter_init_wait(self, attempt: int) -> None:
+        _LOGGER.debug(
+            "%s: Waiting for adapter to initialize; attempt (%s/%s)",
+            self.name,
+            attempt,
+            START_ATTEMPTS,
+        )
 
-            # Everything is fine, break out of the loop
-            break
+    def _log_start_success(self, attempt: int) -> None:
+        _LOGGER.debug(
+            "%s: Success while starting bluetooth; attempt: (%s/%s)",
+            self.name,
+            attempt,
+            START_ATTEMPTS,
+        )
 
-        self.scanning = True
-        self._async_setup_scanner_watchdog()
-        await restore_discoveries(self.scanner, self.adapter)
+    def _log_start_timeout(self, attempt: int) -> None:
+        _LOGGER.debug(
+            "%s: TimeoutError while starting bluetooth; attempt: (%s/%s)",
+            self.name,
+            attempt,
+            START_ATTEMPTS,
+        )
+
+    def _log_start_failed(self, ex: BleakError, attempt: int) -> None:
+        _LOGGER.debug(
+            "%s: BleakError while starting bluetooth; attempt: (%s/%s): %s",
+            self.name,
+            attempt,
+            START_ATTEMPTS,
+            ex,
+            exc_info=True,
+        )
+
+    def _log_start_attempt(self, attempt: int) -> None:
+        _LOGGER.debug(
+            "%s: Starting bluetooth discovery attempt: (%s/%s)",
+            self.name,
+            attempt,
+            START_ATTEMPTS,
+        )
+
+    def _raise_for_file_not_found_error(self, ex: FileNotFoundError) -> None:
+        _LOGGER.debug(
+            "%s: FileNotFoundError while starting bluetooth: %s",
+            self.name,
+            ex,
+            exc_info=True,
+        )
+        if is_docker_env():
+            raise ScannerStartError(
+                f"{self.name}: DBus service not found; docker config may "
+                "be missing `-v /run/dbus:/run/dbus:ro`: {ex}"
+            ) from ex
+        raise ScannerStartError(
+            f"{self.name}: DBus service not found; make sure the DBus socket "
+            f"is available: {ex}"
+        ) from ex
+
+    def _raise_for_broken_pipe_error(self, ex: BrokenPipeError) -> None:
+        """Raise a ScannerStartError for a BrokenPipeError."""
+        _LOGGER.debug("%s: DBus connection broken: %s", self.name, ex, exc_info=True)
+        if is_docker_env():
+            msg = (
+                f"{self.name}: DBus connection broken: {ex}; try restarting "
+                "`bluetooth`, `dbus`, and finally the docker container"
+            )
+        else:
+            msg = (
+                f"{self.name}: DBus connection broken: {ex}; try restarting "
+                "`bluetooth` and `dbus`"
+            )
+        raise ScannerStartError(msg) from ex
+
+    def _raise_for_invalid_dbus_message(self, ex: InvalidMessageError) -> None:
+        """Raise a ScannerStartError for an InvalidMessageError."""
+        _LOGGER.debug(
+            "%s: Invalid DBus message received: %s",
+            self.name,
+            ex,
+            exc_info=True,
+        )
+        msg = (
+            f"{self.name}: Invalid DBus message received: {ex}; "
+            "try restarting `dbus`"
+        )
+        raise ScannerStartError(msg) from ex
 
     def _async_scanner_watchdog(self) -> None:
         """Check if the scanner is running."""
         if not self._async_watchdog_triggered():
             return
         if self._start_stop_lock.locked():
             _LOGGER.debug(
@@ -399,18 +481,21 @@
         """Stop bluetooth scanner."""
         async with self._start_stop_lock:
             self._async_stop_scanner_watchdog()
             await self._async_stop_scanner()
 
     async def _async_stop_scanner(self) -> None:
         """Stop bluetooth discovery under the lock."""
-        if TYPE_CHECKING:
-            assert self.scanner is not None
         self.scanning = False
+        if self.scanner is None:
+            _LOGGER.debug("%s: Scanner is already stopped", self.name)
+            return
         _LOGGER.debug("%s: Stopping bluetooth discovery", self.name)
         try:
-            await self.scanner.stop()
-        except BleakError as ex:
+            async with asyncio.timeout(STOP_TIMEOUT):
+                await self.scanner.stop()
+        except (asyncio.TimeoutError, BleakError) as ex:
             # This is not fatal, and they may want to reload
             # the config entry to restart the scanner if they
             # change the bluetooth dongle.
             _LOGGER.error("%s: Error stopping scanner: %s", self.name, ex)
+        self.scanner = None
```

### Comparing `habluetooth-2.4.2/src/habluetooth/scanner_device.py` & `habluetooth-2.5.0/src/habluetooth/scanner_device.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/usage.py` & `habluetooth-2.5.0/src/habluetooth/usage.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/util.py` & `habluetooth-2.5.0/src/habluetooth/util.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/src/habluetooth/wrappers.py` & `habluetooth-2.5.0/src/habluetooth/wrappers.py`

 * *Files identical despite different names*

### Comparing `habluetooth-2.4.2/setup.py` & `habluetooth-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,25 @@
  'bleak>=0.21.1',
  'bluetooth-adapters>=0.16.1',
  'bluetooth-auto-recovery>=1.2.3',
  'bluetooth-data-tools>=1.16.0']
 
 setup_kwargs = {
     'name': 'habluetooth',
-    'version': '2.4.2',
+    'version': '2.5.0',
     'description': 'High availability Bluetooth',
     'long_description': '# habluetooth\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/habluetooth/actions/workflows/ci.yml?query=branch%3Amain">\n    <img src="https://img.shields.io/github/actions/workflow/status/bluetooth-devices/habluetooth/ci.yml?branch=main&label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://habluetooth.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/habluetooth.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/habluetooth">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/habluetooth.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/habluetooth/">\n    <img src="https://img.shields.io/pypi/v/habluetooth.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/habluetooth.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/habluetooth.svg?style=flat-square" alt="License">\n</p>\n\n---\n\n**Documentation**: <a href="https://habluetooth.readthedocs.io" target="_blank">https://habluetooth.readthedocs.io </a>\n\n**Source Code**: <a href="https://github.com/bluetooth-devices/habluetooth" target="_blank">https://github.com/bluetooth-devices/habluetooth </a>\n\n---\n\nHigh availability Bluetooth\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install habluetooth`\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Copier](https://copier.readthedocs.io/) and the\n[browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-template)\nproject template.\n',
     'author': 'J. Nick Koston',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/habluetooth',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.10,<3.13',
+    'python_requires': '>=3.11,<3.13',
 }
 from build_ext import *
 build(setup_kwargs)
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['habluetooth'] package_data = \ {'': ['*']}
 install_requires = \ ['bleak-retry-connector>=3.3.0', 'bleak>=0.21.1',
 'bluetooth-adapters>=0.16.1', 'bluetooth-auto-recovery>=1.2.3', 'bluetooth-
 data-tools>=1.16.0'] setup_kwargs = { 'name': 'habluetooth', 'version':
-'2.4.2', 'description': 'High availability Bluetooth', 'long_description': '#
+'2.5.0', 'description': 'High availability Bluetooth', 'long_description': '#
 habluetooth\n\n
     \n _\_n_ _[_C_I_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_\_n_ \n _\_n_ _[_T_e_s_t_ _c_o_v_e_r_a_g_e
                                _p_e_r_c_e_n_t_a_g_e_]_\_n_ \n
 \n
            \n _\_n_ _[_P_o_e_t_r_y_]_\_n_ \n _\_n_ _[_b_l_a_c_k_]_\_n_ \n _\_n_ _[_p_r_e_-_c_o_m_m_i_t_]_\_n_ \n
 \n
       \n _\_n_ _[_P_y_P_I_ _V_e_r_s_i_o_n_]_\_n_ \n [Supported Python versions]\n [License]\n
@@ -21,9 +21,9 @@
 specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package
 was created with\n[Copier](https://copier.readthedocs.io/) and the\n
 [browniebroke/pypackage-template](https://github.com/browniebroke/pypackage-
 template)\nproject template.\n', 'author': 'J. Nick Koston', 'author_email':
 'bluetooth@koston.org', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'https://github.com/bluetooth-devices/habluetooth', 'package_dir':
 package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.10,<3.13', } from
+'install_requires': install_requires, 'python_requires': '>=3.11,<3.13', } from
 build_ext import * build(setup_kwargs) setup(**setup_kwargs)
```

### Comparing `habluetooth-2.4.2/PKG-INFO` & `habluetooth-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: habluetooth
-Version: 2.4.2
+Version: 2.5.0
 Summary: High availability Bluetooth
 Home-page: https://github.com/bluetooth-devices/habluetooth
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: bluetooth@koston.org
-Requires-Python: >=3.10,<3.13
+Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: bleak (>=0.21.1)
 Requires-Dist: bleak-retry-connector (>=3.3.0)
 Requires-Dist: bluetooth-adapters (>=0.16.1)
 Requires-Dist: bluetooth-auto-recovery (>=1.2.3)
```

#### html2text {}

```diff
@@ -1,23 +1,22 @@
-Metadata-Version: 2.1 Name: habluetooth Version: 2.4.2 Summary: High
+Metadata-Version: 2.1 Name: habluetooth Version: 2.5.0 Summary: High
 availability Bluetooth Home-page: https://github.com/bluetooth-devices/
 habluetooth License: Apache Software License 2.0 Author: J. Nick Koston Author-
-email: bluetooth@koston.org Requires-Python: >=3.10,<3.13 Classifier:
+email: bluetooth@koston.org Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: Topic :: Software
-Development :: Libraries Requires-Dist: bleak (>=0.21.1) Requires-Dist: bleak-
-retry-connector (>=3.3.0) Requires-Dist: bluetooth-adapters (>=0.16.1)
-Requires-Dist: bluetooth-auto-recovery (>=1.2.3) Requires-Dist: bluetooth-data-
-tools (>=1.16.0) Project-URL: Bug Tracker, https://github.com/bluetooth-
-devices/habluetooth/issues Project-URL: Changelog, https://github.com/
-bluetooth-devices/habluetooth/blob/main/CHANGELOG.md Project-URL:
+:: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development :: Libraries Requires-Dist: bleak (>=0.21.1) Requires-
+Dist: bleak-retry-connector (>=3.3.0) Requires-Dist: bluetooth-adapters
+(>=0.16.1) Requires-Dist: bluetooth-auto-recovery (>=1.2.3) Requires-Dist:
+bluetooth-data-tools (>=1.16.0) Project-URL: Bug Tracker, https://github.com/
+bluetooth-devices/habluetooth/issues Project-URL: Changelog, https://
+github.com/bluetooth-devices/habluetooth/blob/main/CHANGELOG.md Project-URL:
 Documentation, https://habluetooth.readthedocs.io Project-URL: Repository,
 https://github.com/bluetooth-devices/habluetooth Description-Content-Type:
 text/markdown # habluetooth
           _[_C_I_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Documentation**: _h_t_t_p_s_:_/_/_h_a_b_l_u_e_t_o_o_t_h_._r_e_a_d_t_h_e_d_o_c_s_._i_o_ **Source Code**:
```

