# Comparing `tmp/ligo_softioc-0.1.1.tar.gz` & `tmp/ligo_softioc-0.1.2.tar.gz`

## Comparing `ligo_softioc-0.1.1.tar` & `ligo_softioc-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/setup.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/examples/active.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/examples/passive.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/src/ligo_softioc/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/src/ligo_softioc/alarm.py
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/src/ligo_softioc/alarm_family.py
--rw-r--r--   0        0        0    16226 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/src/ligo_softioc/soft_ioc.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/src/ligo_softioc/util.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/.gitignore
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/COPYING
--rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/LICENSE
--rw-r--r--   0        0        0    13045 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    13678 2020-02-02 00:00:00.000000 ligo_softioc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/setup.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/changelog
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/compat
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/control
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/copyright
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/python3-ligo-softioc.install
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/rules
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/debian/source/format
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/examples/active.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/examples/passive.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/alarm.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/alarm_family.py
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/soft_ioc.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/sorted_dict.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/src/ligo_softioc/util.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/COPYING
+-rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/LICENSE
+-rw-r--r--   0        0        0    13095 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13728 2020-02-02 00:00:00.000000 ligo_softioc-0.1.2/PKG-INFO
```

### Comparing `ligo_softioc-0.1.1/examples/active.py` & `ligo_softioc-0.1.2/examples/active.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 X1:IOC-HOSTNAME
 X1:IOC-PROCESS
 X1:IOC-ERROR_MESSAGE
 X1:IOC-ERROR_GPS
 X1:IOC-ERROR_TIMESTAMP
 """
 
-from softioc import SoftIOC
+from ligo_softioc import SoftIOC
 import sys
 
 process_count = 0
 
 def process(ioc: SoftIOC, gps_time_sec: int) -> None:
     """
     Update the custom channels.
```

### Comparing `ligo_softioc-0.1.1/examples/passive.py` & `ligo_softioc-0.1.2/examples/passive.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   X1:SYS-EXAMPLE_LAST_PROCESS_GPS
   X1:SYS-EXAMPLE_LAST_PROCESS_TIMESTAMP
   X1:SYS-EXAMPLE_SINCE_LAST_PROCESS_SEC
   X1:SYS-EXAMPLE_SINCE_LAST_PROCESS_STR
   X1:SYS-EXAMPLE_SERVER_RUNNING
 """
 
-from softioc import SoftIOC
+from ligo_softioc import SoftIOC
 
 if __name__ == "__main__":
     # Setup the IOC with a channel prefix.
     # set `separate_server` to true to make this a passive IOC
     ioc = SoftIOC(
         prefix="X1:SYS-EXAMPLE_",
         separate_server=True
```

### Comparing `ligo_softioc-0.1.1/src/ligo_softioc/alarm.py` & `ligo_softioc-0.1.2/src/ligo_softioc/alarm.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/src/ligo_softioc/alarm_family.py` & `ligo_softioc-0.1.2/src/ligo_softioc/alarm_family.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/src/ligo_softioc/soft_ioc.py` & `ligo_softioc-0.1.2/src/ligo_softioc/soft_ioc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 
+import sys
 import logging
 import re
 import os
 import threading
 from socket import gethostname
 import time
+from configparser import ConfigParser
 
 from gpstime import gpsnow, gpstime
 from pcaspy import Driver, SimpleServer
 
 from typing import Dict, Union, Callable, Optional, Set
 import pcaspy
 from .alarm import Alarm, AlarmGroup
 from .alarm_family import  AlarmFamily
+from .sorted_dict import  SortedDict
 
 
 from .util import gps_to_str, delta_seconds_to_readable, PyIOCError
 
 PREFIX_REGEX = re.compile(r"[A-Z0-9]{2}:[A-Z]{3}-([A-Z0-9]+_)+")
 PREFIX_LIMIT = 40
 SUBPREFIX_REGEX=re.compile(r"([A-Z0-9]+_)*")
@@ -381,25 +384,61 @@
                 self._set_pv_status()
 
             self.updatePVs()
             for af in self.alarm_families:
                 af.check_input_channels(self)
             time.sleep(self.process_period_sec)
 
-    def print_ini(self):
+    def chan_to_type(self, chan: str) -> int:
+        """
+        Return the DAQ type number for the given channel name
+        :param chan:
+        :return:
+        """
+        if 'type' not in self.channels[chan]:
+            t = 'float'
+        else:
+            t = self.channels[chan]['type']
+        if t == 'float':
+            return 4
+        elif t == 'double':
+            return 5
+        elif t == 'int':
+            return 2
+        elif t == 'uint':
+            return 7
+        elif t == 'short':
+            return 1
+        elif t == 'long':
+            return 3
+        else:
+            raise Exception(f"Unhandled type {str(t)} for channel {chan}")
+
+    def write_ini(self, fstream):
         """
         Send to std output, one line per name in alphabetical order, each surrounded by square brackets.
 
         All custom channels that aren't string.
 
         From the automatic channels: START_GPS, GPS, UPTIME_SEC,
 
         If separate_server == True,
         SERVER_START_GPS, SERVER_GPS, SERVER_UPTIME_SEC, LAST_PROCESS_GPS, SINCE_LAST_PROCESS_SEC, SERVER_RUNNING,
 
 
         If there are any alarm families, print the GPS_TIME channel on the alarm family.
+        :param fstream: output file
         :return:
         """
-        chans = [f"[{self.prefix}{x}]" for x in self.ini_channels]
+        cfp = ConfigParser(dict_type=SortedDict)
+
+        chans = list(self.ini_channels)
         chans.sort()
-        print("\n".join(chans))
+        for chan in self.ini_channels:
+            fullname = f"{self.prefix}{chan}"
+            cfp.add_section(fullname)
+            cfp[fullname]['datatype'] = str(self.chan_to_type(chan))
+        cfp.write(fstream)
+
+    def print_ini(self):
+        self.write_ini(sys.stdout)
+
```

### Comparing `ligo_softioc-0.1.1/src/ligo_softioc/util.py` & `ligo_softioc-0.1.2/src/ligo_softioc/util.py`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/COPYING` & `ligo_softioc-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/LICENSE` & `ligo_softioc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/README.md` & `ligo_softioc-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,17 @@
 
 START_GPS        
 : The GPS second recorded when the IOC started.
 
 START_TIMESTAMP
 : The start time formatted the same as TIMESTAMP
 
+UPTIME_SEC
+: Seconds since the start of the IOC.
+
 UPTIME_STR        
 : The uptime of the IOC as an easy to understand string, e.g. "3 weeks".
 
 HOSTNAME
 : The name of the host the IOC is running on
 
 PROCESS
```

### Comparing `ligo_softioc-0.1.1/pyproject.toml` & `ligo_softioc-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ligo_softioc-0.1.1/PKG-INFO` & `ligo_softioc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ligo-softioc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Support library for writing EPICS SoftIOCs in Python.
 Project-URL: Homepage, https://git.ligo.org/cds/admin/softioc
 Project-URL: Issues, https://git.ligo.org/cds/admin/softioc/-/issues
 Author-email: Erik von Reis <evonreis@caltech.edu>
 License-File: COPYING
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -115,14 +115,17 @@
 
 START_GPS        
 : The GPS second recorded when the IOC started.
 
 START_TIMESTAMP
 : The start time formatted the same as TIMESTAMP
 
+UPTIME_SEC
+: Seconds since the start of the IOC.
+
 UPTIME_STR        
 : The uptime of the IOC as an easy to understand string, e.g. "3 weeks".
 
 HOSTNAME
 : The name of the host the IOC is running on
 
 PROCESS
```

