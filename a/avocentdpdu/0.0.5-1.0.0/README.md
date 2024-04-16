# Comparing `tmp/avocentdpdu-0.0.5.tar.gz` & `tmp/avocentdpdu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocentdpdu-0.0.5.tar", last modified: Sun Apr 14 00:57:59 2024, max compression
+gzip compressed data, was "avocentdpdu-1.0.0.tar", last modified: Mon Apr 15 03:52:37 2024, max compression
```

## Comparing `avocentdpdu-0.0.5.tar` & `avocentdpdu-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:57:59.690457 avocentdpdu-0.0.5/
--rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-04-14 00:57:59.683464 avocentdpdu-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-0.0.5/README.md
--rw-rw-rw-   0        0        0      528 2024-04-14 00:49:34.000000 avocentdpdu-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 00:57:59.690457 avocentdpdu-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 00:57:59.629459 avocentdpdu-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 00:57:59.649456 avocentdpdu-0.0.5/src/avocentdpdu/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-0.0.5/src/avocentdpdu/__init__.py
--rw-rw-rw-   0        0        0     6075 2024-04-14 00:45:20.000000 avocentdpdu-0.0.5/src/avocentdpdu/avocentdpdu.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:57:59.681460 avocentdpdu-0.0.5/src/avocentdpdu.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-04-14 00:57:59.000000 avocentdpdu-0.0.5/src/avocentdpdu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-14 00:57:59.000000 avocentdpdu-0.0.5/src/avocentdpdu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:57:59.000000 avocentdpdu-0.0.5/src/avocentdpdu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-14 00:57:59.000000 avocentdpdu-0.0.5/src/avocentdpdu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.923308 avocentdpdu-1.0.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-04-15 03:52:37.921276 avocentdpdu-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.0.0/README.md
+-rw-rw-rw-   0        0        0      528 2024-04-15 03:52:20.000000 avocentdpdu-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:52:37.923570 avocentdpdu-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.872778 avocentdpdu-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.893275 avocentdpdu-1.0.0/src/avocentdpdu/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.0.0/src/avocentdpdu/__init__.py
+-rw-rw-rw-   0        0        0     7801 2024-04-15 03:50:00.000000 avocentdpdu-1.0.0/src/avocentdpdu/avocentdpdu.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.919276 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/top_level.txt
```

### Comparing `avocentdpdu-0.0.5/LICENSE` & `avocentdpdu-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avocentdpdu-0.0.5/PKG-INFO` & `avocentdpdu-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 0.0.5
+Version: 1.0.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `avocentdpdu-0.0.5/README.md` & `avocentdpdu-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `avocentdpdu-0.0.5/pyproject.toml` & `avocentdpdu-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avocentdpdu"
-version = "0.0.5"
+version = "1.0.0"
 authors = [
   { name="William Gibson", email="william.gibson.wg@gmail.com" },
 ]
 description = "Library to control Avocent DPDU10x PDUs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avocentdpdu-0.0.5/src/avocentdpdu/avocentdpdu.py` & `avocentdpdu-1.0.0/src/avocentdpdu/avocentdpdu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module providing a Python interface to the Avocent PDU (e.g. DPDU101 DPDU10x DPDU20x) over HTTP"""
 
 from enum import Enum
 import logging as _LOGGER
-import requests
-
+import asyncio
+import aiohttp
 
 # Avocent PDU DPDU10x
 # Tested on DPDU101
 # Manual UI notes:
 # Press and hold the key after:
 #    1 beep; it can let the meter to show up the current information,
 #      temperature and humidity in sequence.(by model)
@@ -18,46 +18,56 @@
 
 class Outlet():
     """Child class of an Avocent PDU representing a controllable outlet.
     Construct an AvocentDPDU and call .switches() to get a list of these objects.
     """
     name = "ERR: Not Found"
 
-    def __init__(self, avocent_pdu: 'AvocentDPDU', outlet_idx: int, number_outlets: int):
+    def __init__(self, avocent_pdu: 'AvocentDPDU', outlet_idx: int, number_outlets: int, timeout: int):
         self.pdu = avocent_pdu
-        outlet_id = outlet_idx + 1
+        self.outlet_idx = outlet_idx
+        self.outlet_id = outlet_idx + 1
         self.is_on_bool = False
+        self.timeout = timeout
 
         # e.g. 0100000 to control OutletB 
         # or 11111111 to control all outlets on an 8 port unit
         self.switch_flag = '0'*(outlet_idx) + '1' + '0'*(number_outlets-outlet_idx)
 
-        name_resp = requests.get(f'http://{self.pdu.host}/switch{outlet_id}.cgi', timeout=2)
-        if name_resp.ok:
-            self.name = name_resp.text.strip()
-        else:
-            _LOGGER.warning("Could not find Avocent PDU outlet index %d at %s", outlet_idx, self.pdu.host)
+    async def obtain_name(self):
+        """Call after initialization to obtain outlet name from PDU"""
+        async with aiohttp.ClientSession() as session:
+            async with session.get(f'http://{self.pdu.host}/switch{self.outlet_id}.cgi', timeout=self.timeout) as response:
+                if response.status == 200:
+                    html = await response.text()
+                    self.name = html.strip()
+                else:
+                    _LOGGER.warning("Could not find Avocent PDU outlet index %d at %s", self.outlet_idx, self.pdu.host)
 
     def is_on(self):
         """Returns boolean status of this outlet on=True"""
         return self.is_on_bool
 
     def is_on_string(self):
         """Returns status of this outlet as string On/Off"""
         return 'On' if self.is_on_bool else 'Off'
 
-    def turn_on(self):
+    def get_name(self):
+        """Returns Avocent name for the outlet"""
+        return self.name
+
+    async def turn_on(self):
         """Command to turn outlet on"""
         _LOGGER.info('turn_on(%s)', self.name)
-        self.pdu.command_state(SwitchCommand.TURN_ON, self.switch_flag)
+        await self.pdu.command_state(SwitchCommand.TURN_ON, self.switch_flag)
 
-    def turn_off(self):
+    async def turn_off(self):
         """Command to turn outlet off"""
         _LOGGER.info('turn_off(%s)', self.name)
-        self.pdu.command_state(SwitchCommand.TURN_OFF, self.switch_flag)
+        await self.pdu.command_state(SwitchCommand.TURN_OFF, self.switch_flag)
 
     def __repr__(self):
         return f'{self.name}: {self.is_on_string()}'
 
 
 class SwitchCommand(Enum):
     """Enum used to command outlet to change status"""
@@ -67,66 +77,89 @@
 
 
 # Default Username 'snmp'
 # Default Password '1234'
 class AvocentDPDU():
     """Main class representing an Avocent PDU"""
 
-    def __init__(self, host, username, password, number_outlets):
+    def __init__(self, host, username, password, number_outlets, timeout):
         _LOGGER.info('Avocent PDU init')
         self.host = host
         self.username = username
         self.password = password
         self.number_outlets = number_outlets
         self.password_status = "Not attempted"
         self.password_ok = False
-        self.switch_list = [Outlet(self, N, number_outlets) for N in range(self.number_outlets)]
-
-        self.command_state(SwitchCommand.TURN_OFF, "0"*number_outlets)
-        self.update()
+        self.switch_list = [Outlet(self, N, number_outlets, timeout) for N in range(self.number_outlets)]
+        self.timeout = timeout
+        self.pdu_status = "unknown"
+        self.pdu_status_int = -1
+        self.current_deciamps = 0
+        self.password_status = "unknown"
+        self.is_initialized = False
+
+    async def initialize(self) -> None:
+        """Call once after construction to test login, and obtain Outlet names"""
+        await self.command_state(SwitchCommand.TURN_OFF, "0"*self.number_outlets)
+        tasks = []
+        for s in self.switch_list:
+            tasks.append(s.obtain_name())
+        await asyncio.gather(*tasks)
+        self.is_initialized = True
 
-    def command_state(self, cmd_on: SwitchCommand, which_switches: str):
+    async def command_state(self, cmd_on: SwitchCommand, which_switches: str):
         """Command PDU to change one or more outlet states
         Note: The Avocent PDU commits the cardinal sin of using a GET request to change state
         """
 
         endpoint = '1' if cmd_on == SwitchCommand.TURN_ON else '3'
-        requests.get(f'http://{self.host}/{endpoint}?3={self.username},{self.password},{which_switches},', timeout=2)
 
-    def update(self):
+        async with aiohttp.ClientSession() as session:
+            url = f'http://{self.host}/{endpoint}?3={self.username},{self.password},{which_switches},'
+            session.get(url, timeout=self.timeout)
+            # Response is always 404 with no body, even on success. Do nothing.
+
+
+    async def update(self) -> None:
         """Get the status of the PDU"""
-        ctrlResp = requests.get(f'http://{self.host}/control.cgi', timeout=2)
-        if ctrlResp.ok:
-            # Note: Unusual variable names were taken from Avocent Javascript
-            document = ctrlResp.text
-            # Basic HTML parsing
-            if "Z1" in document:
-                name = document.split('name=')[1]
-                _LOGGER.debug('Avocent Status = %s', name)
-                data2 = name.split(',')
-                statuses = data2[0]
-                self.current_deciamps = int(data2[1])
-                self.pdu_status_int = int(data2[2])
-                password_status = int(data2[3])
-
-                for N in range(self.number_outlets):
-                    self.switch_list[N].is_on_bool = statuses[N] == '1'
-
-                if password_status == 2:
-                    self.password_status = "Incorrect username or password"
-                elif password_status == 1:
-                    self.password_status = "Login OK"
-                else:
-                    self.password_status = "Login status unknown"
 
-                self.password_ok = True if password_status == 1 else False
+        if not self.is_initialized:
+            await self.initialize()
 
-                self.pdu_status = "Normal" if self.pdu_status_int == 0 \
-                    else "Warning!" if self.pdu_status_int == 1\
-                    else "Overloading!"
+        async with aiohttp.ClientSession() as session:
+            url = f'http://{self.host}/control.cgi'
+            async with session.get(url, timeout=self.timeout) as response:
+                if response.status == 200:
+                    document = await response.text()
+                    # Basic HTML parsing
+                    if "Z1" in document:
+                        name = document.split('name=')[1]
+                        _LOGGER.debug('Avocent Status = %s', name)
+                        data2 = name.split(',')
+                        statuses = data2[0]
+                        self.current_deciamps = int(data2[1])
+                        self.pdu_status_int = int(data2[2])
+                        password_status = int(data2[3])
+
+                        for N in range(self.number_outlets):
+                            self.switch_list[N].is_on_bool = statuses[N] == '1'
+
+                        if password_status == 2:
+                            self.password_status = "Incorrect username or password"
+                        elif password_status == 1:
+                            self.password_status = "Login OK"
+                        else:
+                            self.password_status = "Login status unknown"
+
+                        self.password_ok = True if password_status == 1 else False
+
+                        self.pdu_status = "Normal" if self.pdu_status_int == 0 \
+                            else "Warning!" if self.pdu_status_int == 1\
+                            else "Overloading!"
+        return
 
     def is_valid_login(self):
         """Returns True if the password was accepted at initialization"""
         return self.password_ok
 
     def switches(self):
         """Returns a list of outlets"""
@@ -147,22 +180,28 @@
     def __repr__(self):
         switch_vals = ', '.join(map(repr, self.switch_list))
         return f"<AvocentPDU host:{self.host}; status:{self.pdu_status};\
         current:{self.current_deciamps/10.0}A;\
         login:{self.password_status}\n {switch_vals} >"
 
 
-if __name__ == "__main__":
-    _LOGGER.basicConfig(level=_LOGGER.INFO)
-    A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 8)
-    print(A)
-
-    switches = A.switches()
-
-    # switch = switches[2]
-    # if switch.is_on:
-    #     switch.turn_off()
-    # else:
-    #     switch.turn_on()
-    #
-    # A.update()
-    # print(switch)
+# async def main():
+#     _LOGGER.basicConfig(level=_LOGGER.INFO)
+#     A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 8, 10)
+#     await A.update()
+#     print(A)
+
+#     switches = A.switches()
+
+#     switch = switches[2]
+#     if switch.is_on():
+#         await switch.turn_off()
+#     else:
+#         await switch.turn_on()
+
+#     await A.update()
+#     print(switch)
+
+# if __name__ == "__main__":
+#     loop = asyncio.get_event_loop()
+#     loop.run_until_complete(main())
+#     loop.close()
```

### Comparing `avocentdpdu-0.0.5/src/avocentdpdu.egg-info/PKG-INFO` & `avocentdpdu-1.0.0/src/avocentdpdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 0.0.5
+Version: 1.0.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

