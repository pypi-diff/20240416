# Comparing `tmp/avocentdpdu-1.0.0.tar.gz` & `tmp/avocentdpdu-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocentdpdu-1.0.0.tar", last modified: Mon Apr 15 03:52:37 2024, max compression
+gzip compressed data, was "avocentdpdu-1.0.1.tar", last modified: Tue Apr 16 01:26:57 2024, max compression
```

## Comparing `avocentdpdu-1.0.0.tar` & `avocentdpdu-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.923308 avocentdpdu-1.0.0/
--rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-04-15 03:52:37.921276 avocentdpdu-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.0.0/README.md
--rw-rw-rw-   0        0        0      528 2024-04-15 03:52:20.000000 avocentdpdu-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 03:52:37.923570 avocentdpdu-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.872778 avocentdpdu-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.893275 avocentdpdu-1.0.0/src/avocentdpdu/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.0.0/src/avocentdpdu/__init__.py
--rw-rw-rw-   0        0        0     7801 2024-04-15 03:50:00.000000 avocentdpdu-1.0.0/src/avocentdpdu/avocentdpdu.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:52:37.919276 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 03:52:37.000000 avocentdpdu-1.0.0/src/avocentdpdu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 01:26:57.006531 avocentdpdu-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-04-16 01:26:57.003531 avocentdpdu-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.0.1/README.md
+-rw-rw-rw-   0        0        0      528 2024-04-16 01:25:31.000000 avocentdpdu-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 01:26:57.006531 avocentdpdu-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 01:26:56.973532 avocentdpdu-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 01:26:56.989529 avocentdpdu-1.0.1/src/avocentdpdu/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.0.1/src/avocentdpdu/__init__.py
+-rw-rw-rw-   0        0        0     7847 2024-04-16 01:19:39.000000 avocentdpdu-1.0.1/src/avocentdpdu/avocentdpdu.py
+drwxrwxrwx   0        0        0        0 2024-04-16 01:26:57.001533 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/top_level.txt
```

### Comparing `avocentdpdu-1.0.0/LICENSE` & `avocentdpdu-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.0.0/PKG-INFO` & `avocentdpdu-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `avocentdpdu-1.0.0/README.md` & `avocentdpdu-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.0.0/pyproject.toml` & `avocentdpdu-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avocentdpdu"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="William Gibson", email="william.gibson.wg@gmail.com" },
 ]
 description = "Library to control Avocent DPDU10x PDUs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avocentdpdu-1.0.0/src/avocentdpdu/avocentdpdu.py` & `avocentdpdu-1.0.1/src/avocentdpdu/avocentdpdu.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         # or 11111111 to control all outlets on an 8 port unit
         self.switch_flag = '0'*(outlet_idx) + '1' + '0'*(number_outlets-outlet_idx)
 
     async def obtain_name(self):
         """Call after initialization to obtain outlet name from PDU"""
         async with aiohttp.ClientSession() as session:
             async with session.get(f'http://{self.pdu.host}/switch{self.outlet_id}.cgi', timeout=self.timeout) as response:
+                html = await response.text()
                 if response.status == 200:
-                    html = await response.text()
                     self.name = html.strip()
                 else:
                     _LOGGER.warning("Could not find Avocent PDU outlet index %d at %s", self.outlet_idx, self.pdu.host)
 
     def is_on(self):
         """Returns boolean status of this outlet on=True"""
         return self.is_on_bool
@@ -111,29 +111,29 @@
         Note: The Avocent PDU commits the cardinal sin of using a GET request to change state
         """
 
         endpoint = '1' if cmd_on == SwitchCommand.TURN_ON else '3'
 
         async with aiohttp.ClientSession() as session:
             url = f'http://{self.host}/{endpoint}?3={self.username},{self.password},{which_switches},'
-            session.get(url, timeout=self.timeout)
-            # Response is always 404 with no body, even on success. Do nothing.
-
+            async with session.get(url, timeout=self.timeout) as response:
+                await response.text()
+                # Response is always 404 with no body, even on success. Do nothing.
 
     async def update(self) -> None:
         """Get the status of the PDU"""
 
         if not self.is_initialized:
             await self.initialize()
 
         async with aiohttp.ClientSession() as session:
             url = f'http://{self.host}/control.cgi'
             async with session.get(url, timeout=self.timeout) as response:
+                document = await response.text()
                 if response.status == 200:
-                    document = await response.text()
                     # Basic HTML parsing
                     if "Z1" in document:
                         name = document.split('name=')[1]
                         _LOGGER.debug('Avocent Status = %s', name)
                         data2 = name.split(',')
                         statuses = data2[0]
                         self.current_deciamps = int(data2[1])
@@ -180,28 +180,29 @@
     def __repr__(self):
         switch_vals = ', '.join(map(repr, self.switch_list))
         return f"<AvocentPDU host:{self.host}; status:{self.pdu_status};\
         current:{self.current_deciamps/10.0}A;\
         login:{self.password_status}\n {switch_vals} >"
 
 
-# async def main():
-#     _LOGGER.basicConfig(level=_LOGGER.INFO)
-#     A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 8, 10)
-#     await A.update()
-#     print(A)
-
-#     switches = A.switches()
-
-#     switch = switches[2]
-#     if switch.is_on():
-#         await switch.turn_off()
-#     else:
-#         await switch.turn_on()
-
-#     await A.update()
-#     print(switch)
-
-# if __name__ == "__main__":
-#     loop = asyncio.get_event_loop()
-#     loop.run_until_complete(main())
-#     loop.close()
+async def main():
+    _LOGGER.basicConfig(level=_LOGGER.INFO)
+    A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 8, 10)
+    await A.update()
+    print(A)
+
+    switches = A.switches()
+
+    switch = switches[2]
+    if switch.is_on():
+        await switch.turn_off()
+    else:
+        await switch.turn_on()
+
+    await A.update()
+    print(switch)
+
+if __name__ == "__main__":
+    print("laksjdla")
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(main())
+    loop.close()
```

### Comparing `avocentdpdu-1.0.0/src/avocentdpdu.egg-info/PKG-INFO` & `avocentdpdu-1.0.1/src/avocentdpdu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

