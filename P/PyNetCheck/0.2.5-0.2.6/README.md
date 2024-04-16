# Comparing `tmp/pynetcheck-0.2.5.tar.gz` & `tmp/pynetcheck-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetcheck-0.2.5.tar", max compression
+gzip compressed data, was "pynetcheck-0.2.6.tar", max compression
```

## Comparing `pynetcheck-0.2.5.tar` & `pynetcheck-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,28 @@
--rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-0.2.5/LICENSE
--rw-r--r--   0        0        0      207 2024-04-01 17:38:30.516449 pynetcheck-0.2.5/pynetcheck/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.517432 pynetcheck-0.2.5/pynetcheck/models/__init__.py
--rw-r--r--   0        0        0     2179 2024-04-01 17:38:30.517432 pynetcheck-0.2.5/pynetcheck/models/device.py
--rw-r--r--   0        0        0      965 2024-04-01 17:38:30.518492 pynetcheck-0.2.5/pynetcheck/models/shared.py
--rw-r--r--   0        0        0      191 2024-04-01 17:38:30.518492 pynetcheck-0.2.5/pynetcheck/pytest.ini
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/cisco/__init__.py
--rw-r--r--   0        0        0      819 2024-04-01 17:38:30.519511 pynetcheck-0.2.5/pynetcheck/tests/cisco/conftest.py
--rw-r--r--   0        0        0     2824 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/cisco/test_servers.py
--rw-r--r--   0        0        0     1520 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-0.2.5/pynetcheck/tests/cve/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 17:38:30.521511 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/__init__.py
--rw-r--r--   0        0        0     5195 2024-04-01 17:38:30.522515 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
--rw-r--r--   0        0        0     1989 2024-04-01 17:38:30.522515 pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py
--rw-r--r--   0        0        0     1321 2024-04-01 17:38:30.523511 pynetcheck-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     8670 2024-04-01 17:38:30.513432 pynetcheck-0.2.5/README.md
--rw-r--r--   0        0        0     9709 1970-01-01 00:00:00.000000 pynetcheck-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-10-17 17:21:13.864484 pynetcheck-0.2.6/LICENSE
+-rw-r--r--   0        0        0      261 2024-04-16 13:43:20.701556 pynetcheck-0.2.6/pynetcheck/__init__.py
+-rw-r--r--   0        0        0    11226 2024-04-16 14:18:36.139811 pynetcheck-0.2.6/pynetcheck/archive/output_1713283371.388187.json
+-rw-r--r--   0        0        0      817 2024-04-16 16:29:18.656699 pynetcheck-0.2.6/pynetcheck/archive/output_1713287098.9189737.json
+-rw-r--r--   0        0        0     6750 2024-04-16 17:04:59.264998 pynetcheck-0.2.6/pynetcheck/archive/output_1713287258.6043513.json
+-rw-r--r--   0        0        0     6750 2024-04-16 17:07:38.964406 pynetcheck-0.2.6/pynetcheck/archive/output_1713287738.6383476.json
+-rw-r--r--   0        0        0     2669 2024-04-16 17:15:39.089976 pynetcheck-0.2.6/pynetcheck/archive/output_1713291137.528805.json
+-rw-r--r--   0        0        0     4475 2024-04-16 18:12:17.905502 pynetcheck-0.2.6/pynetcheck/archive/output_1713291437.5512764.json
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.517432 pynetcheck-0.2.6/pynetcheck/models/__init__.py
+-rw-r--r--   0        0        0     2769 2024-04-16 17:04:37.333457 pynetcheck-0.2.6/pynetcheck/models/device.py
+-rw-r--r--   0        0        0      965 2024-04-16 16:43:18.234801 pynetcheck-0.2.6/pynetcheck/models/shared.py
+-rw-r--r--   0        0        0      222 2024-04-16 13:32:23.519219 pynetcheck-0.2.6/pynetcheck/pytest.ini
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.6/pynetcheck/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.6/pynetcheck/tests/cisco/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-01 17:38:30.519511 pynetcheck-0.2.6/pynetcheck/tests/cisco/conftest.py
+-rw-r--r--   0        0        0     2824 2024-04-01 17:38:30.520511 pynetcheck-0.2.6/pynetcheck/tests/cisco/test_servers.py
+-rw-r--r--   0        0        0     1548 2024-04-16 18:14:28.120896 pynetcheck-0.2.6/pynetcheck/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-0.2.6/pynetcheck/tests/cve/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.521511 pynetcheck-0.2.6/pynetcheck/tests/cve/cisco/__init__.py
+-rw-r--r--   0        0        0     6300 2024-04-16 18:21:14.804601 pynetcheck-0.2.6/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py
+-rw-r--r--   0        0        0     2109 2024-04-16 16:34:44.776638 pynetcheck-0.2.6/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.520511 pynetcheck-0.2.6/pynetcheck/tests/cve/paloalto/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-16 18:25:45.544090 pynetcheck-0.2.6/pynetcheck/tests/cve/paloalto/test_cve_2024_3400.py
+-rw-r--r--   0        0        0        0 2024-04-01 17:38:30.519511 pynetcheck-0.2.6/pynetcheck/tests/paloalto/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-16 14:23:35.321116 pynetcheck-0.2.6/pynetcheck/tests/paloalto/conftest.py
+-rw-r--r--   0        0        0     1342 2024-04-16 18:17:36.151566 pynetcheck-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     8670 2024-04-01 17:38:30.513432 pynetcheck-0.2.6/README.md
+-rw-r--r--   0        0        0     9750 1970-01-01 00:00:00.000000 pynetcheck-0.2.6/PKG-INFO
```

### Comparing `pynetcheck-0.2.5/LICENSE` & `pynetcheck-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.5/pynetcheck/models/device.py` & `pynetcheck-0.2.6/pynetcheck/models/device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import Optional
 
 from ciscoconfparse import CiscoConfParse
 from ipfabric import IPFClient
 from ipfabric.models.device import Device, DeviceConfig
 
 
@@ -31,14 +32,17 @@
         self.site: str = device.site.upper()
         self.loaded: bool = False
 
         # Config will load when test is run and then be removed to saved memory.
         self.config: Optional[DeviceConfig] = None
         self.parsed_config: Optional[ParsedConfig] = None
 
+    def __repr__(self):
+        return f"{self.inventory.hostname}:{self.inventory.sn}"
+
     def load_data(self):
         self.get_config()
         self.loaded = True
 
     def clear_data(self):
         self.config = None
         self.parsed_config = None
@@ -62,11 +66,24 @@
             )
             if self.config.start
             else None
         )
         if self.config.current:
             self.parsed_config = ParsedConfig(current, startup)
 
+    def _palo_alto_config(self):
+        log = self.inventory.get_log_file()
+        user = re.search(r"(\S*)@", log.split("\n")[0]).group(1)
+        self.config = DeviceConfig(
+            currentConfig=re.split(
+                rf"^{user}", log.split("show config merged")[1], flags=re.M
+            )[0].replace("\r\n", "\n"),
+            startupConfig=None,
+            status="N/A",
+        )
+
     def get_config(self):
-        self.config = self.inventory.get_config()
-        if self.config and self.inventory.vendor == "cisco":
+        if self.inventory.vendor == "cisco":
+            self.config = self.inventory.get_config()
             self._cisco_config()
+        elif self.inventory.vendor == "paloalto":
+            self._palo_alto_config()
```

### Comparing `pynetcheck-0.2.5/pynetcheck/models/shared.py` & `pynetcheck-0.2.6/pynetcheck/models/shared.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.5/pynetcheck/tests/cisco/conftest.py` & `pynetcheck-0.2.6/pynetcheck/tests/cisco/conftest.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.5/pynetcheck/tests/cisco/test_servers.py` & `pynetcheck-0.2.6/pynetcheck/tests/cisco/test_servers.py`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.5/pynetcheck/tests/conftest.py` & `pynetcheck-0.2.6/pynetcheck/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
         "--config-dir",
         help="Path to directory with configurations.",
         action="store",
         type=Path,
     )
     parser.addoption(
         "--snapshot",
-        help="IP Fabric Snapshot ID.",
+        help="Optional: IP Fabric Snapshot ID; defaults to `$last`.",
         action="store",
-        default="$last",
+        default=None,
         type=str,
     )
 
 
 def pytest_configure(config):
     global IPF, CONFIGS
```

### Comparing `pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py` & `pynetcheck-0.2.6/pynetcheck/tests/cve/cisco/test_cve_2023_20198_ios_xe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-iosxe-webui-privesc-j22SaA4z
 
 This will test for the following:
     - HTTP(S) Server Disabled
     - If Enabled then test HTTP(S) Server Vulnerable
 """
+
 import pytest
 from ciscoconfparse import CiscoConfParse
+from netutils.os_version import compare_version_loose
 
 from pynetcheck.models.device import IPFDevice
 from pynetcheck.models.shared import return_http_config
 from pynetcheck.tests.cisco.conftest import IOSXE
 from pynetcheck.tests.conftest import CONFIGS, ConfigFile
 
 pytestmark = [pytest.mark.cve, pytest.mark.cisco]
@@ -33,15 +35,15 @@
             device.load_data()
         if not device.parsed_config:
             pytest.skip("No configs for device.")
         yield
         device.clear_data()
 
     @staticmethod
-    def return_module_config(device, server):
+    def return_module_config(device: IPFDevice, server):
         current, startup = return_http_config(device, server)
         if current != "enabled" and startup != "enabled":
             pytest.skip(f"HTTP {server} Disabled")
         line = (
             "^ip http active-session-modules none"
             if server == "server"
             else "^ip http secure-active-session-modules none"
@@ -54,33 +56,57 @@
             mstartup = (
                 "secured"
                 if device.parsed_config.startup.find_lines(line)
                 else "vulnerable"
             )
         return mcurrent, mstartup
 
+    @staticmethod
+    def check_version(device: IPFDevice):
+        if (
+            (compare_version_loose(device.inventory.version, "<=", "17.3.8a"))
+            or (
+                compare_version_loose(device.inventory.version, ">=", "17.4")
+                and compare_version_loose(device.inventory.version, "<", "17.6.6a")
+            )
+            or (
+                compare_version_loose(device.inventory.version, ">=", "17.7")
+                and compare_version_loose(device.inventory.version, "<", "17.9.4a")
+            )
+        ):
+            return True
+        return False
+
     def test_http_server_disabled(self, device: IPFDevice):
         current, startup = return_http_config(device, "server")
         assert current == "disabled", f"{RUNNING} server Enabled"
         if device.config.status != "saved" and startup:
             assert startup == "disabled", f"{STARTUP} server Enabled"
 
     def test_https_server_disabled(self, device: IPFDevice):
         current, startup = return_http_config(device, "secure-server")
         assert current == "disabled", f"{RUNNING} secure-server Enabled"
         if device.config.status != "saved" and startup:
             assert startup == "disabled", f"{STARTUP} secure-server Enabled"
 
     def test_http_server_vulnerable(self, device: IPFDevice):
+        if not self.check_version(device):
+            pytest.skip(
+                f"{device.inventory.hostname}:{device.inventory.sn} is not an affected SW Version {device.inventory.version}."
+            )
         mcurrent, mstartup = self.return_module_config(device, "server")
         assert mcurrent == "secured", f"{RUNNING} server Vulnerable"
         if device.config.status != "saved" and mstartup:
             assert mstartup == "secured", f"{RUNNING} server Vulnerable"
 
     def test_https_server_vulnerable(self, device: IPFDevice):
+        if not self.check_version(device):
+            pytest.skip(
+                f"{device.inventory.hostname}:{device.inventory.sn} is not an affected SW Version {device.inventory.version}."
+            )
         mcurrent, mstartup = self.return_module_config(device, "secure-server")
         assert mcurrent == "secured", f"{RUNNING} server Vulnerable"
         if device.config.status != "saved" and mstartup:
             assert mstartup == "secured", f"{RUNNING} server Vulnerable"
 
 
 # Test each config file in `dir` directory for HTTP(S) Server configuration
```

### Comparing `pynetcheck-0.2.5/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py` & `pynetcheck-0.2.6/pynetcheck/tests/cve/cisco/test_cve_2024_20278.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+https://sec.cloudapps.cisco.com/security/center/content/CiscoSecurityAdvisory/cisco-sa-iosxe-priv-esc-seAx6NLX
+"""
+
 import pytest
 from ciscoconfparse import CiscoConfParse
 
 from pynetcheck.models.device import IPFDevice
 from pynetcheck.models.shared import return_service_config
 from pynetcheck.tests.cisco.conftest import IOSXE
 from pynetcheck.tests.conftest import CONFIGS, ConfigFile
@@ -19,15 +23,15 @@
             device.load_data()
         if not device.parsed_config:
             pytest.skip("No configs for device.")
         yield
         device.clear_data()
 
     def test_netconf_yang_disabled(self, device: IPFDevice):
-        current, startup = return_service_config(device, 'netconf-yang')
+        current, startup = return_service_config(device, "netconf-yang")
         assert current == "disabled", f"Running Config - netconf-yang Enabled"
         if device.config.status != "saved" and startup:
             assert startup == "disabled", f"Startup Config - netconf-yang Enabled"
 
 
 @pytest.mark.parametrize(
     "config_file", CONFIGS, ids=[c.file.name for c in CONFIGS], scope="class"
@@ -47,9 +51,7 @@
         yield
         config_file.parsed = None
         print("TEARDOWN", config_file.file.name)
 
     def test_netconf_yang_disabled(self, config_file):
         line = "^netconf-yang"
         assert not config_file.parsed.find_lines(line), f"Config - netconf-yang Enabled"
-
-
```

### Comparing `pynetcheck-0.2.5/pyproject.toml` & `pynetcheck-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyNetCheck"
-version = "0.2.5"
+version = "0.2.6"
 license = "MIT"
 description = "Python Network device checker using Pytest and IP Fabric."
 authors = [
     "Solution Architecture <solution.architecture@ipfabric.io>",
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
 ]
 readme = "README.md"
@@ -20,14 +20,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 ipfabric = "^6.7.0"
 ciscoconfparse = "^1.9.0"
 pytest = "^8.0.0"
 pytest-html-reporter = "^0.2.9"
+netutils = "^1.8.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pynetcheck-0.2.5/README.md` & `pynetcheck-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pynetcheck-0.2.5/PKG-INFO` & `pynetcheck-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyNetCheck
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python Network device checker using Pytest and IP Fabric.
 Home-page: https://gitlab.com/ip-fabric/integrations/pynetcheck
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Solution Architecture
 Author-email: solution.architecture@ipfabric.io
 Requires-Python: >=3.8.1,<4.0.0
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ciscoconfparse (>=1.9.0,<2.0.0)
 Requires-Dist: ipfabric (>=6.7.0,<7.0.0)
+Requires-Dist: netutils (>=1.8.0,<2.0.0)
 Requires-Dist: pytest (>=8.0.0,<9.0.0)
 Requires-Dist: pytest-html-reporter (>=0.2.9,<0.3.0)
 Project-URL: Changelog, https://gitlab.com/ip-fabric/integrations/pynetcheck/-/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://gitlab.com/ip-fabric/integrations/pynetcheck
 Project-URL: IP Fabric, https://ipfabric.io/
 Project-URL: Repository, https://gitlab.com/ip-fabric/integrations/pynetcheck
 Description-Content-Type: text/markdown
```

